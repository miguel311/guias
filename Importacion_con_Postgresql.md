<h1>Importacion de base de datos postgresql</h1> 

Implementar esto en base de datos
sed -e '/idle_in_transaction_session_timeout/d;/row_security/d' volcado_bd_sipes.sql > volcado_sep.sql

En caso que siga fallando 
sed -e '/idle_in_transaction_session_timeout/d;/SET row_security = off;'  volcado_bd_sipes.sql > volcado_sep.sql

Ingresa en base de datos creada vacia 
psql sipes_10_sep

aparecera algo asi 
sipes_10_sep=#

Comandos apra la importacion segun la ubicación.
begin;
\i /var/www/html/volcado_sep.sql;
commit;

En caso de error en esta parte No finalizar con commit; agregar:
rollback


salimos de postgres 
\q

Y Listo 

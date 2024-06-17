FROM mysql:8.0.33
<<<<<<< HEAD
ENV MYSQL_ROOT_PASSWORD:vprodbpass
ENV MYSQL_DATABASE:accounts
ADD db_backup.sql /docker-entrypoint-initdb.d/db_backup.sql
=======
LABEL "Project"="Vprofile"
LABEL "AUthor"="SSgaikwad"

ENV MYSQL_ROOT_PASSWORD="vprodbpass"
ENV MYSQL_DATABASE="accounts"
ADD db_backup.sql docker-entrypoint-initdb.d/db_backup.sql
>>>>>>> d176436e5e6a6fcab5b9256d30138d59c97f94ab

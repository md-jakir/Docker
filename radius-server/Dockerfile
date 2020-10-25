FROM freeradius/freeradius-server:latest
RUN apt-get update
RUN apt-get install -y mysql-client
COPY raddb/mods-available/sql /etc/raddb/mods-enabled/sql
COPY raddb/sites-available/default /etc/raddb/sites-available/default
COPY raddb/sites-available/inner-tunnel /etc/raddb/sites-available/inner-tunnel

# Note: If getting this error during update
# Release file for http://security.ubuntu.com/ubuntu/dists/bionic-security/InRelease is not valid yet 
# its need to set up date and time using timedatectl in server then error will be fixed. 

pentaho-service-script
======================

Script for installation of Pentaho BI-Server as service


## Installation

* Insert the pentaho file inside /etc/init.d/
* Edit the pentaho file with your configurations;
* Add permissions to execute 

  ```Shell
  sudo chmod a+x /etc/init.d/pentaho
   ```
* Add the script as service 
  - CentOs
  ```Shell
  cd /etc/init.d
  sudo chkconfig --add pentaho
   ```

  - Ubuntu/Debian
  ```Shell
  cd /etc/init.d
  sudo update-rc.d pentaho defaults
   ```

## Usage

* Start Pentaho biserver

  ```Shell
  service pentaho start
   ```
   
* Stop Pentaho biserver

  ```Shell
  service pentaho stop
   ```
   
* Start Pentaho administration-console

  ```Shell
  service pentaho start adm
   ```
   
* Stop Pentaho administration-console

  ```Shell
  service pentaho stop adm
   ```
   
## Credits
Thanks @oDanielRabelo for write the tutorial http://danielrabelo.wordpress.com/2013/09/06/pentaho-4-8-inicializando-como-servico-no-centos-6-2/

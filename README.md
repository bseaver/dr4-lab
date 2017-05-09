# D7

#### Demonstrate Ajax request module and many to many relationships

### Requires previous installation of:
  * Git (https://git-scm.com/downloads)
  * MAMP (https://www.mamp.info/) to host the Website and MySQL Database

### Utilizes:
  * Drupal 7.54 (https://www.drupal.org/)

### Installation Notes From GitHub:
  * git clone this repo on your desktop
  * This cloned folder is the `project` or `site` folder
  * The folder may be renamed at this point to your preference or convenience
  * Database, database user, site administrator and all passwords are `D7`
  * Site database is stored in sites/db-backup/ and needs to be imported into MAMP by opening `localhost:8888/phpmyadmin/`
  * You may need to recreate in MAMP SQL the `D7` administrator database user and password
  * Set MAMP's Host Document Root folder to site folder, restart servers
  * Launch site by opening `localhost:8888/`

### Summary of Steps Used to Create a Drupal Site:
* Copy downloaded Drupal core to the Desktop (for convenience)
* Rename the Drupal core folder to indicate the name of the project
* The following commands apply from the root of the project folder:
* Rename (to effectively remove) .gitignore
* The following may be needed in access controlled environments:
  * $ `chmod -R a+w sites/default`
  * Copy `project/sites/default/default.settings.php` to `project/sites/default/settings.php`
* Set MAMP's Host Document Root folder to project folder, restart servers
* Open SQL page `localhost:8888/phpmyadmin/`
* Create database with collation `utf8_general_ci`
* Create admin user for Drupal site's internal use
* Open `localhost:8888/` for new Drupal site
* Setup: Standard, English, Database, host and port 127.0.0.1 and 8889
* Initial Site name, email, admin user, country, time zone and turn off e-mail notices for demonstration purposes
* Verify initial site is working
* Create a README.md file in the project root
* Commit the README.md
* Commit initial Drupal files and database backup
* Iteratively, add features to site and commit

### Incremental and Final Save of Site Database
* Export MAMP hosted database specifying:
  * Custom, SQL, All Tables (structure and data)
  * Save output to File, Compression: zipped
  * Add option: create database
  * Add option: drop table
* Save zip file to sites/db-backup/ (replacing previous copy if any)
* Add and Commit this file to the git repository

## Copyright (c)
* 2017 Benjamin T. Seaver and Andrew Devlin

## Known Bugs
* No known bugs

## Support and contact details
* None

## License
* MIT

##### End of File

Wagento Meetup module for composer demo
======================

This module for composer demo

Facts
-----
* version: 2.2.1

Description
-----------
01/12/18

* This module use to give composer demo


Requirements
------------
* PHP >= 7.0.2

Compatibility
-------------
* Magento >= 2.1.4

Installation Instructions
-------------------------
The Wagento Meetup module for Magento® 2 is distributed in two formats:
* Drop-In
* [Composer VCS](https://getcomposer.org/doc/05-repositories.md#using-private-repositories)

### Install Source Files ###

The following sections describe how to install the module source files,
depending on the distribution format, to your Magento® 2 instance.

#### Drop-In ####
If you received a single ZIP file with no `composer.json` file included, extract
its contents to the project root directory. The module sources should then be
available in the following sub-directory:

    app
    └── code
        └── Wagento
            └── Meetup

#### VCS ####
If you prefer to install the module using [git](https://git-scm.com/), run the
following commands in your project root directory:

    composer config repositories.wagento-module-meetup git git@github.com:sanjay-wagento/wagento-module-meetup.git
        composer require wagento/module-meetup:2.2.*

### Enable Module ###
Once the source files are available, make them known to the application:

    ./bin/magento module:enable Wagento_Meetup
    ./bin/magento setup:upgrade

Last but not least, flush cache and compile.

    ./bin/magento cache:flush
    ./bin/magento setup:di:compile

Uninstallation
--------------

The following sections describe how to uninstall the module, depending on the
distribution format, from your Magento® 2 instance.

#### Composer Git ####

To unregister the shipping module from the application, run the following command:

    ./bin/magento module:uninstall --remove-data Wagento_Meetup

This will automatically remove source files and clean up the database.

#### Drop-In ####

To uninstall the module manually, run the following commands in your project
root directory:

    ./bin/magento module:disable Wagento_Meetup
    rm -r app/code/Wagento/Meetup

Features
--------------


#### Admin Settings ####
Admin >> Stores > Settings >> Configuration >> Wagento >> Meetup

General
* Enabled


Developer
---------
* Sanjay Patel | [Wagento](https://www.wagento.com/) | sanjay@wagento.com

License
-------
[OSL - Open Software Licence 3.0](http://opensource.org/licenses/osl-3.0.php)
# Trippo File Manager Package (as ResponsiveFileManager)

*********************************************
## Trippo File Manager v2.4.0 - Dec 12th, 2019
*********************************************
## Changelog
* Add firebase/php-jwt package
* Use firebase/php-jwt package as a option secure type
* Update README: add usage guide RFM_SECURE_TYPE
*********************************************
## Trippo File Manager v2.3.0 - Dec 8th, 2019
*********************************************
## Changelog
* Add check subfolder by GET method
*********************************************
## Trippo File Manager v2.2.0 - Dec 8th, 2019
*********************************************
## Changelog
* Clean code unused
*********************************************
Trippo File Manager v2.1.0 - Dec 8th, 2019
*********************************************
## Changelog
* Fix bug `vendor` directory not found on production
*********************************************
Trippo File Manager v2.0.0 - Dec 8th, 2019
*********************************************
## Changelog
* Change `/vendor/` make available production and development
* Add feature: check upload/thumbs dir available in-case it's not created
* Update `.gitignore`
* Add guide: try the demo with a built-in server (available PHP 5.6 or newer)
*********************************************
## Trippo File Manager v1.0.0 - Dec 8th, 2019
*********************************************
## Server Requirements
* OS: Linux 18.04 (recommended)
* PHP: PHP 5.6 or newer

## Installation
1. Run composer require project (for init new project) or update (for reload dependencies on new environment) via command line at root folder
* Require project
```shell
composer require ngthuc/trippo-filemanager
```
* Reload dependencies
```shell
composer update
```
2. Copy file environment from `/vendor/ngthuc/trippo-filemanager/filemanager.env` to the root project structure:
```shell
root                          # → Root Directory
└── vendor/
    └── ngthuc/
        └── trippo-filemanager/
            └── filemanager.env
```
3. Set-up environment if you want use another variable values

## Author of package
* [Nguyen Thuc](https://ngthuc.github.io/)
* Homepage: ngthuc.com
* Packagist: [Trippo File Manager](https://packagist.org/packages/ngthuc/trippo-filemanager) by ngthuc
* Email: contact[at]ngthuc.com
*********************************************

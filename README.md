## Intro for ResponsiveFileManager by trippo

Responsive FileManager is a free open-source file manager made with the jQuery library, CSS3, PHP and HTML5 that offers a nice and elegant way to upload and insert files, images and videos. You can use it as external plugin for TinyMCE version 4.x. or CKEditor and you can also use it as a stand-alone file manager to manage and select files. The script automatically creates thumbnails of images for the preview list and can create also external thumbnails to use in your cms or site. It can be configured for automatic resizing of uploaded images or to automatically limit the size. You can personalize the configuration for each folder. You can set a subfolder as the root and change the configuration for each user, page or FileManager call. Is compatible with multi-user mode and you can edit images with aviary editor, sorting files.

DEMO AND DOCUMENTATION: http://www.responsivefilemanager.com/

PRODUCTION VERSION DOWNLOAD: https://github.com/trippo/ResponsiveFilemanager/releases

Released under Creative Commons Attribution-NonCommercial 3.0 Unported License.

Creator : info@albertoperipolli.com - tr1pp0

## Version ResponsiveFilemanager
[Resposive Filemanager v9.14.0](https://github.com/trippo/ResponsiveFilemanager/releases/latest) (May 5th, 2019)

## Server Requirements
* OS: Linux 18.04 (recommended)
* PHP: PHP 5.6 or newer

## Installation and try demo without AMP stack
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
4. Try demo via command `php -S localhost:80` on root directory

## Secure (optional)
You can choose secure type: none (default), GET method and cookie with JWT and RS256
1. None-Secure (default): nothing change everythings
2. `GET` method: add `user` value to url. Example: `http://domain.of.you/dialog.php?user=username_or_subfolder_name&.....`. Don't forget change environment of `RFM_SECURE_TYPE` to `GET`
3. Cookie with JWT and RS256
* Change environment `RFM_SECURE_TYPE` to path-to-public-key (create with [openssl](https://lunar.lyris.com/help/lm_help/12.0/Content/generating_public_and_private_keys.html)).
* Create token with payload has `sub` param is username or subfolder name and encode with private key
* Add token to cookie with cookie name is `rfm_token`

## OpenSSL Example
1. Install
* Windows: [click-here](https://slproweb.com/products/Win32OpenSSL.html)
* Linux: [view on GitHub](https://github.com/openssl/openssl) or [tutorial](https://www.howtoforge.com/tutorial/how-to-install-openssl-from-source-on-linux/)
2. Generating public and private key with openssl
* Navigate to your project folder (or anywhere you need openssl)
* Open command prompt or terminal
* Generating private key
```
openssl genrsa -out rsa.private 1024
```
* Generating public key with private key
```
openssl rsa -in rsa.private -out rsa.public -pubout -outform PEM
```
* View detail on [website](https://lunar.lyris.com/help/lm_help/12.0/Content/generating_public_and_private_keys.html)

## Author of package
* [Nguyen Thuc](https://ngthuc.github.io/)
* Homepage: ngthuc.com
* Packagist: [Trippo File Manager](https://packagist.org/packages/ngthuc/trippo-filemanager) by ngthuc
* Email: contact[at]ngthuc.com

## Localization (and thanks for contributors)

- AZE [Elshad Agayev]
- BGR [Stanislav Panev]
- BRA [paulomanrique]
- CAT [Manel Peña]
- CHN [Vu Doan Thang]
- CRO
- CZE [jlusticky]
- DAN [Morten Hesselberg Grove]
- ENG
- ESP [Roberto Santamaria]
- FRA [Mathieu Ducharme]
- GER [Oliver Beta]
- GRC [vkouvelis]
- Hebrew [sagie212]
- HUN [Novak Szabolcs]
- IND [urayogi]
- ITA
- JPN [Vu Doan Thang]
- LTU [Tomas Norkūnas]
- MON [Tumenzul Batjargal]
- NLD [Martijn van der Made]
- NOR [Pål Schroeder]
- Persian [web2web esf ir]
- POL [Michell Hoduń]
- POR [Sérgio Lima]
- RUS [vasromand]
- SLO [Roman Šovčík]
- SVN [Peter Benko]
- SWE [Jon Sten]
- TUR [Ahmed Faruk Bora]
- UKR [Sergey]

## Credits

- [Responsive File Manager](https://www.responsivefilemanager.com/)
- [Bootstrap](http://twitter.github.io/bootstrap)
- [Bootstrap Lightbox](http://jbutz.github.io/bootstrap-lightbox)
- [Dropzonejs](http://www.dropzonejs.com)
- [Fancybox](http://fancybox.net)
- [TouchSwipe](http://labs.rampinteractive.co.uk/touchSwipe/demos)
- [PHP Image Magician](http://phpimagemagician.jarrodoberto.com)
- [Mini icons](http://www.fatcow.com/free-icons)
- [Jupload](http://jupload.sourceforge.net)
- [Bootbox](http://bootboxjs.com)
- [jQuery contextMenu](https://swisnl.github.io/jQuery-contextMenu/)
- [Bootstrap-modal](https://github.com/jschr/bootstrap-modal)
- [jPlayer](http://jplayer.org)
- [Lazy Load Plugin for jQuery](http://www.appelsiini.net/projects/lazyload)
- [PHP dotenv by vlucas](https://github.com/vlucas/phpdotenv).
- [PHP-JWT by firebase](https://github.com/firebase/php-jwt).

## License
Trippo File Manager is licensed under the [Creative Commons Attribution-NonCommercial 3.0 Unported License - CC-BY-NC-3.0](LICENSE).

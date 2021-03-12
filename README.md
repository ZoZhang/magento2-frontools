[![Travis branch](https://img.shields.io/travis/SnowdogApps/magento2-frontools/master.svg)](https://travis-ci.org/SnowdogApps/magento2-frontools) [![Packagist](https://img.shields.io/packagist/v/snowdog/frontools.svg)](https://packagist.org/packages/snowdog/frontools) [![Packagist](https://img.shields.io/packagist/dt/snowdog/frontools.svg)](https://packagist.org/packages/snowdog/frontools) [![Greenkeeper badge](https://badges.greenkeeper.io/SnowdogApps/magento2-frontools.svg)](https://greenkeeper.io/)

# Magento 2 Frontools
Set of front-end tools for Magento 2, based on Gulp.js
Fork: https://github.com/SnowdogApps/magento2-frontools
 
## Usage

### Magento 2 Config
```
bin/magento deploy:mode:set developer
bin/magento config:set dev/css/minify_files 0
bin/magento config:set dev/css/merge_css_files 0
bin/magento config:set dev/js/merge_files 0
bin/magento config:set dev/js/minify_files 0
bin/magento config:set dev/js/enable_js_bundling 0
bin/magento config:set weltpixel_googletagmanager/general/enable 0
```

### Terminale
```
brew install yarn
composer require snowdog/frontools --ignore-platform-reqs 
cd vendor/snowdog/frontools
npm install
yarn global add gulp-cli 
gulp setup
cd $ROOT_MAGENTO/tools
gulp dev --theme rsrv-basic
```
###  browser-sync not working
```
npm install -g browser-sync 
// test
browser-sync start --server --files "*.html , css/*.css , js/*.js" 
```
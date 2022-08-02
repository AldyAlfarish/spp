# spp
assalamualaikum, if php requires php ^7.3 but your php version (8.0.0) does not satisfy that requirement

It's because in your project in composer.json file you have:

"require": {
    "php": ">=7.3",
    .....
},

Try to update this requirement to:

"require": {
    "php": "^7.3|^8.0",
    .....
},
Yoy can do with below command

composer install --ignore-platform-reqs

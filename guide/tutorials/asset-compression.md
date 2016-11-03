Assets
======




Asset compression
-----------------

phd bundles the assets in the `:development` Docker container, which comes pre-installed with all required
tools, to make use of Yii 2.0 Framework asset compresssion.

For debugging you can enter a development container

    docker-compose run --rm php bash

and bundle the assets from the container-bash
    
    $ mkdir -p web/assets-prod/js web/assets-prod/css       
    $ yii asset src/config/assets-prod.php src/config/bundle-prod.php
    
> Note! Make sure not to use a backlash `\` at the beginning of your asset-bundle name, since it may conflict with
> the `className()` which returns values without a starting backslash

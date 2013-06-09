PulseStormModuleList
=================

A Magento module that lists other installed modules. 

###Module List

The Module List Module provides you with a list of enabled and disable modules, as well as some simple tools for debugging your own module installation issues.  Module here refers to Magento Code Modules, which are separate from Magento Connect Extensions. 

Original Blog Post: http://alanstorm.com/magento_list_module

###Build Instructions

The `build_module_list.bash` file is a bash script that will create a simple tar archive of the extension files. 

    $ ./build_module_list.bash
    
This script assumes the existence of a `var` folder.    

The `magento-tar-to-connect.modulelist.php` file is a configuration file for the <a href="https://github.com/astorm/MagentoTarToConnect/">MagentoTarToConnect</a> command-line script.  This will allow you to build a Magento Connect 2.0 extension with the following.

    $ magento-tar-to-connect.phar magento-tar-to-connect.modulelist.php
    
See the <a href="https://github.com/astorm/MagentoTarToConnect/#readme">MagentoTarToConnect README.md</a> for more information on how this tool works.     
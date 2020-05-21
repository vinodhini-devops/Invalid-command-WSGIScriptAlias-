# Invalid-command-WSGIScriptAlias-
Invalid command 'WSGIScriptAlias', perhaps misspelled or defined by a module not included in the server configurationAction
**********************************************************************************************************************************

To enable wsgi_mod in httpd, install the module

    command: sudo yum install mod_wsgi
    
and make sure to load the module in the httpd config file

    command: sudo nano /etc/httpd/conf/httpd.conf
    
then add the following line in the config file, to the list of other loaded module:

LoadModule wsgi_module modules/mod_wsgi.so

*************************************************************************************************************************************

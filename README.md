Deploy the app with s2i builder: 

    oc new-app openshift/php~https://github.com/rschumm/hallophp.git

Add a route to the generated Service and open the URL. Add `/webhallo.php` to the URL and you should see the PHP output.  


Doku:   
https://github.com/sclorg/s2i-php-container/blob/master/7.1/README.md






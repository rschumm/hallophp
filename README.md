Minimales Beispiel für eine PHP-Applikation in OpenShift:   
(läuft auf jedem OpenShift Cluster)   

OpenShift erstellt automatisch eine BuildConfig und DeploymentConfig (etc.), baut ein Docker-Image in der internen Registry und lässt es laufen. 


Deploy the app with s2i builder: 

    oc new-app openshift/php~https://github.com/rschumm/hallophp.git

Add a route to the generated Service and open the URL. Add `/webhallo.php` to the URL and you should see the PHP output.  


Doku:   
https://github.com/sclorg/s2i-php-container/blob/master/7.1/README.md






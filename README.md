# Sample Blog site 
Using Spring Web Services, JPA, Core and Security


##Curl Commands
ETag indicates if the data record has been updated. 0 means that no updates has been made. Everytime the records are incremented the version will be increased
+ `curl -H "Accept: application/json" -i http://localhost:8080/posts/1`  - shows all post data
+ `curl -H "Accept: application/json" -H 'If-None-Match: "0"' -i http://localhost:8080/posts/1` - shows post where ETag is not 0, 

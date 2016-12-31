# CORSHttpHandler
A simple CORS enabled http server/handler that help making cross origin AJAX http requests to a CORS disabled web server 

There are cases there , you are in develoment phase and your are developing HTML locally on your machine before you deploy them into actual web server. Here you may need to make ajax requests from HTML to a web server that is not CORS enabled.

This situation is very painful as browsers block these kind of requests if server is not CORS enabled. To solve this issue CORSHttpHandler can be useful. It works as a middle ware between your web application (HTML) and web server.

  
|-- Your Web Aplication --| <-------->  |-- CORSHttpHandler --| <------->  |-- Web Server --|


In your local web application change the ajax request base URL to http:localhost://7000 and CORSHttpHandler change the var remoteUrl = 'your_remote_server_base_url_without_http.com' variable value to your target web server base URL.


  ``` json
 "name": "getBerufeListe",  
 "event": [  
  {  
   "listen": "test",  
   "script": {  
    "exec": [  
     "\r",  
     "pm.test(\"Status code is 200\", function () {\r",  
     "    pm.response.to.have.status(200);\r",  
     "});\r",  
     "\r",  
     "\r",  
     ""  
    ],  
    "type": "text/javascript"  
   }  
  }  
 ],  
 "request": {  
  "method": "GET",  
  "header": [],  
  "url": {  
   "raw": "http://localhost:8080/berufsmodul/api/v1/beruf?leistungsbereichId=2&gueltigVon=2015-01-01T00:00:00.531Z&gueltigBis=2030-03-20T00:00:00.531Z",  
   "protocol": "http",  
   "host": [  
    "localhost"  
   ],  
   "port": "8080",  
   "path": [  
    "berufsmodul",  
    "api",  
    "v1",  
    "beruf"  
   ],  
   "query": [{  
    "key": "leistungsbereichId",  
    "value": "2"  
   },  
   {  
    "key": "gueltigVon",  
    "value": "2015-01-01T00:00:00.531Z"  
   },  
   {  
    "key": "gueltigBis",  
    "value": "2030-03-20T00:00:00.531Z"  
   }]  
  }  
 },  
 "response": []  
}
```


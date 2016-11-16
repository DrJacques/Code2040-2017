# Code2040-2017
import requests
import json 
Jacques_Github = "https://github.com/DrJacques/Code2040-2017"
Jacques_Api="4eeaaf2a6fbaa35302e4c7098bd6b32c"
Registration_endpoint= "http://challenge.code2040.org/api/register"
request = requests.post(Registration_endpoint,  json = {'token':Jacques_Api, 'github':Jacques_Github})
print(request.content)
print(request.text)

# HAX
Humanitarian Activity Exchange
To use the HAX API, the path and payload must be specified.  The Path is based on the CRUD action you want to implement on on the Activity Stream.  For example

Route the incoming request based on type (LaunchRequest, IntentRequest,
 etc.) 
 
 The Payload should be a JSON body in the request that includes
FEEDTYPE, FEEDID, ACTIVITY

FEEDTYPES:
  user  
  notifications   
  alerts    
  organization  
  disaster

FEEDID:

EXAMPLE of HAX Payload.  
{ "feedType" : "organization",
  "feedId" : "xc4rft5s111",
  "activity": {
    "actor": "reliefweb:xc4rft5s111",
    "verb": "posted",
    "object": "document",
    "target": "http://reliefweb.int/report/burundi/burundi-note-d-informations-humanitaires-du-10-octobre-2016"
  }
}


The HAX API takes  incoming payload (Above) 
                          # case '/user/activities/':
                          
                          
                          # case '/user/activities/create/':
                           
                           # case '/user/activities/delete/':
                           # case '/user/activities/update/':
                           # case '/user/followers/':
                          #case '/user/following/':
                          #case '/user/follow/':  
            

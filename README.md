# Node.js Sample App

```cf push```

https://docs.cloudfoundry.org/buildpacks/node/node-tips.html


URL: https://cf-nodejs-silly-serval-eh.cfapps.sap.hana.ondemand.com/test
Output:                                         'path_with_params: /test'

URL: https://cf-nodejs-silly-serval-eh.cfapps.sap.hana.ondemand.com/test?param
Output:                                         'path_with_params: /test?param'

URL: https://cf-nodejs-silly-serval-eh.cfapps.sap.hana.ondemand.com/idp/card-lifecycle/Users?$expand=authorizations,cards
Output:                                         'path_with_params: /idp/card-lifecycle/Users?$expand=authorizations,cards'

URL: https://cf-nodejs-silly-serval-eh.cfapps.sap.hana.ondemand.com/idp/card-lifecycle/Users?$expand=authorizations%2cards
Output:                                         'path_with_params: /idp/card-lifecycle/Users?$expand=authorizations%2cards'


URL: https://cf-nodejs-silly-serval-eh.cfapps.sap.hana.ondemand.com/idp/card-lifecycle/Users?$expand=authorizations,cards;something_else%2more_stuff&more_more$test
Output: '                                        path_with_params: /idp/card-lifecycle/Users?$expand=authorizations,cards;something_else%2more_stuff&more_more$test'

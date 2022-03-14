{
  "openapi" : "3.0.1",
  "info" : {
    "title" : "TESTTEST_2",
    "version" : "v01"
  },
  "servers" : [ {
    "url" : "https://vpsoic02-axxwpguifl86-nt.integration.ocp.oraclecloud.com:443/ic/api/integration/v1/flows/rest/TESTTEST_2/1.0"
  } ],
  "paths" : {
    "/testtest2" : {
      "get" : {
        "responses" : {
          "204" : {
            "description" : "No content defined for this response",
            "content" : { }
          }
        },
        "security" : [ {
          "oauth2Authentication" : [ ]
        }, {
          "basicAuthentication" : [ ]
        } ]
      }
    }
  },
  "components" : {
    "securitySchemes" : {
      "oauth2Authentication" : {
        "type" : "oauth2",
        "flows" : {
          "authorizationCode" : {
            "authorizationUrl" : "https://idcs-de5ad99bf6204a568eda48953173a424.identity.oraclecloud.com:443/oauth2/v1/authorize",
            "tokenUrl" : "https://idcs-de5ad99bf6204a568eda48953173a424.identity.oraclecloud.com:443/oauth2/v1/token",
            "scopes" : {
              "https://vpsoic02-axxwpguifl86-nt.integration.ocp.oraclecloud.com:443urn:opc:resource:consumer::all" : "all"
            }
          }
        }
      },
      "basicAuthentication" : {
        "type" : "http",
        "scheme" : "basic"
      }
    }
  }
}

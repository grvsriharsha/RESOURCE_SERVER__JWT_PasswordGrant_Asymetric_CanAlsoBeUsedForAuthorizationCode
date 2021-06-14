# standAloneRESOURCE_SERVER

when security.oauth2.resource.jwt.key-uri=http://localhost:9092/oauth/token_key
is configured resourse server ,it will automatically
The spring-security on Behalf of Resourse server will automatically downloads/uses the publickey from given end point,converts the token 
and validates the key.For validation Resourse server in JWT doesnt require UserDetailService ,bcz everything is already checked by Authorizationserver
and so Resourceserver just needs to decode and check validity of token.


The Authorization and Resource server connect by

1.ResourceId

2.Private_public key pair

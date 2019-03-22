# RESTful-API-Symfony-4-JWT
RESTful API with Symfony 4 and Json Web Tokens

# Creamos el directorio jwt.
mkdir config/jwt
 
# Generamos el certificado privado utilizando el pass phrase "mykanban".
openssl genrsa -out config/jwt/private.pem -aes256 4096
 
# Generamos el certificado público introduciendo el pass phrase "mykanban"
# cuando nos lo solicite.
openssl rsa -pubout -in config/jwt/private.pem -out config/jwt/public.pem
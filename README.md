# buildpack-pkcs12-cert-importer
Heroku buildpack for certificate import

# Usage
Append the buildpack-pkcs12-cert-importer to your buildpack list:
```
heroku buildpacks:add https://github.com/akaKuruma/buildpack-pkcs12-cert-importer
```

Configure PKCS12_CERT_URL environment variable with the URL of PKCS12 certificate file:

```
heroku config:set PKCS12_CERT_URL="https://secret-location.net/82237EF4-0EDA-4EC0-B674-03A01AE8C958/azure-ldaps-certificate.pfx"
```

Configure PKCS12_CERT_PASSWORD environment variable with the PKCS12 Certificate password:

```
heroku config:set PKCS12_CERT_PASSWORD="CERTIFICATE PASSW0RD"
```

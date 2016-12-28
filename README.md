# ATS REST SERVICES 

# Try

Get http://localhost:8080/deposit/3231231?amount=320&currency=RSD&side=LEFT&comment="Nekakav Comment"
    http://localhost:8080/result/3231231


# Command line arguments
mvn spring-boot:run -Drun.arguments="--url=http://elendil:1860/"
mvn spring-boot:run -Drun.arguments="--url=http://elendil:1860/,--timeout=60"


## --url 
  Http adresa i port na kome radi PASERVER
  
## --timeout 
  Vreme u sekundama posle kojih se odustaje od poziva ka PASERVERU

## Keystore 

keytool -genkey -keyalg RSA -alias atsselfsigned -keystore keystore.jks -storepass anamarija  -validity 360 -keysize 2048

### HTTPS call 
https://user:braca@localhost:8080/deposit/test?amount=1200&currency=RSD&side=LEFT&comment="Nekakav Comment"

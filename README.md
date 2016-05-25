# spring-cloud-config
Spring Cloud Config Server 

Generate keystore

    keytool -genkeypair -keystore config.jks -storepass s3cr3t -alias config \
        -keyalg RSA -keysize 2048 -validity 1000 -keypass s3cr3t \
        -dname "CN=*.local.pcfdev.io,OU=Spring team,O=Pivotal,L=Singapore,S=Singapore,C=SG" -ext SAN=dns:localhost 
        
Next        
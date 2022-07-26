# Spring Boot Login and Registration Backend + Email Verification

- Spring Boot
- Spring Security
- Java Mail
- Email verification with expiry 

# Notes
- Used MySQL Database locally
- You are able to use your local database by updating the `application.yaml` fields
- Used on real email messages. Change mail.username & mail.password in `application.yaml` according to you
- Also default `server.port = 8080`

Folder Structure 
=====================
    ./src/main/java/com/example/demo
    
    ├── appuser                  
        ├── AppUser.java                            # User entity class
        ├── AppUserRole.java                        # User Role entity class
    ├── email                                       # Email sending transactions are handled here
    ├── registration                
        ├── token 
            ├── ConfirmationToken.java              # Token entity class 
            ├── ConfirmationTokenService.java       # Token transactions are handled here
        ├── RegistrationController.java             # Main API ( ADD Users , CONFIRM Tokens ) 
        ├── RegistrationRequest.java                # User creation class just like DTO
    ├── security
    └── DemoApplication.java

# Diagram
[![104789980-15581a00-578e-11eb-998d-30f2e6a9f461.png](https://i.postimg.cc/Qdz4LjDD/104789980-15581a00-578e-11eb-998d-30f2e6a9f461.png)](https://postimg.cc/68dLnJTb)

# Email verification link with expiry
[![de4fd296-397f-414e-abdf-fcc5c6bc911a.jpg](https://i.postimg.cc/PqRKFRNP/de4fd296-397f-414e-abdf-fcc5c6bc911a.jpg)](https://postimg.cc/NyR1Kb6c)

# Example Requests
[![registration1.png](https://i.postimg.cc/ZnCmzgx2/registration1.png)](https://postimg.cc/sGdqpT84)

# Microservice
A microservice is an application architecture that separates each application function into its own service from the others. These services can be deployed independently and are loosely connected that communicate through lightweight protocols.<br>
This microservice performs three tasks :- 
* Error handling - to handle server status
* Visitor counter - to count the number of visitors
* Authentication<br><br>

## Installation
```bash
git clone https://github.com/Ritam02-cyber/Documementation-Microservice.git
```
### Navigation
```bash
cd MicroService/
```
```bash
cd AuthAPI/ or cd ErrorHandler/ or cd ViewCounter/
```

### Installation
```bash
npm init
```
Then install the dependencies - express, mongoose, nodemon, dotenv, jsonwebtoken, bcrypt, validator, fs using :-
```bash
npm i
```

Create a .env file and add the MongoDB database username and password :-
```bash
DATABASE_URL = mongodb+srv://<username>:<password>@cluster0.nv6infp.mongodb.net/test
JWT_TOKEN = stringforjwt
```

### Run server
```bash
npm start
```

## API Reference
### Authentication
#### Sign-up
It returns a token.
```bash
POST http://localhost:3000/api/sign-up
```
| Parameter | Type | Description |
| :---: | :---: | :---:|
| body | email | required |
| body | password | required |

#### Sign-in
It returns a token.
```bash
GET http://localhost:3000/api/sign-in
```
| Parameter | Type | Description |
| :---: | :---: | :---:|
| body | email | required |
| body | password | required |

### Error Handler
It generates a random error message which is handled by ErrorHandler middleware.
```bash
GET http://localhost:3000/api/error
```

AuthAPI micros :- https://web.deta.sh/home/ritam02-cyber/default/micros/AuthAPI<br>
ErrorHandler micros :- https://web.deta.sh/home/ritam02-cyber/default/micros/ErrorHandler<br>
ViewCounter micros :- https://web.deta.sh/home/ritam02-cyber/default/micros/ViewCounter<br>
## Author
-[@Ritam02-cyber](https://github.com/Ritam02-cyber)

# Microservice
#### (Micro-Task 1 and Micro-Task 2)
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

### View Counter
It generates the number of visitors.
```bash
GET http://localhost:3000/api/views
```
<br><br>
AuthAPI micros :- https://web.deta.sh/home/ritam02-cyber/default/micros/AuthAPI<br>
ErrorHandler micros :- https://web.deta.sh/home/ritam02-cyber/default/micros/ErrorHandler<br>
ViewCounter micros :- https://web.deta.sh/home/ritam02-cyber/default/micros/ViewCounter<br>
<br><br>

# GeolocationAPI
#### (Micro-Task 3)<br>
The user's latitude and longitude from the HTML geolocation service is used to develop a location microservice that can use them and provide the address and get latitude and longitude.
<br>
## API Reference
It takes the user's location and returns the address.
```bash
GET https://45gjjg.deta.dev/get-address
```

## Installation
```bash
git clone https://github.com/Ritam02-cyber/GeolocationAPI.git
```
Navigate to :-
```bash
cd GeolocationAPI/
```
Install dependencies using :-
```bash
npm i
```

## Run server
```bash
npm start
```

## Deta server
Link - https://45gjjg.deta.dev/get-address
<br><br>
![Screenshot](https://user-images.githubusercontent.com/62924322/212553909-cbec2ca6-5ce3-4695-b29f-a876f5940bbb.png)


## Author
-[@Ritam02-cyber](https://github.com/Ritam02-cyber)

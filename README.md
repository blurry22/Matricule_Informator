# Sacar Informacion Completa de una Matricula
Very simple script to get all information with just the license plate of the vehicle
Only works for Spain Vehicles


## Requirements
-Node.js (version 14 or higher recommended) [https://nodejs.org/en/download/current]
-Express `npm install express`
-Axios `npm install axios`

## Start the server
-Start the server by running `node main.ts`
-Once you see : "Listening" you can start doing requests

Server = 127.0.0.1:3000
## EndPoints

### GET

- Get Full Information
  `/all/{License_plate}`

  For example : GET http://127.0.0.1:3000/4545JJJ

- Get Model
`/model/{License_plate}`

For example : GET http://127.0.0.1:3000/4545JJJ

- Get VIN
`/vin/{License_plate}`

For example : GET http://127.0.0.1:3000/4545JJJ

-Get Hourse Power
`/power/{License_plate}`

For example : GET http://127.0.0.1:3000/4545JJJ

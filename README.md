# Obtener información completa de la matrícula
Este es un script muy simple para obtener toda la información de un vehículo utilizando solo la matrícula.

Funciona únicamente para vehículos registrados en España.


## Requisitos
-Node.js (se recomienda la versión 14 o superior) [https://nodejs.org/en/download/current]
-Express `npm install express`
-Axios `npm install axios`

## Iniciar el servidor
- Inicia el servidor ejecutando `node main.ts`
- Cuando veas "Listening", puedes comenzar a hacer peticiones

Servidor = 127.0.0.1:3000
## EndPoints

### GET

- Obtener toda la información
  `/{Matricula}`

  Por ejemplo : GET http://127.0.0.1:3000/all/4545JJJ

  
```json
{
  "marca": "Volkswagen",
  "modelo": "Golf",
  "version": "1.6 TDI BlueMotion",
  "Primer_Registro": "2018-05-15",
  "Combustible": "Diesel",
  "Caballos": "110",
  "Automatico_Manual": "Manual",
  "Año_Fabricacion": "2017",
  "VIN": "WVWZZZ1KZPW123456" 
}

```

- Obtener modelo
`/modelo/{Matricula}`

Por ejemplo : GET http://127.0.0.1:3000/model/4545JJJ


```json
{
  "marca": "Volkswagen",
  "modelo": "Golf",
  "version": "1.6 TDI BlueMotion",
}

```

- Obtener VIN
`/vin/{License_plate}`

Por ejemplo : GET http://127.0.0.1:3000/vin/4545JJJ

```json
{
  "VIN": "WVWZZZ1KZPW123456"
}

```


- Obtener Caballos
`/caballos/{Matricula}`

Por ejemplo : GET http://127.0.0.1:3000/power/4545JJJ


```json
{
  "Caballos": "110",
}

```



`Todas las request de ejemplo han sido hechas con una matricula cualquiera al azar (4545JJJ)`

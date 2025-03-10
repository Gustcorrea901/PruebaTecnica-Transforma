Pruebas en Postman

Prueba POST 
requiere todos los campos (menos id por que el incremento es automatico y se asigna solo como lo requeria el problema)
http://localhost:8080/usuarios

{
  "nombre": "Martha prueba3",
  "numeroIdentificacion": "58653453",
  "direccion": "Transversal 85# 6 - 32",
  "telefono": 3235589421,
  "ciudad": "Bogota",
  "estado": false
}

Prueba GET 
http://localhost:8080/usuarios
No requiere ningun parametro para traer toda la información, si se añade algo genera error 


Prueba Put
http://localhost:8080/usuarios/id
http://localhost:8080/usuarios/1   (1 es el id del registro que quiero cambiar)
// se deben agregar todos los campos o genera error

{
  "nombre": "Gustavo prueba4",
  "numeroIdentificacion": "586532483",
  "direccion": "Nueva dirección prueba PUT2",
  "telefono": 3235589421,
  "ciudad": "Bogota",
  "estado": false
}

Prueba Delete
http://localhost:8080/usuarios/id
http://localhost:8080/usuarios/2 

devuelve el codigo 204 No Content lo cual indica que el usuario fue borrado de forma exitosa

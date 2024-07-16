# Foro Hub Challenge
Este proyecto es un foro para tópicos donde se pueden realizar operaciones CRUD.

## Tecnologías utilizadas
- Java
- Spring Boot
- Spring Security
- JWT (JSON Web Token)
- JPA (Java Persistence API)
- Postman (para pruebas de API)
- MySQL (como base de datos)
- Swagger (para documentación de API)

## Funcionamiento
Esta es la vista inicial con Swagger.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/38aa6ea0-84f0-4d30-9a48-e90f4b16c7ee)
![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/b093ba15-ecc6-44b4-b7c3-6d232254a6ef)

Es necesario hacer una autenticación de usuario para poder acceder a los endpoints.<br>
Los usuarios con acceso están guardados en la base de datos.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/7bafbb8f-ef17-4787-985e-9ac1342e637f)

Si el login y la clave ingresados son correctos se devuelve un token.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/b15ce3cb-13be-4ac8-915a-4248d6384999)

Se ingresa el token en la sección de autorización y se le libera el acceso a los endpoints.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/6ddfd6f1-40f6-42a5-bfde-801c0693179a)
![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/8513ed53-d720-4cfc-a94d-51c4b6e012ef)

El primer endpoint muestra los detalles de un solo tópico.<br>
Es necesario ingresar el id del tópico a detallar.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/2d34d415-7019-41ab-acde-5ea74da05282)
![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/c998b704-4e60-42b8-a20a-46e11ecc32f8)

Si el id del tópico no existe, se muestra el siguiente mensae.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/6e4a1d35-5ec2-4b0a-ad84-5118e716f95b)

El segundo endpoint permite actualizar un tópico existente.<br>
Es necesario ingresar el tópico a actualizar y el JSON del tópico.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/9a1f0643-ced3-4f2c-99fd-0c1aeb6cbfcb)

Al actualizar el tópico, se muestran sus detalles.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/68a91d93-6f55-452a-9aa8-549220d6ca6b)

Si ya existe un tópico con el mismo título/mensaje, se muestra el siguiente mensaje.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/b0b5e069-85db-43fe-86af-e96087ef56d1)
![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/c3565964-14c0-4499-b7e8-1d3e9b78a4b5)

El tercer endpoint permite eliminar un tópico existente.<br>
Es necesario ingresar el id del tópico a eliminar.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/89352725-176c-4b73-a3b4-0b85c47abd6f)

Al eliminar un tópico se obtiene el siguiente mensaje.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/86ff42ac-8216-4cab-994a-ad2c849f1224)

Si el id del tópico no existe, se muestra el siguiente mensaje.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/cee6686d-8ecf-4eb8-8987-44aa8cb55970)

El cuarto endpoint muestra una lista de los tópicos existentes ordenados del más al menos recientemente modificado.<br>
Es necesario ingresar el número de página y la cantidad de tópicos que se desea mostrar.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/499045e0-8749-434b-a114-6f9f0a912abf)
![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/0674c5f2-5307-4e5a-9fca-ebfe1f3c2904)

El quinto endpoint permite registrar un nuevo tópico.
Es necesario ingresar el JSON del tópico a registrar.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/1957586d-1b89-43ea-b41f-7aa584152675)

Al registrar el tópico, se muestran sus detalles.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/6a09769e-e9e7-433e-9d7e-f359c0be8837)

Si ya existe un tópico con el mismo título/mensaje, se muestra el siguiente mensaje.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/be5d3cc9-4a81-4028-a58f-51a8362167e2)
![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/437f611b-0ce4-43fc-a9c1-4deddcde1557)

Si alguno de los campos no se ingresa en el JSON, aparece el siguiente mensaje.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/129b4913-6e10-49a8-8174-e78ba7644241)

Si no se ingresa nada o algo que no es un JSON, aparece el siguiente mensaje.

![image](https://github.com/raul-hdz-garcia/foro-hub-challenge/assets/157054531/abcebe75-6f7a-4c5e-8b19-1aa46af7129d)

Las mismas exepciones están disponibles para el endpoint PUT (actualizar un tópico registrado).

Eso es todo. ¡Hasta luego!

# ACT3.-Windows
1. Cambia la velocidad de repetición del teclado a una posición intermedia. Haz una captura.

abrimos el panel de control y buscamos teclado
   
![image](https://github.com/user-attachments/assets/4fa56025-1d2d-4448-ac7a-f2050e04503d)

2. Crea un Documento de texto en el escritorio y ponle tu apellido , en mi caso Lopez.txt utilizando el “Teclado en pantalla”. Haz una captura mostrando el archivo y el “Teclado en pantalla”
   
![image](https://github.com/user-attachments/assets/e0f14bcf-9985-4b3e-ba42-fae7c0b2708a)

3. ¿Qué combinación de teclado y ratón hay que utilizar para crear un acceso directo del archivo anterior?
   
arrastrando el archivo con la tecla alt pulsada
   
![image](https://github.com/user-attachments/assets/79f57b58-7e68-41ff-a64c-24af0fa6645e)

4. Configura Windows para que solo haya que hacer un click para abrir un elemento. Haz una captura.

abrimos opciones del explorador de archivos y elegimos la opcion de un solo click

![image](https://github.com/user-attachments/assets/39328c81-c8bc-4717-be5a-298ad5b9d37f)


5. Configura Windows para que muestre la extensión de todos los archivos. Haz una captura.

Abrimos el explorador de archivos y marcamos la casilla Extensiones de nombre de archivo

![image](https://github.com/user-attachments/assets/7f6b6598-b565-4c3b-9d67-6230da3851a7)


6. Muestra adicionalmente la hora de Fiyi. Haz una captura mostrando los dos relojes.



7. Activa un plan de energía para que el equipo funcione a máximo rendimiento. Haz una captura.

abrimos el panel de control, vamos a opciones de energia y seleccionamos la casilla alto rendimiento

![image](https://github.com/user-attachments/assets/de86b7ca-b1cc-47e0-b5eb-09cc20ed93fb)


8. Ajusta el tamaño del texto de Windows al 115%. Haz una captura.

configuracion,sistema,pantalla seleccionas configuracion avanzada de escala y pones 115

![image](https://github.com/user-attachments/assets/ab83c3d7-5209-432b-9252-7c6dd57d098f)


9. Activa la opción para que al crear una nueva cuenta la contraseña cumpla con los siguientes requisitos:

· No contener el nombre de cuenta del usuario o partes del nombre completo del usuario en más de dos caracteres consecutivos

· Tener una longitud mínima de seis caracteres

· Incluir caracteres de tres de las siguientes categorías:

o Mayúsculas (de la A a la Z)

o Minúsculas (de la a a la z)

o Dígitos de base 10 (del 0 al 9)

o Caracteres no alfanuméricos (por ejemplo, !, $, #, %)

Haz una captura.

10. Desactiva el poder acceder al “cmd” de Windows. Haz una captura

Abrimos Editor de directivas local vamos a configuracion de usuario,Sistema,Impedir el acceso al simbolo del sistema

![image](https://github.com/user-attachments/assets/b1801c7f-8090-452a-9f4c-ccbac1aee305)

11. Habilita Windows para que pueda recibir y establecer conexiones remotas. Haz una captura

Vamos a configuracion,sistema y a Escritorio remoto y activamos la opcion (no sale nada porque estoy usando el windows de mi ordenador)

![image](https://github.com/user-attachments/assets/4712609b-94be-4b94-acd3-e392ba9da849)

12. ¿Qué comando hay que utilizar para forzar la actualización de la configuración de la directiva de grupo?
   
tienes que poner gpupdate /force  en el cmd

13. ¿Qué comando sirve ejecutar la aplicación “Conexión a escritorio remoto”? Haz una captura.

presionamos Windows+R y escribimos mstsc

![image](https://github.com/user-attachments/assets/00cb4352-6660-4f9d-8d0a-861affb5f997)

14. Cambia el nombre de equipo a Equipode+Tunombre en mi caso, EquipodeAlexandre. Haz una captura.

abre cmd y escribe WMIC computersystem where name="%computername%" call rename name="GeorgiGeorgiev"

![image](https://github.com/user-attachments/assets/f0746b41-25fc-42d7-acb6-fdcc2fcdc48e)

15. Crea un nuevo grupo denominado 2FPB. Haz una captura.

abre cmd y pon net localgroup 2FPB /add

![image](https://github.com/user-attachments/assets/5b98c4eb-7bb2-4c39-8550-e5af26845442)

16. Crea un usuario utilizado la primera inicial de tu nombre+tu apellido, en mi caso alopez. Haz que ese usuario forme parte del grupo 2FPB y del grupo administradores. ¿Qué opción hay que habilitar para que haya que cambiar la contraseña una que un usuario nuevo inicie sesión en Windows por primera vez? Haz capturas donde se vea todo lo que pide.

net user ggeorgiev Contraseña123 /add
net localgroup 2FPB ggeorgiev /add
net localgroup Administradores ggeorgiev /add
wmic useraccount where name='ggeorgiev' set PasswordExpires=True

![image](https://github.com/user-attachments/assets/5b5ece8a-5dc5-4a42-8b72-202ea37db988)

17. Crea una carpeta en el escritorio en el Escritorio denominada carpetade+Tunombre, en mi caso “CarpetadeAlexandre”. Dentro de la carpeta crea un archivo .txt denominado archivode+Tunombre en mi caso archivodeAlexandre.txt. Comparte esta carpeta. Sólo tienen que tener acceso de escritura los usuarios del grupo 2FPB. Haz una captura de pantalla.

![image](https://github.com/user-attachments/assets/40cd1c4b-0368-41d1-a735-cc8ce75f18d5)


18. Crea una unidad de red utilizando la carpeta creada en el punto anterior. Haz una captura.

![image](https://github.com/user-attachments/assets/52b43c9b-3c12-4754-af1c-ecc890471daa)

19. Crea una Tarea programada para qué el equipo se apague a las 15:30 del dia 10 de febrero de 2035. Haz una captura donde se vea claramente la hora del sistema y la hora de cuando se apagará la máquina.

Abrimos el programador de tareas ponemos nombre a la tarea luego ponemos la fecha y la hora luego configuramos la accion como “iniciar un programa“ y en programa o script escribimos ”shutdown” y ”/s /f /t 0” en agregar argumentos para quitar cualquier restriccion

![image](https://github.com/user-attachments/assets/4d9f5d99-fe4e-4e81-b1df-2b44ef17fc1c)

![image](https://github.com/user-attachments/assets/d1ffa347-4304-4225-9366-852f6da51ede)

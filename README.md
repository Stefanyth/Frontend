# Frontend


 
 Frontend.
Este código define un componente de Angular para un formulario de inicio de sesión. Component: Importa la clase Component para definir el componente.
CommonModule: Importa el módulo CommonModule que proporciona directivas comunes de Angular.
FormsModule: Importa el módulo FormsModule para trabajar con formularios.
Router: Importa el servicio Router para la navegación.
AuthService: Importa el servicio AuthService para manejar la autenticación.
selector: Define el selector del componente (<app-login>).
standalone: Indica que el componente es independiente.
imports: Especifica los módulos que el componente necesita (CommonModule y FormsModule). templateUrl: La ruta al archivo HTML del componente.
styleUrls: La ruta al archivo CSS del componente.
form: Un objeto que almacena los valores del formulario (email y password). constructor: Inicializa el componente e inyecta el Router y AuthService.
validateEmail: Valida el formato del correo electrónico utilizando una expresión regular. validatePassword: Verifica que la contraseña tenga al menos 6 caracteres.
    ![login component](https://github.com/user-attachments/assets/d68616da-c6ea-4191-b2e5-e5a36bb8337d)

 onSubmit: Maneja el evento de envío del formulario:
Previene el comportamiento por defecto del formulario.
Valida el correo electrónico y la contraseña.
Si las validaciones pasan, llama al método login del AuthService.
Maneja la respuesta de la autenticación: redirige a /menu si es exitosa o muestra un error si falla.
navigateToRegister: Maneja la navegación al formulario de registro: Previene el comportamiento por defecto del evento.
Navega a la ruta /register.
  ![login component2](https://github.com/user-attachments/assets/485fbf58-9ef5-4943-a6fa-7d4479a67309)

 Codigo html de la vista.
Component: Importa la clase Component para definir el componente.
CommonModule: Importa el módulo CommonModule que proporciona directivas comunes de Angular.
RouterModule: Importa el módulo RouterModule para manejar la navegación dentro del componente.
selector: Define el selector del componente (<app-menu>).
standalone: Indica que el componente es independiente.
imports: Especifica los módulos que el componente necesita (CommonModule y RouterModule).
templateUrl: La ruta al archivo HTML del componente.
styleUrls: La ruta al archivo CSS del componente.
   ![menu component](https://github.com/user-attachments/assets/3835d1ce-ad02-4eed-8c91-3dc558ff5ed5)

 Propiedades:
isUserMenuOpen: Almacena el estado del menú de usuario (abierto o cerrado). isEventMenuOpen: Almacena el estado del menú de eventos (abierto o cerrado).
isMenuOpen: Almacena el estado general del menú (abierto o cerrado).
Métodos:
toggleUserMenu: Alterna el estado de isUserMenuOpen entre true y false, abriendo o cerrando el menú de usuario.
toggleEventMenu: Alterna el estado de isEventMenuOpen entre true y false, abriendo o cerrando el menú de eventos.
toggleMenu: Alterna el estado de isMenuOpen entre true y false, abriendo o cerrando el menú general.
Vista del menu.
  
 Component: Importa la clase Component para definir el componente.CommonModule: Importa el módulo CommonModule para usar directivas comunes de Angular.FormsModule: Importa el módulo FormsModule para trabajar con formularios.Router: Importa el servicio Router para la navegación.AuthService: Importa el servicio AuthService para manejar la lógica de autenticación y actualización de usuarios.
form: Un objeto que almacena los valores del formulario (name y email). constructor: Inicializa el componente e inyecta los servicios Router y AuthService.
onSubmit: Maneja el evento de envío del formulario:
Obtiene el userId del localStorage.
Verifica que userId no sea nulo.
Llama al método updateUser del AuthService pasando el userId y los datos del formulario. Maneja la respuesta de la actualización:
Si es exitosa, muestra un mensaje de éxito y redirige al menú. Si hay un error, muestra un mensaje de error apropiado.
    ![menu component2](https://github.com/user-attachments/assets/de54172d-ab9e-402b-a902-e9fb6aa7cf19)

 Vista modificar usuario.
Component: Importa la clase Component para definir el componente.
CommonModule: Importa el módulo CommonModule para usar directivas comunes de Angular. FormsModule: Importa el módulo FormsModule para trabajar con formularios.
Router: Importa el servicio Router para la navegación.
AuthService: Importa el servicio AuthService para manejar la lógica de autenticación y registro de usuarios.
form: Un objeto que almacena los valores del formulario (username, email, password y confirmPassword).
constructor: Inicializa el componente e inyecta los servicios Router y AuthService.
   
 validateEmail: Verifica que el correo electrónico tenga un formato válido.
validatePassword: Verifica que la contraseña tenga al menos 6 caracteres.
validateForm: Realiza todas las validaciones del formulario y muestra alertas si alguna de ellas falla.
onSubmit: Maneja el evento de envío del formulario:
Previene el comportamiento predeterminado del formulario. Verifica si el formulario es válido.
Crea un objeto user con los datos del formulario.
Llama al método register del AuthService para registrar al usuario. Maneja la respuesta del registro:
Si es exitosa, muestra un mensaje de éxito y redirige al login.
Si hay un error, muestra un mensaje de error.
  
![editar component](https://github.com/user-attachments/assets/817bfff6-6a45-4139-a0e0-12260f45b2a4)
![editar component2](https://github.com/user-attachments/assets/bf7eb0ac-2f2c-45c5-8eb8-ee82a0c233a6)
  


Al final de todo el proyecto queda de esta manera 

Crear producto
![crear producto](https://github.com/user-attachments/assets/a27b97e6-e75e-4f4e-9744-8a0c21dc66f8)


editar producto

![editar producto](https://github.com/user-attachments/assets/f178dfef-6754-4454-9728-3c7abfb70358)


lista de usuarios

![lista de usuarios](https://github.com/user-attachments/assets/39abd684-2536-4d96-a1ce-b8a246927d85)

lista de productos
![listadeproductos](https://github.com/user-attachments/assets/636e0adf-6bc5-4675-b3eb-f6f6f703888a)


login
![login](https://github.com/user-attachments/assets/63a42ecf-3257-4921-be51-4cbcdd14a812)


menu
![menu](https://github.com/user-attachments/assets/3cb41274-4373-4f13-b7cf-1ed7ea3c8f1c)


modificar usuario

![modificarUsuario](https://github.com/user-attachments/assets/bb69644f-83c7-4bbf-8d2d-a87323eba5d9)

registrarse

![registrarse](https://github.com/user-attachments/assets/e6f89255-b725-46d8-9c72-59b3b2cc8494)

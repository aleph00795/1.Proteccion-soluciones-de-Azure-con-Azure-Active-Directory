https://learn.microsoft.com/es-es/training/modules/azure-active-directory/?WT.mc_id=cloudskillschallenge_38B9BB2D-F0E1-4B09-9159-0C5E9353EC85&ns-enrollment-type=Collection&ns-enrollment-id=gm3rbgd2jnw1

## Tarea1: Revision de AzureAD

En esta tarea, revisaremos las licencias y los inquilinos de Azure Active Directory.

En el Portal, busque Azure Active Directory y selecciónelo.
En la página Información general, busque la información de la licencia.

![image](https://user-images.githubusercontent.com/110675810/188756328-aaa806ab-9c29-4df4-a4c3-3006cc60cf88.png)

Vaya a la página de precios de Azure AD y revise las características y los precios de cada edición.

https://azure.microsoft.com/es-es/pricing/details/active-directory/

![image](https://user-images.githubusercontent.com/110675810/188715759-38995241-f767-4200-828a-33d6d16308d1.png)

## Tarea 2: Administración de usuarios y grupos

Nota: Esta tarea requiere que se rellenen algunos usuarios y grupos. Los grupos dinámicos requieren una licencia Premium P1.

En esta tarea, crearemos usuarios y grupos.

1. En la hoja Administrar, haga clic en Usuarios.
2. Revise los distintos Orígenes como Windows Server AD, Usuario invitado, Cuenta Microsoft y Azure Active Directory externo.
3. Observe la opción para Nuevo usuario invitado.
4. Haga clic en Nuevo usuario.
5. Revise las dos maneras de crear un usuario: Crear usuario e Invitar usuario.
![image](https://user-images.githubusercontent.com/110675810/188757614-86ea3860-7511-49ac-aeea-a0ebd505e458.png)

6. Cree un nuevo usuario. Revise Identidad, Grupos y roles, Configuración e Información del trabajo.
![image](https://user-images.githubusercontent.com/110675810/188757932-28ccdf5e-8dad-4b08-aeb2-48e9407453b5.png)

![image](https://user-images.githubusercontent.com/110675810/188758006-b926c1b4-dc91-4c75-b667-02ffadaa2c01.png)

7. Al volver a Azure AD, en Administrar, haga clic en Grupos.
8. Revise los Tipos de grupos: Seguridad y Microsoft 365.
![image](https://user-images.githubusercontent.com/110675810/188758749-6a1c8615-bccb-4f6c-9b52-ea58d7ce0d7d.png)

9. Cree un grupo haciendo clic en "Nuevo grupo" con el Tipo de pertenencia establecido en Asignado.
10. Agregue un usuario al mismo grupo.
![image](https://user-images.githubusercontent.com/110675810/188758397-511726a3-dc3c-4a43-bc8f-47c0f2182020.png)

![image](https://user-images.githubusercontent.com/110675810/188758514-12a31703-50ad-42a9-9e7e-18fe5d528bed.png)

11. Cree otro grupo con el Tipo de pertenencia como Usuario dinámico.
![image](https://user-images.githubusercontent.com/110675810/188759161-99ae2b46-5322-49aa-a9e6-0a3d3a079f76.png)

12. Revise los detalles para crear reglas de pertenencia dinámica a grupos.
![image](https://user-images.githubusercontent.com/110675810/188759961-0bfbd365-b950-43d7-828e-ef17a270f4ec.png)
![image](https://user-images.githubusercontent.com/110675810/188760014-78412954-a73a-4ea4-ad6c-415a4d47eb61.png)
![image](https://user-images.githubusercontent.com/110675810/188760058-37bfc9c9-43ee-4ae7-8bcd-6a40c3282446.png)

## Tarea 3: Autenticacion multifactor en Azure

Nota: Esta tarea requiere una cuenta de usuario, AZ500User1.

![image](https://user-images.githubusercontent.com/110675810/188760605-bad082d1-a4b2-4d1f-8620-4e0eaf98e6c9.png)

En esta demostración, configuraremos y probaremos MFA.

### CONFIGURACION DE MFA

En esta tarea, habilitaremos MFA para un usuario.

1. En el Portal, busque Azure Active Directory y selecciónelo.
2. En Administrar, seleccione Seguridad.
3. En Administrar, seleccione MFA.
4. En el panel del centro, en Configurar, seleccione Configuración adicional de MFA basado en la nube.

![image](https://user-images.githubusercontent.com/110675810/188755424-1e3ff379-c285-4fb3-ae71-65ce7931bc96.png)

5. Seleccione la pestaña Usuarios.

![image](https://user-images.githubusercontent.com/110675810/188762804-3516330f-67ff-41a5-985e-dd227036a42a.png)

6. Seleccione AZ500User1. Anote su nombre de usuario con el formato user@domain.com.
7. En el extremo derecho, haga clic en Habilitar.

![image](https://user-images.githubusercontent.com/110675810/188763013-e656d3e4-cc50-436c-a7c5-2bc989bd3c2a.png)

8. Lea la información sobre cómo habilitar la autenticación multifactor en Azure.

https://docs.microsoft.com/es-es/azure/active-directory/authentication/howto-mfa-getstarted

9. Haga clic en habilitar autenticación multifactor.

![image](https://user-images.githubusercontent.com/110675810/188763248-aa092a2d-b0d3-4219-9e49-4a5b22e39c19.png)

10. Espere a la actualización. AZ500User1 deberá ahora proporcionar una autenticación de dos factores.

### PRUEBA DE FMA
Nota: Para probar MFA, se requiere un número de teléfono.

En esta tarea, probaremos el requisito de MFA.

1. Inicie sesión en Portal como AZ500User1. Use su nombre de usuario del paso anterior.

![image](https://user-images.githubusercontent.com/110675810/188764064-5892ffaf-4a6f-4e8a-ae6f-a3a50ba69e25.png)

![image](https://user-images.githubusercontent.com/110675810/188764126-69e93edc-e911-49c7-9436-9a3c45015969.png)

2. Proporcione la contraseña y haga clic en Siguiente.
3. Tenga en cuenta que se requiere más información. Haga clic en Siguiente.
5. Revise la página de verificación Seguridad adicional.
6. En el paso 1, escriba su número de teléfono y asegúrese de que la opción Enviarme un código en un mensaje de texto está activa.
7. Haga clic en Siguiente.

![image](https://user-images.githubusercontent.com/110675810/188764285-9ba0ee57-0af0-4f43-8ffc-bb8513e57380.png)

8. En el paso 2, escriba el código de verificación del mensaje de texto.

![image](https://user-images.githubusercontent.com/110675810/188764397-097fc7ac-2d85-4401-b77d-a556a80a773f.png)

9. Haga clic en Comprobar.

![image](https://user-images.githubusercontent.com/110675810/188764499-cabe2e91-823c-46dc-9ec6-65a87bbab199.png)

![image](https://user-images.githubusercontent.com/110675810/188765379-6ebfec9c-8d89-41be-a1dc-e4225b0b1a12.png)

10. En el paso 3, lea sobre cómo mantener las aplicaciones existentes en funcionamiento.
11. Haga clic en Empiece con esta contraseña de la aplicación.
12. Si se le solicita, haga clic en Permitir acceso.
13. Haga clic en Done(Listo).
14. En la pantalla Actualizar contraseña, proporcione y confirme una nueva contraseña.
15. Haga clic en Iniciar sesión.
16. Confirme que ahora puede acceder al portal.

![image](https://user-images.githubusercontent.com/110675810/191128411-badd1fa8-f7e3-4749-a95b-997e46d696a5.png)

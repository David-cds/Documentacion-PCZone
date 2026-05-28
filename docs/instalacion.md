# ⚙️ Guía de Instalación y Despliegue Local

Para ejecutar y testear el proyecto **PCZone** en un entorno de desarrollo local, siga los pasos que se detallan a continuación.

## 📋 Requisitos Previos

Antes de comenzar, asegúrese de tener instalado en su equipo:
* Un servidor local compatible con PHP (se recomienda **XAMPP**, Laragon o Wampserver).
* Versión de **PHP 8.x** o superior.
* Gestor de bases de datos **MySQL / MariaDB** (incluido en XAMPP a través de phpMyAdmin).

---

## 🛠️ Pasos para la Configuración

### 1. Clonar o copiar el proyecto
Mueva o clone la carpeta completa del proyecto `pczone` dentro del directorio raíz de su servidor web local:
* En **XAMPP**: `C:\xampp\htdocs\`
* En **Laragon**: `C:\laragon\www\`

### 2. Importar la Base de Datos
1. Inicie los módulos de **Apache** y **MySQL** desde el panel de control de su servidor local.
2. Abra su navegador web e ingrese a `http://localhost/phpmyadmin/`.
3. Cree una nueva base de datos haciendo clic en "Nueva" y asígnele el nombre `pczone`.
4. Seleccione la base de datos recién creada, diríjase a la pestaña **Importar**, seleccione el archivo `.sql` ubicado en la raíz del proyecto y haga clic en **Importar** (o Continuar).

### 3. Configuración de la Conexión en PHP
El proyecto incluye un script de conexión que gestiona el acceso a la base de datos. Asegúrese de que las credenciales coincidan con su configuración local. Por defecto, los parámetros configurados son:

* **Servidor:** `localhost`
* **Usuario:** `root`
* **Contraseña:** `""` (vacío en XAMPP)
* **Base de Datos:** `pczone`

### 4. Ejecución de la Aplicación
Una vez completados los pasos anteriores, abra su navegador web y acceda a la siguiente URL para interactuar con el sistema:
```text
http://localhost/pczone/

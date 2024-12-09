Instalación
Sigue estos pasos para instalar el proyecto:

Clonar el repositorio:

bash
Copiar código
git clone https://github.com/usuario/mydrive.git
cd mydrive
Configurar el entorno del backend (Python):

bash
Copiar código
cd Back
python3 -m venv entornop
source entornop/bin/activate
pip install -r requirements.txt
Configurar el frontend (PHP):

Mueve la carpeta del proyecto al directorio de Apache:
bash
Copiar código
cp -r grafiles_mia /opt/lampp/htdocs/
Asegúrate de que Apache esté corriendo.
Configurar la base de datos:

Configura la conexión con MySQL y MongoDB utilizando la siguiente URI:
mongodb://pr2mia2024:1234@localhost:27017/proyecto2Mia?authSource=admin.
Iniciar el contenedor Docker:

bash
Copiar código
docker-compose up
Uso
Inicia Apache desde XAMPP o usando el comando:

bash
Copiar código
sudo /opt/lampp/lampp start
Accede a la aplicación en tu navegador:
http://localhost/grafiles_mia

Utiliza las credenciales predeterminadas para ingresar:

Administrador:
Usuario: admin
Contraseña: admin123
Usuario común:
Usuario: usuario
Contraseña: usuario123
Requisitos
Sistema operativo: Ubuntu (se recomienda la extensión "Windows List").
PHP: 8.3.11 o superior.
Python: 3.8+ con entorno virtual configurado.
Docker: Instalado y configurado.
Base de datos: MySQL y MongoDB.
Servidor web: Apache (XAMPP).

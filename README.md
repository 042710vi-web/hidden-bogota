# Hidden Bogotá

Aplicación web para conectar turistas con comercios locales de Bogotá. El proyecto usa React y Vite en el cliente, Node.js y Express en el servidor, y MySQL para almacenar la información.

## Requisitos

- Node.js 18 o superior
- MySQL
- npm

## Instalación local

1. Crea la base de datos ejecutando `database/hiddenbogota.sql` en MySQL Workbench. **Ese script recrea la base de datos; no lo ejecutes sobre una base que contenga información que quieras conservar.**
2. En la carpeta `server`, copia `.env.example` a `.env` y configura tus propios valores.
3. En una terminal:

   ```powershell
   cd server
   npm install
   npm start
   ```

4. En otra terminal:

   ```powershell
   cd client
   npm install
   npm run dev
   ```

5. Abre http://localhost:5173.

## Funciones

- Registro e inicio de sesión para turistas y comercios.
- Exploración de comercios, favoritos, reseñas y perfiles.
- Panel para que cada comercio administre su perfil y galería.
- Área administrativa para revisar publicaciones.
- Páginas de costos, privacidad, tratamiento de datos, respaldo, cookies y créditos.
- Plan destacado de $80.000 COP mensuales.
- La pantalla actual de tarjeta valida la marca y muestra confirmación de demostración; **no procesa ni recibe dinero real**.

## Variables de entorno

Usa `server/.env.example` como guía y crea `server/.env` localmente. Los archivos `.env`, las dependencias instaladas, el build y las imágenes cargadas en `server/uploads` se excluyen de Git.

Para usar una pasarela de pagos real se requiere una integración activa, credenciales válidas del titular de la cuenta y verificación del estado del pago en el servidor. No publiques claves ni datos de tarjetas.

## Compilar el cliente

```powershell
cd client
npm run build
```

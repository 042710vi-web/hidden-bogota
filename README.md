# Hidden Bogotá

Aplicación web para conectar turistas con comercios locales de Bogotá. Está construida con React, Vite, Node.js, Express y MySQL.

## Requisitos

- Node.js 18 o superior
- MySQL
- npm

## Instalación local

1. Ejecuta database/hiddenbogota.sql en MySQL Workbench para crear la base hiddenbogota. El script recrea la base de datos; no lo ejecutes si ya tienes información que quieras conservar.
2. En server, copia .env.example a .env y completa la configuración local.
3. En una terminal, ejecuta:
   cd server
   npm install
   npm start
4. En otra terminal, ejecuta:
   cd client
   npm install
   npm run dev
5. Abre http://localhost:5173.

## Funcionalidades

- Registro e inicio de sesión para turistas y comercios.
- Exploración de perfiles, favoritos y reseñas.
- Panel de comercios y revisión administrativa.
- Plan destacado de $80.000 COP mensuales.
- Formulario de tarjeta que reconoce marcas y muestra un resultado de demostración.

## Pagos

La pantalla de tarjeta incluida en esta entrega es una demostración de interfaz: no valida fondos, no confirma que la tarjeta exista y no realiza cobros. No ingreses datos reales de tarjetas. Para recibir dinero se necesita integrar y verificar una pasarela de pagos real en el servidor.

## Seguridad

El archivo server/.env contiene configuración privada y no se debe subir a GitHub. El repositorio incluye server/.env.example con valores de muestra. Las dependencias instaladas, carpetas de compilación y archivos cargados por usuarios se excluyen del repositorio.

## Compilar el cliente

En client ejecuta:
npm run build


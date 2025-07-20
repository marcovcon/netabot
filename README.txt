
# Netabot - Configuración de Despliegue

Este paquete incluye los archivos esenciales para desplegar Netabot:

## Archivos incluidos:
- vercel.json → Configuración para frontend en Vercel (Next.js)
- render.yaml → Configuración para backend en Render (FastAPI)
- .env.example → Variables de entorno necesarias
- README.txt → Esta guía

## 🟢 Frontend (Vercel)
1. Sube tu frontend de Next.js a GitHub
2. Importa el repo en Vercel y usa el archivo vercel.json
3. Conecta el subdominio 'chat.netabot.com'
4. Agrega el CNAME en tu dominio (Neubox) hacia Vercel

## 🔵 Backend (Render)
1. Sube tu backend de FastAPI a GitHub
2. Crea un nuevo Web Service en Render
3. Usa el render.yaml para configurar automáticamente
4. Llena tu archivo .env con las variables correctas

## 🌐 DNS en Neubox
- Dominio principal: apuntar nameservers a Hostinger
- Subdominio chat.netabot.com: CNAME → cname.vercel-dns.com

Listo. Tu sistema quedará en producción.

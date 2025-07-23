# Colegio Liahona - Sitio Web

Sitio web oficial del Colegio Liahona con sus 4 sedes en Chile.

## 🚀 Tecnologías

- HTML5/CSS3/JavaScript
- Netlify (Hosting)
- Decap CMS (Content Management)
- GitHub (Version Control)

## 📍 Sedes

1. **Gran Avenida (El Bosque)**
   - Dirección: Gran Av. José Miguel Carrera 9598, El Bosque
   - Teléfono: 232782740
   - Email: colegio@colegioliahona.cl

2. **Pucón**
   - Dirección: Cam. Internacional 1525, Pucón
   - Teléfono: 45 2378 980
   - Email: pucon@colegioliahona.cl

3. **El Belloto (Quilpué)**
   - Dirección: Pedro de Valdivia 115, Quilpué
   - Teléfono: 32 2296 826
   - Email: belloto@colegioliahona.cl

4. **La Florida**
   - Dirección: Sta. Amalia 285, La Florida
   - Teléfono: 232782730
   - Email: florida@colegioliahona.cl

## 🛠️ Instalación y Desarrollo Local

### Prerrequisitos
- Git
- Un navegador web moderno

### Pasos para desarrollo local

1. Clonar el repositorio:
```bash
git clone https://github.com/fercastillo/liahona-web.git
cd liahona-web
```

2. Para desarrollo local con Decap CMS:
```bash
# Instalar Decap CMS localmente (opcional)
npm install -g decap-server

# Ejecutar el servidor local
decap-server
```

3. Abrir el sitio en un servidor local:
```bash
# Con Python 3
python -m http.server 8000

# O con Node.js
npx http-server
```

4. Visitar `http://localhost:8000` en tu navegador

## 📝 Administración de Contenido

El sitio utiliza Decap CMS para la gestión de contenido. Para acceder al panel de administración:

1. Navegar a `/admin` en el sitio desplegado
2. Autenticarse con Netlify Identity
3. Gestionar contenido desde la interfaz visual

### Colecciones disponibles:
- **Configuración**: Ajustes generales del sitio
- **Sedes**: Información de cada campus
- **Noticias**: Publicaciones y anuncios
- **Eventos**: Calendario de actividades
- **Equipo**: Personal docente y administrativo

## 🚀 Deploy en Netlify

### Deploy automático desde GitHub

1. Conectar tu cuenta de GitHub con Netlify
2. Crear nuevo sitio desde Git
3. Seleccionar el repositorio `liahona-web`
4. Configuración de build:
   - Build command: (dejar vacío)
   - Publish directory: `.`
5. Deploy!

### Configuración post-deploy

1. **Habilitar Netlify Identity**:
   - Ir a Site settings → Identity
   - Enable Identity service
   - Configurar Registration preferences
   - Enable Git Gateway

2. **Configurar dominio personalizado** (opcional):
   - Site settings → Domain management
   - Add custom domain

3. **Invitar usuarios del CMS**:
   - Identity → Invite users
   - Los usuarios recibirán un email de invitación

## 🔧 Configuración adicional

### Variables de entorno
No se requieren variables de entorno para el funcionamiento básico.

### Webhooks
Netlify automáticamente reconstruye el sitio cuando hay cambios en GitHub.

### Formularios
Los formularios de contacto utilizan Netlify Forms. No requieren configuración adicional.

## 📁 Estructura del proyecto

```
liahona-web/
├── admin/              # Panel de administración CMS
│   ├── index.html     # Entrada del CMS
│   └── config.yml     # Configuración del CMS
├── css/               # Hojas de estilo
├── js/                # Scripts JavaScript
├── fonts/             # Fuentes tipográficas
├── images/            # Imágenes del sitio
├── upload/            # Contenido multimedia
├── plugins/           # Plugins adicionales
├── index.html         # Página principal
├── netlify.toml       # Configuración de Netlify
├── README.md          # Este archivo
└── .gitignore         # Archivos ignorados por Git
```

## 🤝 Contribuir

1. Fork el proyecto
2. Crear una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abrir un Pull Request

## 📞 Soporte

Para soporte técnico relacionado con el sitio web, contactar al administrador del sistema.

## 📄 Licencia

© 2025 Colegio Liahona. Todos los derechos reservados.
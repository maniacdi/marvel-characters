# 🦸 Marvel Explorer

Aplicación interactiva para explorar el universo Marvel utilizando la API oficial de Marvel. Busca personajes, comics, series y eventos del universo cinematográfico y de cómics de Marvel.

## 📋 Descripción

Marvel Explorer es un proyecto que integra la Marvel API oficial para proporcionar una experiencia de exploración del extenso catálogo de Marvel. Implementa búsqueda, filtrado y visualización de personajes, cómics y series con una interfaz moderna.

## ✨ Características

- 🦸 Búsqueda de personajes de Marvel
- 📚 Exploración de cómics y series
- 🔍 Filtros avanzados por categorías
- 📊 Visualización de estadísticas
- 🎨 Interfaz responsive y moderna
- ⚡ Sistema de caché optimizado

## 🛠️ Tecnologías

- **Framework:** React/Next.js (o tu stack actual)
- **Lenguaje:** TypeScript
- **API:** Marvel API
- **Styling:** CSS/SCSS
- **HTTP Client:** Axios/Fetch

## 🚀 Instalación

```bash
# Clonar el repositorio
git clone https://github.com/maniacdi/marvel-explorer.git

# Instalar dependencias
npm install

# Configurar API Key de Marvel
cp .env.example .env
# Editar .env y agregar tu Marvel API Key
```

### 🔑 Obtener Marvel API Key

1. Regístrate en [Marvel Developer Portal](https://developer.marvel.com/)
2. Crea una aplicación
3. Copia tu Public Key y Private Key
4. Agrégalas a tu archivo `.env`:

```env
MARVEL_PUBLIC_KEY=tu_public_key_aqui
MARVEL_PRIVATE_KEY=tu_private_key_aqui
```

```bash
# Ejecutar en modo desarrollo
npm run dev
```

## 📡 Funcionalidades

### Búsqueda de Personajes
```typescript
// Ejemplo de uso
searchCharacter("Spider-Man")
  .then(character => console.log(character));
```

### Explorar Cómics
- Filtrar por serie
- Ordenar por fecha de publicación
- Ver detalles completos

### Exploración de Series
- Timeline de eventos
- Información de creadores
- Covers y artwork

## 📂 Estructura

```
marvel-explorer/
├── src/
│   ├── components/     # Componentes React
│   ├── services/       # Integración con Marvel API
│   ├── hooks/          # Custom hooks
│   ├── utils/          # Utilidades y helpers
│   └── types/          # Tipos TypeScript
├── public/             # Assets estáticos
└── .env.example        # Template de variables de entorno
```

## 🎯 Endpoints Implementados

- `/characters` - Listado de personajes
- `/characters/:id` - Detalle de personaje
- `/comics` - Exploración de cómics
- `/series` - Series de Marvel
- `/events` - Eventos del universo Marvel

## 🖼️ Capturas

*(Agrega aquí capturas de tu aplicación cuando las tengas)*

## 🔐 Autenticación Marvel API

La Marvel API requiere autenticación mediante:
- Public Key
- Private Key
- Timestamp
- Hash MD5

Este proyecto maneja automáticamente la autenticación en cada petición.

## 📊 Límites de la API

- 3000 peticiones por día
- Rate limit: 100 peticiones por minuto
- Sistema de caché implementado para optimizar consumo

## 🚧 Roadmap

- [ ] Sistema de favoritos persistente
- [ ] Comparador de personajes
- [ ] Quiz interactivo
- [ ] Integración con Marvel Cinematic Universe timeline
- [ ] Modo oscuro

## 🐛 Problemas Conocidos

- La Marvel API puede tener delays ocasionales
- Algunas imágenes pueden no estar disponibles
- Ciertos personajes antiguos tienen información limitada

## 👤 Autor

**Javier García Magaldi**
- GitHub: [@maniacdi](https://github.com/maniacdi)
- Portfolio: [magaldidev.com](https://magaldidev.com)

## 📄 Licencia

Este proyecto es de código abierto y está disponible bajo la licencia MIT.

## 🙏 Agradecimientos

- [Marvel API](https://developer.marvel.com/) por proporcionar acceso a su base de datos
- Comunidad de desarrolladores de Marvel

---

**Nota:** Este proyecto usa la Marvel API oficial. Data provided by Marvel. © 2024 MARVEL

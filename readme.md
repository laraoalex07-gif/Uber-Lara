# Multi Servicios LARA - Sistema de Gestión

Sistema completo de gestión para servicios de transporte privado con funcionalidades PWA.

## 🚀 Características Nuevas

### ✅ Mejoras Implementadas

1. **Codificación UTF-8 Correcta**
   - Todos los emojis funcionan correctamente
   - Caracteres especiales en español sin problemas

2. **Indicadores de Carga**
   - Loader animado durante operaciones largas
   - Feedback visual al guardar/cargar datos
   - Mejor experiencia de usuario

3. **Validación Mejorada en Importación**
   - Verifica estructura del archivo JSON
   - Valida campos requeridos
   - Filtra registros inválidos
   - Mensajes de error descriptivos

4. **Gráficos de Estadísticas**
   - Gráfico de barras de últimos 6 meses
   - Comparación visual de ingresos vs gastos
   - Tooltips informativos

5. **Búsqueda en Tiempo Real**
   - Campo de búsqueda instantánea en registros
   - Busca en categorías, detalles y montos
   - Combinable con filtros de fecha

6. **PWA Completa**
   - Instalable en dispositivos móviles
   - Funciona offline
   - Atajos de aplicación
   - Icono personalizado

7. **Botón Borrar Arreglado**
   - Modal de confirmación funcional
   - No se queda trabado
   - Actualiza vistas automáticamente

## 📁 Estructura de Archivos

```
proyecto/
├── index.html          # Aplicación principal
├── manifest.json       # Configuración PWA
├── sw.js              # Service Worker
├── aa.jpg             # Logo de la app
└── README.md          # Este archivo
```

## 🌐 Despliegue en GitHub Pages

### Opción 1: Con GitHub Desktop

1. Crea un nuevo repositorio en GitHub
2. Arrastra todos los archivos a la carpeta del repositorio
3. Haz commit con mensaje: "Initial commit - LARA App"
4. Push a GitHub
5. Ve a Settings → Pages
6. Selecciona branch `main` y carpeta `/ (root)`
7. Guarda y espera 1-2 minutos
8. Tu app estará en: `https://tuusuario.github.io/nombre-repo/`

### Opción 2: Desde la Web de GitHub

1. Crea un nuevo repositorio
2. Arrastra los archivos directamente al navegador
3. Haz commit
4. Activa GitHub Pages en Settings
5. ¡Listo!

## 📱 Convertir a App con WebIntoApp

### Método Rápido

1. Descarga WebIntoApp desde:
   - Google Play Store (Android)
   - App Store (iOS)

2. Abre WebIntoApp y crea nueva app:
   - URL: `https://tuusuario.github.io/nombre-repo/`
   - Nombre: "Multi Servicios LARA"
   - Icono: Sube `aa.jpg`

3. Configura opciones:
   - ✅ Habilitar modo offline
   - ✅ Ocultar barra de direcciones
   - ✅ Permitir descargas
   - ✅ Guardar datos localmente

4. Exporta APK (Android) o comparte link (iOS)

### Configuración Avanzada WebIntoApp

```javascript
// Configuración recomendada
{
  "url": "https://tuusuario.github.io/lara/",
  "name": "LARA",
  "theme_color": "#0b6efd",
  "background_color": "#0f172a",
  "display": "standalone",
  "orientation": "portrait",
  "cache_enabled": true,
  "offline_enabled": true,
  "share_enabled": true
}
```

## 🔧 Solución de Problemas

### La app no carga offline
- Verifica que el Service Worker esté registrado
- Abre la app al menos una vez con internet
- Revisa la consola del navegador (F12)

### Los emojis no se ven
- Asegúrate que el archivo tenga encoding UTF-8
- Verifica el meta charset en el HTML

### El botón borrar no funciona
- Ahora usa modal de confirmación mejorado
- Se actualiza correctamente después de borrar

### Error al importar JSON
- Verifica que el archivo sea válido (prueba en jsonlint.com)
- Asegúrate que contenga las claves correctas
- Usa solo archivos exportados desde la misma app

## 📊 Uso de la Aplicación

### Nuevo Registro
1. Ve a "Registro" en el menú
2. Selecciona tipo (Ingreso/Gasto)
3. Ingresa fecha y monto
4. Usa la calculadora integrada si necesitas
5. Guarda

### Búsqueda Rápida
1. En Historial de Registros
2. Usa el campo de búsqueda superior
3. Escribe cualquier término
4. Los resultados se filtran en tiempo real

### Ver Estadísticas
1. Ve a "Resumen" en el menú
2. Observa el gráfico de 6 meses
3. Revisa totales por categoría
4. Exporta a Excel o PDF si necesitas

### Backup de Datos
1. Ve a Resumen
2. Click en "Respaldar Datos (JSON)"
3. Guarda el archivo en lugar seguro
4. Para restaurar: "Importar Respaldo"

## 🎨 Personalización

La app se puede personalizar desde la pantalla de bienvenida:
- Logo personalizado
- Nombre de la empresa
- Eslogan
- Colores (edita CSS en index.html)

## 📱 Instalación como PWA

### En Android
1. Abre la app en Chrome
2. Menú (⋮) → "Agregar a pantalla de inicio"
3. La app se instala como nativa

### En iOS
1. Abre en Safari
2. Toca el botón compartir
3. "Agregar a pantalla de inicio"

## 💾 Límites de Almacenamiento

- LocalStorage: ~5-10 MB
- Si llegas al límite, exporta datos antiguos
- Borra registros viejos que ya no necesites
- Usa la función de exportar Excel regularmente

## 🔒 Privacidad

- Todos los datos se guardan localmente
- No hay conexión a servidores externos
- Solo tú tienes acceso a tu información
- Haz backups periódicos por seguridad

## 📞 Soporte

Para problemas o sugerencias:
1. Revisa esta documentación
2. Verifica la consola del navegador
3. Asegúrate de usar la última versión

## 🎯 Próximas Mejoras Sugeridas

- [ ] Reportes avanzados con más gráficos
- [ ] Exportar a PDF con diseño mejorado
- [ ] Recordatorios de pagos
- [ ] Múltiples usuarios/perfiles
- [ ] Sincronización en la nube (opcional)
- [ ] Temas de color adicionales

---

**Versión:** 1.0.0  
**Última actualización:** Enero 2026  
**Compatible con:** GitHub Pages, WebIntoApp, Netlify, Vercel

## ⚡ Quick Start

```bash
# 1. Clona o descarga los archivos
# 2. Abre index.html en un navegador
# 3. ¡Listo para usar!

# Para desarrollo local con live server:
npx serve .
```

¡Gracias por usar Multi Servicios LARA! 🚗✨
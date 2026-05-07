# VPN World - Telegram Mini App

**Objetivo:** Crear una miniapp de Telegram que muestre servidores VPN de todos los países del mundo, con interfaz tipo dashboard oscura.

## Arquitectura

- **Frontend:** HTML/CSS/JS vanilla — una sola página, sin frameworks pesados
- **Tema oscuro** inspirado en la UI de Magnus
- **Integración Telegram Web App API** (colores nativos, botones, haptics)
- **Backend:** Opcional — empezamos con datos mock/estáticos

## Fases

### Fase 1: Estructura base del proyecto ✅
- Crear estructura de archivos
- HTML base con meta tags para Telegram Web App
- Script de Telegram Web App SDK

### Fase 2: UI - Layout y tema oscuro
- Grid de países con banderas
- Diseño responsive (móvil-first, para Telegram)
- Colores: fondo oscuro, acentos teal/verde
- Componentes: header, buscador, grid de países, modal de detalle

### Fase 3: Datos de países y servidores VPN
- Array con todos los países + banderas (emoji flags)
- Datos mock de servidores VPN por país
- Estructura de datos para IPs, protocolos (WireGuard, OpenVPN)

### Fase 4: Interactividad
- Búsqueda/filtro de países
- Click en país → modal con servidores disponibles
- Copiar configuración al portapapeles
- Animaciones y transiciones

### Fase 5: Integración Telegram
- Configurar Telegram Bot con BotFather
- Web App setup (menu button, etc.)
- Adaptar colores al tema de Telegram
- Haptics y botones nativos

### Fase 6: Despliegue
- Preparar para deploy (GitHub Pages, Vercel, o similar)
- Instrucciones paso a paso para configurar en Telegram

## Notas
- VPN real requiere infraestructura de servidores — esta app es el frontend/directorio
- Para una VPN real, necesitaríamos un backend con WireGuard/OpenVPN
- Los datos de servidores son configurables

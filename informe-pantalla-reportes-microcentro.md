# Informe — Pantalla "Reportes en Microcentro"

**Materia:** Aplicaciones Móviles
**Alumno:** Villanueva, Lautaro
**Comisión:** ACN4A
**Repositorio:** parcial-1-am-acn4a-villanueva

---

## 1. Objetivo de la pantalla

Mostrar en una lista los reportes activos de estacionamiento en la zona de Microcentro (CABA) — controles policiales y lugares libres — reportados por los propios usuarios, permitiendo agregar un nuevo reporte de forma rápida.

## 2. Descripción visual

La pantalla se divide en tres bloques:

- **Header**: fondo oscuro con el título "REPORTES - MICROCENTRO" y un ícono de perfil de usuario a la derecha.
- **Lista de reportes**: tarjetas apiladas verticalmente, cada una con un ícono de estado, el tipo de reporte (Control policial / Lugar libre) y la ubicación. El color de fondo de cada tarjeta indica el tipo: rojo para controles, verde para lugares libres.
- **Botón de acción**: botón inferior "+ REPORTAR" en color ámbar, para agregar un nuevo reporte a la lista.

## 3. Funcionalidad esperada

Al tocar el botón "+ REPORTAR", se agrega dinámicamente una nueva tarjeta a la lista (sin recargar la pantalla ni requerir conexión a un servidor en esta primera entrega), simulando el comportamiento que tendría la app completa al recibir un reporte real de otro usuario.

## 4. Flujo de uso

1. El usuario abre la app y ve la lista de reportes activos en Microcentro.
2. Recorre la lista (scrollable) para ver los controles y lugares libres reportados.
3. Si detecta algo nuevo (un control o un lugar libre), toca "+ REPORTAR".
4. Se agrega una nueva tarjeta a la lista, visible de inmediato para el usuario.

## 5. Componentes técnicos utilizados

- `ConstraintLayout` — estructura general de la pantalla
- `LinearLayout` horizontal y vertical — organización interna de cada tarjeta y de la lista completa
- `TextView` — título del reporte y ubicación
- `Button` — acción de reportar
- Elemento agregado dinámicamente por código Java — nueva tarjeta al presionar "Reportar"
- Variables organizadas en `colors.xml`, `strings.xml` y `dimens.xml`

## 6. Paleta y tipografía

**Colores:**
- Azul noche `#1E2A3B` — header
- Ámbar `#F4A73C` — botón de acción
- Rojo `#E5484D` — tarjetas de control policial
- Verde `#2F9E44` — tarjetas de lugar libre

**Tipografía:**
- Poppins (ExtraBold / SemiBold) — título y botón
- Inter (Medium / Regular) — contenido de las tarjetas

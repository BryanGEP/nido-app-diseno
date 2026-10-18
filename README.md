# 🏡 Nido — App para residentes de coliving

![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)
![Claude](https://img.shields.io/badge/Claude_Design-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![UI/UX](https://img.shields.io/badge/UI%2FUX-Design_System-2F6B5A?style=for-the-badge)
![Estado](https://img.shields.io/badge/Estado-Concepto-B24A28?style=for-the-badge)

![Portada de Nido](assets/portada.png)

**Nido** es el concepto de una app móvil para residentes de un coliving en Guadalajara. Desde ahí el residente consulta su estancia, se integra a la comunidad, reserva espacios de coworking y pide servicios del edificio.

Es un **proyecto de práctica** para explorar el diseño de interfaces asistido por IA, sin perder la calidad de un sistema de diseño profesional. La marca "Nido" es ficticia.

🔗 **[Ver el archivo en Figma](https://www.figma.com/design/UfdaYLcSMFD2oCDriXJQ6h)**

---

## 🎯 El problema

En un coliving, el residente necesita resolver cosas operativas (pagos, reservas, limpieza) y sociales (eventos, conocer vecinos). Normalmente eso ocurre en grupos de WhatsApp, correos y formularios separados.

**Nido junta todo en una sola app** con una idea central: que se sienta como *la puerta de una casa compartida*, no como un sistema de reservas.

## 📱 Pantallas

| Inicio | Comunidad | Reservar coworking | Solicitar servicio |
|:---:|:---:|:---:|:---:|
| ![Inicio](assets/pantallas/inicio.png) | ![Comunidad](assets/pantallas/comunidad.png) | ![Reservar coworking](assets/pantallas/reservar-coworking.png) | ![Solicitar servicio](assets/pantallas/solicitar-servicio.png) |
| Resumen de la estancia, accesos rápidos y el evento de la semana | Filtros, evento destacado y próximas actividades | Selección de día, espacio y horario, con resumen fijo abajo | Tipo de servicio, descripción, foto adjunta y permiso de acceso |

## 🛠️ Proceso

1. **Sistema de diseño primero.** Antes de dibujar pantallas definí los fundamentos en **Claude Design**: paleta, tipografía, espaciado, radios y sombras, con tema claro y oscuro.
2. **Pantallas a partir del sistema.** Las 4 pantallas usan solo esos tokens, así que el botón principal, los colores y la tipografía son idénticos en todas.
3. **Ilustraciones propias.** 12 ilustraciones planas (habitación, terraza, espacios, avatares) hechas con la paleta de la marca.
4. **Paso a Figma como sistema real.** Con el conector de Figma convertí el diseño en un archivo profesional:
   - **Variables** de color, espaciado, radios y tamaños, con su nombre en código (`var(--terracota-500)`).
   - **Estilos** de texto y de sombra.
   - **21 componentes** (15 con variantes) y propiedades editables (texto, intercambio de ícono e imagen, mostrar/ocultar).
   - **Pantallas armadas con instancias:** si cambias un color o un componente, se actualizan todas.

## 🎨 Sistema de diseño

![Fundamentos](assets/fundamentos.png)

### Principios
- **Cálido, no corporativo:** colores tierra sobre una base crema y títulos en serif.
- **Una acción clara por pantalla:** el botón primario aparece una sola vez por vista.
- **Lo social se distingue de lo operativo:** verde agave para comunidad y terracota para reservas y servicios.
- **Lo importante primero:** la fecha antes que el título y el resumen antes que el botón.

### Color
| Rol | Token | Claro | Oscuro |
|---|---|---|---|
| Marca / acción | `terracota-500` | `#B24A28` | `#E07A55` |
| Comunidad | `agave-600` | `#2F6B5A` | `#6FB39D` |
| Realce | `sol-400` | `#E8B04B` | `#E8B04B` |
| Texto principal | `tinta` | `#2A211B` | `#F3ECE3` |
| Texto secundario | `tinta-suave` | `#6B5E54` | `#B8AA9D` |
| Fondo | `superficie-0` | `#FAF6F0` | `#1C1714` |

### Tipografía
- **Fraunces** (títulos): le da el carácter de hogar.
- **DM Sans** (interfaz): legible a tamaños pequeños.
- Escala: 34 · 24 · 22 · 17 · 15 · 14 · 13 · 12 px.

### Componentes
`Button` · `Chip` · `Badge` · `Avatar` · `Card` · `StayCard` · `EventCard` · `ListItem` · `QuickAction` · `OptionCard` · `DayPicker` · `TimeSlot` · `TextField` · `Switch` · `AppBar` · `TabBar` · `ActionBar`

## ♿ Accesibilidad
- Contraste verificado en **ambos temas**: texto ≥ 4.5:1 y controles ≥ 3:1.
- El color nunca es la única señal: los estados llevan texto o forma (por ejemplo, un horario ocupado va tachado y con borde punteado).
- Zonas táctiles de al menos 44 px.

## 🧰 Herramientas
- **Claude Design:** sistema de diseño, pantallas e ilustraciones.
- **Figma:** variables, componentes con propiedades y pantallas finales.
- **Conector Figma (MCP):** paso automatizado del diseño a Figma.

## 💡 Aprendizajes
- Definir el sistema **antes** de las pantallas hace que la IA genere rápido **y** consistente.
- Las propiedades de componente evitan hacer *detach* y mantienen todo vinculado.
- **Variables → marca, componentes → estructura, instancias → contenido.**

---

👤 **Bryan Gael Esquivel Pérez** — Ingeniería en Sistemas Computacionales, TecNM Jiquilpan
[LinkedIn](https://www.linkedin.com/in/bryan-esquivel-perez) · [GitHub](https://github.com/BryanGEP)

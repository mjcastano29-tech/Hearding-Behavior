# Herding Behavior — Simulación de Burbuja Financiera

Simulación interactiva de **herding behavior** en mercados financieros, mostrando la formación y colapso de una burbuja especulativa basada en el modelo de Hyman Minsky.

## Demo

Abre `index.html` directamente en tu navegador — no requiere servidor ni instalación.

> Si el repositorio tiene GitHub Pages activo, puedes verlo en:
> `https://tu-usuario.github.io/nombre-del-repo`

---

## Qué muestra la simulación

La simulación modela **90 agentes** que toman decisiones de compra/venta en un mercado. El comportamiento colectivo genera cinco fases clásicas de una burbuja:

| Fase | Descripción |
|------|-------------|
| **Stealth** | El *smart money* (5% de agentes) acumula silenciosamente sin que el mercado lo note |
| **Awareness** | Cobertura mediática; primeros inversores retail se suman al rally |
| **Mania** | FOMO masivo — el herding está en su punto máximo, el precio se desacopla del valor fundamental |
| **Blow-off** | El smart money ya está saliendo; el retail sigue comprando en el tope |
| **Crash** | Herding inverso: el pánico se contagia y todos venden al mismo tiempo |

### Elementos visuales

- **Canvas de agentes** — cada punto es un agente: verde (comprando), rojo (vendiendo), gris (neutral), morado (smart money)
- **Gráfico de precio** — línea roja = precio del activo, línea verde punteada = valor fundamental
- **Métricas en tiempo real** — precio, % comprando, % vendiendo, valor fundamental
- **Log de eventos** — registra los hitos clave de cada fase

---

## Parámetros del modelo

Los parámetros están fijos para mantener la simulación enfocada en la narrativa:

| Parámetro | Valor | Descripción |
|-----------|-------|-------------|
| Herding strength | 75% | Qué tanto los agentes copian a la mayoría |
| N° de agentes | 90 | Total de participantes en el mercado |
| Smart money | 5% | Fracción de agentes con información superior |
| Velocidad | 2x | Velocidad de avance de la simulación |

---

## Fundamento teórico

La simulación ilustra tres conceptos clave de las finanzas conductuales:

**Herding behavior** — los agentes ignoran su propia información privada y copian las decisiones de la mayoría. A mayor *herding strength*, más pronunciada es la burbuja y más abrupto el colapso.

**Desacople precio–fundamental** — durante la fase de Mania, el precio puede superar al valor fundamental en un 40–80%. Este desacople es la definición operativa de burbuja especulativa.

**Herding inverso en el crash** — el pánico es simétricamente contagioso: los mismos mecanismos que inflan la burbuja la colapsan, generando ventas en cascada.

---

## Referencias

- Minsky, H. (1986). *Stabilizing an Unstable Economy*. Yale University Press.
- Shiller, R. (2000). *Irrational Exuberance*. Princeton University Press.
- Scharfstein, D. & Stein, J. (1990). Herd Behavior and Investment. *American Economic Review*, 80(3), 465–479.
- Bikhchandani, S., Hirshleifer, D. & Welch, I. (1992). A Theory of Fads, Fashion, Custom, and Cultural Change as Informational Cascades. *Journal of Political Economy*, 100(5), 992–1026.

---

## Tecnologías

- HTML5 / CSS3 / JavaScript vanilla
- [Chart.js 4.4](https://www.chartjs.org/) para el gráfico de precios
- Canvas API para la visualización de agentes
- Sin dependencias adicionales — un solo archivo `index.html`

---

*Simulación educativa para presentaciones de finanzas conductuales.*

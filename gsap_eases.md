# GSAP Easing Functions

GSAP provides a wide variety of easing functions. Most of these can be used with `.in`, `.out`, or `.inOut` suffixes (e.g., `power2.in`, `power2.out`, `power2.inOut`). 

The default ease is `power1.out`.

## 1. Standard Eases
These are the most commonly used eases, ranging from subtle to dramatic.

| Ease Name | Description |
| :--- | :--- |
| `none` | Linear movement (constant speed). |
| `power1` | Very subtle (Quad-like). |
| `power2` | Subtle (Cubic-like). |
| `power3` | Decent amount of weight (Quart-like). |
| `power4` | Strong / Heavy (Quint-like). |
| `expo` | Extreme acceleration/deceleration. |
| `sine` | Smooth and natural (think of a pendulum). |
| `circ` | Accelerates quickly, then stops abruptly (like a quarter circle). |

## 2. Dynamic / Physics Eases
These mimics physical properties like gravity or springiness.

| Ease Name | Description |
| :--- | :--- |
| `back` | Over shoots the target value and then "backs" into it. (Configurable: `back.out(1.7)`) |
| `elastic` | "Boing!" effect. (Configurable: `elastic.out(1, 0.3)`) |
| `bounce` | Bounces like a ball when it hits the target. |

## 3. Specialized Eases
Require specific configuration strings.

| Ease Name | Description |
| :--- | :--- |
| `steps(n)` | Moves in discrete steps rather than a smooth curve. |
| `rough` | Adds "noise" to the movement. |
| `slow` | Slows down in the middle of the animation. |
| `custom` | Allows you to draw your own curve (via CustomEase plugin). |

## Variation Suffixes
*   `.out`: Starts fast, ends slow (Best for UI entrances). **GSAP Default**.
*   `.in`: Starts slow, ends fast (Best for UI exits).
*   `.inOut`: Starts slow, speeds up in the middle, then ends slow (Best for looping or point-to-point movement).

---
**Note:** In GSAP 3, you can use the string syntax (e.g., `"power2.out"`) or the shorter dot syntax (`power2.out`).

# Parte 3 – Respuesta, Corrección de la Auditoría y Código Actualizado

## 1. Tabla de respuesta a los hallazgos del auditor

| N.º de hallazgo | Decisión (acepta o refuta) | Justificación con la norma | Evidencia antes y después | Commit |
| :---: | :---: | :--- | :--- | :--- |
| **1** | Acepta | Se acepta el hallazgo. El meta viewport estaba comentado, lo que impedía la correcta visualización y adaptación responsiva en dispositivos móviles, infringiendo WCAG 1.4.10 (Reflow). | `[antes](evidencias/fer-01-celular.png)` / `[después](evidencias/correc-01.png)` | `a1b2c3d` |
| **2** | Acepta | Se acepta el hallazgo. El mapa (iframe) poseía un ancho fijo de 600px que desbordaba la pantalla en viewports estrechos de 360px, afectando el diseño adaptativo (WCAG 1.4.10). | `[antes](evidencias/fer-02-360px.png)` / `[después](evidencias/correc-02.png)` | `b2c3d4e` |
| **3** | Acepta | Se acepta el hallazgo. La imagen principal del hero carecía del atributo `alt`, lo que genera un fallo directo en accesibilidad según WCAG 1.1.1 (Contenido no textual). | `[antes](evidencias/fer-03-validador.png)` / `[después](evidencias/correc-03.png)` | `c3d4e5f` |
| **4** | Acepta | Se acepta el hallazgo. Se utilizaban colores fijos (`#ddd`, `#555`, `#ccc`) directamente en lugar de emplear el sistema centralizado de variables personalizadas requerido en el Requisito Base 5. | `[antes](evidencias/fer-04a.png)` / `[después](evidencias/correc-04.png)` | `d4e5f6g` |
| **5** | Acepta | Se acepta el hallazgo. Se implementaron los pseudo-clases `:user-valid` y `:user-invalid`, pero la Ficha N.º 14 exigía específicamente el uso de `:valid` e `:invalid` en combinación con `:has()`. | `[antes](evidencias/fer-05-css.png)` / `[después](evidencias/correc-05.png)` | `e5f6g7h` |
| **6** | Acepta | Se acepta el hallazgo. La omisión de la etiqueta `<meta charset="utf-8">` provocaba que el validador W3C Nu interpretara erróneamente la codificación de caracteres predeterminada. | `[antes](evidencias/fer-03-validador.png)` / `[después](evidencias/correc-06.png)` | `f6g7h8i` |

---
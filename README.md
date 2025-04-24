# Calculadora de Trading Forex

Esta herramienta te permite calcular el tamaño óptimo de lotes para tus operaciones de trading Forex basándose en la gestión de riesgo del 2% y la distribución recomendada de lotes 70/15/15 para los diferentes Take Profits.

## Características

- **Cálculo de lotes basado en gestión de riesgo**: Asegura que nunca arriesgues más del 2% de tu capital por operación.
- **Distribución óptima para múltiples Take Profits**: División automática de 70/15/15 para TP1, TP2 y TP3.
- **Análisis de escenarios post-TP1**: Evalúa diferentes estrategias para mover el stop loss después de alcanzar el primer take profit.
- **Soporte para cualquier par de divisas**: Detecta automáticamente pares con JPY para cálculos precisos de pips.
- **Interfaz intuitiva**: Fácil de usar, solo necesitas introducir tus datos de trading.

## Demo

Puedes ver una demo de la calculadora [aquí](https://tu-usuario.github.io/forex-calculator) (actualiza este enlace cuando tengas el proyecto publicado).

## Cómo usar

1. Introduce el tamaño de tu cuenta en dólares.
2. Ingresa la señal de trading en el formato: `PAR DIRECCIÓN PRECIO` (ejemplo: `GBPNZD BUY 2.2220`).
3. Ingresa los niveles de TP y SL en el formato: `TP PRECIO1 TP PRECIO2 TP PRECIO3 SL PRECIO` (ejemplo: `TP 2.2250 TP 2.2270 TP 2.2320 SL 2.2125`).
4. Haz clic en "Calcular".
5. Revisa los resultados, que incluyen:
   - Tamaño de lote recomendado para cada nivel de TP.
   - Análisis de los diferentes escenarios para gestionar el SL después del TP1.
   - Recomendación del mejor escenario basado en la relación ganancia/riesgo.

## Estrategias de Stop Loss después del TP1

La calculadora analiza 5 escenarios para mover el SL después de que se alcance el TP1:

1. **SL en punto de entrada para ambas posiciones restantes**: Elimina el riesgo pero limita las ganancias.
2. **SL en punto de entrada para TP2, mitad del SL original para TP3**: Balance entre seguridad y potencial.
3. **Mitad del SL original para ambas posiciones**: Enfoque equilibrado.
4. **Mitad del SL original para TP2, SL original para TP3**: Mayor riesgo para TP3.
5. **SL original para ambas posiciones**: Máximo riesgo pero potencial de capturar todo el movimiento.

## Instalación

### Método 1: GitHub Pages (recomendado)

1. Haz un fork de este repositorio.
2. Ve a Settings > Pages y activa GitHub Pages eligiendo la rama main.
3. Tu calculadora estará disponible en `https://tu-usuario.github.io/forex-calculator`.

### Método 2: Descarga directa

1. Descarga el archivo `index.html` de este repositorio.
2. Abre el archivo en cualquier navegador web moderno.

### Método 3: Incluir en tu web

Simplemente copia el código HTML de `index.html` y pégalo en tu propia página web.

## Personalización

Puedes personalizar la calculadora ajustando estos parámetros en el código:

- **Porcentaje de riesgo**: Por defecto es 2%. Cambia el valor `accountSize * 0.02` para ajustarlo.
- **Distribución de lotes**: Por defecto es 70/15/15. Modifica estos valores si prefieres otra distribución.
- **Valor del pip**: Por defecto es $10 por pip para un lote de 1.0. Ajústalo si trabajas con otro valor.

## Contribuciones

Las contribuciones son bienvenidas. Por favor, sigue estos pasos:

1. Haz un fork del repositorio.
2. Crea una rama para tu feature (`git checkout -b feature/nueva-caracteristica`).
3. Haz commit de tus cambios (`git commit -m 'Añadir nueva característica'`).
4. Haz push a la rama (`git push origin feature/nueva-caracteristica`).
5. Abre un Pull Request.

## Próximas mejoras

- [ ] Añadir soporte para diferentes monedas de cuenta
- [ ] Incluir gráficos visuales de riesgo/recompensa
- [ ] Añadir historial de operaciones
- [ ] Implementar exportación de resultados a CSV
- [ ] Añadir soporte para estrategias de trailing stop

## Licencia

Este proyecto está licenciado bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.

## Descargo de responsabilidad

Esta herramienta es solo informativa y no constituye asesoramiento financiero. El trading conlleva riesgos significativos y debes operar bajo tu propia responsabilidad.

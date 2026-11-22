# Corrección de NPSHa por Altitud Andina (0 a 4.500 msnm) y Redes 50 Hz / 60 Hz

Referencia técnica en español elaborada por **[YSM Pumps (Jinan Yingsiman Machinery Co., Ltd.)](https://ysmbombas.com/)** para ingenieros de proceso, confiabilidad y mantenimiento en operaciones mineras y químicas de **Chile, Perú, Bolivia, Argentina, Colombia, México y España**.

> Guía técnica interactiva completa: [Cálculo de NPSHa en Altitud Andina y Prevención de Cavitación](https://ysmbombas.com/guia-tecnica/calculo-npsha-altitud-andina-cavitacion-bombas/)

## 1. Pérdida de Presión Atmosférica y Carga Neta Positiva de Succión (NPSHa) por Altitud

En operaciones de minería de cobre (SX-EW), salares de litio y plantas químicas sobre 2.000 msnm, la caída de presión atmosférica reduce directamente el **NPSHa** disponible en la brida de succión de bombas centrífugas **ANSI/ASME B73.1** e **ISO 5199**:

| Altitud (msnm) | Presión Atmosférica (kPa) | Presión Atmosférica (bar) | Altura Equivalente de Agua a 20 °C (m) | Pérdida de NPSHa respecto al Nivel del Mar (m) | Operaciones de Referencia |
| ---: | ---: | ---: | ---: | ---: | :--- |
| 0 m | 101,3 | 1,013 | 10,33 m | 0,00 m | Puertos, refinerías costeras, España |
| 1.000 m | 89,9 | 0,899 | 9,17 m | -1,16 m | Plantas industriales en valles interiores |
| 1.500 m | 84,6 | 0,846 | 8,63 m | -1,70 m | Zonas mineras de media altura (México, Colombia) |
| 2.000 m | 79,5 | 0,795 | 8,11 m | -2,22 m | Altiplano mexicano, sierra peruana baja |
| 2.500 m | 74,7 | 0,747 | 7,62 m | -2,71 m | Salares de litio (Salar de Atacama ~2.300 m) |
| 3.000 m | 70,1 | 0,701 | 7,15 m | -3,18 m | Operaciones cupríferas norte de Chile |
| 3.500 m | 65,8 | 0,658 | 6,71 m | -3,62 m | Minería andina de cobre y molibdeno |
| 4.000 m | 61,6 | 0,616 | 6,28 m | -4,05 m | Salares de litio NOA Argentina / Altiplano Perú-Bolivia |
| 4.500 m | 57,7 | 0,577 | 5,89 m | -4,44 m | Faenas de gran altitud (Antofagasta, Apurímac, Moquegua) |

### Fórmula práctica de verificación

```text
NPSHa = (Patm(altitud) - Pvapor(T)) / (rho * g) + hz - hf_succion
```

- **Regla de seguridad recomendada**: mantener `NPSHa >= NPSHr + 1,0 m` (o margen superior en lodos, salmueras de litio y soluciones calientes de ácido sulfúrico).
- Cuando la temperatura del ácido o salmuera sube de 20 °C a 60 °C, la presión de vapor del agua se multiplica de ~2,3 kPa a ~19,9 kPa, restando otros **~1,8 m** adicionales al margen de succión.

## 2. Diferencia Eléctrica 50 Hz vs. 60 Hz (Leyes de Afinidad)

| Región / Países | Frecuencia de Red | Velocidad Síncrona (2 polos / 4 polos) | Efecto Hidráulico vs. 50 Hz (mismo diámetro de impulsor) |
| :--- | :---: | :---: | :--- |
| Chile, Argentina, Bolivia, Uruguay, España | **50 Hz** | 2.900 / 1.450 rpm | Base de diseño 50 Hz |
| México, Perú, Colombia, Ecuador, Centroamérica | **60 Hz** | 3.500 / 1.750 rpm | Caudal ×1,20 · Altura (TDH) ×1,44 · Potencia ×1,73 |

> Al reemplazar impulsores o bombas completas patrón **Goulds 3196** o **Durco Mark 3**, verifique siempre la frecuencia de red (50 Hz vs. 60 Hz) y el diámetro de recorte (*trim diameter*) en planta.

## Recursos Relacionados en ysmbombas.com
- [Bombas para Minería de Cobre (SX-EW) y Litio](https://ysmbombas.com/aplicaciones/bombas-para-mineria-cobre-y-litio/)
- [Buscador Interactivo de 223 Códigos OEM ANSI B73.1](https://ysmbombas.com/repuestos-ansi/)
- [Solicitar Verificación Hidráulica y Cotización Directa (Respuesta ≤ 48 h)](https://ysmbombas.com/solicitar-cotizacion/)

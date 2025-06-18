# PFC-CS
Técnicas:
1. D2-Net
2. ALIKED
3. LoFTR
4. ELoFTR
   
## Métricas

Las siguientes tablas presentan los resultados de evaluación obtenidos usando el dataset [Aachen Day-Night](https://www.visuallocalization.net/datasets/), que contiene imágenes urbanas tomadas en condiciones diurnas y nocturnas. Se evaluaron las cuatro técnicas de coincidencia.

Las métricas consideradas son:

- `num_matches`: número de coincidencias detectadas
- `efficiency`: eficiencia de coincidencia (coincidencias válidas / total)
- `avg_distance`: distancia promedio entre descriptores coincidentes
- `spatial_entropy`: entropía espacial de la distribución de los matches

### Imágenes de Día

| Técnica         | num_matches | efficiency | avg_distance  | spatial_entropy  |
|-----------------|-------------|------------|---------------|------------------|
| D2Net           |             |            |               |                  |
| ALIKED          |             |            |               |                  |
| LoFTR           |             |            |               |                  |
| EfficientLoFTR  |             |            |               |                  |

### Imágenes de Noche

| Técnica         | num_matches | efficiency | avg_distance  | spatial_entropy  |
|-----------------|-------------|------------|---------------|------------------|
| D2Net           |             |            |               |                  |
| ALIKED          |             |            |               |                  |
| LoFTR           |             |            |               |                  |
| EfficientLoFTR  |             |            |               |                  |


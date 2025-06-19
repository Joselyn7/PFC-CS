# PFC-CS
Técnicas:
1. D2-Net
2. ALIKED
3. LoFTR
4. ELoFTR

## Configuración Experimental

- Todas las imágenes del dataset Aachen Day & Night fueron redimensionadas a **1280 × 720 píxeles** para asegurar uniformidad en el procesamiento y reducir la carga computacional.
- Se utilizó el algoritmo de coincidencia **Fuerza Bruta (Brute-Force Matcher)** con distancia euclidiana para todas las técnicas evaluadas (D2-Net, ALIKED, LoFTR y EfficientLoFTR), con el objetivo de mantener consistencia en la comparación de descriptores.
  
## Métricas

Las siguientes tablas presentan los resultados de evaluación obtenidos usando el dataset [Aachen Day-Night](https://www.visuallocalization.net/datasets/), que contiene imágenes urbanas tomadas en condiciones diurnas y nocturnas. Se evaluaron las cuatro técnicas de coincidencia.

Las métricas consideradas son:

- `num_matches`: número de coincidencias detectadas
- `efficiency`: eficiencia de coincidencia (coincidencias válidas / total)
- `avg_distance`: distancia promedio entre descriptores coincidentes
- `spatial_entropy`: entropía espacial de la distribución de los matches

### Imágenes de Día

| Técnica         | num_matches | efficiency | avg_distance  | spatial_entropy  |
|----------------|-------------|------------|---------------|------------------|
| D2Net           |  1,107      | 1.03       | 0.58          | 1.97             |
| ALIKED          |  1,289      | 1.25       | 0.52          | 2.10             |
| LoFTR           |  2,476      | 2.50       | 0.39          | 2.40             |
| EfficientLoFTR  |  2,322      | 2.70       | 0.42          | 2.35             |

### Imágenes de Noche

| Técnica         | num_matches | efficiency | avg_distance  | spatial_entropy  |
|----------------|-------------|------------|---------------|------------------|
| D2Net           | 763         | 0.80       | 0.66          | 1.55             |
| ALIKED          | 897         | 0.95       | 0.58          | 1.70             |
| LoFTR           | 1,842       | 2.10       | 0.45          | 2.10             |
| EfficientLoFTR  | 1,679       | 2.30       | 0.47          | 2.05             |


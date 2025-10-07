# Scraping de Competencia de Vehículos

Este proyecto contiene notebooks y scripts para realizar scraping de diferentes plataformas de venta de vehículos en Chile, incluyendo Yapo, MercadoLibre, Macal, Autopia, Kavak, Clicar, Dily, BravoAuto, Auto.cl, Venpu, Marketplace, Linze, Udach, Chilemotos y Autocosmos.

## Notebooks principales

- **SELENIUM-2.ipynb**: Scraping paginado y detallado de Yapo.cl, guarda resultados de cada auto en un CSV.
- **selenium.ipynb**: Ejemplos y scripts para scraping de múltiples plataformas, cada celda corresponde a una fuente distinta.

## Archivos generados

- `yapo_autos_1.csv`: Resultados detallados del scraping de Yapo (autos, vendedor, precio, ubicación, etc).
- `vehiculos_totales.csv`: Totales de vehículos por plataforma y fecha.
- `competencia.csv`: Detalle de categorías y cantidades por competencia.
- Otros CSV: Resultados específicos por plataforma (ej: `mercadolibre_autos.csv`, `yapo_filters.csv`, etc).

## Requisitos

- Python 3.8+
- Google Chrome
- [Selenium](https://pypi.org/project/selenium/)
- [webdriver-manager](https://pypi.org/project/webdriver-manager/)
- [BeautifulSoup4](https://pypi.org/project/beautifulsoup4/)
- [pandas](https://pypi.org/project/pandas/)
- [requests](https://pypi.org/project/requests/)
- Otros: playwright, playwright-stealth, dotenv (según el notebook)

Instala los paquetes necesarios con:

```bash
pip install selenium webdriver-manager beautifulsoup4 pandas requests
```

## Ejecución

1. Abre el notebook que corresponda (`SELENIUM-2.ipynb` para Yapo, `selenium.ipynb` para multi-plataforma) en VSCode o Jupyter.
2. Configura los parámetros de scraping (página de inicio, fin, batch size, etc.) según tus necesidades.
3. Ejecuta las celdas del notebook. Los resultados se guardan en archivos CSV en la misma carpeta.
4. Analiza los datos usando pandas u otras herramientas.

## Notas

- Algunos scripts requieren cookies para acceder a MercadoLibre. Consulta los notebooks para instrucciones.
- El scraping puede demorar dependiendo de la cantidad de páginas y anuncios.
- Revisa los selectores y URLs si las plataformas cambian su diseño.
- Respeta las políticas de uso de cada sitio web.

## Autor

hfuentes.ca


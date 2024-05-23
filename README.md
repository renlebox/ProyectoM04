### Pasos per desplegar l'aplicatiu:

1. **Requisitos**: Lista los requisitos del proyecto, incluyendo Python y pip.
2. **Configuración del Entorno Virtual**: Proporciona instrucciones para instalar `virtualenv`, crear y activar el entorno virtual, y instalar las dependencias.
3. **Iniciar la Aplicación**: Explica cómo iniciar la aplicación Flask.
4. **Uso del Modo Remoto o Local**: Detalla cómo cambiar entre el modo remoto y local para el XML de La Vanguardia.
5. **Recursos**: Incluye enlaces a la documentación de Flask y a la guía sobre entornos virtuales de Python.
6. **Estructura del Proyecto**: Muestra la estructura del proyecto para ayudar a los usuarios a entender dónde deben ir los archivos.
7. **Contribuciones**: Invita a la comunidad a contribuir al proyecto.


# Configuración del Entorno y Ejecución de la Aplicación Flask

## Requisitos

- Python 3.x
- pip (Python package installer)
- Virtualenv (opcional pero recomendado)

## Configuración del Entorno Virtual

### Instalación de Virtualenv

Si no tienes `virtualenv` instalado, puedes instalarlo usando `pip`:

```bash
pip install virtualenv
``` 
# Creacion y activacion del entorno 
```bash
virtualenv venv

``` 
## Activar el entorno virtual:
```bash
venv\Scripts\activate

``` 
## Instalación de Dependencias
```bash
pip install -r requirements.txt


``` 
# Iniciar la Aplicación
```bash
flask run

``` 

## Modos de uso: 
### Uso del Modo Remoto o Local
La aplicación puede funcionar en modo remoto, descargando el XML directamente de la web de La Vanguardia, o en modo local, utilizando un archivo XML descargado.

### Modo Remoto
El modo remoto está configurado por defecto. La aplicación descargará el XML de La Vanguardia cada vez que se acceda a una sección.

### Modo Local
Para utilizar el modo local, comenta la línea del modo remoto y descomenta la línea del modo local en la función get_rss_lavanguardia en app.py:
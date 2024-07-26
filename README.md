# CI/CD Pipeline with GitHub Actions

Este repositorio contiene un ejemplo de pipeline de CI/CD utilizando GitHub Actions. La aplicación es una simple aplicación "Hello World" en Python.

## Estructura del Proyecto

- `hello.py`: Código de la aplicación "Hello World".
- `tests/test_hello.py`: Pruebas unitarias para la aplicación utilizando `pytest`.
- `.github/workflows/ci-cd.yml`: Configuración del pipeline de CI/CD en GitHub Actions.

## Requisitos

- Python 3.x
- pytest

## Configuración del Pipeline de CI/CD

El pipeline de CI/CD está configurado en el archivo `.github/workflows/ci-cd.yml`. Este pipeline realiza las siguientes acciones:

1. **Clonación del Repositorio**: Clona el repositorio en el entorno de GitHub Actions.
2. **Configuración del Entorno de Python**: Instala Python y configura la versión especificada.
3. **Instalación de Dependencias**: Actualiza `pip` e instala `pytest`.
4. **Ejecución de Pruebas Unitarias**: Ejecuta las pruebas unitarias utilizando `pytest`.
5. **Despliegue de la Aplicación**: (Opcional) Puedes agregar comandos para desplegar la aplicación en un entorno de prueba.

## Ejecutar Localmente

Para ejecutar la aplicación y las pruebas en tu entorno local, sigue estos pasos:

1. Clona el repositorio:
    ```bash
    git clone https://github.com/tu-usuario/ci-cd-github-actions.git
    cd ci-cd-github-actions
    ```

2. Crea un entorno virtual e instala las dependencias:
    ```bash
    python -m venv venv
    source venv/bin/activate  # En Windows usa: venv\Scripts\activate
    pip install pytest
    ```

3. Ejecuta la aplicación:
    ```bash
    python hello.py
    ```

4. Ejecuta las pruebas:
    ```bash
    pytest
    ```

## Despliegue

El paso de despliegue en el pipeline de CI/CD está configurado para ejecutar un servidor HTTP simple. Puedes personalizar esta sección en el archivo `.github/workflows/ci-cd.yml` según tus necesidades de despliegue.

## Contribuciones

Si deseas contribuir a este proyecto, por favor abre un issue o envía un pull request. Asegúrate de que tu código pase las pruebas antes de enviar el pull request.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para obtener más detalles.

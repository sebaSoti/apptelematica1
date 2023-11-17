# apptelematica1
# Infraestructura para Microservicios

Este repositorio contiene la definición de infraestructura utilizando Terraform para desplegar dos microservicios basados en Java en Docker.

## Estructura del Repositorio

- `microservicio1`: Contiene el código fuente y el Dockerfile para el primer microservicio.
- `microservicio2`: Contiene el código fuente y el Dockerfile para el segundo microservicio.
- `main.tf`: Archivo principal de Terraform que define la infraestructura en AWS.
- `terraform.tf`: Archivo de variables Terraform para personalizar la configuración.
- `script.sh`: Script de automatización que ejecuta el despliegue completo.

## Despliegue Automático

### Requisitos Previos

- Tener Terraform instalado en tu máquina.
- Configurar las credenciales de AWS en tu entorno.

### Pasos para el Despliegue

1. Clona el Repositorio:

    ```bash
    git clone https://github.com/tu-usuario/tu-repositorio.git
    cd tu-repositorio
    ```

2. Personaliza la Configuración:

    - Ajusta las variables en `terraform.tf` según tus necesidades.

3. Ejecuta el Script de Despliegue Automático:

    ```bash
    ./script.sh
    ```

    Este script realizará las siguientes acciones:
    - Construirá y desplegará los contenedores Docker para cada microservicio.
    - Inicializará y aplicará la configuración de Terraform para la infraestructura en AWS.

4. Accede a tus Microservicios:

    - Después de que el script se ejecute con éxito, podrás acceder a tus microservicios en las direcciones especificadas por Terraform.

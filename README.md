# Sistema de Gestion de Inventario

Aplicacion de escritorio desarrollada en Python para la administracion de stock y productos. El sistema integra una interfaz grafica de usuario (GUI) moderna y un esquema de persistencia de datos basado en archivos CSV para facilitar su despliegue y portabilidad.

## Descripcion

Este software proporciona una solucion integral para el control de inventarios, permitiendo la gestion del ciclo de vida completo de un producto. Esta optimizado para entornos que requieren una herramienta ligera y eficaz, eliminando la necesidad de configurar motores de bases de datos complejos.

## Funcionalidades Principales

* Gestion de Registros (CRUD): Implementacion completa de las operaciones de creacion, lectura, actualizacion y eliminacion.
* Automatizacion de Datos: Generacion automatica del archivo de persistencia (inventario.csv) en el primer arranque del sistema.
* Identificadores Unicos: Algoritmo de asignacion de ID autoincremental para asegurar la integridad de cada registro.
* Interfaz Optimizada: Diseño basado en la libreria CustomTkinter con visualizacion tabular organizada mediante Treeview.
* Validacion de Datos: Capa de control de entrada para prevenir campos vacios o tipos de datos incorrectos.

## Especificaciones Tecnicas

* Lenguaje: Python 3.x
* Framework GUI: CustomTkinter
* Componentes de Tabla: Tkinter (Treeview)
* Almacenamiento: CSV (Comma-Separated Values)

## Instalacion y Uso

1. Clonar el repositorio o descargar los archivos fuente.
2. Instalar la dependencia necesaria mediante el gestor de paquetes pip:

   pip install customtkinter

3. Ejecutar la aplicacion:

   python main.py

## Estructura del Almacenamiento

Los datos se guardan de forma local en un archivo plano con la siguiente jerarquia de columnas:

ID | Nombre | Categoria | Cantidad | Precio

## Consideraciones Generales

* El sistema realiza escrituras sincronas en el archivo CSV para garantizar que los cambios se reflejen de inmediato.
* Se recomienda no manipular manualmente el archivo inventario.csv mientras la aplicacion se encuentre en ejecucion para evitar conflictos de escritura.

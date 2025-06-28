## Como crear un entorno virtual en Python
Un entorno virtual en Python es una herramienta que permite crear un espacio aislado para instalar paquetes y dependencias sin tener que afectar al sistema global de Python.
es especialmente útil para gestionar proyectos con diferentes requisitos de versiones de paquetes.

### 1. Abre la terminal o consola de comandos.
 
### 2. Encima de la carpeta de tu proyecto ejecuta esta linea de commando:
```bash
python -m venv nombre_del_entorno
```
Automaticamente se creara una carpeta llamada nombre_del_entorno, dentro de la cual se encontraran los archivos necesarios para el entorno virtual.
los archivos mas importantes son:
- `activate`: un script que activa el entorno virtual.
- `deactivate`: un script que desactiva el entorno virtual.


### 3. Para *activar* el entorno virtual:
  1. dirigete a la carpeta donde se encuentra el entorno virtual:
      ```bash
      cd nombre_del_entorno\Scripts 
      ```
  2. ejecuta el script de activacion:
      ```bash
        activate
        ```
      si no funciona, prueba con:
      ```bash
       .\activate
        ```
      
Vas a saber que estas dentro del entorno virtual porque el nombre del entorno virtual aparecera al inicio de la terminal, por ejemplo:
```bash
(.venv) venv tut\.venv\Scripts> 
```
 
### 4. Para *desactivar* el entorno virtual:
    ```bash
    deactivate
    ```

## Para instalar paquetes dependencias en el entorno virtual:
### una vez creado y activado el entorno virtual, puedes usar pip para instalar paquetes como siempre 

```bash
pip install nombre_del_paquete
```
### Por ejemplo, para instalar multiples paquetes a la vez:
```bash
pip install package1 package2 package3
```
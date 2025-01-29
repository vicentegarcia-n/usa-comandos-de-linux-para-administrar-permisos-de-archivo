# usa-comandos-de-linux-para-administrar-permisos-de-archivo
Proyecto hecho en el curso #4 "Herramientas del oficio: Linux y SQL" del Certificado de Ciberseguridad de Google

### 🖥️ Usa comandos de Linux para administrar permisos de archivo

**Descripción:**  
Este proyecto demuestra el uso de **comandos de Linux** para administrar los permisos de archivos y directorios en un entorno organizacional. Se realizó un análisis detallado de los permisos actuales en el sistema de archivos y se aplicaron modificaciones según las políticas de acceso de la empresa.

**📌 Objetivo del proyecto:**

- Examinar los permisos existentes en los archivos y directorios.
- Identificar accesos innecesarios o riesgosos.
- Modificar los permisos para **proteger información confidencial** y evitar accesos no autorizados.

**🔍 Pasos realizados:**

1. **Verificación de permisos de archivos y directorios:**
   - Se utilizó el comando `ls -la` para listar los archivos con sus permisos.
   - Se identificaron archivos con accesos indebidos.

2. **Análisis de la cadena de permisos:**
   - Se interpretaron los permisos de archivos con la notación de **10 caracteres** (`drwxrwxrwx`).
   - Se explicó el significado de cada permiso para usuario, grupo y otros.

3. **Modificación de permisos con `chmod`:**
   - **Quitar permisos de escritura a usuarios no autorizados:**
     ```bash
     chmod o-w project_k.txt
     ```
   - **Modificar permisos de un archivo oculto:**
     ```bash
     chmod u-w,g-w,g+r .project_x.txt
     ```
   - **Otorgar permisos de ejecución a un directorio:**
     ```bash
     chmod g+x drafts
     ```
   - Se verificaron los cambios con `ls -la` después de cada modificación.

**🛠️ Herramientas utilizadas:**

- **Linux Terminal**
- **Comandos básicos:** `ls -la`, `chmod`
- **Administración de permisos en archivos y directorios**

**📌 Aprendizajes clave:**

- Cómo interpretar y modificar permisos en Linux.
- La importancia de restringir accesos innecesarios para mejorar la **seguridad**.
- Uso de `chmod` con distintas combinaciones para cambiar permisos de archivos y directorios.

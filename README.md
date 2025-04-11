# Aplicacion-de-gestion-de-tiempos
## Fase 4 Resumen ejecutivo
Como todo proyecto se requiere un analisis, una planeacion, una ejecucion y al final el uso o  trabajo del mismo de tal manera que se decidio lo siguiente:
- Descripcion: Aplicacion para registro de tiempos agregados
- Problema identificado: No hay control de registros de tiempos muertos y tiempos de produccion.
- Solucion: Implementacion de una aplicacion que registre los tiempos muertos y tiempos de valor agregado.
- Arquitectura: Entorno de desarrollo amigable y facil manejo, USUARIO, ACTIVIDAD, TIEMPO y REGISTRO
## REQUERIMIENTOS, INSTALACION Y CONFIGURACION
### Requisitos de Hardware
- Servidor (si es instalación on-premise o local)  
-	Mínimo 2 núcleos (recomendado 4+ para alta carga de usuarios).  
-	RAM: 4 GB (8 GB para entornos con muchos usuarios o integraciones complejas).  
-	Almacenamiento: SSD con capacidad suficiente para la base de datos y backups
-	Dispositivos cliente
-	Tablets: Procesador de 1 GHz, 2 GB de RAM, sistema operativo actualizado (Windows 10, macOS 10.13, Linux.

### Servidor
-	Sistema operativo: Windows Serve r 2016, Ubuntu LTS 20.04, CentOS 7.
-	Base de datos: MySQL 5.7, PostgreSQL 12, Microsoft SQL Server 2016.  
-	Servidor web : Apache 2.4, Nginx 1.18.  
- Entorno de ejecución: Node.js 14, Java JDK 11, .NET Core 3.1


### **Guía para Instalar un Ambiente de Desarrollo**   

#### **1. Elegir el lenguaje de programación**  
- Ejemplos: Python, JavaScript, Java, C++, etc.  
- Define qué tecnología usarás (ej: desarrollo web, móvil, ciencia de datos).  

---

#### **2. Instalar un editor de código o IDE**  
- **Visual Studio Code** (recomendado para principiantes):  
  - Descarga desde [code.visualstudio.com](https://code.visualstudio.com/).  
  - Extensiones útiles: Prettier (formateo), ESLint (calidad de código), Python, Java Extension Pack, etc.  
- **Alternativas**:  
  - **PyCharm** (Python), **IntelliJ IDEA** (Java), **Eclipse** (Java/C++), **Sublime Text**.  

---

#### **3. Configurar herramientas del lenguaje**  
**Python**:  
1. Descarga Python desde [python.org](https://www.python.org/).  
2. Verifica instalación:  
  
   python --version  
     
3. Crea un entorno virtual:  
   
   python -m venv mi_entorno  
 

**JavaScript/Node.js**:  
1. Instala Node.js (incluye npm) desde [nodejs.org](https://nodejs.org/).  
2. Verifica instalación:  
   
   node -v  
   npm -v  
 

**Java**:  
1. Instala **JDK** (Kit de Desarrollo de Java) desde [Oracle](https://www.oracle.com/java/) o usa [OpenJDK](https://adoptium.net/).  
2. Configura la variable de entorno `JAVA_HOME`.  
3. Verifica:  
   
   javac -version  
 

**C/C++**:  
- En Windows: Usa **MinGW** o **Microsoft Visual Studio**.  
- En Linux/macOS: Instala `gcc` desde la terminal.  

---

#### **4. Sistema de control de versiones (Git)**  
1. Descarga Git desde [git-scm.com](https://git-scm.com/).  
2. Configura usuario:  
 
   git config --global user.name "Tu Nombre"  
   git config --global user.email "tu@email.com"  
   
3. Opcional: Usa **GitHub Desktop** para una interfaz gráfica.  

---

#### **5. Gestores de paquetes**  
- **Python**: `pip` (viene con Python).  
  
  pip install nombre_paquete  
  
- **JavaScript**: `npm` o `yarn`.  
   
  npm install nombre_paquete  
 
- **Java**: Maven o Gradle.  

---

#### **6. Bases de datos (si aplica)**  
- **MySQL**: Instala desde [mysql.com](https://www.mysql.com/).  
- **MongoDB**: Sigue guías en [mongodb.com](https://www.mongodb.com/).  
- **SQLite**: Viene incluido en muchos sistemas.  

---

#### **7. Herramientas de testing**  
- **Python**: `pytest` (instala con `pip install pytest`).  
- **JavaScript**: Jest (`npm install jest --save-dev`).  
- **Java**: JUnit (agrega dependencia en Maven/Gradle).  

---

#### **8. Configuración final**  
- **Variables de entorno**: Asegúrate de que el PATH incluya las rutas de tus herramientas (ej: JDK, Python).  
- **Reinicia la terminal** después de instalar programas para aplicar cambios.  

---

#### **9. Verificación del ambiente**  
- Ejecuta un programa simple (ej: "Hola Mundo") en tu lenguaje.  
- Ejemplo en Python:  

  print("¡Ambiente listo!")  
  
# USO Y CONTRIBUCION
### **1. Referencia Usuario**  
Los usuarios suelen ser empleados, colaboradores o estudiantes que necesitan registrar el tiempo dedicado a tareas, proyectos o actividades.  

#### **Funcionalidades clave**:  
- **Registrar tiempo manual o automático**:  
  - **Manual**: Introducir horas, minutos, fecha y descripción de la actividad.  
  - **Automático**: Usar un cronómetro para iniciar/pausar/detener el tiempo en tiempo real.  
- **Asignar tiempo a proyectos/tareas**: Seleccionar un proyecto o categoría específica desde un menú desplegable.  
- **Adjuntar comentarios o documentos**: Añadir notas explicativas o archivos relacionados (ej: capturas de pantalla).  
- **Visualizar historial**: Revisar registros diarios, semanales o mensuales.  
- **Solicitar ajustes**: Enviar solicitudes de corrección si hay errores en el registro (ej: horas mal ingresadas).  

#### **Pasos típicos para un usuario**:  
1. **Iniciar sesión**: Con credenciales (usuario y contraseña).  
2. **Seleccionar proyecto/tarea**: Desde una lista predefinida por el administrador.  
3. **Activar cronómetro o ingresar tiempo manual**:  
   - Ejemplo: *"Proyecto: Desarrollo Web | Tarea: Diseño de interfaz | Tiempo: 2 horas"*.  
4. **Guardar y enviar para aprobación**: Si la empresa/institución requiere validación del supervisor.  
5. **Consultar reportes**: Ver resúmenes de tiempo invertido por proyecto o período.  

---

### **2. Referencia Administrador**  
El administrador suele ser un líder de equipo, profesor o gestor que supervisa y gestiona los registros.  

#### **Funcionalidades clave**:  
- **Gestionar usuarios**:  
  - Crear/eliminar cuentas.  
  - Asignar roles (ej: usuario básico, supervisor).  
- **Configurar proyectos y tareas**:  
  - Definir proyectos, categorías y asignarlos a usuarios.  
- **Aprobar/rechazar registros**: Validar o solicitar correcciones en los tiempos reportados.  
- **Generar reportes**:  
  - Exportar datos en formatos como Excel, PDF o integrar con herramientas como Excel o Google Sheets.  
  - Analizar métricas: Horas totales, productividad por usuario, avance de proyectos.  
- **Configurar permisos**: Restringir o habilitar acceso a ciertas funciones.  

#### **Pasos típicos para un administrador**:  
1. **Acceder al panel de control**: Con credenciales de administrador.  
2. **Crear un proyecto**:  
   - Ejemplo: *"Proyecto: Curso de Herramientas Tecnológicas | Tareas: Investigación, Prácticas, Examen"*.  
3. **Asignar usuarios al proyecto**: Desde una lista de usuarios registrados.  
4. **Revisar registros pendientes**: Aprobar o solicitar modificaciones.  
5. **Generar reportes mensuales**:  
   - Ejemplo: *"Total de horas invertidas en 'Prácticas' por todos los estudiantes"*.  

---

### **3. Tecnologías Comunes en Estas Aplicaciones**  
- **Frontend**: Interfaz web o móvil (React, Angular, Flutter).  
- **Backend**: APIs para gestionar datos (Node.js, Django, Firebase).  
- **Base de datos**: Almacenar registros (MySQL, MongoDB).  
- **Integraciones**: Con herramientas como Slack, Trello o Microsoft Teams.  

---

### **4. Beneficios de Usar una Aplicación de Registro de Tiempos**  
- **Transparencia**: Claridad en cómo se distribuye el tiempo.  
- **Productividad**: Identificar tareas que consumen más recursos.  
- **Cumplimiento**: Útil para justificar horas en proyectos académicos o laborales.  

---

### **5. Posibles Desafíos**  
- **Resistencia al cambio**: Usuarios que prefieren métodos tradicionales (ej: Excel).  
- **Errores en registros**: Tiempos mal ingresados que requieren corrección.  
- **Privacidad**: Gestionar acceso a datos sensibles.  





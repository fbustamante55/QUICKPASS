# Quickpass - Sistema de Gestión de Pases Rápidos

Sistema de gestión de Quickpasses desarrollado en Java que permite administrar pases rápidos con interfaz gráfica mediante JOptionPane.

## 📋 Descripción

Quickpass es una aplicación de escritorio desarrollada en Java que facilita la gestión de pases rápidos para vehículos. El sistema permite registrar, consultar, modificar y eliminar Quickpasses, además de mantener un historial completo de todas las operaciones realizadas.

## ✨ Características

- **Gestión de Quickpasses**: Agregar, eliminar y modificar pases rápidos
- **Validación de Códigos**: Los códigos deben iniciar con "101" y tener 10 dígitos en total
- **Estados**: Cada Quickpass puede estar Activo o Inactivo
- **Consultas Avanzadas**: 
  - Por código
  - Por filial
  - Por rango de fechas
  - Por código o placa
- **Historial de Operaciones**: Registro completo de todas las acciones realizadas
- **Estadísticas**: Visualización de totales de accesos, Quickpasses activos, inactivos y eliminados

## 🛠️ Requisitos

- Java JDK 8 o superior
- NetBeans IDE (recomendado) o cualquier IDE compatible con Java
- Sistema operativo: Windows, Linux o macOS

## 📁 Estructura del Proyecto

```
Quickpass/
├── src/
│   ├── main.java              # Clase principal con menú de opciones
│   ├── Quickpass.java         # Clase modelo para Quickpass
│   ├── GestorQuickpass.java   # Gestor de operaciones CRUD
│   └── ArchivoHistorial.java  # Gestión del historial de operaciones
├── build/
│   └── classes/               # Archivos compilados (.class)
├── build.xml                  # Archivo de configuración de Ant
└── Historial.txt              # Archivo de registro de operaciones
```

## 🚀 Instalación y Compilación

### Opción 1: Usando NetBeans

1. Abre NetBeans IDE
2. Selecciona `File` → `Open Project`
3. Navega hasta la carpeta `Quickpass`
4. Abre el proyecto
5. Compila el proyecto con `Build` → `Build Project` (F11)
6. Ejecuta el proyecto con `Run` → `Run Project` (F6)

### Opción 2: Compilación Manual

```bash
# Navegar a la carpeta src
cd Quickpass/src

# Compilar todos los archivos Java
javac *.java

# Ejecutar la aplicación
java main
```

## 📖 Uso

Al ejecutar la aplicación, se mostrará un menú con las siguientes opciones:

1. **Agregar Quickpass**: Registra un nuevo Quickpass con filial, código y placa
2. **Eliminar Quickpass por Código**: Elimina un Quickpass usando su código
3. **Eliminar Quickpass por Placa**: Elimina un Quickpass usando su placa
4. **Visualizar Quickpasses**: Muestra todos los Quickpasses activos
5. **Visualizar Quickpasses Eliminados**: Muestra todos los Quickpasses eliminados
6. **Consultar Quickpass**: Consulta el estado de un Quickpass por código
7. **Consultar por Filial**: Muestra todos los accesos de una filial específica
8. **Consultar por Rango de Fechas**: Consulta accesos entre dos fechas
9. **Consultar por Código o Placa**: Busca accesos por código o placa
10. **Cambiar Estado Quickpass**: Activa o desactiva un Quickpass
11. **Total de accesos registrados**: Muestra el historial completo
12. **Total de accesos por filial**: Consulta accesos por filial
13. **Total de quickpass registrados**: Muestra el total de Quickpasses registrados
14. **Total de quickpass Activos e Inactivos**: Estadísticas de estados
15. **Total de quickpass eliminados**: Cantidad de Quickpasses eliminados
16. **Salir**: Cierra la aplicación

## 🔑 Validación de Códigos

Los códigos de Quickpass deben cumplir con el siguiente formato:
- Deben iniciar con "101"
- Deben tener exactamente 10 dígitos en total
- Ejemplo válido: `1011234567`

## 📝 Historial de Operaciones

Todas las operaciones se registran automáticamente en el archivo `Historial.txt` con la siguiente información:
- Acción realizada
- Código del Quickpass
- Placa del vehículo
- Filial
- Resultado (Aceptado/Rechazado)
- Fecha y hora de la operación

## 👥 Autor

**Fabia**

## 📄 Licencia

Este proyecto está bajo la licencia por defecto de NetBeans.

## 🔧 Tecnologías Utilizadas

- Java
- Swing (JOptionPane)
- Ant (build.xml)

## 📞 Soporte

Para reportar problemas o sugerencias, por favor contacta al autor del proyecto.


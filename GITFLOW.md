# Gitflow

Gitflow es una metodología de ramificación (branching) para el control de versiones con Git, que se enfoca en el manejo de versiones de software en proyectos complejos con varios desarrolladores y ramas de desarrollo activas.

## Principales características
Utiliza dos ramas principales: master y develop.
Utiliza ramas secundarias para el desarrollo de características (feature), correcciones de errores (hotfix), versiones de lanzamiento (release) y versiones estables (support).
Las ramas feature se crean a partir de develop y se fusionan de nuevo en develop cuando la característica está completa.
Las ramas hotfix se crean a partir de master y se fusionan de nuevo en master y develop una vez que el error ha sido corregido.
Las ramas release se crean a partir de develop y se fusionan en master y develop una vez que la versión de lanzamiento está completa.
Las ramas support se crean a partir de master para el mantenimiento de versiones antiguas de un proyecto.

### Ventajas

- Facilita el manejo de versiones de software en proyectos complejos con varios desarrolladores y ramas de desarrollo activas.
- Permite una separación clara entre el desarrollo de nuevas características, corrección de errores y mantenimiento de versiones antiguas.
- Ayuda a garantizar que las versiones de producción sean estables y estén libres de errores críticos.

### Desventajas

- Puede resultar complejo de implementar y mantener en proyectos pequeños o con pocos desarrolladores.
- Puede resultar en un gran número de ramas, lo que puede ser confuso para algunos desarrolladores.


## Flujo de trabajo

El flujo de trabajo de Gitflow se basa en las siguientes fases:

1. Creación de la rama develop a partir de master.
2. Creación de ramas feature a partir de develop para desarrollar nuevas características.
3. Una vez completada una característica, se fusiona la rama feature de nuevo en develop.
4. Creación de la rama release a partir de develop para preparar la versión de lanzamiento.
5. Una vez completada la versión de lanzamiento, se fusiona la rama release en master y develop.
6. Creación de la rama hotfix a partir de master para corregir errores críticos en la versión en producción.
7. Una vez corregido el error, se fusiona la rama hotfix de nuevo en master y develop.
8. Creación de la rama support a partir de master para el mantenimiento de versiones antiguas.

### Ejemplo
Creación de ramas paso a paso

### **Ramas Principales**
![Gitflow - 1](https://github.com/ErikssonHerlo/ManualControlVersiones/blob/main/images/gitflow-1.svg)

### **Ramas de Función o Features**
![Gitflow - 1](https://github.com/ErikssonHerlo/ManualControlVersiones/blob/main/images/gitflow-2.svg)

### **Ramas de Publicación o Realeses**
![Gitflow - 1](https://github.com/ErikssonHerlo/ManualControlVersiones/blob/main/images/gitflow-3.svg)

### **Ramas de Corrección o Hotfixes**
![Gitflow - 4](https://github.com/ErikssonHerlo/ManualControlVersiones/blob/main/images/gitflow-4.svg)





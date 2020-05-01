# Gitflow

![](https://ws001.sspa.juntadeandalucia.es/unifica/documents/1912026/21060440/image2017-3-22+12-25-43.png/a252c84b-b427-41bf-9b81-b0dd971757b4?t=1497250956690)


Gitflow Workflow es un diseño de flujo de trabajo Git; es ideal para proyectos que tienen un ciclo de lanzamiento programado, ademas de ser un flujo de trabajo que no agrega ningún concepto o comando nuevo más allá de lo basico, sin embargo, asigna roles muy específicos a diferentes ramas y define cómo y cuándo deben interactuar.

## Ramas principales
 Gitflow se basa en dos ramas principales con una vida útil infinita: 

- **`master-`** es la rama principal donde el código fuente de HEAD siempre refleja un estado listo para producción.

- **`develop-`** es la rama principal donde el código fuente de HEAD refleja un estado con los últimos cambios de desarrollo entregados para la próxima versión 

## Ramas de soporte
> Durante el ciclo de desarrollo de un proyecto bajo la modalidad de gitflow, se utiliza una variedad de ramas de soporte que puede ayudar al desarrollo paralelo entre los miembros de un equipo, esto facilita el seguimiento de las características, prepararse para lanzamientos de producción y ayudar a solucionar rápidamente los problemas de producción en vivo; a diferencia de las ramas principales, estas ramas siempre tienen un tiempo de vida limitado, ya que posteriormente se eliminarán: 

- ### Ramas de caracteristicas
    **`feature-*-`** Las ramas de características se utilizan para desarrollar nuevas características para los próximos lanzamientos. Puede ramificarse `develop` y debe fusionarse `develop`. 

- ### Ramas de revisión
    **`hotfix-*-`** Las ramas de revisión son necesarias para actuar inmediatamente sobre un estado no deseado de master. Puede ramificarse de master y debe fusionarse si o si con `master` y `develop`. 

- ### Ramas sucurzales de lanzamiento
    **`release-*-`** Las sucursales de lanzamiento apoyan la preparación de una nueva versión de producción. Permiten corregir muchos errores menores y preparar metadatos para un lanzamiento. Puede ramificarse de`develop` y debe fusionarse con `master` y `develop`.

# Diferencias entre git merge y git merge --no--ff
## git merge
>git marge sirve para unir dos o mas historias de desarrollo juntas, es decir, que sirve para incorporar cambios en los comits, nombrados en la rama actual.
!["Imagen de referencia"](https://wac-cdn.atlassian.com/dam/jcr:86eba9ec-9391-45ea-800a-948cec1f2ed7/Branch-2.png?cdnVersion=983)
![](https://wac-cdn.atlassian.com/dam/jcr:83323200-3c57-4c29-9b7e-e67e98745427/Branch-1.png?cdnVersion=983)
Las confirmaciones de fusión son únicas frente a otras confirmaciones en el hecho de que tienen dos confirmaciones principales. Al crear una confirmación de fusión, Git intentará fusionar automáticamente las historias separadas. Si Git encuentra un dato que se cambia en ambos historiales, no podrá combinarlos automáticamente. Este escenario es un conflicto de control de versiones y Git necesitará la intervención del usuario para continuar. 
## git merge --no--ff
>En cambio **git merge --no--ff** es una extencion de git marge que puede crear una confirmacin de fución en todos los casos, incluso cuando la fusión podría resolverse con un avance rápido.


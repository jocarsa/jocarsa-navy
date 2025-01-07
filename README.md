# jocarsa-navy
## Librería PHP para convertir automáticamente Markdown a HTML

Mediante esta librería es posible convertir archivos de markdown directamente en HTML

### Escenarios de uso:

* Documentación de aplicaciones
* Creación de documentos en línea
* Escribir libros 

### Instrucciones para su uso:

1. Descarga la librería desde GitHub
   1. Accede a la url: [Enlace al repositorio de GitHub](URL "https://github.com/jocarsa/jocarsa-navy/")
   2. Utiliza el botón para descargar repositorio completo
3. Situa la librería cerca de tu proyecto
4. Incluye la librería en tu proyecto con **include** o **require**
5. Llama a la librería para convertir tu documento (*Sigue el ejemplo que te indicamos a continuación*)

### URL para conseguir la librería:
Puedes conseguir la librería desde: 
[Enlace al repositorio de GitHub](URL "https://github.com/jocarsa/jocarsa-navy/")

### Ejemplo de uso

Para insertar el código dentro de tu proyecto, debes hacerlo mediante el comando **include**:

``` include "jocarsa | navy.php"; ```

Ejemplo completo de uso:

```
<?php
	include "jocarsa | navy.php";
	$markdownFile = "muestra.md";
	$markdownContent = file_get_contents($markdownFile);
	$htmlContent = markdownToHtml($markdownContent);
?>
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Conversión Markdown a HTML</title>
</head>
<body>
<?php
echo $htmlContent;
?>
</body>
</html>
```

### Historial de características

- [x] Publicar librería
- [x] Soporte para markdown
- [ ] Eliminar caracter | para compatibilidad con Windows

Separador en HTML
<hr>
Separador en markdown:

****

Esto es  un texto

### Estado actual del soporte de elementos en la librería:

| Nombre de la característica | Estado             |
|-----------------------------|--------------------|
|Titulares                    |[x]Implementado     |
|Enlaces                      |[x]Implementado     |
|Gráficas                     |[ ]Pendiente        |


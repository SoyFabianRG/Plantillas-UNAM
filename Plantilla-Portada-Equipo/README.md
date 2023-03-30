<h1 align="center"> Plantilla Portada Equipo </h1>

Este proyecto es una plantilla de portada para tus tareas y trabajos en equipo en la Facultad de Ciencias.

## Tabla de Contenido

- [Demo](#demo)
- [Características](#características)
- [Licencia](#licencia)
- [Autor](#autor)

## Demo

<div align="center">

<img src="https://i.imgur.com/5uWAz5w.jpg" width="300">

</div>

## Características

Esta plantilla fue diseñada para ser usada por estudiantes de la Facultad de Ciencias de la UNAM. Si prefieres los escudos en color negro, dentro directorio [Graphics](../Graphics) los podrás encontrar: recuerda reemplazar la ruta en el comando `\includegraphics` para poderlos cambiar.

En caso de que seas estudiante de otra facultad o institución, puedes cambiar los escudos de la parte superior por los de tu respectiva escuela siguiendo estos pasos:

1. Agregar los escudos en formato jpg, png o pdf al directorio [Graphics](../Graphics).
2. Reemplazar la ruta del archivo dentro del código en el comando `\includegraphics` y realizar los ajustes de tamaño que consideres pertinentes.

### Nota:

Puede ser que al incorporar este código a tu proyecto tengas algún error debido a los márgenes, ya sea que la portada se vea chueca o te aparezca una advertencia del tipo `\vbox` y `\hbox`. Este documento fue diseñado con un margen de 2.54 cm (que es el estándar de las normas APA); sin embargo, si tu proyecto tiene un margen distinto, deberás hacer lo siguiente para corregir los posibles errores:

1. Dentro del entorno `titlepage` y antes del comando `\centering`, agrega el comando
    ```latex
    \newgeometry{margin=2.54cm}
    ```
    el cual hará que a partir de ahí se establezca un margen de 2.54 cm en el documento.

2. Después del comando `\end{titlpage}`, debes agregar el comando
    ```latex
    \restoregeometry
    ```
    para que el margen de 2.54 cm afecte únicamente a la hoja con la portada. Esto hará que LaTeX regrese al margen que habías especificado en tu preámbulo y puedas seguir trabajando con él por el resto del documento.

Una opción alternativa a la anterior es que realices la portada en un archivo diferente, luego podrás juntar el documento con la portada y el documento con tu proyecto usando alguna herramienta como [iLovePDF](https://www.ilovepdf.com/es) u otra.

## Licencia

> This project is licensed under the MIT License

## Autor

Hecho por [Fabián Ríos](https://www.linkedin.com/in/soyfabianrg/)

# Proyecto-Zamora

**Contenido**

Para el desarrollo de este proyecto, se utilizaron las herramientas de Unity y Visual Studio Code con HLSL. En base a lo solicitado, el shader cuenta con

- Un color albedo para la iluminación.
- Un mapa de textura y un mapa de normales.
- Parámetros para controlar la intensidad del mapa de normales.
- Está codificado con Lambert.
- Cuenta Phong, Rim y Ramp Texture con Banded.

**Desarrollo**

- Para este proyecto se tomaron de referencia los trabajos realizados en el transcurso del primer parcial, aplicando los conocimientos adquiridos dentro del código del proyecto y se descargó un modelo 3D del sitio www.assetstore.unity.com, de donde se decidió trabajar con el modelo llamado Angry Log.

- Se manejó un Shader en Unlit con un modelo básico de luz Lambert y una estructura de código que incluye nombre, las propiedades, el subshader, tags y cgprogram, en los cuales se codifica lo necesario para lograr el efecto deseado. Además, se utiliza el pragma para mostrar el sombreador de superficie.
- Se trabaja con efectos como el Phong para para crear un efecto de brillo incluyendo dentro de él características como el SpecularColor que es el color de la luz, el SpecularPower que controla la intensidad de la luz, el SpecularGloss que mide la extensión del brillo y el GlossSteps que permite agrandar los pasos de cada sección. También se codifica un Normal Map para dar textura tipo relieve al modelo junto con el Normal Strenght para poder configurar la dureza de la textura.
- El Wrap sirve para controlar la caída de la sombra, así como su claridad y oscuridad. El Rim Light es para lograr un efecto de iluminación en las orillas del modelo.
- Banded nos da una iluminación con que va desde el blanco hasta el negro, y funciona a través de steps para controlar la cantidad de veces que aparecerá en el modelo 3D.
- Por último, se incorpora el Ramp Texture que nos agrega una imagen en escala de grises en base al modelo que se está trabajando.

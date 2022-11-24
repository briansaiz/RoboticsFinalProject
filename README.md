
<h1 align="center"> :star2:  Robótica - Proyecto Final :star2: </h1> 

Desarrollo de un sistema robotizado Pick and Place, para la automatización de procesos de ensamble de herramientas de sujeción (gripper), a partir de la implementación de un mecanismo neumatico adaptado al robot industrial ABB IRB 140.

---


> ## Autores
> 
> - [Camilo Andrés Borda Gil](https://github.com/Canborda) (caabordagi@unal.edu.co) 
> - [Daniel Alexander Cruz Ruiz ](https://github.com/Danacruzrui) (danacruzrui@unal.edu.co) 
> - [Cristhian Ferney Pulido Garcia](https://github.com/CristhianPu) (cfpulidog@unal.edu.co) 
> - [Brian Camilo Saiz Cavanzo](https://github.com/briansaiz) (brcsaizca@unal.edu.co)
---


## Diseño de herramienta porta ventosa 
Para el desarrollo de este proyecto se inció con el diseño de la herramienta porta ventosa, partiendo de las [especifiaciones del producto](https://library.e.abb.com/public/81a35b138c2342b5b9455e5696a09484/3HAC027400%20PM%20IRB%20140-en.pdf) del manipulador IRB 140, especificamente de las dimensiones de la brida para herramientas y las cuales se pueden ver acontinuación

<p align="center"><img height=250 src="./assets/flange.png" alt="holes on mounting flange" /></p>

A partir de las dimensiones de las ventosas y acoples dispuestos en el laboratorio y de la brida para herramientas del manipulador IRB 140 se diseño el porta ventosa tal que se adaptase a cada uno de estos elementos.

Como desde un principio se establecio que el proceso de fabricación de la herramienta iba a ser por manufactura aditiva se tuvo que disminuir los concetradores de esfuerzos a traves de la presencia de chaflanes de radios bastantes pronuncioados, todo esto para evitar la fractura de la herramienta por lo anisotropia que se presentan en las piezas fabricadas por MDF en las secciones paralelas a la base de construcción.

Adicionalmente, se estableció como criterio de diseño que el TCP deberia estar alineado al eje deacción de la articulación seis, de tal manera que esta fuese "simetrica" al rededor del eje z. Es así, que la herramienta porta ventosa final diseñada es la que se puede observar a continuación

<p align="center">
    <img src="https://user-images.githubusercontent.com/22859451/203667176-c2b69f29-7fee-4a53-9b09-2f1c754cb256.gif" alt="tool" width="400" /> <br/>
    <a href="https://cad.onshape.com/documents/87fae4edd689d660c54eaff0/w/6fba91a9acc885ef7d218d0f/e/0715371a4d1c41e46584bd85">
        OnShape modelo CAD de la herramienta porta ventosa 
    </a>
</p>

Para poder interactuar y ver con mayor profundidad la herramienta porta ventosa se sugiere verla en <a target="_blank" href="https://cad.onshape.com/documents/87fae4edd689d660c54eaff0/w/6fba91a9acc885ef7d218d0f/e/0715371a4d1c41e46584bd85"> OnShape</a>.

Los planos de fabricación se pueden ver en la carpeta de [planos](https://github.com/briansaiz/RoboticsFinalProject/blob/main/planos/Portaherramienta.pdf)

## Diseño del Gripper
De cara a hacer el proceso de ensamble lo más ágil posible se decidió que el gripper debería tener el menor número de piezas, es por esto que el gripper diseñado tiene tan sólo cinco piezas.

Dado que el diametro interior de la ventosa es de 21 mm se tuvo como requisito de diseño adicional de que las piezas deberían medir por lo menos 25 mm de ancho, de esta manera se garantizaría que no hubiesen fugas de aire al momento de que la ventosa sujetase alguna pieza. 

Es así que el gripper diseñado fue el siguiente.

<p align="center">
    <img src="https://user-images.githubusercontent.com/22859451/203692858-d24da7a8-6eb1-4fa2-83ce-b48311b2ce65.gif" alt="tool" width="400" /> <br/>
    <a href="https://cad.onshape.com/documents/c2d00034c333774d1d1069d7/w/73e6d23a367311dee87d113d/e/b44da0999e3f25b7aa20ed3b?renderMode=0&uiState=637ef10935e2210728d412a8">
        OnShape modelo CAD del Gripper
    </a>
</p>

Al momento de crear las diferentes trayectorias en Robot Studio se encontró con que se dificultaba el proceso de situar los targets en las piezas en los lugares especificos y necesarios para que la ventosa se ubicara adecuadamente. Es por esto que lo que se decidio fue crear elementos facilitacen la ubicación de los targets en Robot Studio, de ahí que las piezas tanto del gripper como de las bases del Pick y del Place tengan trazadas circunferencias en posiciones determinadas.


Para poder interactuar y ver con mayor profundidad la herramienta porta ventosa se sugiere verla en <a target="_blank" href="https://cad.onshape.com/documents/c2d00034c333774d1d1069d7/w/73e6d23a367311dee87d113d/e/b44da0999e3f25b7aa20ed3b"> OnShape</a>.

Los planos de fabricación se pueden ver en la carpeta de [planos](https://github.com/briansaiz/RoboticsFinalProject/blob/main/planos/GRIPPER.pdf).


A continuación se puede observar como el diseño del gripper es totalmente funcional.

<p align="center">
    <img src="https://user-images.githubusercontent.com/22859451/203696397-a5736d6c-0529-418b-860c-52b43215df62.gif" alt="tool" width="400" /> <br/>
    <a href="https://cad.onshape.com/documents/c2d00034c333774d1d1069d7/w/73e6d23a367311dee87d113d/e/b44da0999e3f25b7aa20ed3b?renderMode=0&uiState=637ef10935e2210728d412a8">
        OnShape modelo CAD del Gripper funcionando
    </a>
</p>

## Modelo RobotStudio 

<p align="center">
    <img src="https://user-images.githubusercontent.com/53317895/203775781-52d16c12-24b1-4f01-b353-3115c0787dd2.gif" alt="tool" width="400" /> <br/>
 
        OnShape modelo CAD del Gripper funcionando
    </a>
</p>


![RobotStudio](https://user-images.githubusercontent.com/53317895/203775781-52d16c12-24b1-4f01-b353-3115c0787dd2.gif)
-
## Código RAPID


## Desarrollo  (video tipo presentación)

## Conclusiones 

* Al momento de diseñar un proceso de ensamble, manufactura o de cualquier indole industrial es preciso tener en cuenta cuales son los requisitos y limitaciones tanto de espacio, dispositivo como a tareas a realizar, pues son estas las que definiran los diseños desde herramientas hasta los procesos mismos.



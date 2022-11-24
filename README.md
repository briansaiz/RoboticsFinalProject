# RoboticsFinalProject



<h1 align="center"> :star2:  Robótica - Proyecto Final :star2: </h1> 

Desarrollo de un sistema robotizado Pick and Place, para la automatización de procesos de ensamble de herramientas de sujeción (gripper), a partir de la implementación de un mecanismo neumatico adaptado al robot industrial ABB IRB 140.

---


> ## Autores
> 
> - [Camilo Andrés Borda Gil](https://github.com/Canborda) (caabordagi@unal.edu.co)  :+1:
> - [Daniel Alexander Cruz Ruiz ](https://github.com/Danacruzrui) (danacruzrui@unal.edu.co) 🥒👌 
> - [Cristhian Ferney Pulido Garcia](https://github.com/CristhianPu) (cfpulidog@unal.edu.co) :hibiscus:
> - [Brian Camilo Saiz Cavanzo](https://github.com/briansaiz) (brcsaizca@unal.edu.co) 🌞
---


## Diseño de la herramienta porta ventosa 
Para el desarrollo de este proyecto se inció con el diseño de la herramienta porta ventosa, por lo cual se partió de las [especifiaciones del producto](https://library.e.abb.com/public/81a35b138c2342b5b9455e5696a09484/3HAC027400%20PM%20IRB%20140-en.pdf) del manipulador IRB 140, en dónde se busco las dimensiones de la brida para herramientas las cuales se pueden ver acontinuación

<p align="center"><img height=250 src="./assets/flange.png" alt="holes on mounting flange" /></p>

A partir de las dimensiones de las ventosas y acoples dispuestos en el laboratorio y de la brida para herramientas del manipulador IRB 140 se diseño el porta ventosa tal que se adaptase a cada uno de estos elementos.

Adicionalmente, se estableció como criterio de diseño en el grupo que el TCP deberia estar alineado al eje deacción de la articulación seis de tal manera que está fuese "simetrica" al rededor del eje z. Es así que la herramienta porta ventosa final es la que se observa a continuación.


https://user-images.githubusercontent.com/22859451/203666171-937f94a2-ad40-4552-934c-bee334c8245c.MOV

https://user-images.githubusercontent.com/22859451/203666726-d15d8a68-45b0-4754-b631-551346763640.mp4

<p align="center">
    <img src="https://user-images.githubusercontent.com/22859451/203666171-937f94a2-ad40-4552-934c-bee334c8245c.MOV
" alt="tool" width="400" /> <br/>
    <a href="https://cad.onshape.com/documents/f980fe7178465a5e85356d19/w/a751aae7c3f868ba172fc952/e/3687fe216ca7c6a9660936e8?renderMode=0&uiState=62b8723dcd67bc23dc436eb9">
        OnShape CAD Model 
    </a>
</p>


https://cad.onshape.com/documents/682c4abdff8d5b1968578e1c/w/8376a3a698a6c6d8a3e2e53d/e/6255906a6bfccb92809b06ab?renderMode=0&uiState=637eae52fdd77b21d4b9de0d

Based on those dimensions, the team designed the tool shown below, made up of four parts: a base and a cap build with 3D printing, a spring and a marker. To see the tool model with more detail go to <a target="_blank" href="https://cad.onshape.com/documents/02a2a5fe444c220951f7859a/w/4de4b01172907f48fb48adbe/e/481b6444fafd2e1357d20adc">Visualize CAD model with OnShape</a>.

## Diseño del Gripper 
## Modelo RobotStudio 
## Código RAPID
## Desarrollo  (video tipo presentación)
## Conclusiones 

{% assign imagesample = site.data[site.metadata] | where_exp: 'item','item.format contains "image"' | first %}
{% capture imagesampleid %}{{imagesample.objectid | default: "https://www.lib.uidaho.edu/collectionbuilder/demo-objects/mg101_b6_photographs_01.jpg"}}{% endcapture %}

## Ida Esbra. 
A mediados de la década de 1970, el arte conceptual irrumpió en el panorama artístico, impulsando a una nueva generación de fotógrafos a explorar nuevas formas de expresión. Entre ellos se encontraba Ida Esbra (Holanda,1929- Barranquilla, 2009). Una artista cuya obra de transita entre dos caminos: el antropológico y el documental-artístico. Esbra experimentó con diversas técnicas fotográficas e introdujo elementos que alteraban el paisaje en la fotografía, a través del juego con la luz, texturas y composición. Su trabajo es un testimonio de los procesos artísticos de experimentación y exploración del arte conceptual entre los años setenta y ochenta en Colombia. 


### Include Collection Items

The template provides includes to pull your collection objects and metadata into your interpretive page, allowing you to write with your materials directly embedded in the content.

#### Include an Image

- Image --> `{% raw %}{% include feature/image.html objectid="coll031" width="75" %}{% endraw %}`

{% include feature/image.html objectid=imagesampleid width="75" %}




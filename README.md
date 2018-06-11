# Diccionario de hunspell para el idioma chaná

| This readme in other languages |
| --------- |
| [English](README-en.md) · [Español](README.md)|

## Sobre este proyecto
### El idioma chaná
El idioma chaná es una lengua originaria de la cuenca del Plata de América del Sur, en lo que 
actualmente son las Repúblicas de Argentina y Uruguay, hablada por la etnia chaná, que habitó 
esos territorios durante mucho tiempo antes de la llegada de la conquista española.

Como todas las lenguas indígenas de América (el "Abya Yala"), sufrió un proceso de declive 
producto de las políticas represivas de los gobiernos de la época y la persecusión de estas 
naciones por parte del conquistador. A diferencia de las grandes lenguas indígenas americanas 
como el náhuatl, el quechua o el guaraní que fueron utilizados como vehículos para la 
evangelización de los nativos, las lenguas de la cuenca del Plata, dada su escasa población, 
fueron perdiendo terreno y para mediados del siglo XIX ya casi no habían hablantes. Durante 
mucho tiempo se creyó que no habían quedado registros más que unos breves textos (el "Códice 
Vilardebó" para el charrúa, el "Compendio del idioma de la Nación Chaná" para el chaná y el 
"Catecismo güenoa" para el güenoa).

Sin embargo, este trozo de cultura que se pensaba que estaba perdido volvió a la luz cuando en 
el año 2005 el entrerriano Blas Jaime, posiblemente el último hablante de esta lengua, comenzó a 
buscar gente que hablara la lengua a través de los medios de prensa. Y con ayuda del lingüista 
Pedro Viegas Barros, comenzó un trabajo de recuperación y difusión para que las nuevas 
generaciones de esas tierras pudieran conocer un pasado propio que les es desconocido.

### El proyecto
Este proyecto intenta ofrecer al público de forma accesible un diccionario para la lengua chaná
que permita a aquellos quienes escriban texto en este idioma, obtener una verificación 
ortográfica automática de las palabras mal escritas según han sido descritas.

Dado que no hay un estándar oficial, se intenta seguir las denominaciones dadas por los 
respectivos autores de las fuentes consultadas, las cuales son fuente de inspiración de 
esta obra.

El "diccionario" se compone de un archivo de diccionario, que no es más que un archivo de texto 
con la lista de palabras y unas denominaciones de formato, y otro archivo de afijos, que define 
esos formatos entre otras configuraciones. El archivo de diccionario no se trata de un 
diccionario en el sentido de la palabra (una lista de palabras y su definición), sino 
simplemente una lista de las palabras o unidad conceptual, que el software (hunspell) toma como 
referencia para comparar con la palabra escrita por el usuario.

### Código de idioma
La lengua chaná actualmente no posee un código ISO 639, por lo cual se usa el pseudocódigo 
`sai-chn`, compuesto de la siguiente forma: el código [ISO 639-5](https://www.loc.gov/standards/iso639-5/id.php) `sai` ("South American Indian languages")
más las letras `chn` de "CHaNá".

## Fuentes consultadas
* Larrañaga, Dámaso Antonio (1923) [1815]. "[Compendio del idioma de la Nación Chaná](http://etnolinguistica.wdfiles.com/local--files/biblio%3Alarranaga-1923-compendio/larranaga_1923_compendio.pdf)". Escritos de D. Antonio Larrañaga. III. Instituto Histórico y Geográfico del Uruguay.
* Sabat Pebet, Juan Carlos. Figueira, José Joaquín (1969). "[Las lenguas indígenas del Uruguay](https://www.estudioshistoricos-en.edu.uy/assets/080-bolet%C3%ADn-hist%C3%B3rico-n%C2%BA-120---123---a%C3%B1o-1969.pdf)". 120-123. Boletín Histórico del Ejército. Estado Mayor General del Ejército, Uruguay. pp 188-220.
* Jaime, Blas. Viegas Barros, Pedro (2013). "La lengua Chaná: patrimonio cultural de Entre Ríos". Editorial de Entre Ríos. p 144.

## Instalación
Actualmente no hay paquetes disponibles para la instalación a través de repositorios o tiendas 
de aplicaciones.

Para instalar manualmente:
1. Hacer una copia local de este repositorio con git:
```
git clone https://github.com/fuckyourselfup/hunspell-sai-chn.git
```
2. Moverse a la carpeta descargada y copiar los archivos de diccionario en la ubicación indicada, por ejemplo en GNU/Linux en "/usr/share/hunspell":
```
cd hunspell-sai-chn
sudo mv sai-chn.* /usr/share/hunspell
```
3. Probar el diccionario. En una terminal, ejecutar el siguiente comando:
```
hunspell -d sai-chn
```
En el interactivo, escribir la palabra seguida de ENTRAR (para salir: Ctrl+C). Ejemplo de salida:
```Shell
usuario@localhost:~$ hunspell -d sai-chn
Hunspell 1.6.2
uelcaimarr
& uelcaimarr 1 0: uelcaimár

opatiam
& opatiam 1 0: opatimá
```

## Colaboración
Toda colaboración es bienvenida. Por cualquier comentario, sugerencia o petición, diríjase a la 
sección "Issues" y abra un nuevo *ticket* explicando su intención.

## Licencia y términos de uso
Consulte el archivo [LICENSE.md](LICENSE.md) para conocer los términos de uso de esta obra.


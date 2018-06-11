# Hunspell dictionary for chaná language

| This readme in other languages |
| --------- |
| [English](README-en.md) · [Español](README.md) |

## About this project
### About chaná language
TO DO

### About the project
TO DO

### Language code
Chaná language currently does not have a ISO 639 code, therefore it is used a pseudocode `sai-chn`,
which was made as follows: the [ISO 639-5](https://www.loc.gov/standards/iso639-5/id.php) code `sai` ("South American Indian languages") plus
`chn` characters from "CHaNá".

## Used sources
* Larrañaga, Dámaso Antonio (1923) [1815]. "[Compendio del idioma de la Nación Chaná](http://etnolinguistica.wdfiles.com/local--files/biblio%3Alarranaga-1923-compendio/larranaga_1923_compendio.pdf)". Escritos de D. Antonio Larrañaga. III. Instituto Histórico y Geográfico del Uruguay.
* Sabat Pebet, Juan Carlos. Figueira, José Joaquín (1969). "[Las lenguas indígenas del Uruguay](https://www.estudioshistoricos-en.edu.uy/assets/080-bolet%C3%ADn-hist%C3%B3rico-n%C2%BA-120---123---a%C3%B1o-1969.pdf)". 120-123. Boletín Histórico del Ejército. Estado Mayor General del Ejército, Uruguay. pp 188-220.
* Jaime, Blas. Viegas Barros, Pedro (2013). "La lengua Chaná: patrimonio cultural de Entre Ríos". Editorial de Entre Ríos. p 144.

## Installation
Currently there is not any precompiled package available for installation through repositories or 
app stores.

To install it manually:
1. Make a local copy of this repository by running git:
```
git clone https://github.com/fuckyourselfup/hunspell-sai-chn.git
```
2. Move to downloaded folder and copy dictionary files to the right location, for example in GNU/Linux to "/usr/share/hunspell":
```
cd hunspell-sai-chn
sudo mv sai-chn.* /usr/share/hunspell
```
3. Test dictionary. Open a terminal and run the following command:
```
hunspell -d sai-chn
```
In the interactive mode opened, write the desired word followed by ENTER key (to exit press: Ctrl+C). For example, the output could be like this one:
```Shell
user@localhost:~$ hunspell -d sai-chn
Hunspell 1.6.2
uelcaimarr
& uelcaimarr 1 0: uelcaimár

opatiam
& opatiam 1 0: opatimá
```

## Contribute
All help is welcome. To make any comment, suggestion or request, please go to "Issues" and open a new ticket explaining there what you want or need.

## License and terms of use
To know about this work's term of use please read [LICENSE.md](LICENSE.md).


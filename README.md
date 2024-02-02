# Taller1scripting
## Punto 3 Lista de comandos usados
- Caracol: echo hello world
- Mariposa: pwd
- Oruga: ls
- Hormiga: cat access.log
- Telaraña: tail -5 access.log
- Ballena: cd > take-the-command-challenge
- Cachalote: mkdir tmp tmp/files
- Delfín: cp take-the-command-challenge to tmp/files
- Pez: mv take-the-command-challenge tmp/files
- Pez rayado: cp -s tmp/files/take-the-command-challenge take-the-command-challenge
- Pez globo: find -delete
- Lobo: find . -name "*.doc" -delete
- Avispa: grep  GET access.log
- Mariquita: grep -l 500 **
- Grillo: ls access.*
- Araña: grep '500' -rh
- Escorpión: find . -name 'access.log*' -exec awk '{print $1}' {} \;
- Mosca: ls -s | wc -l
- Gusano: sort access.log
- Bacteria: grep -c 'GET' access.log
- Simio: tr ';' '\n' <split-me.txt
- Perro: echo {1..100}
- Zorro: rm -r **/*.txt
- Gato: jq -s add *
- Felino: find -type f -exec basename {} \;
- Tigre: rm .r *
- Caballo: ls | tr " " .
- Unicornio: dirname **/*.tf| sort -u
- Vaca: basename -s **/[0-9]*;
- Cerdo: sed -n '25p' faces.txt
- Ratón: tac reverse-me.txt
- Hámster: cat -n faces.txt | sort -u -k 2 | sort -n | cut -f 2
- Oso: sort < random-numbers.txt | uniq | factor | awk 'NF==2' | wc -l
- Panda: cat access.log.* | awk '{print $1}' | sort | uniq -d
- Pollito: grep -h -B1 404 **/access.log*|grep -vE '404|--'
- Pavo Real: for f in t*; do cmp -s bas* $f || echo $f; done
- Rana: cat "`find -type f`"
- Dragon: cat file-with-tabs.txt | grep -P '\t' | wc -l
- Flor: find . | grep -vE '.txt$|.exe$' |xargs rm
- Flor roja: rm ./-*
- Flor rosa:sort -unk2 *
- Flor amarilla: awk '/tcp .*LISTEN$/{print $4}' netstat*|awk -F: '{print $2}'|sort -nr
![image](https://github.com/ilpalomo/Taller1scripting/assets/113053206/2de259e9-2121-4305-84cd-adfb684c2f15)
### Descripción breve de lo realizado
Gracias a la información proporcionada en "https://www.stationx.net/unix-commands-cheat-sheet/" se lograron realizar con éxito algunos de los comandos en el desafío, sin embargo algunos de estos eran bastante complejos y se optó por leer las posibles soluciones que brindaba la página; esto se analizaba y se entendió que eran una serie de combinaciones de comandos previamente aprendidos pero con cierta dificultad en la escritura de estos mismos.

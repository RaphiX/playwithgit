# Tipps zu Git

## Status des Projektes (Repository) anzeigen
    git status

## Dateien hinzufügen (vormerken) zu Git
    git add DATEINAME

## Vorgemerkte Dateien als neue Version ablegen
    git commit -m "MEINE MESSAGE ZUM COMMIT"

## Commit (Version) hochladen auf Github
    git push origin master

## Geschichte anzeigen 
    git log

### Geschichte schöner anzeigen lassen
    git log --pretty=oneline --graph

# Coole Features zu Git

## Video erstellen
gource

## schnelleres Video erstellen
gource -i 0 -s 0.1

## Video speichern
gource -1920x1080 -o - -i 0 -s 0.1 | ffmpeg -y -r 60 -f image2pipe -vcodec ppm -i - -vcodec libx264 -preset ultrafast -pix_fmt yuv420p -crf 1 -threads 0 -bf 0 gource.mp4

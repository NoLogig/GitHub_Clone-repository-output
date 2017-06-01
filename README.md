
Wenn ein Repository zusätzlich an einem weiteren Ort gespiegelt werden soll, 
können einfach weitere push-URLs hinzugefügt werden, die auf andere Repositories verweisen.

## 1. Repository Klonen, welches gespiegelt werden soll.
```bash

  git clone https://github.com/NoLogig/MirrorTestRepo4Blog.git    

```

## 2. ins geklonte Repository-Verzeichnis wechseln
```bash

cd MirrorTestRepo4Blog

```

## 3. push-URL hinzufügen
```bash

git remote set-url --add origin https://github.com/NoLogig/MirrorOutputRepo4Blog.git

```

## 4. fetch/- und push-URL’s zur Kontrolle ausgeben
```bash

git remote –v 

```

## 5. Test: Ein push, wird nun beide Repositories updaten
```bash
touch testDatei.txt
git add .
git commit -m “test commit”
git push
```




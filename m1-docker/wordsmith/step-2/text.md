The repository contains instructions in English and French.
<br/>
For now, we only care about the first part (about writing Dockerfiles).
<br/>
Place each Dockerfile in its own directory, like this:
```
├── LICENSE
├── README
├── db/
│   ├── `Dockerfile`
│   └── words.sql
├── web/
│   ├── `Dockerfile`
│   ├── dispatcher.go
│   └── static/
└── words/
    ├── `Dockerfile`
    ├── pom.xml
    └── src/
```

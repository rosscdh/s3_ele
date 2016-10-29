# s3_ele
wrapper for elephant


Install
=======

1. Elasticsearch v2.4.1
2. pip install -r requirements.txt

Run
===

```
honcho start web
```

Useage
======

using httpie client

```
http -j POST http://127.0.0.1:5000/ X-Key:xxxxxx first_name=Ross last_name="Crawford-d'Heureuse"
http -j POST http://127.0.0.1:5000/ X-Key:xxxxxx first_name=Isabelle last_name="d'Heureuse"
http -j GET http://127.0.0.1:5000/?q='first_name=Ross' X-Key:xxxxxx
http -j GET http://127.0.0.1:5000/?q='first_name=Ross OR first_name=Isabelle' X-Key:xxxxxx
http -j GET http://127.0.0.1:5000/\?q\="last_name=Crawford" X-Key:xxxxxx
http -j GET http://127.0.0.1:5000/\?q\="last_name=d'Heureuse" X-Key:xxxxxx
http -j GET http://127.0.0.1:5000/67c7b7bd-6b6e-4997-a673-76a65c662278 X-Key:xxxxxx
```
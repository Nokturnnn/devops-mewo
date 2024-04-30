# Atelier Docker - HandBrake

## Quelle commande utiliseriez-vous pour télécharger l'image Docker de HandBrake?

```bash
docker pull jlesage/handbrake
```

## Comment lanceriez-vous un conteneur HandBrake pour traiter une vidéo située sur votre machine hôte?

```bash
docker run -v /chemin/vers/votre/video:/media/input jlesage/handbrake`
```

## Quelles commandes permettent d'inspecter les détails et les logs d'un conteneur actif?

```bash
docker inspect <ID ou nom du conteneur>
docker logs <ID ou nom du conteneur>
```

## Comment arrêter, redémarrer, et finalement supprimer un conteneur et une image?

```bash
docker stop <ID ou nom du conteneur>
docker restart <ID ou nom du conteneur>
docker rm <ID ou nom du conteneur>
docker rmi <ID ou nom de l'image>
```

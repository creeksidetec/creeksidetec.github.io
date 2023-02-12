# Creekside Tech Web updates

Using Jekyll to format site pages.
```bash
docker run --rm --volume="/minikube-host/creeksidetec.github.io/:/srv/jekyll" -it jekyll/jekyll jekyll build
docker run --rm --volume="/minikube-host/creeksidetec.github.io/:/srv/jekyll" -it jekyll/jekyll bundle update
docker run --rm --volume="/minikube-host/creeksidetec.github.io/:/srv/jekyll" --env JEKYLL_ENV=development -p 4000:4000 jekyll/jekyll jekyll serve
```

# k8s.helm.charts
kubernetes 包管理器的chart模板仓库

# How It Works

set up GitHub Pages to point to the `docs` folder. From there, I can
create and publish docs like this:

```console
$ helm create light
$ helm package light
$ mv light-0.1.0.tgz docs
$ helm repo index docs --url https://justmine66.github.io/k8s.helm.charts
$ git add -i
$ git commit -av
$ git push origin master
```

From there, I can do a `helm repo add tscharts 
https://justmine66.github.io/k8s.helm.charts`


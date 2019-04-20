# Image manifest tool

Just for inspect a repository on a Docker registry and fetch images layers. The inspect command can show you which tags are available for the given repository, the labels the image has, the creation date and operating system of the image and more.

e.g.

```
(MoeLove) ➜  ~ docker run --rm taobeier/image-manifest bash -c 'skopeo inspect docker://docker.io/taobeier/docker | jq -r ".RepoTags | .[]"'
18.03-dind
18.03-git
18.03
latest
stable-dind
stable-git
stable
```

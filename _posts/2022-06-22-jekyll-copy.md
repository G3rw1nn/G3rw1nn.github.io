---
layout: post
title: Second post - TEST
date: 2022-06-21 17:11:00 -0500
category: [documentation,software,markup]
tags: [markup, cheatsheet] # Tags should alwasy be lowercase
---

# Testint this update

## Subtitle

* list item 1
* list item 2

**Bold text**

~~Strikethrough~~

- [x] Tasklist item one
- [ ] Tasklist item two
- [ ] Tasklist item three

## Code block JavaScript
```javascript
console.log('hello world');
```

## Code block Yaml
```yml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
  labels:
    app: nginx
spec:
  replicas: 3
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: nginx
        image: nginx:1.14.2
        ports:
        - containerPort: 80
```

## Code block bash
```bash
JEKYLL_ENV=production bundle exec jekyll b
```

## Building with Docker

Create a `Dockerfile` with the following

```Dockerfile
FROM nginx:stable-alpine
COPY _site /usr/share/nginx/html
```

> Jekyll can delay posts which have the date/time set for a point in the future determined by the "front matter" section at the top of your post file. Check the date & time as well as time zone if you don't see a post appear shortly after re-build.
{: .prompt-tip }

## Photos
![imgage-test](/homelab%20avatar.png)
_My Avatar_

[source](https://docs.technotim.live/posts/jekyll-docs-site/)

See more post formatting rules on the [Jekyll site](https://jekyllrb.com/docs/posts/)
build-lists: true
autoscale: true

## Ember-cli deployment pipeline with travis-ci

![inline](./img/GitHub.png)

![inline](./img/travis-ci.png) ![inline](./img/ember-cli-deploy.png)

![inline](./img/aws-s3.png) ![inline](./img/aws-cloudfront.png)

---

![left](./img/profile.jpg)

Alexey (*Alex*) Kulakov


- Semios
- @akulakov
- aklkv.com

---
## Ember-cli deployment pipeline with travis-ci

![inline](./img/GitHub.png)

![inline](./img/travis-ci.png) ![inline](./img/ember-cli-deploy.png)

![inline](./img/aws-s3.png) ![inline](./img/aws-cloudfront.png)

---

![right 80%](./img/ember-cli-deploy.png)

- [Introduction to ember-cli-deploy by Mattia Gheda](https://vimeo.com/158447249)
- [EmberCamp London 2015: Ember CLI Deploy by Aaron Chambers and Luke Melia](https://www.youtube.com/watch?v=fcSL5poJ1gQ)

---

#### Ember-cli + AWS S3 (CloudFront) via travis-ci
![inline](./img/diagram.png)

---

### Ember-cli-deploy AWS pack

- [ember-cli-deploy-aws-pack](https://github.com/kpfefferle/ember-cli-deploy-aws-pack)
- [Deploying Ember to AWS CloudFront](http://blog.testdouble.com/posts/2015-11-03-deploying-ember-to-aws-cloudfront-using-ember-cli-deploy.html)

```bash
ember install ember-cli-deploy
ember install ember-cli-deploy-aws-pack
```

^
- deploy.js
- environment.js
- templates/application.js
- controllers/application.js

---

![inline 90%](./img/travis-ci.png)

- travis-ci.com
  - private
- travis-ci.org
  - public
  - free

^
- travis.yml

---

##

```bash
  ember deploy <development target>
```




```bash
    # .travis.yml
    script:
    - if [ "$TRAVIS_BRANCH" == "dev" ]; then ember deploy development --verbose; elif
      [ "$TRAVIS_BRANCH" == "stage" ]; then ember deploy staging --verbose; elif [ "$TRAVIS_BRANCH"
      == "master" ]; then ember deploy production --verbose; fi
```

---

![inline](https://m.popkey.co/3bcbd8/AoYjv.gif)


---

![left 90%](./img/semios.png)

# We are hiring

- akulakov@semios.com
- semios.com

---

### Thank you

- [source code and slides](https://github.com/aklkv/emberjs-talk-example)

---

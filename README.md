New Media Design III 2017-2018
==============================

Studenten:

 - «JULIE» «VAN DE WEERD»
 - «JULIE» «MATTELAER»

> Artevelde University College Ghent

Productiedossier
----------------

### Installatie

#### Installatie kloon

```
PS> c
PS> git clone «REPOSITORY-URL» «MAPNAAM»
PS> c «MAPNAAM»
PS> git submodule update --init
PS> git submodule foreach 'git checkout v4-dev'
```

```
PS> c «MAPNAAM»
PS> cd docs
PS> bundle update
PS> bundle exec jekyll serve
```

#### Origineel

Als je aan een eigen project Bootstrap als een **Git Submodule** wil toevoegen.

```
PS> c
PS> mkdir «MAPNAAM»
PS> c «MAPNAAM»
PS> git init
PS> git submodule add --branch v4-dev --depth 1 https://github.com/twbs/bootstrap/ docs/_vendor/bootstrap
PS> git submodule foreach 'git checkout v4-dev'
```

### Jekyll-configuratie

In `docs/_config.yml` pas je de `baseurl` aan, van:

```
# Site settings
# ─────────────
baseurl: /1718-nmd3-project # the subpath of your site, e.g. /blog
```

naar `/«REPOSITORYNAAM»` (bv. `/1718-nmd3-project-Bartmi`):

```
# Site settings
# ─────────────
baseurl: /«REPOSITORYNAAM» # the subpath of your site, e.g. /blog
```

### GitHub Pages Configuratie

Op GitHub ga je naar je repository en klik op **Settings**. Scroll naar beneden tot aan **GitHub Pages**, zet de **Source** op `master branch /docs folder` en klik op **Save** om te bewaren.

### Voorbeeldsite

 - Basissjabloon <https://gdmgent-1718-nmd3.github.io/1718-nmd3-project>
 - Persoonlijke repo van Bart Missant <https://gdmgent-1718-nmd3.github.io/1718-nmd3-project-Bartmi>
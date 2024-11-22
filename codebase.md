# _config.yml

```yml
##############################################################################
# Content
##############################################################################

# Link to a page that gives an overview of all your projects.
# This can be an external link (e.g., to you GitHub profile) or to another
# page within your website.
projects_url: http://github.com/probberechts

# Set the page direction to RTL or LTR. default is LTR. (if you set it 'rtl', the 'vazir' font will be loaded.)
direction: ltr
# Configure the navigation menu.
# A pair 'Key: url' will result in a link to 'url' with the name 'Key' in the
# navigation menu. Optionally, you can add translations for the 'Key' in
# languages/*.yml
nav:
  home: /
  about: /about/
  articles: /archives/
  projects: http://github.com/probberechts


# Links to your social media accounts.
# The 'icon' keys should correspond to Fontawesome icon names
# (see https://fontawesome.com/icons?d=gallery&s=brands);
# only 'mail' is an exception.
# You can optionally add a 'label' key to set the title attribute on the link. 
# 'icon' value will be used as title when 'label' is missing.
social_links:
  -
    icon: github
    link: http://github.com/probberechts/cactus-dark
  -
    icon: twitter
    link: /
  -
    icon: facebook
    link: /
  -
    icon: mail
    link: mailto:name@email.com
  -
    icon: mastodon
    label: mastodon.social
    link: https://mastodon.social/@alice
  -
    icon: mastodon
    label: fosstodon.org
    link: https://fosstodon.org/@alice

# Customize the overview with displaying a tagcloud on the index page.
# Options: https://hexo.io/docs/helpers.html#tagcloud
tags_overview: false

# Customize the overview with the most recent blog posts on the index page.
# Options:
#   - show_all_posts: whether to show all available posts.
#   - post_count: whether to show only the x most recent posts.
#   - sort_updated: sort posts by last modification date instead of creation date.
posts_overview:
  show_all_posts: false
  post_count: 5
  sort_updated: false

# Customize the archive view.
# Options:
#   - sort_updated: sort posts by last modification date instead of creation date.
# Note: this does not work together with pagination, since the pagination
# plugin will sort pages by date of creation.
archive:
  sort_updated: false

# Customize the article view.
# Options:
#   - show_updated: show the last modification date.
post:
  show_updated: false

# Customize the copyright years
# Note: if start_year/end_year not provided, will use current year.
copyright:
  start_year: 2016
  end_year:

# Customize the 404 page
# Options:
#   - enabled: whether to enable the 404 page (404.html).
error_404:
  enabled: true
  title: "404 Page Not Found"
  description: "The page you are looking for might have been removed, had its name changed, or is temporarily unavailable."


##############################################################################
# Look and Feel
##############################################################################

# Customize the logo (i.e., the cactus) in the header.
# Options:
#   - enabled: whether to show (true) or hide (false) the logo.
#   - width: width of the logo in pixel units
#   - height: height of the logo in pixel units
#   - url: where the logo can be found
#   - gravatar: whether to use your Gravatar as the logo
#   - grayout: whether to enable a hover effect on the logo
logo:
  enabled: true
  width: 50
  height: 50
  url: /images/logo.png
  gravatar: false
  grayout: true

# Customize the favicons.
# Cactus supports a limited set of the three most important icons:
#   - desktop: The classic favion.ico file.
#   - android: A 192x192 PNG file.
#   - apple:  A 180x180 PNG file.
# These can be generated with http://realfavicongenerator.net/
# Options:
#   - url: where the icon can be found
#   - gravatar: whether to create a favicon from your Gravatar
favicon:
  desktop:
    url: /images/favicon.ico
    gravatar: false
  android:
    url: /images/favicon-192x192.png
    gravatar: false
  apple:
    url: /images/apple-touch-icon.png
    gravatar: false

# The color scheme that should be used to highlight codeblocks.
# See source/css/_highlight for a list of all available color schemes.
# highlight: rainbow

# Set the color scheme.
# Available color schemes are 'dark', 'light', 'classic' and 'white'.
# Alternatively, add your own custom color scheme to source/css/_colors.
colorscheme: dark

# Maximal width of the page in rem units.
page_width: 48


##############################################################################
# Miscellaneous
##############################################################################

# Enable or disable the RSS feed.
rss: false

# Turn your web pages into graph objects (see http://ogp.me).
open_graph:
  fb_app_id:
  fb_admins:
  twitter_id:
  google_plus:


##############################################################################
# Plugins
##############################################################################

# Enable MathJax support for Latex
mathjax:
  enabled: false

# Fill in your Disqus Comments Shortname to enable Disqus comments.
disqus:
  enabled: false
  shortname: cactus-1

# Fill in your Utterances data to enable Utterances comments
utterances:
  enabled: false
  repo: owner/githubrepo
  issue_term: pathname
  label: Comment
  theme: github-dark

# Fill in your Google Analytics tracking ID to enable Google Analytics.
google_analytics:
  enabled: false
  id: UA-86660611-1

# Fill in your Baidu Analytics tracking ID to enable Baidu Analytics.
baidu_analytics:
  enabled: false
  id: 2e6da3c375c8a87f5b664cea6d4cb29c

# Fill in your Cloudflare Analytics tracking ID to enable Cloudflare Analytics.
cloudflare_analytics:
  enabled: false
  id: 0dabb6e21848405483a237e6a7b6ed04

# Fill in your Umami Analytics tracking ID to enable Umami Analytics.
umami_analytics:
  enabled: false
  id: e77e68be-f6e4-4br3-9365-2b76b57cd571
  host: https://analytics.domain.com
  script_name: umami.js

# Fill in you Gravatar email or hash if you want to use your gravatar as the
# logo and/or favicons of you website.
# To generate hash: `$ echo -n "name@email.com" | md5`.
gravatar:
  email: name@email.com
  hash: d41d8cd98f00b204e9800998ecf8427e

# loads libraries and styles from CDN instead or relying on local files
cdn:
  enable: true
  jquery: https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js
  clipboard: https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/2.0.7/clipboard.min.js
  font_awesome: https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css
  justified_gallery_css: https://cdnjs.cloudflare.com/ajax/libs/justifiedGallery/3.8.1/css/justifiedGallery.min.css
  justified_gallery_js: https://cdnjs.cloudflare.com/ajax/libs/justifiedGallery/3.8.1/js/jquery.justifiedGallery.min.js

```

# .gitignore

```
.DS_Store
.idea/
*.log
*.iml
.tern-port
yarn.lock
package-lock.json
node_modules/
.vscode
```

# .jshintrc

```
{
  "asi": false,
  "bitwise": true,
  "browser": true,
  "camelcase": true,
  "curly": true,
  "forin": true,
  "immed": true,
  "latedef": "nofunc",
  "maxlen": 120,
  "newcap": true,
  "noarg": true,
  "noempty": true,
  "nonew": true,
  "predef": [
    "$"
  ],
  "quotmark": true,
  "trailing": true,
  "undef": true,
  "unused": true,

  "expr": true
}

```

# .stylintrc

```
{
    "blocks": false,
    "brackets": "never",
    "colons": "always",
    "colors": "always",
    "commaSpace": "always",
    "commentSpace": "always",
    "cssLiteral": "never",
    "customProperties": [],
    "depthLimit": false,
    "duplicates": true,
    "efficient": "always",
    "exclude": ["source/css/_highlight/*"],
    "extendPref": false,
    "globalDupe": false,
    "groupOutputByFile": true,
    "indentPref": 2,
    "leadingZero": "never",
    "maxErrors": false,
    "maxWarnings": false,
    "mixed": false,
    "mixins": [],
    "namingConvention": "lowercase-dash",
    "namingConventionStrict": true,
    "none": "always",
    "noImportant": true,
    "parenSpace": "never",
    "placeholders": "always",
    "prefixVarsWithDollar": "always",
    "quotePref": "double",
    "reporterOptions": {
        "columns": ["lineData", "severity", "description", "rule"],
        "columnSplitter": "  ",
        "showHeaders": false,
        "truncate": true
    },
    "semicolons": "never",
    "sortOrder": "grouped",
    "stackedProperties": "never",
    "trailingWhitespace": "never",
    "universal": false,
    "valid": true,
    "zeroUnits": false,
    "zIndexNormalize": false
}

```

# gulpfile.js

```js
import decompress from 'gulp-decompress';
import { deleteAsync } from 'del';
import download from "gulp-download-stream";
import fs from 'fs';
import gulp from 'gulp';
import path from 'path';
import stylint from 'gulp-stylint';
import stylelintFormatter from 'stylelint-formatter-pretty';
import jshint from 'gulp-jshint';
import jshintFormatter from 'jshint-stylish';
import yaml from 'js-yaml';


gulp.task('lib:clean',function(){
  return deleteAsync([ './source/lib/*' ]);
})

gulp.task('lib:fontAwesome',function(){
  return gulp.src([
    'node_modules/@fortawesome/fontawesome-free/webfonts/*',
    'node_modules/@fortawesome/fontawesome-free/css/all.min.css'
  ], {base: 'node_modules/@fortawesome/fontawesome-free'})
    .pipe(gulp.dest('./source/lib/font-awesome'))
})

gulp.task('lib:download_mesloFont', function () {
  return download('https://github.com/andreberg/Meslo-Font/raw/master/dist/v1.2.1/Meslo%20LG%20v1.2.1.zip?raw=true')
    .pipe(gulp.dest("/tmp"));
})

gulp.task('lib:install_mesloFont', function () {
  return gulp.src('/tmp/Meslo%20LG%20v1.2.1.zip')
    .pipe(decompress({
      filter: file => path.extname(file.path) == '.ttf',
      strip: 1
    }))
    .pipe(gulp.dest('./source/lib/meslo-LG'));
});

gulp.task('lib:vazirFont',function(){
  return gulp.src([
    'node_modules/vazir-font/dist/*',
  ], {base: 'node_modules/vazir-font/dist'})
    .pipe(gulp.dest('./source/lib/vazir-font'))
})

gulp.task('lib:justifiedGallery',function(){
  return gulp.src([
    'node_modules/justifiedGallery/dist/css/*.min.css',
    'node_modules/justifiedGallery/dist/js/*.min.js'
  ], {base: 'node_modules/justifiedGallery/dist'})
    .pipe(gulp.dest('./source/lib/justified-gallery'))
})

gulp.task('lib:jQuery',function(){
  return gulp.src(['node_modules/jquery/dist/jquery.min.js'])
    .pipe(gulp.dest('./source/lib/jquery'))
})

gulp.task('lib:clipboard',function(){
  return gulp.src(['node_modules/clipboard/dist/clipboard.min.js'])
    .pipe(gulp.dest('./source/lib/clipboard'))
})

gulp.task('lint:js', function() {
  return gulp.src([
    './source/js/**/*.js',
  ]).pipe(jshint())
    .pipe(jshint.reporter(jshintFormatter));
});

gulp.task('lint:stylus', function () {
  return gulp.src([
    './source/css/*.styl',
    './source/css/_partial/*.styl',
    './source/css/_colors/*.styl'
  ]).pipe(stylint({
      config: '.stylintrc',
      reporters: [
        {formatter: stylelintFormatter, console: true}
      ]
    }))
});

gulp.task('validate:config', function(cb) {
  var themeConfig = fs.readFileSync(path.join(path.resolve(), '_config.yml'));

  try {
    yaml.load(themeConfig);
    cb();
  } catch(error) {
    cb(new Error(error));
  }
});

gulp.task('validate:languages', function(cb) {
  var languagesPath = path.join(path.resolve(), 'languages');
  var languages = fs.readdirSync(languagesPath);
  var errors = [];
  for (var i in languages) {
    var languagePath = path.join(languagesPath, languages[i]);
    try {
      yaml.load(fs.readFileSync(languagePath), {
        filename: path.relative(path.resolve(), languagePath)
      });
    } catch(error) {
      errors.push(error);
    }
  }
  if (errors.length == 0) {
    cb();
  } else {
    cb(errors);
  }
});

gulp.task('lib', gulp.series(
  'lib:clean', 'lib:jQuery', 'lib:clipboard', 'lib:fontAwesome',
  'lib:download_mesloFont', 'lib:install_mesloFont', 'lib:vazirFont',
  'lib:justifiedGallery'));
gulp.task('lint', gulp.parallel('lint:js', 'lint:stylus'));
gulp.task('validate', gulp.parallel('validate:config', 'validate:languages'));
gulp.task('default', gulp.parallel('lint', 'validate'));

```

# languages/ar.yml

```yml
nav:
  home: الرئيسية
  about: معلومات عنّي
  articles: منشورات
  tag: تسمية
  category: تصنيف
  projects: مشاريع
  search: بحث

icons:
  menu: القائمة
  top: الأعلى

footer:
  copyright: حقوق النشر

index:
  find_me_on: يمكننا التواصل من خلال
  enum_comma: ","
  enum_and: و
  articles: منشورات
  projects: مشاريع
  topics: مواضيع
  most_recent: المنشور مؤخراً

post:
  desktop:
    previous: المنشور السابق
    next: المنشور التالي
    back_to_top: العودة إلى الأعلى
    share: مشاركة المنشور
  mobile:
    menu: القائمة
    toc: المحتويات
    back_to_top: العودة إلى الأعلى
    share: مشاركة

search:
  search: بحث...
  no_results: لم يتم العثور على نتائج.

tag_cloud:
  zero: لايوجد تسميات

pagination:
  page: الصفحة %d من أصل %d

counter:
  tag_cloud:
    zero: لايوجد تسميات
    one: ""
    other: ""

  categories:
    zero: لايوجد تصنيفات
    one: ""
    other: ""

  archive_posts:
    zero: لايوجد منشورات.
    one: ""
    other: ""

comments:
  no_js: يرجى تفعيل JavaScript في المتصفح لعرض التعليقات.

tooltip:
  copy_tip: انسخ!
  copied: تم النسخ!

```

# languages/ca.yml

```yml
nav:
  home: Inici
  about: Qui som 
  articles: Articles
  projects: Projectes
  search: Buscar

footer:
  copyright: Copyright

index:
  find_me_on: Trobem a
  enum_comma: ','
  enum_and: i
  articles: Articles
  projects: Projectes

post:
  desktop:
    previous: Post Anterior
    next: Post Següent
    back_to_top: Adalt
    share: Compartir Post
  mobile:
    menu: Menú
    toc: TOC
    back_to_top: Cap amunt
    share: Compartir

search:
  search: Buscar...
  no_results: No s'han trobat resultats.

pagination:
  page: Pàgina %d de %d

comments:
  no_js: Si us plau, activa JavaScript per poder veure el contingut.

```

# languages/de.yml

```yml
nav:
  home: Startseite
  about: Über diese Webseite
  articles: Artikel
  tag: Tag
  category: Kategorie
  projects: Projekte
  search: Suche

footer:
  copyright: Copyright

index:
  find_me_on: Finde mich auf
  enum_comma: ','
  enum_and: und
  articles: Artikel
  projects: Projekte
  topics: Themen
  most_recent: Neueste

post:
  desktop:
    previous: Vorheriger Beitrag
    next: Nächster Beitrag
    back_to_top: Zurück zum Anfang
    share: Beitrag teilen
  mobile:
    menu: Menü
    toc: TOC
    back_to_top: Nach oben
    share: Teilen

search:
  search: Suche...
  no_results: Keine Ergebnisse gefunden.

tag_cloud:
  zero: Keine Tags

pagination:
  page: Seite %d von %d

counter:
  tag_cloud:
    zero: Keine Tags
    one: ""
    other: ""

  categories:
    zero: Keine Kategorien
    one: ""
    other: ""

  archive_posts:
    zero: Keine Beiträge.
    one: ""
    other: ""

comments:
  no_js: Bitte aktivieren Sie JavaScript um die Kommentare anzuzeigen.

tooltip:
  copy_tip: In die Zwischenablage kopiert!
  copied: Kopiert!
```

# languages/default.yml

```yml
nav:
  home: Home
  about: About
  articles: Writing
  tag: Tag
  category: Category
  projects: Projects
  search: Search

icons:
  menu: Menu
  top: Top

footer:
  copyright: Copyright

index:
  find_me_on: Find me on
  enum_comma: ','
  enum_and: and
  articles: Writing
  projects: Projects
  topics: Topics
  most_recent: Most recent

post:
  desktop:
    previous: Previous post
    next: Next post
    back_to_top: Back to top
    share: Share post
  mobile:
    menu: Menu
    toc: TOC
    back_to_top: Top
    share: Share

search:
  search: Search...
  no_results: No results found.

tag_cloud:
  zero: No tags

pagination:
  page: Page %d of %d

counter:
  tag_cloud:
    zero: No tags
    one: ""
    other: ""

  categories:
    zero: No categories
    one: ""
    other: ""

  archive_posts:
    zero: No posts.
    one: ""
    other: ""

comments:
  no_js: Please enable JavaScript to view the comments.

tooltip:
  copy_tip: Copy to clipboard!
  copied: Copied!
```

# languages/en.yml

```yml
nav:
  home: Home
  about: About
  articles: Writing
  tag: Tag
  category: Category
  projects: Projects
  search: Search

icons:
  menu: Menu
  top: Top

footer:
  copyright: Copyright

index:
  find_me_on: Find me on
  enum_comma: ','
  enum_and: and
  articles: Writing
  projects: Projects
  topics: Topics
  most_recent: Most recent

post:
  desktop:
    previous: Previous post
    next: Next post
    back_to_top: Back to top
    share: Share post
  mobile:
    menu: Menu
    toc: TOC
    back_to_top: Top
    share: Share

search:
  search: Search...
  no_results: No results found.

tag_cloud:
  zero: No tags

pagination:
  page: Page %d of %d

counter:
  tag_cloud:
    zero: No tags
    one: ""
    other: ""

  categories:
    zero: No categories
    one: ""
    other: ""

  archive_posts:
    zero: No posts.
    one: ""
    other: ""

comments:
  no_js: Please enable JavaScript to view the comments.

tooltip:
  copy_tip: Copy to clipboard!
  copied: Copied!
```

# languages/es.yml

```yml
nav:
  home: Inicio
  about: Acerca de
  articles: Articulos
  projects: Proyectos
  search: Buscar

footer:
  copyright: Copyright

index:
  find_me_on: Encuentrame en
  enum_comma: ','
  enum_and: y
  articles: Articulos
  projects: Proyectos

post:
  desktop:
    previous: Post Anterior
    next: Post Siguiente
    back_to_top: Arriba
    share: Compartir Post
  mobile:
    menu: Menu
    toc: TOC
    back_to_top: Top
    share: Compartir

search:
  search: Buscar...
  no_results: No se encontraron resultados.

pagination:
  page: Pagina %d de %d

comments:
  no_js: Por favor activa JavaScript para ver el contenido.

```

# languages/fa.yml

```yml
nav:
  home: خانه
  about: درباره
  articles: نوشته‌ها
  projects: پروژه‌ها
  search: جست‌وجو

footer:
  copyright: حق‌کپی

index:
  find_me_on: مرا در این شبکه‌ها دنبال کنید
  enum_comma: '،'
  enum_and: و
  articles: نوشته‌ها
  projects: پروژه‌ها

post:
  desktop:
    previous: پست پیشین
    next: پست یعدی
    back_to_top: بازگشت به بالا
    share: اشتراک‌گذاری
  mobile:
    menu: منو
    toc: محتوا
    back_to_top: بالا
    share: اشتراک‌گذاری

search:
  search: جست‌وجو...
  no_results: نتیجه‌ای یافت نشد.

pagination:
  page: برگه %d از %d

comments:
  no_js: برای مشاهده دیدگاه‌ها، لطفا جاوااسکریپت را فعال کنید.

```

# languages/fr.yml

```yml
nav:
  home: Accueil
  about: A propos
  articles: Archives
  projects: Projets
  search: Rechercher

footer:
  copyright: Copyright

index:
  find_me_on: Retrouve moi sur
  enum_comma: ','
  enum_and: et
  articles: Articles
  projects: Projets

post:
  desktop:
    previous: Article précédent
    next: Article suivant
    back_to_top: Retour en haut
    share: Partager
  mobile:
    menu: Menu
    toc: Sections
    back_to_top: Début
    share: Partager

search:
  search: rechercher...
  no_results: Aucun résultat trouvé.

pagination:
  page: Page %d sur %d

comments:
  no_js: Veuillez activer JavaScript pour voir les réactions.

```

# languages/it.yml

```yml
nav:
  home: Home
  about: About
  articles: Articoli
  projects: Progetti
  search: Cerca

footer:
  copyright: Copyright

index:
  find_me_on: Mi trovi su
  enum_comma: ','
  enum_and: e
  articles: Articoli
  projects: Progetti
  all_tags: Tags

post:
  desktop:
    previous: Articolo precedente
    next: Articolo successivo
    back_to_top: Torna all'inizio
    share: Condividi articolo
  mobile:
    menu: Menu
    toc: TOC
    back_to_top: Top
    share: Condividi

search:
  search: Cerca...
  no_results: Nessun risultato.

pagination:
  page: Pagina %d di %d

comments:
  no_js: Abilita javascript per vedere i commenti.

```

# languages/kr.yml

```yml
nav:
  home: 홈
  about: 소개
  articles: 글 목록
  tag: 태그
  category: 카테고리
  projects: 프로젝트
  search: 검색

footer:
  copyright: 저작권

index:
  find_me_on: 찾기
  enum_comma: ','
  enum_and: 그리고
  articles: 글 목록
  projects: 프로젝트
  topics: 주제
  most_recent: 가장 최근

post:
  desktop:
    previous: 이전
    next: 다음
    back_to_top: 맨 위로
    share: 공유
  mobile:
    menu: 메뉴
    toc: TOC
    back_to_top: 맨 위로
    share: 공유

search:
  search: 검색중...
  no_results: 검색 결과가 없습니다.

tag_cloud:
  zero: 태그가 없습니다.

pagination:
  page: 총 %d 중 %d

counter:
  tag_cloud:
    zero: 태그가 없습니다.
    one: ""
    other: ""

  categories:
    zero: 카테고리가 없습니다.
    one: ""
    other: ""

  archive_posts:
    zero: 등록된 글이 없습니다.
    one: ""
    other: ""

comments:
  no_js: 코멘트를 보려면 자바스크립트를 활성화하세요.

tooltip:
  copy_tip: 클립보드에 복사하였습니다!
  copied: 복사하였습니다!

```

# languages/nl.yml

```yml
nav:
  home: Home
  about: Over mij
  articles: Blog
  projects: Projecten
  search: Zoeken

footer:
  copyright: Copyright

index:
  find_me_on: Je vindt me op
  enum_comma: ','
  enum_and: en
  articles: Blogposts
  projects: Projecten

post:
  desktop:
    previous: Vorige post
    next: Volgende post
    back_to_top: Naar boven
    share: Deel deze post
  mobile:
    menu: Menu
    toc: Inhoudsopgave
    back_to_top: Top
    share: Deel

search:
  search: zoeken...
  no_results: Geen resultaten gevonden.

pagination:
  page: Pagina %d van %d

comments:
  no_js: Activeer Javascript om de commentaarsectie te kunnen bekijken.

```

# languages/pl.yml

```yml
nav:
  home: Strona główna
  about: O mnie
  articles: Artykuły
  tag: Tagi
  category: Kategorie
  projects: Projekty
  search: Wyszukiwanie

footer:
  copyright: Prawa autorskie

index:
  find_me_on: Znajdź mnie na
  enum_comma: ','
  enum_and: i
  articles: Artykuły
  projects: Projekty
  topics: Tematy
  most_recent: Najnowsze

post:
  desktop:
    previous: Poprzedni post
    next: Następny post
    back_to_top: Powrót do góry
    share: Udostępnij post
  mobile:
    menu: Menu
    toc: TOC
    back_to_top: Powrót do góry
    share: Udostępnij

search:
  search: Wyszukaj...
  no_results: Nic nie znaleziono.

tag_cloud:
  zero: Brak tagów

pagination:
  page: Strona %d z %d

counter:
  tag_cloud:
    zero: Brak tagów
    one: ""
    other: ""

  categories:
    zero: Brak kategorii
    one: ""
    other: ""

  archive_posts:
    zero: Brak postów.
    one: ""
    other: ""

comments:
  no_js: Proszę włączyć obsługę JavaScript, żeby zobaczyć komentarze.

```

# languages/pt-br.yml

```yml
nav:
  home: Início
  about: Sobre
  articles: Artigos
  projects: Projetos
  search: Buscar

footer:
  copyright: Copyright

index:
  find_me_on: Me encontre em 
  enum_comma: ','
  enum_and: e
  articles: Artigos
  projects: Projetos

post:
  desktop:
    previous: Post Anterior
    next: Post Seguinte
    back_to_top: Acima
    share: Compartihar Post
  mobile:
    menu: Menu
    toc: TOC
    back_to_top: Top
    share: Compartilhar

search:
  search: Buscar...
  no_results: Nenhum resultado encontrado.

pagination:
  page: Página %d de %d

comments:
  no_js: Por favor, ative o JavaScript para visualizar o conteúdo.
```

# languages/ru.yml

```yml
nav:
  home: Главная
  about: Обо мне
  articles: Блог
  projects: Проекты
  search: Искать

footer:
  copyright: ' '

index:
  find_me_on: 'Свяжитесь со мной:'
  enum_comma: ','
  enum_and: и
  articles: Блог
  projects: Проекты

post:
  desktop:
    previous: Предыдущая запись
    next: Следующая запись
    back_to_top: В начало
    share: Поделиться
  mobile:
    menu: Меню
    toc: Оглавление
    back_to_top: В начало
    share: Поделиться

search:
  search: Искать...
  no_results: Ничего не найдено.

pagination:
  page: Страница %d из %d

comments:
  no_js: Включите JavaScript, чтобы читать комментарии.

```

# languages/tr.yml

```yml
nav:
  home: Ana Sayfa
  about: Hakkımda
  articles: Yazılar
  tag: Etiketler
  category: Kategoriler
  projects: Projeler
  search: Ara

icons:
  menu: Menü
  top: Üst

footer:
  copyright: Tüm Hakları Saklıdır

index:
  find_me_on: 'Bana ulaşın:'
  enum_comma: ','
  enum_and: ','
  articles: Yazılar
  projects: Projeler
  topics: Başlıklar
  most_recent: En yeni

post:
  desktop:
    previous: Önceki gönderi
    next: Sonraki gönderi
    back_to_top: Başa dön
    share: Gönderiyi paylaş
  mobile:
    menu: Menü
    toc: İçindekiler
    back_to_top: Başa dön
    share: Paylaş

search:
  search: Ara...
  no_results: Hiçbir sonuç bulunamadı.

tag_cloud:
  zero: Etiket yok

pagination:
  page: 'Sayfa %d/%d'

counter:
  tag_cloud:
    zero: Etiket yok
    one: ""
    other: ""

  categories:
    zero: Kategori yok
    one: ""
    other: ""

  archive_posts:
    zero: Gönderi yok
    one: ""
    other: ""

comments:
  no_js: "Yorumları görebilmek için lütfen JavaScript'e izin verin."

tooltip:
  copy_tip: Kopyala
  copied: Kopyalandı!

```

# languages/ua.yml

```yml
nav:
  home: Головна
  about: Про мене
  articles: Статті
  tag: Теґи
  category: Категорії
  projects: Проєкти
  search: Пошук

icons:
  menu: Меню
  top: Вгору

footer:
  copyright: Copyright

index:
  find_me_on: Знайди мене в
  enum_comma: ','
  enum_and: і
  articles: Статті
  projects: Проєкти
  topics: Теми
  most_recent: Нові

post:
  desktop:
    previous: Попередній допис
    next: Наступний допис
    back_to_top: Вгору
    share: Поширити допис
  mobile:
    menu: Меню
    toc: TOC
    back_to_top: Вгору
    share: Поширити

search:
  search: Пошук...
  no_results: Нічого не знайдено.

tag_cloud:
  zero: Теґи відсутні

pagination:
  page: Сторінка %d з %d

counter:
  tag_cloud:
    zero: Теґи відсутні
    one: ""
    other: ""

  categories:
    zero: Категорії відсутні
    one: ""
    other: ""

  archive_posts:
    zero: Дописи відсутні
    one: ""
    other: ""

comments:
  no_js: Це не працювавтиме без JavaScript.

tooltip:
  copy_tip: Скопіювати до буферу обміну!
  copied: Скопійовано!

```

# languages/vi.yml

```yml
nav:
  home: Trang chủ
  about: Giới thiệu
  articles: Bài viết
  tag: Thẻ
  category: Thể loại
  projects: Dự án
  search: Tìm kiếm

footer:
  copyright: Bản quyền

index:
  find_me_on: Tìm tôi trên
  enum_comma: ','
  enum_and: and
  articles: Bài viết
  projects: Dự án
  topics: Chủ đề
  most_recent: Gần đây nhất

post:
  desktop:
    previous: Bài trước
    next: Bài tiếp theo
    back_to_top: Về đầu trang
    share: Chia sẻ bài viết
  mobile:
    menu: Menu
    toc: TOC
    back_to_top: Về đầu trang
    share: Chia sẻ

search:
  search: Tìm kiếm...
  no_results: Không tìm thấy kết quả.

tag_cloud:
  zero: Không có thẻ

pagination:
  page: Trang% d của% d

counter:
  tag_cloud:
    zero: Không có thẻ
    one: ""
    other: ""
    
categories:
  zero: không có danh mục 
  one: ""
  other: ""

archive_posts:
  zero: Không có bài viết.
  one: ""
  other: ""

comments:
  no_js: Vui lòng kích hoạt JavaScript để xem các bình luận.



```

# languages/zh-CN.yml

```yml
nav:
  home: 首页
  about: 关于
  articles: 归档
  projects: 项目
  tag: 标签
  category: 分类
  search: 搜索
  
icons:
  menu: 目录
  top: 顶部

footer:
  copyright: Copyright

index:
  find_me_on: 在这里找到我：
  enum_comma: '，'
  enum_and: 和
  articles: 文章
  projects: 项目
  topics: 标签
  most_recent: 最新发布

post:
  desktop:
    previous: 上一篇
    next: 下一篇
    back_to_top: 返回顶部
    share: 分享文章
  mobile:
    menu: 菜单
    toc: 目录
    back_to_top: 返回顶部
    share: 分享

search:
  search: 搜索...
  no_results: 抱歉，没有符合您搜索条件的结果。请换其它关键词再试。

tag_cloud:
  zero: 没有标签

pagination:
  page: 第 %d 页，共 %d 页
 
counter:
  tag_cloud:
    zero: 没有标签
    one: ""
    other: ""

  categories:
    zero: 没有分类
    one: ""
    other: ""

  archive_posts:
    zero: 没有归档
    one: ""
    other: ""

comments:
  no_js: 加载评论需要在浏览器启用 JavaScript 脚本支持。

tooltip:
  copy_tip: 复制到粘贴板！
  copied: 复制成功！

```

# languages/zh-TW.yml

```yml
nav:
  home: 首頁
  about: 關於
  articles: 文章
  tag: 標籤
  category: 分類
  projects: 項目
  search: 搜尋

icons:
  menu: 目錄
  top: 頂部

footer:
  copyright: Copyright

index:
  find_me_on: 出沒地 
  enum_comma: ','
  enum_and: 和
  articles: 文章
  projects: 項目
  topics: 標題
  most_recent: 最近新增

post:
  desktop:
    previous: 上一篇
    next: 下一篇 
    back_to_top: 回到頁首
    share: 分享
  mobile:
    menu: 選單
    toc: 文章目錄
    back_to_top: 頁首
    share: 分享

search:
  search: 搜尋...
  no_results: 沒有結果

tag_cloud:
  zero: 目前還沒有標籤

pagination:
  page: 第 %d 頁，共 %d 頁

counter:
  tag_cloud:
    zero: 目前沒有標籤
    one: ""
    other: ""

  categories:
    zero: 目前沒有分類
    one: ""
    other: ""

  archive_posts:
    zero: 沒有文章哦！
    one: ""
    other: ""

comments:
  no_js: 請開啟 JavaScript 功能來使用留言系統

tooltip:
  copy_tip: 複製到剪貼簿！
  copied: 複製成功！

```

# layout/_partial/comments.ejs

```ejs
<% if(page.comments && theme.disqus.enabled){ %>
    <div class="blog-post-comments">
        <div id="disqus_thread">
            <noscript><%= __('comments.no_js') %></noscript>
        </div>
    </div>
<% } %>
<% if(page.comments && theme.utterances.enabled){ %>
    <div class="blog-post-comments">
        <div id="utterances_thread">
            <noscript><%= __('comments.no_js') %></noscript>
        </div>
    </div>
<% } %>
```

# layout/_partial/footer.ejs

```ejs
<footer id="footer">
  <div class="footer-left">
    <%= __('footer.copyright') %> &copy;
    <% var endYear = (theme.copyright && theme.copyright.end_year) ? theme.copyright.end_year : new Date().getFullYear() %>
    <% var startYear = (theme.copyright && theme.copyright.start_year) ? theme.copyright.start_year : new Date().getFullYear() %>
    <%= startYear >= endYear ? endYear : startYear + "-" + endYear %>
    <%= config.author || config.title %>
  </div>
  <div class="footer-right">
    <nav>
      <ul>
        <% for (var i in theme.nav) { %><!--
       --><li><a href="<%- url_for(theme.nav[i]) %>"><%= __('nav.'+i).replace("nav.", "") %></a></li><!--
     --><% } %>
      </ul>
    </nav>
  </div>
</footer>

```

# layout/_partial/google_analytics.ejs

```ejs
<!-- Google Analytics -->
<% if (theme.google_analytics.enabled && theme.google_analytics.id){ %>
  <script async src="https://www.googletagmanager.com/gtag/js?id=<%= theme.google_analytics.id %>"></script>
  <script>
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());
      gtag('config', '<%= theme.google_analytics.id %>');
  </script>
<% } %>

```

# layout/_partial/head.ejs

```ejs
<head>
    <!-- so meta -->
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="HandheldFriendly" content="True">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=5" />
    <%- open_graph({
        image:          thumbnail(page),
        fb_app_id:      theme.open_graph.fb_app_id,
        fb_admins:      theme.open_graph.fb_admins,
        twitter_id:     theme.open_graph.twitter_id,
        google_plus:    theme.open_graph.google_plus,
    }) %>
    <%- meta(page) %>
    <% if (theme.favicon) { %>
      <% if (theme.favicon.desktop) { %>
        <% if (theme.gravatar && (theme.gravatar.email || theme.gravatar.hash) && theme.favicon.desktop.gravatar) { %>
          <% if (theme.gravatar.email) { %>
            <link rel="shortcut icon" href="<%= gravatar(theme.gravatar.email, 48) %>">
          <% } else { %>
            <link rel="shortcut icon" href="https://www.gravatar.com/avatar/<%= theme.gravatar.hash %>?s=48">
          <% } %>
        <% } else { %>
          <link rel="shortcut icon" href="<%= url_for(theme.favicon.desktop.url) %>">
        <% } %>
      <% } %>
      <% if (theme.favicon.android) { %>
        <% if (theme.gravatar && (theme.gravatar.email || theme.gravatar.hash) && theme.favicon.android.gravatar) { %>
          <% if (theme.gravatar.email) { %>
            <link rel="icon" type="image/png" href="<%= gravatar(theme.gravatar.email, 192) %>" sizes="192x192">
          <% } else { %>
            <link rel="icon" type="image/png" href="https://www.gravatar.com/avatar/<%= theme.gravatar.hash %>?s=192">
          <% } %>
        <% } else { %>
          <link rel="icon" type="image/png" href="<%= url_for(theme.favicon.android.url) %>" sizes="192x192">
        <% } %>
      <% } %>
      <% if (theme.favicon.apple) { %>
        <% if (theme.gravatar && (theme.gravatar.email || theme.gravatar.hash) && theme.favicon.apple.gravatar) { %>
          <% if (theme.gravatar.email) { %>
            <link rel="apple-touch-icon" sizes="180x180" href="<%= gravatar(theme.gravatar.email, 180) %>">
          <% } else { %>
            <link rel="apple-touch-icon" size="180x180" href="https://www.gravatar.com/avatar/<%= theme.gravatar.hash %>?s=180">
          <% } %>
        <% } else { %>
          <link rel="apple-touch-icon" sizes="180x180" href="<%= url_for(theme.favicon.apple.url) %>">
        <% } %>
      <% } %>
    <% } %>
    <!-- title -->
    <title><%= page_title() %></title>
    <!-- async scripts -->
    <%- partial('./google_analytics.ejs') %>
    <%- partial('./umami_analytics.ejs') %>
    <!-- styles -->
    <%- css('css/style') %>
    <!-- persian styles -->
    <% if (theme.direction && theme.direction === 'rtl') { %>
      <%- css('css/rtl') %>
    <% } %>
    <!-- rss -->
    <% if (theme.rss === '' && config.feed && config.feed.path) { %>
      <% theme.rss = config.feed.path %>
    <% } %>
    <% if (theme.rss) { %>
      <link rel="alternate" href="<%= url_for(theme.rss) %>" title="<%= config.title %>" type="application/atom+xml" />
    <% } %>
	<!-- mathjax -->
	<% if (theme.mathjax.enabled) {%>
		<script type="text/x-mathjax-config">
		  MathJax.Hub.Config({
			tex2jax: {
			  skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
			  inlineMath: [['$','$']]
			}
		  });
		</script>
		<script src='https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/latest.js?config=TeX-MML-AM_CHTML' async></script>
	<% } %>
</head>

```

# layout/_partial/header.ejs

```ejs
<header id="header">
  <a class="u-url u-uid" href="<%- url_for("/") %>">
  <% if (theme.logo && theme.logo.enabled) { %>
    <% if (theme.gravatar && (theme.gravatar.email || theme.gravatar.hash) && theme.logo.gravatar) { %>
      <% if (theme.gravatar.email) { %>
        <img id="logo" alt class="u-logo"
          srcset="<%- gravatar(theme.gravatar.email) %>?s=<%= theme.logo.width %>, <%- gravatar(theme.gravatar.email) %>?s=<%= theme.logo.width*1.5 %> 1.5x, <%- gravatar(theme.gravatar.email) %>?s=<%= theme.logo.width*2 %> 2x"
          src="<%- gravatar(theme.gravatar.email) %>" />
      <% } else { %>
        <img id="logo" alt class="u-logo"
          srcset="https://www.gravatar.com/avatar/<%= theme.gravatar.hash %>?s=<%= theme.logo.width %>, https://www.gravatar.com/avatar/<%= theme.gravatar.hash %>?s=<%= theme.logo.width*1.5 %> 1.5x, https://www.gravatar.com/avatar/<%= theme.gravatar.hash %>?s=<%= theme.logo.width*2 %> 2x"
          src="https://www.gravatar.com/avatar/<%= theme.gravatar.hash %>" />
      <% } %>
    <% } else { %>
      <img id="logo" alt class="u-logo" src="<%- url_for(theme.logo.url) %>" />
    <% } %>
  <% } %>
    <div id="title">
      <h1 class="p-name"><%= config.title %></h1>
    </div>
  </a>
  <div id="nav">
    <ul>
      <li class="icon">
        <a href="#" aria-label="<%- __('icons.menu') %>"><i class="fa-solid fa-bars fa-2x"></i></a>
      </li>
      <% for (var i in theme.nav) { %><!--
     --><li><a href="<%- url_for(theme.nav[i]) %>"><%= __('nav.'+i).replace("nav.", "") %></a></li><!--
   --><% } %>
    </ul>
  </div>
</header>

```

# layout/_partial/pagination.ejs

```ejs
<% if (page.total > 1) { %>
    <div class="pagination">
        <% if (page.prev) { %>
            <a href="<%- url_for(page.prev_link) %>"><i class="fa-solid fa-angle-left"></i></a>
        <% } %>
        <span class="page-number"><%= __('pagination.page', page.current, page.total) %></span>
        <% if (page.next) { %>
            <a href="<%- url_for(page.next_link) %>"><i class="fa-solid fa-angle-right"></i>
            </a>
        <% } %>
    </div>
<% } %>

```

# layout/_partial/post/actions_desktop.ejs

```ejs
<div id="header-post">
  <a id="menu-icon" href="#" aria-label="<%- __('icons.menu') %>"><i class="fa-solid fa-bars fa-lg"></i></a>
  <a id="menu-icon-tablet" href="#" aria-label="<%- __('icons.menu') %>"><i class="fa-solid fa-bars fa-lg"></i></a>
  <a id="top-icon-tablet" href="#" aria-label="<%- __('icons.top') %>" onclick="$('html, body').animate({ scrollTop: 0 }, 'fast');" style="display:none;"><i class="fa-solid fa-chevron-up fa-lg"></i></a>
  <span id="menu">
    <span id="nav">
      <ul>
        <% for (var i in theme.nav) { %><!--
       --><li><a href="<%- url_for(theme.nav[i]) %>"><%= __('nav.'+i).replace("nav.", "") %></a></li><!--
     --><% } %>
      </ul>
    </span>
    <br/>
    <span id="actions">
      <ul>
        <% if (page.prev) { %>
        <li><a class="icon" aria-label="<%- __('post.desktop.previous') %>" href="<%- url_for(page.prev.path) %>"><i class="fa-solid fa-chevron-left" aria-hidden="true" onmouseover="$('#i-prev').toggle();" onmouseout="$('#i-prev').toggle();"></i></a></li>
        <% } %>
        <% if (page.next) { %>
        <li><a class="icon" aria-label="<%- __('post.desktop.next') %>" href="<%- url_for(page.next.path) %>"><i class="fa-solid fa-chevron-right" aria-hidden="true" onmouseover="$('#i-next').toggle();" onmouseout="$('#i-next').toggle();"></i></a></li>
        <% } %>
        <li><a class="icon" aria-label="<%- __('post.desktop.back_to_top') %>" href="#" onclick="$('html, body').animate({ scrollTop: 0 }, 'fast');"><i class="fa-solid fa-chevron-up" aria-hidden="true" onmouseover="$('#i-top').toggle();" onmouseout="$('#i-top').toggle();"></i></a></li>
        <li><a class="icon" aria-label="<%- __('post.desktop.share') %>" href="#"><i class="fa-solid fa-share-alt" aria-hidden="true" onmouseover="$('#i-share').toggle();" onmouseout="$('#i-share').toggle();" onclick="$('#share').toggle();return false;"></i></a></li>
      </ul>
      <span id="i-prev" class="info" style="display:none;"><%= __('post.desktop.previous') %></span>
      <span id="i-next" class="info" style="display:none;"><%= __('post.desktop.next') %></span>
      <span id="i-top" class="info" style="display:none;"><%= __('post.desktop.back_to_top') %></span>
      <span id="i-share" class="info" style="display:none;"><%= __('post.desktop.share') %></span>
    </span>
    <br/>
    <div id="share" style="display: none">
      <%- partial('_partial/post/share', { icon_class_name: '' }) %>
    </div>
    <% let tocHTML = toc(page.content) %>
    <% if (tocHTML !== '') { %>
      <div id="toc">
        <%- tocHTML %>
      </div>
    <% } %>
  </span>
</div>

```

# layout/_partial/post/actions_mobile.ejs

```ejs
<div id="footer-post-container">
  <div id="footer-post">

    <div id="nav-footer" style="display: none">
      <ul>
        <% for (var i in theme.nav) { %>
          <li><a href="<%- url_for(theme.nav[i]) %>"><%= __('nav.'+i).replace("nav.", "") %></a></li>
        <% } %>
      </ul>
    </div>

    <% let tocHTML = toc(page.content) %>
    <% if (tocHTML !== '') { %>
      <div id="toc-footer" style="display: none">
        <%- toc(page.content) %>
      </div>
    <% } %>

    <div id="share-footer" style="display: none">
      <%- partial('_partial/post/share', { icon_class_name: 'fa-lg' }) %>
    </div>

    <div id="actions-footer">
        <a id="menu" class="icon" href="#" onclick="$('#nav-footer').toggle();return false;"><i class="fa-solid fa-bars fa-lg" aria-hidden="true"></i> <%= __('post.mobile.menu') %></a>
        <% if (tocHTML !== '') { %>
          <a id="toc" class="icon" href="#" onclick="$('#toc-footer').toggle();return false;"><i class="fa-solid fa-list fa-lg" aria-hidden="true"></i> <%= __('post.mobile.toc') %></a>
        <% } %>
        <a id="share" class="icon" href="#" onclick="$('#share-footer').toggle();return false;"><i class="fa-solid fa-share-alt fa-lg" aria-hidden="true"></i> <%= __('post.mobile.share') %></a>
        <a id="top" style="display:none" class="icon" href="#" onclick="$('html, body').animate({ scrollTop: 0 }, 'fast');"><i class="fa-solid fa-chevron-up fa-lg" aria-hidden="true"></i> <%= __('post.mobile.back_to_top') %></a>
    </div>

  </div>
</div>

```

# layout/_partial/post/category.ejs

```ejs
<% if (page.categories && page.categories.length) { %>
    <div class="article-category">
        <i class="fa-solid fa-archive"></i>
        <%- list_categories(page.categories, { show_count: false, style: 'link', separator: ' › ' }) %>
    </div>
<% } %>

```

# layout/_partial/post/date.ejs

```ejs
<% if (post.date) { %>
    <div class="<%= class_name %>">
      <% if (is_post()) { %>
        <time datetime="<%= date_xml(post.date) %>" class="dt-published" itemprop="datePublished"><%= date(post.date, config.date_format) %></time>
        <% if (theme.post.show_updated && post.date !== post.updated) { %>
        (Updated: <time datetime="<%= date_xml(post.updated) %>" class="dt-updated" itemprop="dateModified"><%= date(post.updated, config.date_format) %></time>)
        <% } %>
      <% } else { %>
        <% if (is_home() && theme.posts_overview.sort_updated || is_archive() && theme.archive.sort_updated ) { %>
          <time datetime="<%= date_xml(post.updated) %>" class="dt-updated" itemprop="dateModified"><%= date(post.updated, config.date_format) %></time>
        <% } else { %>
          <time datetime="<%= date_xml(post.date) %>" class="dt-published" itemprop="datePublished"><%= date(post.date, config.date_format) %></time>
        <% } %>
      <% } %>
    </div>
<% } %>

```

# layout/_partial/post/gallery.ejs

```ejs
<% if (page.photos && page.photos.length) { %>
<div class="article-gallery">
    <% page.photos.forEach(function(photo, i) { %>
    <a class="gallery-item" href="<%- url_for(photo) %>" rel="gallery_<%= page._id %>">
        <img src="<%- url_for(photo) %>" itemprop="image" />
    </a>
    <% }) %>
</div>
<% } %>

```

# layout/_partial/post/share.ejs

```ejs
<ul>
  <li><a class="icon" href="http://www.facebook.com/sharer.php?u=<%= page.permalink %>"><i class="fab fa-facebook <%= icon_class_name %>" aria-hidden="true"></i></a></li>
  <li><a class="icon" href="https://twitter.com/share?url=<%= page.permalink %>&text=<%= page.title %>"><i class="fab fa-twitter <%= icon_class_name %>" aria-hidden="true"></i></a></li>
  <li><a class="icon" href="http://www.linkedin.com/shareArticle?url=<%= page.permalink %>&title=<%= page.title %>"><i class="fab fa-linkedin <%= icon_class_name %>" aria-hidden="true"></i></a></li>
  <li><a class="icon" href="https://pinterest.com/pin/create/bookmarklet/?url=<%= page.permalink %>&is_video=false&description=<%= page.title %>"><i class="fab fa-pinterest <%= icon_class_name %>" aria-hidden="true"></i></a></li>
  <li><a class="icon" href="mailto:?subject=<%= page.title %>&body=Check out this article: <%= page.permalink %>"><i class="fa-solid fa-envelope <%= icon_class_name %>" aria-hidden="true"></i></a></li>
  <li><a class="icon" href="https://getpocket.com/save?url=<%= page.permalink %>&title=<%= page.title %>"><i class="fab fa-get-pocket <%= icon_class_name %>" aria-hidden="true"></i></a></li>
  <li><a class="icon" href="http://reddit.com/submit?url=<%= page.permalink %>&title=<%= page.title %>"><i class="fab fa-reddit <%= icon_class_name %>" aria-hidden="true"></i></a></li>
  <li><a class="icon" href="http://www.stumbleupon.com/submit?url=<%= page.permalink %>&title=<%= page.title %>"><i class="fab fa-stumbleupon <%= icon_class_name %>" aria-hidden="true"></i></a></li>
  <li><a class="icon" href="http://digg.com/submit?url=<%= page.permalink %>&title=<%= page.title %>"><i class="fab fa-digg <%= icon_class_name %>" aria-hidden="true"></i></a></li>
  <li><a class="icon" href="http://www.tumblr.com/share/link?url=<%= page.permalink %>&name=<%= page.title %>&description=<%= page.excerpt %>"><i class="fab fa-tumblr <%= icon_class_name %>" aria-hidden="true"></i></a></li>
  <li><a class="icon" href="https://news.ycombinator.com/submitlink?u=<%= page.permalink %>&t=<%= page.title %>"><i class="fab fa-hacker-news <%= icon_class_name %>" aria-hidden="true"></i></a></li>
</ul>

```

# layout/_partial/post/tag.ejs

```ejs
<% if (page.tags && page.tags.length) { %>
    <div class="article-tag">
        <i class="fa-solid fa-tag"></i>
        <%- list_tags(page.tags, { show_count: false, style: 'link', class: {a: 'p-category' }}) %>
    </div>
<% } %>

```

# layout/_partial/post/title.ejs

```ejs
<% if (index) { %>
    <% if (post.link) { %>
        <a class="<%= class_name %>" href="<%- url_for(post.link) %>" target="_blank" itemprop="url"><%= post.title %></a>
    <% } else if (post.title) { %>
        <a class="<%= class_name %>" href="<%- url_for(post.path) %>"><%= post.title %></a>
    <% } else { %>
        <a class="<%= class_name %>" href="<%- url_for(post.path) %>">Untitled</a>
    <% } %>
<% } else { %>
    <h1 class="<%= class_name %> p-name" itemprop="name headline">
        <%= post.title %>
    </h1>
<% } %>


```

# layout/_partial/scripts.ejs

```ejs
<!-- jquery -->
<% if (isCdnEnable('jquery')) {%>
  <%- getCdnScript('jquery') %>
<% } else { %>
  <%- js('lib/jquery/jquery.min') %>
<% } %>

<% if (page.photos && page.photos.length) { %>
  <% if (isCdnEnable('justified_gallery_js')) {%>
    <%- getCdnScript('justified_gallery_js') %>
  <% } else { %>
    <%- js('lib/justified-gallery/js/jquery.justifiedGallery.min.js') %>
  <% } %>
<% } %>

<!-- clipboard -->
<% if (is_post()){ %>
  <% if (isCdnEnable('clipboard')) { %>
    <%- getCdnScript('clipboard') %>
  <% } else { %>
    <%- js('lib/clipboard/clipboard.min') %>
  <% } %>
  <script type="text/javascript">
  $(function() {
    // copy-btn HTML
    var btn = "<span class=\"btn-copy tooltipped tooltipped-sw\" aria-label=\"<%= __('tooltip.copy_tip') %>\">";
    btn += '<i class="fa-regular fa-clone"></i>';
    btn += '</span>';
    // mount it!
    $(".highlight table").before(btn);
    var clip = new ClipboardJS('.btn-copy', {
      text: function(trigger) {
        return Array.from(trigger.nextElementSibling.querySelectorAll('.code')).reduce((str,it)=>str+it.innerText+'\n','')
      }
    });
    clip.on('success', function(e) {
      e.trigger.setAttribute('aria-label', "<%= __('tooltip.copied') %>");
      e.clearSelection();
    })
  })
  </script>
<% } %>
<%- js('js/main') %>
<!-- search -->
<% if (config.search && (page.search || page.type === "search")){ %>
  <%- js('js/search.js') %>
  <script type="text/javascript">
  $(function() {

    var $inputArea = $("input#search-input");
    var $resultArea = document.querySelector("div#search-result");

    $inputArea.focus(function() {
      var search_path = "<%= config.search.path %>";
      if (search_path.length == 0) {
        search_path = "search.xml";
      }
      var path = "<%= config.root %>" + search_path;
      searchFunc(path, 'search-input', 'search-result');
    });

    $inputArea.keydown(function(e) {
      if (e.which == 13) {
        e.preventDefault();
      }
    });

    var observer = new MutationObserver(function(mutationsList, observer) {
      if (mutationsList.length == 1) {
        if (mutationsList[0].addedNodes.length) {
          $(".search-no-result").hide();
        } else if (mutationsList[0].removedNodes.length) {
          $(".search-no-result").show(200);
        }
      }
    });

    observer.observe($resultArea, { childList: true });

  });
  </script>
<% } %>
<!-- Baidu Analytics -->
<% if (theme.baidu_analytics.enabled && theme.baidu_analytics.id){ %>
  <script type="text/javascript">
        var _hmt = _hmt || [];
        (function() {
          var hm = document.createElement("script");
          hm.src = "https://hm.baidu.com/hm.js?<%= theme.baidu_analytics.id %>";
          var s = document.getElementsByTagName("script")[0];
          s.parentNode.insertBefore(hm, s);
        })();
        </script>
<% } %>
<!-- Cloudflare Analytics -->
<% if (theme.cloudflare_analytics.enabled && theme.cloudflare_analytics.id){ %>
  <script defer src='https://static.cloudflareinsights.com/beacon.min.js' data-cf-beacon='{"token": "<%= theme.cloudflare_analytics.id %>"}'></script>
<% } %>
<!-- Disqus Comments -->
<% if (page.comments && theme.disqus.enabled && theme.disqus.shortname){ %>
    <script type="text/javascript">
        var disqus_shortname = '<%= theme.disqus.shortname %>';

        (function(){
            var dsq = document.createElement('script');
            dsq.type = 'text/javascript';
            dsq.async = true;
            dsq.src = '//' + disqus_shortname + '.disqus.com/<% if (page.comments){ %>embed.js<% } else { %>count.js<% } %>';
            (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq);
        }());
    </script>
<% } %>
<!-- utterances Comments -->
<% if (page.comments && theme.utterances.enabled && theme.utterances.repo && theme.utterances.issue_term && theme.utterances.theme){ %>
    <script type="text/javascript">
      var utterances_repo = '<%= theme.utterances.repo %>';
      var utterances_issue_term = '<%= theme.utterances.issue_term %>';
      var utterances_label = '<%= theme.utterances.label %>';
      var utterances_theme = '<%= theme.utterances.theme %>';

      (function(){
          var script = document.createElement('script');

          script.src = 'https://utteranc.es/client.js';
          script.setAttribute('repo', utterances_repo);
          script.setAttribute('issue-term', 'pathname');
          script.setAttribute('label', utterances_label);
          script.setAttribute('theme', utterances_theme);
          script.setAttribute('crossorigin', 'anonymous');
          script.async = true;
          (document.getElementById('utterances_thread')).appendChild(script);
      }());
  </script>
<% } %>
```

# layout/_partial/search.ejs

```ejs
<section id="search">
  <form>
    <input type="text" class="search-input" id="search-input" placeholder="<%= __('search.search') %>">
  </form>
  <div id="search-result"></div>
  <p class="search-no-result"><%= __('search.no_results') %></p>
</section>

```

# layout/_partial/styles.ejs

```ejs
<!-- styles -->
<% if (page.photos && page.photos.length) { %>
  <% if (isCdnEnable('justified_gallery_css')) { %>
    <%- getCdnLink('justified_gallery_css', {preload: true}) %> 
  <% } else { %> 
    <link
      rel="preload"
      href="<%- url_for('/lib/justified-gallery/css/justifiedGallery.min.css') %>"
      as="style"
      onload="this.onload=null;this.rel='stylesheet'"/>
    <noscript>
      <link
        rel="stylesheet"
        href="<%- url_for('/lib/justified-gallery/css/justifiedGallery.min.css')  %>"/>
    </noscript>
  <% } %> 
<% } %>

<% if (isCdnEnable('font_awesome')) { %>
  <%- getCdnLink('font_awesome', {preload: true}) %>
<% } else { %> 
  <link
    rel="preload"
    href="<%- url_for('/lib/font-awesome/css/all.min.css') %>"
    as="style"
    onload="this.onload=null;this.rel='stylesheet'"
  />
  <noscript
    ><link
      rel="stylesheet"
      href="<%- url_for('/lib/font-awesome/css/all.min.css') %>"
  /></noscript>
<% } %>

```

# layout/_partial/umami_analytics.ejs

```ejs
<!-- Umami Analytics -->
<% if (theme.umami_analytics.enabled && theme.umami_analytics.id && theme.umami_analytics.host && theme.umami_analytics.script_name){ %>
    <script async defer
            data-website-id="<%= theme.umami_analytics.id %>"
            src="<%= theme.umami_analytics.host %>/<%= theme.umami_analytics.script_name %>">
    </script>
<% } %>

```

# layout/404.ejs

```ejs
<article class="post" itemscope itemtype="http://schema.org/BlogPosting">
    <%- partial('_partial/post/gallery') %>
    <div class="content" itemprop="articleBody">
        <% if (theme.error_404.enabled && theme.error_404.title && theme.error_404.description ) { %>
            <h1><%= theme.error_404.title %></h1>
            <p><%= theme.error_404.description %></p>
        <% } %>
    </div>
</article>
```

# layout/archive.ejs

```ejs
<div id="archive">
  <ul class="post-list">
    <% var year = 0 %>
    <% var change = false %>
    <% var field_sort = theme.archive.sort_updated ? 'updated' : 'date' %>
    <% page.posts.sort(field_sort, 'desc').each(function(post) { %>
      <% var itemYear = date(post[field_sort], 'YYYY') %>
      <% change = year !== itemYear %>
      <% year = change ? itemYear : year %>
      <% if (change) { %>
        <li class="post-year"><h2><%= year %></h2></li>
      <% } %>
      <li class="post-item">
        <%- partial('_partial/post/date', { post: post, class_name: 'meta' }) %>
        <span><%- partial('_partial/post/title', { post: post, index: true, class_name: '' }) %></span>
      </li>
    <% }); %>
  </ul>
  <%- partial('_partial/pagination') %>
</div>

```

# layout/index.ejs

```ejs
<section id="about" class="p-note">
  <% if (config.description) { %>
    <%- markdown(config.description) %>
  <% } %>
  <% if (theme.social_links) { %>
    <p>
      <%= __('index.find_me_on') %>
      <% var nb_links = theme.social_links.length %>
      <% var i = 0 %>
      <% for(var {label, icon, link} of theme.social_links) { %>
        <% var title = label || icon %>
        <% if (icon == 'mail') { %>
          <a class="icon u-email" target="_blank" rel="noopener" href="<%- link %>" aria-label="<%- title %>" title="<%- title %>">
            <i class="fa-solid fa-envelope"></i><!--
      ---></a>
        <% } else if (icon == 'rss') { %>
          <a class="icon" target="_blank" rel="noopener" href="<%- link %>" aria-label="<%- title %>" title="<%- title %>">
            <i class="fa-solid fa-rss"></i>
          </a>
        <% } else { %>
          <a class="icon u-url" target="_blank" rel="noopener me" href="<%- url_for(link) %>" aria-label="<%- title %>" title="<%- title %>">
            <i class="fa-brands fa-<%= icon %>"></i><!--
      ---></a><!--
    ---><% } %><!--
    ---><%= ( nb_links > 0 && i < nb_links-1 ?
            ( i == nb_links-2 ? ' '+__('index.enum_and')+' '
            : __('index.enum_comma')+' ' )
            : '.' ) %>
        <% i+=1 %>
      <% } %>
    </p>
  <% } %>
</section>

<section id="writing">
  <span class="h1"><a href="<%- url_for(theme.nav.articles) %>"><%= __('index.articles') %></a></span>
  <% if (theme.tags_overview && site.tags.length) { %>
  <span class="h2"><%= __('index.topics') %></span>
  <span class="widget tagcloud">
    <%- tagcloud(theme.tags_overview) %>
  </span>
  <span class="h2"><%= __('index.most_recent') %></span>
  <% } %>
  <ul class="post-list">
    <% var field_sort = theme.posts_overview.sort_updated ? 'updated' : 'date' %>
    <% if (theme.posts_overview.show_all_posts) { %>
      <% var show_posts = page.posts.sort(field_sort, 'desc') %>
    <% } else { %>
      <% var show_posts = site.posts.sort(field_sort, 'desc').limit(theme.posts_overview.post_count || 5) %>
    <% } %>
    <% show_posts.each(function(post, i){ %>
      <li class="post-item">
        <%- partial('_partial/post/date', { post: post, class_name: 'meta' }) %>
        <span><%- partial('_partial/post/title', { post: post, index: true, class_name: '' }) %></span>
      </li>
    <% }); %>
  </ul>
  <% if (theme.posts_overview.show_all_posts) { %>
    <%- partial('_partial/pagination') %>
  <% } %>
</section>

<% if (site.data.projects) { %>
<section id="projects">
  <span class="h1"><a href="<%- url_for(theme.projects_url) %>"><%= __('index.projects') %></a></span>
  <ul class="project-list">
    <% for(var obj in site.data.projects){ %>
      <li class="project-item">
        <a href="<%= site.data.projects[obj].url %>"><%= site.data.projects[obj].name %></a>: <%- markdown(site.data.projects[obj].desc) %>
      </li>
    <% } %>
  </ul>
</section>
<% } %>

```

# layout/layout.ejs

```ejs
<!DOCTYPE html>
<html<%= config.language ? " lang=" + config.language.substring(0, 2) : ""%>>
<%- partial('_partial/head') %>
<body class="max-width mx-auto px3 <%- theme.direction -%>">
    <% if (is_post()) { %>
      <%- partial('_partial/post/actions_desktop') %>
    <% } %>
    <div class="content index py4 <%= is_home() ? 'h-card' : '' %>">
        <% if (!is_post()) { %>
          <%- partial('_partial/header') %>
        <% } %>
        <%- body %>
        <% if (is_post()) { %>
          <%- partial('_partial/post/actions_mobile') %>
        <% } %>
        <%- partial('_partial/footer') %>
    </div>
    <%- partial('_partial/styles') %>
    <%- partial('_partial/scripts') %>
</body>
</html>

```

# layout/page.ejs

```ejs
<article class="post" itemscope itemtype="http://schema.org/BlogPosting">
  <%- partial('_partial/post/gallery') %>
  <div class="content" itemprop="articleBody">
      <% if (page.search || page.type === "search") { %>
        <%- partial('_partial/search') %>
      <% } else if (page.type === "tags") { %>
          <div id="tag-cloud">
            <div class="tag-cloud-title">
                <% var visibleTags = 0 %>
                <% site.tags.each(function(tag){ %>
                  <% if (tag.length) { %>
                    <% visibleTags += 1 %>
                  <% } %>
                <% }) %>
                <%- _p('counter.tag_cloud', visibleTags) %>
            </div>
            <div class="tag-cloud-tags">
              <%- tagcloud({min_font: 12, max_font: 30, amount: 300}) %>
            </div>
          </div>
        <% } else if (page.type === 'categories') { %>
          <div id="categories">
            <div class="category-list-title">
                <% var visibleCategories = 0 %>
                <% site.categories.each(function(cat){ %>
                  <% if (cat.length) { %>
                    <% visibleCategories += 1 %>
                  <% } %>
                <% }) %>
                <%- _p('counter.categories', visibleCategories) %>
            </div>
            <div class="category-list">
              <%- list_categories() %>
            </div>
          </div>
        <% } else { %>
          <%- page.content %>
        <% } %>
  </div>
</article>

```

# layout/post.ejs

```ejs
<article class="post h-entry" itemscope itemtype="http://schema.org/BlogPosting">
  <header>
    <%- partial('_partial/post/title', { post: page, index: false, class_name: 'posttitle' }) %>
    <div class="meta">
      <span class="author p-author h-card" itemprop="author" itemscope itemtype="http://schema.org/Person">
        <span class="p-name" itemprop="name"><% if (page.author) { %><%- page.author %><% } else { %><%- config.author %><% } %></span>
      </span>
      <%- partial('_partial/post/date', { post: page, class_name: 'postdate' }) %>
      <%- partial('_partial/post/category') %>
      <%- partial('_partial/post/tag') %>
    </div>
  </header>
  <%- partial('_partial/post/gallery') %>
  <div class="content e-content" itemprop="articleBody">
    <%- page.content %>
  </div>
</article>
<%- partial('_partial/comments') %>

```

# LICENSE

```
The MIT License (MIT)

Copyright (c) 2016 Pieter Robberechts
Copyright (c) 2017 Gabriela Thumé (light colorscheme)
Copyright (c) 2017 Natalya Kosenko (white colorscheme)


Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

```

# package.json

```json
{
  "name": "hexo-theme-cactus",
  "version": "3.0.0",
  "description": "A responsive, clean and simple theme for Hexo.",
  "main": "index.js",
  "scripts": {
    "lint": "gulp lint --silent",
    "test": "gulp validate --silent",
    "clean": "stylus-supremacy format source/css/**/*.styl --options .stylintrc -r"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/probberechts/cactus-dark.git"
  },
  "keywords": [
    "Hexo",
    "Theme",
    "Cactus"
  ],
  "author": "Pieter Robberechts",
  "license": "MIT",
  "bugs": {
    "url": "https://github.com/probberechts/cactus-dark/issues"
  },
  "homepage": "https://github.com/probberechts/cactus-dark#readme",
  "type": "module",
  "devDependencies": {
    "del": "*",
    "gulp": "^4.0.0",
    "gulp-decompress": "*",
    "gulp-download-stream": "*",
    "gulp-jshint": "*",
    "gulp-stylint": "*",
    "js-yaml": "*",
    "jshint": "^2.9.6",
    "jshint-stylish": "*",
    "stylelint-formatter-pretty": "^3.1.0",
    "stylint": "*",
    "stylus-supremacy": "^2.12.2"
  },
  "dependencies": {
    "@fortawesome/fontawesome-free": "*",
    "clipboard": "^2.0.4",
    "jquery": "^3.3.1",
    "justifiedGallery": "^3.6.5",
    "vazir-font": "*"
  }
}

```

# README.md

```md
# Cactus

A responsive, clean and simple [Hexo](http://hexo.io) theme for a personal website.

:cactus: [Demo](https://probberechts.github.io/hexo-theme-cactus/)

![screenshot](https://user-images.githubusercontent.com/2175271/137625287-24a4ac77-fbc9-4c99-a4cd-90455d93d13c.png)

## Summary

- [General](#general)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Install](#install)
- [Configuration](#configuration)
- [License](#license)

## General

- **Version** : 3.0
- **Compatibility** : Hexo 3 or later

## Features

- Fully responsive
- Multiple color schemes
- Pick your own code highlighting scheme
- Configurable navigation menu
- Support for local search
- Projects list
- I18n support
- Disqus / Utterances
- Google analytics / Baidu Tongji / [Umami Analytics](https://umami.is) 
- Font Awesome icons
- Simplicity

## Prerequisites

1. In order to use this theme you must have installed [hexo](https://hexo.io/docs/).

2. Create the `root` directory for the blog by initializing it with hexo:

    \`\`\`sh
    $ hexo init my-blog
    \`\`\`

3. Navigate into the new directory:

    \`\`\`sh
    $ cd my-blog
    \`\`\`

## Install

1. In the `root` directory:

    \`\`\`sh
    $ git clone https://github.com/probberechts/hexo-theme-cactus.git themes/cactus
    \`\`\`

2. Change the `theme` property in the `_config.yml` file.

    \`\`\`yml
    # theme: landscape
    theme: cactus
    \`\`\`
   
   See below for more information on how to customize this theme.

3. Create pages and articles with the `hexo new [layout] <title>` command.
   For example, to create an "about me" page, run:
   
    \`\`\`sh
    $ hexo new page about
    \`\`\`
   
   This will create a new file in `source/about/index.md`
   Similarly, you can create a new article with
   
    \`\`\`sh
    $ hexo new post "hello world"
    \`\`\`
   
   and add some interesting content in `source/_posts/hello-world.md`.

4. Run: `hexo generate` and `hexo server`

5. [Publish your blog](https://hexo.io/docs/one-command-deployment.html)!

## Configuration

You can (and should) modify a couple of settings. An overview of all settings
can be found in  [_config.yml](_config.yml). The most important ones are
discussed below.

There are two possible methods to override the defaults. As a first option,
you could fork the theme and maintain a custom branch with your settings.
Alternatively, you can configure it from your site's primary configuration
file. Therefore, define your custom settings under the `theme_config` variable.
For example:

\`\`\`yml
# _config.yml
theme_config:
  colorscheme: white
\`\`\`

\`\`\`yml
# themes/cactus/_config.yml
colorscheme: dark
\`\`\`

This will override the default black colorscheme in `themes/cactus/_config.yml`.

### Color scheme

Currently, this theme is delivered with four color schemes: [dark](https://probberechts.github.io/hexo-theme-cactus/cactus-dark/public/), [light](https://probberechts.github.io/hexo-theme-cactus/cactus-light/public/),
[white](https://probberechts.github.io/hexo-theme-cactus/cactus-white/public/) and [classic](https://probberechts.github.io/hexo-theme-cactus/cactus-classic/public/). Set your preferred color scheme in the `_config.yml` file.

\`\`\`yml
colorscheme: light
\`\`\`

Alternatively, you can easily create your own color scheme by creating a new
file in `source/css/_colors`.

### Navigation

Set up the navigation menu in the `_config.yml`:

\`\`\`yml
nav:
  home: /
  about: /about/
  articles: /archives/
  projects: http://github.com/probberechts
  LINK_NAME: URL
\`\`\`

### Blog posts list on home page

You have two options for the list of blog posts on the home page:

  - Show only the 5 most recent posts (default)

    \`\`\`yml
    posts_overview:
      show_all_posts: false
      post_count: 5
    \`\`\`

  - Show all posts

    \`\`\`yml
    posts_overview:
      show_all_posts: true
    \`\`\`

### Projects list

Create a projects file `source/_data/projects.json` to show a list of your projects on the index page.

\`\`\`json
[
    {
       "name":"Hexo",
       "url":"https://hexo.io/",
       "desc":"A fast, simple & powerful blog framework"
    },
    {
       "name":"Font Awesome",
       "url":"http://fontawesome.io/",
       "desc":"The iconic font and CSS toolkit"
    }
]
\`\`\`

### Social media links

Cactus can automatically add links to your social media accounts.
Therefore, update the theme's `_config.yml`:

\`\`\`yml
social_links:
  -
    icon: github
    link: your-github-url
  -
    icon: twitter
    label: "@your-twitter-handle"
    link: your-twitter-url
  -
    icon: NAME
    label: LABEL
    link: your-NAME-url
\`\`\`

where `NAME` is the name of a [Font Awesome icon](https://fontawesome.com/icons?d=gallery&s=brands), and LABEL is an optional value used as a title attribute on the link (NAME value is used if LABEL is missing).

### Copyright years

By default, Cactus will use current year in your copyright year information.
If there is a need to customize, please update `_config.yml`:

\`\`\`yml
copyright:
  start_year: 2016
  end_year:
\`\`\`

### Language configuration

If you are new to Hexo and internationalization (i18n), please read
[Hexo documentation - internationalization (i18n) section](https://hexo.io/docs/internationalization.html)

Currently, the theme is delivered with support for:

- English (en), default
- Arabic (ar)
- Brazilian Portuguese (pt-BR)
- Catalan (ca)
- Chinese (Simplified, PRC) (zh-CN)
- Dutch (nl)
- French (fr)
- German (de)
- Italian (it)
- Korean (kr)
- Persian (fa)
- Polish (pl)
- Russian (ru)
- Spanish (es)
- Taiwanese (Taiwanese Mandarin) (zh-TW)
- Turkish (tr)
- Ukrainian (ua)
- Vietnamese (vi)

If you would like to use one the languages listed above, simply set `language`
to the desired language (e.g., `fr`) in `_config.yml`.
Otherwise, you can follow the steps below (E.g., to add a Japanese (ja) translation):

1. Set `language` to `ja` in Hexo configuration file `_config.yml`
2. Create a `ja.yml` file in the `themes/cactus/languages/` folder
3. Copy the content of `themes/cactus/languages/default.yml` and paste it it into the `ja.yml` file
4. Replace all English strings by their Japanese translation

**Note: Cactus does not support multi-language sites.**

### RTL support

This theme support RTL languages for Persian and Arabic language.
If you would like to use RTL layout, change `direction` attribute in `_config.yml` to `rtl`.
Note that this also will change the font to [Vazir](https://github.com/rastikerdar/vazir-font), which is a Persian font.

\`\`\`
direction: rtl
\`\`\`

### RSS

Set the `rss` field in the `_config.yml` to one of the following values:

1. `rss: false` will totally disable rss (default).
2. `rss: atom.xml` sets a specific feed link.
3. `rss:`leave empty to use the [hexo-generator-feed](https://github.com/hexojs/hexo-generator-feed) plugin.

### Analytics

Add you Google, Baidu, Cloudflare or Umami Analytics `tracking_id` to the `_config.yml`.

\`\`\`yml
google_analytics:
  enabled: true
  id: 'UA-49627206-1'

baidu_analytics:
  enabled: true
  id: 2e6da3c375c8a87f5b664cea6d4cb29c

cloudflare_analytics:
  enabled: true
  id: 0dabb6e21848405483a237e6a7b6ed04

umami_analytics:
  enabled: false
  id: e77e68be-f6e4-4br3-9365-2b76b57cd571
  host: https://analytics.domain.com
  script_name: umami.js
\`\`\`

### CDN

Load Javascript and CSS resources from a CDN. Enabled by default, loads all resources from [cdnjs](https://cdnjs.com/).

\`\`\`yml
cdn:
  enable: true
  jquery: 'url'
  clipboard: 'url'
  font_awesome: 'url'
  justified_gallery_css: 'url'
  justified_gallery_js: 'url'
\`\`\`

Set `enable: false` to completely disable CDN and load all resources from your domain. If you want to disable it only for specific resource(s) then just remove the corresponding entry(s).

\`\`\`yml
cdn:
  enable: true
  jquery: 'url'
\`\`\`

Only JQuery will be loaded from the specified CDN.

### Comments

Cactus supports two commenting systems: [Disqus](https://disqus.com) and [Utterances](https://utteranc.es).

#### Disqus

First, create a site on Disqus: [https://disqus.com/admin/create/](http://disqus.com/admin/create/).

Next, update the `_config.yml` file:

\`\`\`yml
disqus:
  enabled: true
  shortname: SITENAME
\`\`\`

where `SITENAME` is the name you gave your site on Disqus.

#### Utterances

First, follow the instructions on the [oficial website](https://utteranc.es/) to setup an issue tracker Utterances will connect to.

Next, update the `_config.yml` file:

\`\`\`yml
utterances:
  enabled: true
  repo: owner/githubrepo
  issue_term: pathname
  label: utteranc
  theme: themename
\`\`\`

where each of the parameters are the respective values ​​provided during the configuration of the Utterances:

* `repo`:  the repository Utterances will connect to.
* `issue_term`: the mapping between blog posts and GitHub issues.
* `label`: the label that will be assigned to issues created by Utterances
* `theme`: the selected Utterances theme.

### Code Highlighting

Pick one of [the available colorschemes](https://github.com/probberechts/hexo-theme-cactus/tree/master/source/css/_highlight) and add it to the `_config.yml`:

\`\`\`yml
highlight: COLORSCHEME_NAME
\`\`\`

### Tags and categories

Tags and categories can be included in the front-matter of your posts. For example:

\`\`\`markdown
title: Tags and Categories
date: 2017-12-24 23:29:53
tags:
- Foo
- Bar
categories: 
- Baz
---

This post contains 2 tags and 1 category.
\`\`\`

You can create a page with a tag cloud by running:

\`\`\`sh
$ hexo new page tags
\`\`\`

Next, add `type: tags` to the front-matter of `source/tags/index.md`. You can also
add a tag cloud to the home page by setting the `tags_overview` option to `true`.

Similarly, you can create a page with an overview of all categories by running:

\`\`\`sh
$ hexo new page categories
\`\`\`

and adding `type: categories` to the front-matter of `source/categories/index.md`. 

Finally, don't forget to create a link to these pages, for example in the navigation menu:

\`\`\`yml
nav:
  tag: /tags/
  category: /categories/
\`\`\`

### Local search

First, install the [hexo-generate-search](https://www.npmjs.com/package/hexo-generator-search)
plugin, which will generate a search index file.

\`\`\`git
$ npm install hexo-generator-search --save
\`\`\`

Next, create a page to display the search engine:

\`\`\`sh
$ hexo new page search
\`\`\`

and put `type: search` in the front-matter.

\`\`\`markdown
title: Search
type: search
---
\`\`\`

Finally, edit the `_config.yml` and add a link to the navigation menu.

\`\`\`yml
nav:
  search: /search/
\`\`\`

## License

MIT

```

# scripts/cdn.js

```js
/**
 * returns true if cdn is enabled and there's an entry for the specified
 * resource
 */
hexo.extend.helper.register('isCdnEnable', function (resource) {
  return (
    hexo.theme.config.cdn &&
    hexo.theme.config.cdn.enable &&
    hexo.theme.config.cdn[resource]
  );
});

/**
 * returns the script tag to load the specified resource from a CDN
 */
hexo.extend.helper.register('getCdnScript', function (resource) {
  return `<script src="${hexo.theme.config.cdn[resource]}" crossorigin="anonymous"></script>`;
});

/**
 * returns the link tag to load the specified resource from a CDN
 */
hexo.extend.helper.register('getCdnLink', function (resource, options) {
  options = options || {};
  if (options.preload) {
    return `<link rel="preload" as="style" href="${hexo.theme.config.cdn[resource]}" crossorigin="anonymous" onload="this.onload=null;this.rel='stylesheet'"/>`
  }
  return `<link rel="stylesheet" href="${hexo.theme.config.cdn[resource]}" crossorigin="anonymous" />`;
});

```

# scripts/error_404.js

```js
/**
* error 404 page Generator
* @description generate the 404.html in root directory
*/

hexo.extend.generator.register('error_404', function (locals) {
    return {
        path: '404.html',
        data: locals.posts,
        layout: '404'
    }
})
```

# scripts/merge-configs.js

```js
/**
* Merge all `theme_config.*` options from main Hexo config into hexo.theme.config.
* This fixes an issue with hexo-renderer-stylus, which otherwise ignores these
* configuration overrides.
*/
hexo.on('generateBefore', function () {
  hexo.theme.config = Object.assign({}, hexo.theme.config, hexo.config.theme_config);
});

```

# scripts/meta.js

```js
/**
* Meta Helper
* @description Generate meta tags for HTML header
* @example
*     <%- meta(post) %>
*/
function trim (str) {
    return str.trim().replace(/^"(.*)"$/, '$1').replace(/^'(.*)'$/, '$1');
}

function split (str, sep) {
    var result = [];
    var matched = null;
    while (matched = sep.exec(str)) {
        result.push(matched[0]);
    }
    return result;
}

hexo.extend.helper.register('meta', function (post) {
    var metas = post.meta || [];
    var metaDOMArray = metas.map(function (meta) {
        var entities = split(meta, /(?:[^\\;]+|\\.)+/g);
        var entityArray = entities.map(function (entity) {
            var keyValue = split(entity, /(?:[^\\=]+|\\.)+/g);
            if (keyValue.length < 2) {
                return null;
            }
            var key = trim(keyValue[0]);
            var value = trim(keyValue[1]);
            return key + '="' + value + '"';
        }).filter(function (entity) {
            return entity;
        });
        return '<meta ' + entityArray.join(' ') + ' />';
    });
    return metaDOMArray.join('\n');
});

```

# scripts/page_title.js

```js
/**
 * Page Title Helper
 * @description Generate page title.
 * @example
 *     <%- page_title() %>
 */
hexo.extend.helper.register("page_title", function () {
  var title = this.page.title ? this.page.title : this.config.title;

  if (this.is_archive()) {
    title = this.__("nav.articles");

    if (this.is_month()) {
      title += ": " + this.page.year + "/" + this.page.month;
    } else if (this.is_year()) {
      title += ": " + this.page.year;
    }
  } else if (this.is_category()) {
    title = this.__("nav.category") + ": " + this.page.category;
  } else if (this.is_tag()) {
    title = this.__("nav.tag") + ": " + this.page.tag;
  }

  return title;
});

```

# scripts/thumbnail.js

```js
/**
* Thumbnail Helper
* @description Get the thumbnail url from a post
* @example
*     <%- thumbnail(post) %>
*/
hexo.extend.helper.register('thumbnail', function (post) {
    return post.thumbnail || post.banner || '';
});

```

# source/css/_colors/classic.styl

```styl
$color-background = #fafafa
$color-footer-mobile-1 = darken($color-background, 2%)
$color-footer-mobile-2 = darken($color-background, 10%)
$color-background-code = darken($color-background, 2%)
$color-border = #666
$color-scrollbar = #AAA
$color-meta = #666
$color-meta-code = lighten($color-meta, 10%)
$color-link = rgba(86, 124, 119, .4)
$color-text = #22272a
$color-accent-1 = #cc2a41
$color-accent-2 = rgba(86, 124, 119, .8)
$color-accent-3 = #666
$color-quote = #cc2a41
$highlight = hexo-config("highlight") || "github"

```

# source/css/_colors/dark.styl

```styl
$color-background = #1d1f21
$color-footer-mobile-1 = lighten($color-background, 2%)
$color-footer-mobile-2 = lighten($color-background, 10%)
$color-background-code = lighten($color-background, 2%)
$color-border = #908d8d
$color-scrollbar = #999
$color-meta = #908d8d
$color-meta-code = #908d8d
$color-link = rgba(212, 128, 170, 1)
$color-text = #c9cacc
$color-accent-3 = #cccccc
$color-accent-2 = #eeeeee
$color-accent-1 = #2bbc8a
$color-quote = #ccffb6
$highlight = hexo-config("highlight") || "rainbow"

```

# source/css/_colors/light.styl

```styl
// by @GabiThume (https://github.com/gabithume)
$color-background = #e2e0de
$color-footer-mobile-1 = darken($color-background, 2%)
$color-footer-mobile-2 = darken($color-background, 10%)
$color-background-code = darken($color-background, 2%)
$color-border = #666
$color-scrollbar = #999
$color-meta = #666
$color-meta-code = lighten($color-meta, 10%)
$color-link = rgba(43, 188, 138, 1)
$color-text = #363533
$color-accent-3 = #666666
$color-accent-2 = #111111
$color-accent-1 = #d44375
$color-quote = #ab2251
$highlight = hexo-config("highlight") || "github"

```

# source/css/_colors/white.styl

```styl
// by @sergodeeva (https://github.com/sergodeeva)
$color-background = #FFFFFF
$color-footer-mobile-1 = darken($color-background, 2%)
$color-footer-mobile-2 = darken($color-background, 10%)
$color-background-code = darken($color-background, 2%)
$color-border = #666
$color-scrollbar = #AAA
$color-meta = #666
$color-meta-code = lighten($color-meta, 10%)
$color-link = rgba(212, 128, 170, 1)
$color-text = #383838
$color-accent-3 = #8c8c8c
$color-accent-2 = #383838
$color-accent-1 = #2bbc8a
$color-quote = #2bbc8a
$highlight = hexo-config("highlight") || "atelier-cave-light"

```

# source/css/_extend.styl

```styl
$base-style
  h1, .h1
    display: block
    margin-top: 3rem
    margin-bottom: 1rem
    color: $color-accent-1
    letter-spacing: .01em
    font-weight: 700
    font-style: normal
    font-size: 1.5em

    antialias()

  h2, .h2
    position: relative
    display: block
    margin-top: 2rem
    margin-bottom: .5rem
    color: $color-accent-2
    text-transform: none
    letter-spacing: normal
    font-weight: bold
    font-size: 1rem

  h3
    color: $color-accent-2
    text-decoration: underline
    font-weight: bold
    font-size: .9rem

  h4
  h5
  h6
    display: inline
    text-decoration: none
    color: $color-accent-3
    font-weight: bold
    font-size: .9rem

  h3
  h4
  h5
  h6
    margin-top: .9rem
    margin-bottom: .5rem

  hr
    border: .5px dashed $color-accent-3
    opacity: .5
    margin: 0
    margin-top: 20px
    margin-bottom: 20px

  strong
    font-weight: bold

  em
  cite
    font-style: italic

  sup
  sub
    position: relative
    vertical-align: baseline
    font-size: .75em
    line-height: 0

  sup
    top: -.5em

  sub
    bottom: -.2em

  small
    font-size: .85em

  acronym
  abbr
    border-bottom: 1px dotted

  ul
  ol
  dl
    line-height: $line-height

  ul
  ol
    ul
    ol
      margin-top: 0
      margin-bottom: 0

  ol
    list-style: decimal

  dt
    font-weight: bold

  table
    width: 100%
    border-collapse: collapse
    text-align: left
    font-size: $font-size - 2px
    overflow: auto
    display: block

  th
    padding: 8px
    border-bottom: 1px dashed $color-border
    color: $color-accent-2
    font-weight: bold
    font-size: $font-size - 1px

  td
    padding: 0 8px
    border-bottom: none

```

# source/css/_fonts.styl

```styl
@font-face
  font-style: normal
  font-family: "Meslo LG"
  src: local("Meslo LG S"), url("../lib/meslo-LG/MesloLGS-Regular.ttf") format("truetype")

```

# source/css/_highlight/agate.styl

```styl
/*
 * Agate by Taufik Nurrohman <https://github.com/tovic>
 * ----------------------------------------------------
 * 
 * #ade5fc
 * #a2fca2
 * #c6b4f0
 * #d36363
 * #fcc28c
 * #fc9b9b
 * #ffa
 * #fff
 * #333
 * #62c8f3
 * #888
 * 
 */
.highlight
  background: #333
  color: white

  .code
    .name, .strong
      font-weight: bold

    .code, .emphasis
      font-style: italic

    .tag
      color: #62c8f3

    .variable, .template-variable, .selector-id, .selector-class
      color: #ade5fc

    .string, .bullet
      color: #a2fca2

    .type, .title, .section, .attribute, .quote, .built_in, .builtin-name
      color: #ffa

    .number, .symbol, .bullet
      color: #d36363

    .keyword, .selector-tag, .literal
      color: #fcc28c

    .comment, .deletion, .code
      color: #888

    .regexp, .link
      color: #c6b4f0

    .meta
      color: #fc9b9b

    .deletion
      background-color: #fc9b9b
      color: #333

    .addition
      background-color: #a2fca2
      color: #333

    .highlight a
      color: inherit

    .highlight a:focus, .highlight a:hover
      color: inherit
      text-decoration: underline

```

# source/css/_highlight/androidstudio.styl

```styl
/*
   Date: 24 Fev 2015
   Author: Pedro Oliveira <kanytu@gmail . com>
*/
.highlight
  background: #282b2e
  color: #a9b7c6

  .code
    .number, .literal, .symbol, .bullet
      color: #6897BB

    .keyword, .selector-tag, .deletion
      color: #cc7832

    .variable, .template-variable, .link
      color: #629755

    .comment, .quote
      color: #808080

    .meta
      color: #bbb529

    .string, .attribute, .addition
      color: #6A8759

    .section, .title, .type
      color: #ffc66d

    .name, .selector-id, .selector-class
      color: #e8bf6a

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/arduino-light.styl

```styl
/*

Arduino® Light Theme - Stefania Mellai <s.mellai@arduino.cc>

*/

.highlight
    color: #434f54
    background: #FFFFFF
    .code
        .subst
            color: #434f54

        .keyword,
        .attribute,
        .selector-tag,
        .doctag,
        .name
            color: #00979D

        .built_in,
        .literal,
        .bullet,
        .code,
        .addition
            color: #D35400

        .regexp,
        .symbol,
        .variable,
        .template-variable,
        .link,
        .selector-attr,
        .selector-pseudo
            color: #00979D

        .type,
        .string,
        .selector-id,
        .selector-class,
        .quote,
        .template-tag,
        .deletion
            color: #005C5F

        .title,
        .section
            color: #880000
            font-weight: bold

        .comment
            color: rgba(149,165,166,.8)

        .meta-keyword
            color: #728E00

        .meta
            color: #728E00
            color: #434f54

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

        .function
            color: #728E00

        .number
            color: #8A7B52

```

# source/css/_highlight/arta.styl

```styl
/*
   Date: 17.V.2011
   Author: pumbur <pumbur@pumbur.net>
*/
.highlight
  background: #222
  color: #aaa

  .code
    .subst
      color: #aaa

    .section
      color: #fff

    .comment, .quote, .meta
      color: #444

    .string, .symbol, .bullet, .regexp
      color: #ffcc33

    .number, .addition
      color: #00cc66

    .built_in, .builtin-name, .literal, .type, .template-variable, .attribute, .link
      color: #32aaee

    .keyword, .selector-tag, .name, .selector-id, .selector-class
      color: #6644aa

    .title, .variable, .deletion, .template-tag
      color: #bb1166

    .section, .doctag, .strong
      font-weight: bold

    .emphasis
      font-style: italic

```

# source/css/_highlight/ascetic.styl

```styl
/*

Original style from softwaremaniacs.org (c) Ivan Sagalaev <Maniac@SoftwareManiacs.Org>

*/

.highlight
    color: black
    background: white
    .code
        .string,
        .variable,
        .template-variable,
        .symbol,
        .bullet,
        .section,
        .addition,
        .attribute,
        .link
            color: #888

        .comment,
        .quote,
        .meta,
        .deletion
            color: #ccc

        .keyword,
        .selector-tag,
        .section,
        .name,
        .type,
        .strong
            font-weight: bold

        .emphasis
            font-style: italic

```

# source/css/_highlight/atelier-cave-dark.styl

```styl
/* Base16 Atelier Cave Dark - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/cave) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */
.highlight
  background: #19171c
  color: #8b8792

  .code
    /* Atelier-Cave Comment */
    .comment, .quote
      color: #7e7887

    /* Atelier-Cave Red */
    .variable, .template-variable, .attribute, .regexp, .link, .tag, .name, .selector-id, .selector-class
      color: #be4678

    /* Atelier-Cave Orange */
    .number, .meta, .built_in, .builtin-name, .literal, .type, .params
      color: #aa573c

    /* Atelier-Cave Green */
    .string, .symbol, .bullet
      color: #2a9292

    /* Atelier-Cave Blue */
    .title, .section
      color: #576ddb

    /* Atelier-Cave Purple */
    .keyword, .selector-tag
      color: #955ae7

    .deletion, .addition
      display: inline-block
      width: 100%
      color: #19171c

    .deletion
      background-color: #be4678

    .addition
      background-color: #2a9292

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/atelier-cave-light.styl

```styl
/* Base16 Atelier Cave Light - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/cave) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */

.highlight
    color: #585260
    background: #efecf4
    .code
        /* Atelier-Cave Comment */
        .comment,
        .quote
            color: #655f6d

        /* Atelier-Cave Red */
        .variable,
        .template-variable,
        .attribute,
        .tag,
        .name,
        .regexp,
        .link,
        .name,
        .name,
        .selector-id,
        .selector-class
            color: #be4678

        /* Atelier-Cave Orange */
        .number,
        .meta,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params
            color: #aa573c

        /* Atelier-Cave Green */
        .string,
        .symbol,
        .bullet
            color: #2a9292

        /* Atelier-Cave Blue */
        .title,
        .section
            color: #576ddb

        /* Atelier-Cave Purple */
        .keyword,
        .selector-tag
            color: #955ae7

        .deletion,
        .addition
            color: #19171c
            display: inline-block
            width: 100%

        .deletion
            background-color: #be4678

        .addition
            background-color: #2a9292

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/atelier-dune-dark.styl

```styl
/* Base16 Atelier Dune Dark - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/dune) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */
.highlight
  background: #20201d
  color: #a6a28c

  .code
    /* Atelier-Dune Comment */
    .comment, .quote
      color: #999580

    /* Atelier-Dune Red */
    .variable, .template-variable, .attribute, .tag, .name, .regexp, .link, .name, .selector-id, .selector-class
      color: #d73737

    /* Atelier-Dune Orange */
    .number, .meta, .built_in, .builtin-name, .literal, .type, .params
      color: #b65611

    /* Atelier-Dune Green */
    .string, .symbol, .bullet
      color: #60ac39

    /* Atelier-Dune Blue */
    .title, .section
      color: #6684e1

    /* Atelier-Dune Purple */
    .keyword, .selector-tag
      color: #b854d4

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/atelier-dune-light.styl

```styl
/* Base16 Atelier Dune Light - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/dune) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */

.highlight
    color: #6e6b5e
    background: #fefbec
    .code
        /* Atelier-Dune Comment */
        .comment,
        .quote
            color: #7d7a68

        /* Atelier-Dune Red */
        .variable,
        .template-variable,
        .attribute,
        .tag,
        .name,
        .regexp,
        .link,
        .name,
        .selector-id,
        .selector-class
            color: #d73737

        /* Atelier-Dune Orange */
        .number,
        .meta,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params
            color: #b65611

        /* Atelier-Dune Green */
        .string,
        .symbol,
        .bullet
            color: #60ac39

        /* Atelier-Dune Blue */
        .title,
        .section
            color: #6684e1

        /* Atelier-Dune Purple */
        .keyword,
        .selector-tag
            color: #b854d4

        .highlight
            display: block
            overflow-x: auto
            background: #fefbec
            color: #6e6b5e
            padding: 0.5em

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/atelier-estuary-dark.styl

```styl
/* Base16 Atelier Estuary Dark - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/estuary) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */
.highlight
  background: #22221b
  color: #929181

  .code
    /* Atelier-Estuary Comment */
    .comment, .quote
      color: #878573

    /* Atelier-Estuary Red */
    .variable, .template-variable, .attribute, .tag, .name, .regexp, .link, .name, .selector-id, .selector-class
      color: #ba6236

    /* Atelier-Estuary Orange */
    .number, .meta, .built_in, .builtin-name, .literal, .type, .params
      color: #ae7313

    /* Atelier-Estuary Green */
    .string, .symbol, .bullet
      color: #7d9726

    /* Atelier-Estuary Blue */
    .title, .section
      color: #36a166

    /* Atelier-Estuary Purple */
    .keyword, .selector-tag
      color: #5f9182

    .deletion, .addition
      display: inline-block
      width: 100%
      color: #22221b

    .deletion
      background-color: #ba6236

    .addition
      background-color: #7d9726

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/atelier-estuary-light.styl

```styl
/* Base16 Atelier Estuary Light - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/estuary) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */

.highlight
    color: #5f5e4e
    background: #f4f3ec
    .code
        /* Atelier-Estuary Comment */
        .comment,
        .quote
            color: #6c6b5a

        /* Atelier-Estuary Red */
        .variable,
        .template-variable,
        .attribute,
        .tag,
        .name,
        .regexp,
        .link,
        .name,
        .selector-id,
        .selector-class
            color: #ba6236

        /* Atelier-Estuary Orange */
        .number,
        .meta,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params
            color: #ae7313

        /* Atelier-Estuary Green */
        .string,
        .symbol,
        .bullet
            color: #7d9726

        /* Atelier-Estuary Blue */
        .title,
        .section
            color: #36a166

        /* Atelier-Estuary Purple */
        .keyword,
        .selector-tag
            color: #5f9182

        .deletion,
        .addition
            color: #22221b
            display: inline-block
            width: 100%

        .deletion
            background-color: #ba6236

        .addition
            background-color: #7d9726

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/atelier-forest-dark.styl

```styl
/* Base16 Atelier Forest Dark - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/forest) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */
.highlight
  background: #1b1918
  color: #a8a19f

  .code
    /* Atelier-Forest Comment */
    .comment, .quote
      color: #9c9491

    /* Atelier-Forest Red */
    .variable, .template-variable, .attribute, .tag, .name, .regexp, .link, .name, .selector-id, .selector-class
      color: #f22c40

    /* Atelier-Forest Orange */
    .number, .meta, .built_in, .builtin-name, .literal, .type, .params
      color: #df5320

    /* Atelier-Forest Green */
    .string, .symbol, .bullet
      color: #7b9726

    /* Atelier-Forest Blue */
    .title, .section
      color: #407ee7

    /* Atelier-Forest Purple */
    .keyword, .selector-tag
      color: #6666ea

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/atelier-forest-light.styl

```styl
/* Base16 Atelier Forest Light - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/forest) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */

.highlight
    color: #68615e
    background: #f1efee
    .code
        /* Atelier-Forest Comment */
        .comment,
        .quote
            color: #766e6b

        /* Atelier-Forest Red */
        .variable,
        .template-variable,
        .attribute,
        .tag,
        .name,
        .regexp,
        .link,
        .name,
        .selector-id,
        .selector-class
            color: #f22c40

        /* Atelier-Forest Orange */
        .number,
        .meta,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params
            color: #df5320

        /* Atelier-Forest Green */
        .string,
        .symbol,
        .bullet
            color: #7b9726

        /* Atelier-Forest Blue */
        .title,
        .section
            color: #407ee7

        /* Atelier-Forest Purple */
        .keyword,
        .selector-tag
            color: #6666ea

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/atelier-heath-dark.styl

```styl
/* Base16 Atelier Heath Dark - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/heath) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */
.highlight
  background: #1b181b
  color: #ab9bab

  .code
    /* Atelier-Heath Comment */
    .comment, .quote
      color: #9e8f9e

    /* Atelier-Heath Red */
    .variable, .template-variable, .attribute, .tag, .name, .regexp, .link, .name, .selector-id, .selector-class
      color: #ca402b

    /* Atelier-Heath Orange */
    .number, .meta, .built_in, .builtin-name, .literal, .type, .params
      color: #a65926

    /* Atelier-Heath Green */
    .string, .symbol, .bullet
      color: #918b3b

    /* Atelier-Heath Blue */
    .title, .section
      color: #516aec

    /* Atelier-Heath Purple */
    .keyword, .selector-tag
      color: #7b59c0

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/atelier-heath-light.styl

```styl
/* Base16 Atelier Heath Light - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/heath) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */

.highlight
    color: #695d69
    background: #f7f3f7
    .code
        /* Atelier-Heath Comment */
        .comment,
        .quote
            color: #776977

        /* Atelier-Heath Red */
        .variable,
        .template-variable,
        .attribute,
        .tag,
        .name,
        .regexp,
        .link,
        .name,
        .selector-id,
        .selector-class
            color: #ca402b

        /* Atelier-Heath Orange */
        .number,
        .meta,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params
            color: #a65926

        /* Atelier-Heath Green */
        .string,
        .symbol,
        .bullet
            color: #918b3b

        /* Atelier-Heath Blue */
        .title,
        .section
            color: #516aec

        /* Atelier-Heath Purple */
        .keyword,
        .selector-tag
            color: #7b59c0

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/atelier-lakeside-dark.styl

```styl
/* Base16 Atelier Lakeside Dark - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/lakeside) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */
.highlight
  background: #161b1d
  color: #7ea2b4

  .code
    /* Atelier-Lakeside Comment */
    .comment, .quote
      color: #7195a8

    /* Atelier-Lakeside Red */
    .variable, .template-variable, .attribute, .tag, .name, .regexp, .link, .name, .selector-id, .selector-class
      color: #d22d72

    /* Atelier-Lakeside Orange */
    .number, .meta, .built_in, .builtin-name, .literal, .type, .params
      color: #935c25

    /* Atelier-Lakeside Green */
    .string, .symbol, .bullet
      color: #568c3b

    /* Atelier-Lakeside Blue */
    .title, .section
      color: #257fad

    /* Atelier-Lakeside Purple */
    .keyword, .selector-tag
      color: #6b6bb8

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/atelier-lakeside-light.styl

```styl
/* Base16 Atelier Lakeside Light - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/lakeside) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */

.highlight
    color: #516d7b
    background: #ebf8ff
    .code
        /* Atelier-Lakeside Comment */
        .comment,
        .quote
            color: #5a7b8c

        /* Atelier-Lakeside Red */
        .variable,
        .template-variable,
        .attribute,
        .tag,
        .name,
        .regexp,
        .link,
        .name,
        .selector-id,
        .selector-class
            color: #d22d72

        /* Atelier-Lakeside Orange */
        .number,
        .meta,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params
            color: #935c25

        /* Atelier-Lakeside Green */
        .string,
        .symbol,
        .bullet
            color: #568c3b

        /* Atelier-Lakeside Blue */
        .title,
        .section
            color: #257fad

        /* Atelier-Lakeside Purple */
        .keyword,
        .selector-tag
            color: #6b6bb8

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/atelier-plateau-dark.styl

```styl
/* Base16 Atelier Plateau Dark - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/plateau) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */
.highlight
  background: #1b1818
  color: #8a8585

  .code
    /* Atelier-Plateau Comment */
    .comment, .quote
      color: #7e7777

    /* Atelier-Plateau Red */
    .variable, .template-variable, .attribute, .tag, .name, .regexp, .link, .name, .selector-id, .selector-class
      color: #ca4949

    /* Atelier-Plateau Orange */
    .number, .meta, .built_in, .builtin-name, .literal, .type, .params
      color: #b45a3c

    /* Atelier-Plateau Green */
    .string, .symbol, .bullet
      color: #4b8b8b

    /* Atelier-Plateau Blue */
    .title, .section
      color: #7272ca

    /* Atelier-Plateau Purple */
    .keyword, .selector-tag
      color: #8464c4

    .deletion, .addition
      display: inline-block
      width: 100%
      color: #1b1818

    .deletion
      background-color: #ca4949

    .addition
      background-color: #4b8b8b

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/atelier-plateau-light.styl

```styl
/* Base16 Atelier Plateau Light - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/plateau) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */

.highlight
    color: #585050
    background: #f4ecec
    .code
        /* Atelier-Plateau Comment */
        .comment,
        .quote
            color: #655d5d

        /* Atelier-Plateau Red */
        .variable,
        .template-variable,
        .attribute,
        .tag,
        .name,
        .regexp,
        .link,
        .name,
        .selector-id,
        .selector-class
            color: #ca4949

        /* Atelier-Plateau Orange */
        .number,
        .meta,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params
            color: #b45a3c

        /* Atelier-Plateau Green */
        .string,
        .symbol,
        .bullet
            color: #4b8b8b

        /* Atelier-Plateau Blue */
        .title,
        .section
            color: #7272ca

        /* Atelier-Plateau Purple */
        .keyword,
        .selector-tag
            color: #8464c4

        .deletion,
        .addition
            color: #1b1818
            display: inline-block
            width: 100%

        .deletion
            background-color: #ca4949

        .addition
            background-color: #4b8b8b

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/atelier-savanna-dark.styl

```styl
/* Base16 Atelier Savanna Dark - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/savanna) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */
.highlight
  background: #171c19
  color: #87928a

  .code
    /* Atelier-Savanna Comment */
    .comment, .quote
      color: #78877d

    /* Atelier-Savanna Red */
    .variable, .template-variable, .attribute, .tag, .name, .regexp, .link, .name, .selector-id, .selector-class
      color: #b16139

    /* Atelier-Savanna Orange */
    .number, .meta, .built_in, .builtin-name, .literal, .type, .params
      color: #9f713c

    /* Atelier-Savanna Green */
    .string, .symbol, .bullet
      color: #489963

    /* Atelier-Savanna Blue */
    .title, .section
      color: #478c90

    /* Atelier-Savanna Purple */
    .keyword, .selector-tag
      color: #55859b

    .deletion, .addition
      display: inline-block
      width: 100%
      color: #171c19

    .deletion
      background-color: #b16139

    .addition
      background-color: #489963

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/atelier-savanna-light.styl

```styl
/* Base16 Atelier Savanna Light - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/savanna) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */

.highlight
    color: #526057
    background: #ecf4ee
    .code
        /* Atelier-Savanna Comment */
        .comment,
        .quote
            color: #5f6d64

        /* Atelier-Savanna Red */
        .variable,
        .template-variable,
        .attribute,
        .tag,
        .name,
        .regexp,
        .link,
        .name,
        .selector-id,
        .selector-class
            color: #b16139

        /* Atelier-Savanna Orange */
        .number,
        .meta,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params
            color: #9f713c

        /* Atelier-Savanna Green */
        .string,
        .symbol,
        .bullet
            color: #489963

        /* Atelier-Savanna Blue */
        .title,
        .section
            color: #478c90

        /* Atelier-Savanna Purple */
        .keyword,
        .selector-tag
            color: #55859b

        .deletion,
        .addition
            color: #171c19
            display: inline-block
            width: 100%

        .deletion
            background-color: #b16139

        .addition
            background-color: #489963

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/atelier-seaside-dark.styl

```styl
/* Base16 Atelier Seaside Dark - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/seaside) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */
.highlight
  background: #131513
  color: #8ca68c

  .code
    /* Atelier-Seaside Comment */
    .comment, .quote
      color: #809980

    /* Atelier-Seaside Red */
    .variable, .template-variable, .attribute, .tag, .name, .regexp, .link, .name, .selector-id, .selector-class
      color: #e6193c

    /* Atelier-Seaside Orange */
    .number, .meta, .built_in, .builtin-name, .literal, .type, .params
      color: #87711d

    /* Atelier-Seaside Green */
    .string, .symbol, .bullet
      color: #29a329

    /* Atelier-Seaside Blue */
    .title, .section
      color: #3d62f5

    /* Atelier-Seaside Purple */
    .keyword, .selector-tag
      color: #ad2bee

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/atelier-seaside-light.styl

```styl
/* Base16 Atelier Seaside Light - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/seaside) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */

.highlight
    color: #5e6e5e
    background: #f4fbf4
    .code
        /* Atelier-Seaside Comment */
        .comment,
        .quote
            color: #687d68

        /* Atelier-Seaside Red */
        .variable,
        .template-variable,
        .attribute,
        .tag,
        .name,
        .regexp,
        .link,
        .name,
        .selector-id,
        .selector-class
            color: #e6193c

        /* Atelier-Seaside Orange */
        .number,
        .meta,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params
            color: #87711d

        /* Atelier-Seaside Green */
        .string,
        .symbol,
        .bullet
            color: #29a329

        /* Atelier-Seaside Blue */
        .title,
        .section
            color: #3d62f5

        /* Atelier-Seaside Purple */
        .keyword,
        .selector-tag
            color: #ad2bee

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/atelier-sulphurpool-dark.styl

```styl
/* Base16 Atelier Sulphurpool Dark - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/sulphurpool) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */
.highlight
  background: #202746
  color: #979db4

  .code
    /* Atelier-Sulphurpool Comment */
    .comment, .quote
      color: #898ea4

    /* Atelier-Sulphurpool Red */
    .variable, .template-variable, .attribute, .tag, .name, .regexp, .link, .name, .selector-id, .selector-class
      color: #c94922

    /* Atelier-Sulphurpool Orange */
    .number, .meta, .built_in, .builtin-name, .literal, .type, .params
      color: #c76b29

    /* Atelier-Sulphurpool Green */
    .string, .symbol, .bullet
      color: #ac9739

    /* Atelier-Sulphurpool Blue */
    .title, .section
      color: #3d8fd1

    /* Atelier-Sulphurpool Purple */
    .keyword, .selector-tag
      color: #6679cc

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/atelier-sulphurpool-light.styl

```styl
/* Base16 Atelier Sulphurpool Light - Theme */
/* by Bram de Haan (http://atelierbram.github.io/syntax-highlighting/atelier-schemes/sulphurpool) */
/* Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16) */

.highlight
    color: #5e6687
    background: #f5f7ff
    .code
        /* Atelier-Sulphurpool Comment */
        .comment,
        .quote
            color: #6b7394

        /* Atelier-Sulphurpool Red */
        .variable,
        .template-variable,
        .attribute,
        .tag,
        .name,
        .regexp,
        .link,
        .name,
        .selector-id,
        .selector-class
            color: #c94922

        /* Atelier-Sulphurpool Orange */
        .number,
        .meta,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params
            color: #c76b29

        /* Atelier-Sulphurpool Green */
        .string,
        .symbol,
        .bullet
            color: #ac9739

        /* Atelier-Sulphurpool Blue */
        .title,
        .section
            color: #3d8fd1

        /* Atelier-Sulphurpool Purple */
        .keyword,
        .selector-tag
            color: #6679cc

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/brown-paper.styl

```styl
/*

Brown Paper style from goldblog.com.ua (c) Zaripov Yura <yur4ik7@ukr.net>

*/

.highlight
    color: #363c69
    background:#b7a68e url(./brown-papersq.png)
    .code
        .keyword,
        .selector-tag,
        .literal
            color:#005599
            font-weight:bold

        .highlight,
        .subst
            color: #363c69

        .string,
        .title,
        .section,
        .type,
        .attribute,
        .symbol,
        .bullet,
        .built_in,
        .addition,
        .variable,
        .template-tag,
        .template-variable,
        .link,
        .name
            color: #2c009f

        .comment,
        .quote,
        .meta,
        .deletion
            color: #802022

        .keyword,
        .selector-tag,
        .literal,
        .doctag,
        .title,
        .section,
        .type,
        .name,
        .strong
            font-weight: bold

        .emphasis
            font-style: italic

```

# source/css/_highlight/brown-papersq.png

This is a binary file of the type: Image

# source/css/_highlight/codepen-embed.styl

```styl
/*
   codepen.io Embed Theme
   Author: Justin Perry <http://github.com/ourmaninamsterdam>
   Original theme - https://github.com/chriskempson/tomorrow-theme
*/
.highlight
  background: #222
  color: #fff

  .code
    .comment, .quote
      color: #777

    .variable, .template-variable, .tag, .regexp, .meta, .number, .built_in, .builtin-name, .literal, .params, .symbol, .bullet, .link, .deletion
      color: #ab875d

    .section, .title, .name, .selector-id, .selector-class, .type, .attribute
      color: #9b869b

    .string, .keyword, .selector-tag, .addition
      color: #8f9c6c

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/color-brewer.styl

```styl
/*

Colorbrewer theme
Original: https://github.com/mbostock/colorbrewer-theme (c) Mike Bostock <mike@ocks.org>
Ported by Fabrício Tavares de Oliveira

*/

.highlight
    color: #000
    background: #fff
    .code
        .subst
            color: #000

        .string,
        .meta,
        .symbol,
        .template-tag,
        .template-variable,
        .addition
            color: #756bb1

        .comment,
        .quote
            color: #636363

        .number,
        .regexp,
        .literal,
        .bullet,
        .link
            color: #31a354

        .deletion,
        .variable
            color: #88f



        .keyword,
        .selector-tag,
        .title,
        .section,
        .built_in,
        .doctag,
        .type,
        .tag,
        .name,
        .selector-id,
        .selector-class,
        .strong
            color: #3182bd

        .emphasis
            font-style: italic

        .attribute
            color: #e6550d

```

# source/css/_highlight/dark.styl

```styl
/*
   
   Dark style from softwaremaniacs.org (c) Ivan Sagalaev <Maniac@SoftwareManiacs.Org>
   
*/
.highlight
  background: #444
  color: #ddd

  .code
    .keyword, .selector-tag, .literal, .section, .link
      color: white

    .subst
      color: #ddd

    .string, .title, .name, .type, .attribute, .symbol, .bullet, .built_in, .addition, .variable, .template-tag, .template-variable
      color: #d88

    .comment, .quote, .deletion, .meta
      color: #777

    .keyword, .selector-tag, .literal, .title, .section, .doctag, .type, .name, .strong
      font-weight: bold

    .emphasis
      font-style: italic

```

# source/css/_highlight/darkula.styl

```styl
/*
   
   Darkula color scheme from the JetBrains family of IDEs
   
*/
.highlight
  background: #2b2b2b
  color: #bababa

  .code
    .strong, .emphasis
      color: #a8a8a2

    .bullet, .quote, .link, .number, .regexp, .literal
      color: #6896ba

    .code, .selector-class
      color: #a6e22e

    .emphasis
      font-style: italic

    .keyword, .selector-tag, .section, .attribute, .name, .variable
      color: #cb7832

    .params
      color: #b9b9b9

    .string, .subst, .type, .built_in, .builtin-name, .symbol, .selector-id, .selector-attr, .selector-pseudo, .template-tag, .template-variable, .addition
      color: #e0c46c

    .comment, .deletion, .meta
      color: #7f7f7f

```

# source/css/_highlight/docco.styl

```styl
/*
Docco style used in http://jashkenas.github.com/docco/ converted by Simon Madine (@thingsinjars)
*/

.highlight
    color: #000
    background: #f8f8ff
    .code
        .comment,
        .quote
            color: #408080
            font-style: italic

        .keyword,
        .selector-tag,
        .literal,
        .subst
            color: #954121

        .number
            color: #40a070

        .string,
        .doctag
            color: #219161

        .selector-id,
        .selector-class,
        .section,
        .type
            color: #19469d

        .params
            color: #00f

        .title
            color: #458
            font-weight: bold

        .tag,
        .name,
        .attribute
            color: #000080
            font-weight: normal

        .variable,
        .template-variable
            color: #008080

        .regexp,
        .link
            color: #b68

        .symbol,
        .bullet
            color: #990073

        .built_in,
        .builtin-name
            color: #0086b3

        .meta
            color: #999
            font-weight: bold

        .deletion
            background: #fdd

        .addition
            background: #dfd

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/far.styl

```styl
/*
   
   FAR Style (c) MajestiC <majestic2k@gmail.com>
   
*/
.highlight
  background: #000080
  color: #0ff

  .code
    .subst
      color: #0ff

    .string, .attribute, .symbol, .bullet, .built_in, .builtin-name, .template-tag, .template-variable, .addition
      color: #ff0

    .keyword, .selector-tag, .section, .type, .name, .selector-id, .selector-class, .variable
      color: #fff

    .comment, .quote, .doctag, .deletion
      color: #888

    .number, .regexp, .literal, .link
      color: #0f0

    .meta
      color: #008080

    .keyword, .selector-tag, .title, .section, .name, .strong
      font-weight: bold

    .emphasis
      font-style: italic

```

# source/css/_highlight/foundation.styl

```styl
/*
Description: Foundation 4 docs style for highlight.js
Author: Dan Allen <dan.j.allen@gmail.com>
Website: http://foundation.zurb.com/docs/
Version: 1.0
Date: 2013-04-02
*/

.highlight
    color: black
    background: #eee
    .code
        .link,
        .emphasis,
        .attribute,
        .addition
            color: #070

        .emphasis
            font-style: italic

        .strong,
        .string,
        .deletion
            color: #d14

        .strong
            font-weight: bold

        .quote,
        .comment
            color: #998
            font-style: italic

        .section,
        .title
            color: #900

        .class .title,
        .type
            color: #458

        .variable,
        .template-variable
            color: #336699

        .bullet
            color: #997700

        .meta
            color: #3344bb

        .code,
        .number,
        .literal,
        .keyword,
        .selector-tag
            color: #099

        .regexp
            background-color: #fff0ff
            color: #880088

        .symbol
            color: #990073

        .tag,
        .name,
        .selector-id,
        .selector-class
            color: #007700

```

# source/css/_highlight/github-gist.styl

```styl
/**
 * GitHub Gist Theme
 * Author : Louis Barranqueiro - https://github.com/LouisBarranqueiro
 */

.highlight
    padding: 0.5em
    color: #333333
    .code
        .comment,
        .meta
            color: #969896

        .string,
        .variable,
        .template-variable,
        .strong,
        .emphasis,
        .quote
            color: #df5000

        .keyword,
        .selector-tag,
        .type
            color: #a71d5d

        .literal,
        .symbol,
        .bullet,
        .attribute
            color: #0086b3

        .section,
        .name
            color: #63a35c

        .tag
            color: #333333

        .title,
        .attr,
        .selector-id,
        .selector-class,
        .selector-attr,
        .selector-pseudo
            color: #795da3

        .addition
            color: #55a532
            background-color: #eaffea

        .deletion
            color: #bd2c00
            background-color: #ffecec

        .link
            text-decoration: underline

```

# source/css/_highlight/github.styl

```styl
/*

github.com style (c) Vasily Polovnyov <vast@whiteants.net>

*/

.highlight
    color: #333
    background: #f8f8f8
    .code
        .comment,
        .quote
            color: #998
            font-style: italic

        .keyword,
        .selector-tag,
        .subst
            color: #333
            font-weight: bold

        .number,
        .literal,
        .variable,
        .template-variable,
        .tag .attr
            color: #008080

        .string,
        .doctag
            color: #d14

        .title,
        .section,
        .selector-id
            color: #900
            font-weight: bold

        .subst
            font-weight: normal

        .type,
        .class .title
            color: #458
            font-weight: bold

        .tag,
        .name,
        .attribute
            color: #000080
            font-weight: normal

        .regexp,
        .link
            color: #009926

        .symbol,
        .bullet
            color: #990073

        .built_in,
        .builtin-name
            color: #0086b3

        .meta
            color: #999
            font-weight: bold

        .deletion
            background: #fdd

        .addition
            background: #dfd

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/googlecode.styl

```styl
/*

Google Code style (c) Aahan Krish <geekpanth3r@gmail.com>

*/

.highlight
    color: black
    background: white
    .code
        .comment,
        .quote
            color: #800

        .keyword,
        .selector-tag,
        .section,
        .title,
        .name
            color: #008

        .variable,
        .template-variable
            color: #660

        .string,
        .selector-attr,
        .selector-pseudo,
        .regexp
            color: #080

        .literal,
        .symbol,
        .bullet,
        .meta,
        .number,
        .link
            color: #066

        .title,
        .doctag,
        .type,
        .attr,
        .built_in,
        .builtin-name,
        .params
            color: #606

        .attribute,
        .subst
            color: #000

        .formula
            background-color: #eee
            font-style: italic

        .selector-id,
        .selector-class
            color: #9B703F

        .addition
            background-color: #baeeba

        .deletion
            background-color: #ffc8bd

        .doctag,
        .strong
            font-weight: bold

        .emphasis
            font-style: italic

```

# source/css/_highlight/grayscale.styl

```styl
/*

grayscale style (c) MY Sun <simonmysun@gmail.com>

*/

.highlight
    color: #333
    background: #fff
    .code
        .comment,
        .quote
            color: #777
            font-style: italic

        .keyword,
        .selector-tag,
        .subst
            color: #333
            font-weight: bold

        .number,
        .literal
            color: #777

        .string,
        .doctag,
        .formula
            color: #333
            background: url('data:image/pngbase64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAAJ0lEQVQIW2O8e/fufwYGBgZBQUEQxcCIIfDu3Tuwivfv30NUoAsAALHpFMMLqZlPAAAAAElFTkSuQmCC') repeat

        .title,
        .section,
        .selector-id
            color: #000
            font-weight: bold

        .subst
            font-weight: normal

        .class .title,
        .type,
        .name
            color: #333
            font-weight: bold

        .tag
            color: #333

        .regexp
                color: #333
                background: url('data:image/pngbase64,iVBORw0KGgoAAAANSUhEUgAAAAoAAAAICAYAAADA+m62AAAAPUlEQVQYV2NkQAN37979r6yszIgujiIAU4RNMVwhuiQ6H6wQl3XI4oy4FMHcCJPHcDS6J2A2EqUQpJhohQDexSef15DBCwAAAABJRU5ErkJggg==') repeat

        .symbol,
        .bullet,
        .link
            color: #000
            background: url('data:image/pngbase64,iVBORw0KGgoAAAANSUhEUgAAAAUAAAAFCAYAAACNbyblAAAAKElEQVQIW2NkQAO7d+/+z4gsBhJwdXVlhAvCBECKwIIwAbhKZBUwBQA6hBpm5efZsgAAAABJRU5ErkJggg==') repeat

        .built_in,
        .builtin-name
            color: #000
            text-decoration: underline

        .meta
            color: #999
            font-weight: bold

        .deletion
            color: #fff
            background:url('data:image/pngbase64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAADCAYAAABS3WWCAAAAE0lEQVQIW2MMDQ39zzhz5kwIAQAyxweWgUHd1AAAAABJRU5ErkJggg==') repeat

        .addition
            color: #000
            background: url('data:image/pngbase64,iVBORw0KGgoAAAANSUhEUgAAAAkAAAAJCAYAAADgkQYQAAAALUlEQVQYV2N89+7dfwYk8P79ewZBQUFkIQZGOiu6e/cuiptQHAPl0NtNxAQBAM97Oejj3Dg7AAAAAElFTkSuQmCC') repeat

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/gruvbox-dark.styl

```styl
/*
   Gruvbox Dark style - ported by Michell Stuttgart - github.com/mstuttgart
*/
.highlight
  background: #282828
  color: #ddd

  .code
    .tag, .keyword, .selector-tag, .literal, .strong, .name
      color: #fb4934

    .code
      color: #458588

    .class .title
      color: #83a598

    .attribute, .symbol, .regexp, .link
      color: #458588

    .string, .bullet, .subst, .title, .section, .emphasis, .type, .built_in, .builtin-name, .selector-attr, .selector-pseudo, .addition, .variable, .template-tag, .template-variable
      color: #b8bb26

    .comment, .quote, .deletion, .meta
      color: #a89984

    .keyword, .selector-tag, .literal, .doctag, .title, .section, .type, .selector-id
      font-weight: bold

    .number
      color: #b16286

    .operator
      color: #fe8019


```

# source/css/_highlight/highlightjs.styl

```styl
/*

Original highlight.js style (c) Ivan Sagalaev <maniac@softwaremaniacs.org>

*/

.highlight
    color: #444
    background: #F0F0F0
    .code
        .subst
            color: #444

        .keyword,
        .attribute,
        .selector-tag,
        .meta-keyword,
        .doctag,
        .name
            font-weight: bold

        .built_in,
        .literal,
        .bullet,
        .code,
        .addition
            color: #1F811F

        .regexp,
        .symbol,
        .variable,
        .template-variable,
        .link,
        .selector-attr,
        .selector-pseudo
            color: #BC6060

        .type,
        .string,
        .number,
        .selector-id,
        .selector-class,
        .quote,
        .template-tag,
        .deletion
            color: #880000

        .title,
        .section
            color: #880000
            font-weight: bold

        .comment
            color: #888888

        .meta
            color: #2B6EA1

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/hopscotch.styl

```styl
/*
 * Hopscotch
 * by Jan T. Sott
 * https://github.com/idleberg/Hopscotch
 * 
 * This work is licensed under the Creative Commons CC0 1.0 Universal License
 */
.highlight
  background: #322931
  color: #b9b5b8

  .code
    /* Comment */
    .comment, .quote
      color: #989498

    /* Red */
    .variable, .template-variable, .attribute, .tag, .name, .selector-id, .selector-class, .regexp, .link, .deletion
      color: #dd464c

    /* Orange */
    .number, .built_in, .builtin-name, .literal, .type, .params
      color: #fd8b19

    /* Yellow */
    .class .title
      color: #fdcc59

    /* Green */
    .string, .symbol, .bullet, .addition
      color: #8fc13e

    /* Aqua */
    .meta
      color: #149b93

    /* Blue */
    .function, .section, .title
      color: #1290bf

    /* Purple */
    .keyword, .selector-tag
      color: #c85e7c

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/hybrid.styl

```styl
/*
   
   vim-hybrid theme by w0ng (https://github.com/w0ng/vim-hybrid)
   
*/
/* background color */
.highlight
  background: #1d1f21
  color: #c5c8c6

  /* selection color */
  &::selection, span::selection
    background: #373b41

  &::-moz-selection, span::-moz-selection
    background: #373b41

  .code
    /* color: fg_yellow */
    .title, .name
      color: #f0c674

    /* color: fg_comment */
    .comment, .meta, .meta .keyword
      color: #707880

    /* color: fg_red */
    .number, .symbol, .literal, .deletion, .link
      color: #cc6666

    /* color: fg_green */
    .string, .doctag, .addition, .regexp, .selector-attr, .selector-pseudo
      color: #b5bd68

    /* color: fg_purple */
    .attribute, .code, .selector-id
      color: #b294bb

    /* color: fg_blue */
    .keyword, .selector-tag, .bullet, .tag
      color: #81a2be

    /* color: fg_aqua */
    .subst, .variable, .template-tag, .template-variable
      color: #8abeb7

    /* color: fg_orange */
    .type, .built_in, .builtin-name, .quote, .section, .selector-class
      color: #de935f

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/idea.styl

```styl
/*

Intellij Idea-like styling (c) Vasily Polovnyov <vast@whiteants.net>

*/

.highlight
    color: #000
    background: #fff
    .code
        .subst,
        .title
            font-weight: normal
            color: #000

        .comment,
        .quote
            color: #808080
            font-style: italic

        .meta
            color: #808000

        .tag
            background: #efefef

        .section,
        .name,
        .literal,
        .keyword,
        .selector-tag,
        .type,
        .selector-id,
        .selector-class
            font-weight: bold
            color: #000080

        .attribute,
        .number,
        .regexp,
        .link
            font-weight: bold
            color: #0000ff

        .number,
        .regexp,
        .link
            font-weight: normal

        .string
            color: #008000
            font-weight: bold

        .symbol,
        .bullet,
        .formula
            color: #000
            background: #d0eded
            font-style: italic

        .doctag
            text-decoration: underline

        .variable,
        .template-variable
            color: #660e7a

        .addition
            background: #baeeba

        .deletion
            background: #ffc8bd

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/index.styl

```styl
.highlight
    margin: 0px
    display: block
    overflow-x: auto
    padding: 15px 20px
    font-size: font-size
    font-family: font-mono
    line-height: font-size * line-height
    table
        margin: 0
        width: auto
        td
            border: none
        td.code
            padding-right: 20px
    .gutter
        pre
            color: #666
            text-align: right
            padding-right: 20px

.article-entry
    .highlight
        margin: 1.6em 0
        .line
            height: 1.6em;

@import "_highlight/" + highlight
```

# source/css/_highlight/ir-black.styl

```styl
/*
   IR_Black style (c) Vasily Mikhailitchenko <vaskas@programica.ru>
*/
.highlight
  background: #000
  color: #f8f8f8

  .code
    .comment, .quote, .meta
      color: #7c7c7c

    .keyword, .selector-tag, .tag, .name
      color: #96cbfe

    .attribute, .selector-id
      color: #ffffb6

    .string, .selector-attr, .selector-pseudo, .addition
      color: #a8ff60

    .subst
      color: #daefa3

    .regexp, .link
      color: #e9c062

    .title, .section, .type, .doctag
      color: #ffffb6

    .symbol, .bullet, .variable, .template-variable, .literal
      color: #c6c5fe

    .number, .deletion
      color: #ff73fd

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/kimbie.dark.styl

```styl
/*
        Name:         Kimbie (dark)
        Author:     Jan T. Sott
        License:    Creative Commons Attribution-ShareAlike 4.0 Unported License
        URL:            https://github.com/idleberg/Kimbie-highlight.js
*/

.highlight
    color: #d3af86
    background: #221a0f
    .code
        /* Kimbie Comment */
        .comment,
        .quote
            color: #d6baad

        /* Kimbie Red */
        .variable,
        .template-variable,
        .tag,
        .name,
        .selector-id,
        .selector-class,
        .regexp,
        .meta
            color: #dc3958

        /* Kimbie Orange */
        .number,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params,
        .deletion,
        .link
            color: #f79a32

        /* Kimbie Yellow */
        .title,
        .section,
        .attribute
            color: #f06431

        /* Kimbie Green */
        .string,
        .symbol,
        .bullet,
        .addition
            color: #889b4a

        /* Kimbie Purple */
        .keyword,
        .selector-tag,
        .function
            color: #98676a

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/kimbie.light.styl

```styl
/*
        Name:         Kimbie (light)
        Author:     Jan T. Sott
        License:    Creative Commons Attribution-ShareAlike 4.0 Unported License
        URL:            https://github.com/idleberg/Kimbie-highlight.js
*/

.highlight
    color: #84613d
    background: #fbebd4
    .code
        /* Kimbie Comment */
        .comment,
        .quote
            color: #a57a4c

        /* Kimbie Red */
        .variable,
        .template-variable,
        .tag,
        .name,
        .selector-id,
        .selector-class,
        .regexp,
        .meta
            color: #dc3958

        /* Kimbie Orange */
        .number,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params,
        .deletion,
        .link
            color: #f79a32

        /* Kimbie Yellow */
        .title,
        .section,
        .attribute
            color: #f06431

        /* Kimbie Green */
        .string,
        .symbol,
        .bullet,
        .addition
            color: #889b4a

        /* Kimbie Purple */
        .keyword,
        .selector-tag,
        .function
            color: #98676a

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/kimbie.styl

```styl
/*
   Name:         Kimbie (dark)
   Author:     Jan T. Sott
   License:    Creative Commons Attribution-ShareAlike 4.0 Unported License
   URL:            https://github.com/idleberg/Kimbie-highlight.js
*/
.highlight
  background: #221a0f
  color: #d3af86

  .code
    /* Kimbie Comment */
    .comment, .quote
      color: #d6baad

    /* Kimbie Red */
    .variable, .template-variable, .tag, .name, .selector-id, .selector-class, .regexp, .meta
      color: #dc3958

    /* Kimbie Orange */
    .number, .built_in, .builtin-name, .literal, .type, .params, .deletion, .link
      color: #f79a32

    /* Kimbie Yellow */
    .title, .section, .attribute
      color: #f06431

    /* Kimbie Green */
    .string, .symbol, .bullet, .addition
      color: #889b4a

    /* Kimbie Purple */
    .keyword, .selector-tag, .function
      color: #98676a

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/magula.styl

```styl
/*
Description: Magula style for highligh.js
Author: Ruslan Keba <rukeba@gmail.com>
Website: http://rukeba.com/
Version: 1.0
Date: 2009-01-03
Music: Aphex Twin / Xtal
*/

.highlight
    background-color: #f4f4f4
    .code
        .highlight,
        .subst
            color: black

        .string,
        .title,
        .symbol,
        .bullet,
        .attribute,
        .addition,
        .variable,
        .template-tag,
        .template-variable
            color: #050

        .comment,
        .quote
            color: #777

        .number,
        .regexp,
        .literal,
        .type,
        .link
            color: #800

        .deletion,
        .meta
            color: #00e

        .keyword,
        .selector-tag,
        .doctag,
        .title,
        .section,
        .built_in,
        .tag,
        .name
            font-weight: bold
            color: navy

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/mono-blue.styl

```styl
/*
    Five-color theme from a single blue hue.
*/
.highlight
    color: #00193a
    background: #eaeef3
    .code
        .keyword,
        .selector-tag,
        .title,
        .section,
        .doctag,
        .name,
        .strong
            font-weight: bold

        .comment
            color: #738191

        .string,
        .title,
        .section,
        .built_in,
        .literal,
        .type,
        .addition,
        .tag,
        .quote,
        .name,
        .selector-id,
        .selector-class
            color: #0048ab

        .meta,
        .subst,
        .symbol,
        .regexp,
        .attribute,
        .deletion,
        .variable,
        .template-variable,
        .link,
        .bullet
            color: #4c81c9

        .emphasis
            font-style: italic

```

# source/css/_highlight/monokai-sublime.styl

```styl
/*
   
   Monokai Sublime style. Derived from Monokai by noformnocontent http://nn.mit-license.org/
   
*/
.highlight
  background: #23241f
  color: #f8f8f2

  .code
    .highlight, .tag, .subst
      color: #f8f8f2

    .strong, .emphasis
      color: #a8a8a2

    .bullet, .quote, .number, .regexp, .literal, .link
      color: #ae81ff

    .code, .title, .section, .selector-class
      color: #a6e22e

    .strong
      font-weight: bold

    .emphasis
      font-style: italic

    .keyword, .selector-tag, .name, .attr
      color: #f92672

    .symbol, .attribute
      color: #66d9ef

    .params, .class .title
      color: #f8f8f2

    .string, .type, .built_in, .builtin-name, .selector-id, .selector-attr, .selector-pseudo, .addition, .variable, .template-variable
      color: #e6db74

    .comment, .deletion, .meta
      color: #75715e

```

# source/css/_highlight/monokai.styl

```styl
/*
   Monokai style - ported by Luigi Maselli - http://grigio.org
*/
.highlight
  background: #272822
  color: #ddd

  .code
    .tag, .keyword, .selector-tag, .literal, .strong, .name
      color: #f92672

    .code
      color: #66d9ef

    .class .title
      color: white

    .attribute, .symbol, .regexp, .link
      color: #bf79db

    .string, .bullet, .subst, .title, .section, .emphasis, .type, .built_in, .builtin-name, .selector-attr, .selector-pseudo, .addition, .variable, .template-tag, .template-variable
      color: #a6e22e

    .comment, .quote, .deletion, .meta
      color: #75715e

    .keyword, .selector-tag, .literal, .doctag, .title, .section, .type, .selector-id
      font-weight: bold

```

# source/css/_highlight/obsidian.styl

```styl
/**
 * Obsidian style
 * ported by Alexander Marenin (http://github.com/ioncreature)
 */
.highlight
  background: #282b2e
  color: #e0e2e4

  .code
    .keyword, .selector-tag, .literal, .selector-id
      color: #93c763

    .number
      color: #ffcd22

    .attribute
      color: #668bb0

    .code, .class .title, .section
      color: white

    .regexp, .link
      color: #d39745

    .meta
      color: #557182

    .tag, .name, .bullet, .subst, .emphasis, .type, .built_in, .selector-attr, .selector-pseudo, .addition, .variable, .template-tag, .template-variable
      color: #8cbbad

    .string, .symbol
      color: #ec7600

    .comment, .quote, .deletion
      color: #818e96

    .selector-class
      color: #A082BD

    .keyword, .selector-tag, .literal, .doctag, .title, .section, .type, .name, .strong
      font-weight: bold

```

# source/css/_highlight/paraiso-dark.styl

```styl
/*
        Paraíso (dark)
        Created by Jan T. Sott (http://github.com/idleberg)
        Inspired by the art of Rubens LP (http://www.rubenslp.com.br)
*/

.highlight
    color: #a39e9b
    background: #2f1e2e
    .code
        /* Paraíso Comment */
        .comment,
        .quote
            color: #8d8687

        /* Paraíso Red */
        .variable,
        .template-variable,
        .tag,
        .name,
        .selector-id,
        .selector-class,
        .regexp,
        .link,
        .meta
            color: #ef6155

        /* Paraíso Orange */
        .number,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params,
        .deletion
            color: #f99b15

        /* Paraíso Yellow */
        .title,
        .section,
        .attribute
            color: #fec418

        /* Paraíso Green */
        .string,
        .symbol,
        .bullet,
        .addition
            color: #48b685

        /* Paraíso Purple */
        .keyword,
        .selector-tag
            color: #815ba4

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/paraiso-light.styl

```styl
/*
        Paraíso (light)
        Created by Jan T. Sott (http://github.com/idleberg)
        Inspired by the art of Rubens LP (http://www.rubenslp.com.br)
*/

.highlight
    color: #4f424c
    background: #e7e9db
    .code
        /* Paraíso Comment */
        .comment,
        .quote
            color: #776e71

        /* Paraíso Red */
        .variable,
        .template-variable,
        .tag,
        .name,
        .selector-id,
        .selector-class,
        .regexp,
        .link,
        .meta
            color: #ef6155

        /* Paraíso Orange */
        .number,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params,
        .deletion
            color: #f99b15

        /* Paraíso Yellow */
        .title,
        .section,
        .attribute
            color: #fec418

        /* Paraíso Green */
        .string,
        .symbol,
        .bullet,
        .addition
            color: #48b685

        /* Paraíso Purple */
        .keyword,
        .selector-tag
            color: #815ba4

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/paraiso.styl

```styl
/*
   Paraíso (dark)
   Created by Jan T. Sott (http://github.com/idleberg)
   Inspired by the art of Rubens LP (http://www.rubenslp.com.br)
*/
.highlight
  background: #2f1e2e
  color: #a39e9b

  .code
    /* Paraíso Comment */
    .comment, .quote
      color: #8d8687

    /* Paraíso Red */
    .variable, .template-variable, .tag, .name, .selector-id, .selector-class, .regexp, .link, .meta
      color: #ef6155

    /* Paraíso Orange */
    .number, .built_in, .builtin-name, .literal, .type, .params, .deletion
      color: #f99b15

    /* Paraíso Yellow */
    .title, .section, .attribute
      color: #fec418

    /* Paraíso Green */
    .string, .symbol, .bullet, .addition
      color: #48b685

    /* Paraíso Purple */
    .keyword, .selector-tag
      color: #815ba4

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/pojoaque.jpg

This is a binary file of the type: Image

# source/css/_highlight/pojoaque.styl

```styl
/*
   
   Pojoaque Style by Jason Tate
   http://web-cms-designs.com/ftopict-10-pojoaque-style-for-highlight-js-code-highlighter.html
   Based on Solarized Style from http://ethanschoonover.com/solarized
   
*/
.highlight
  background: url("./pojoaque.jpg") repeat scroll left top #181914
  color: #dccf8f

  .code
    .comment, .quote
      color: #586e75
      font-style: italic

    .keyword, .selector-tag, .literal, .addition
      color: #b64926

    .number, .string, .doctag, .regexp
      color: #468966

    .title, .section, .built_in, .name
      color: #ffb03b

    .variable, .template-variable, .class .title, .type, .tag
      color: #b58900

    .attribute
      color: #b89859

    .symbol, .bullet, .link, .subst, .meta
      color: #cb4b16

    .deletion
      color: #dc322f

    .selector-id, .selector-class
      color: #d3a60c

    .formula
      background: #073642

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/railscasts.styl

```styl
/*
   
   Railscasts-like style (c) Visoft, Inc. (Damien White)
   
*/
.highlight
  background: #232323
  color: #e6e1dc

  .code
    .comment, .quote
      color: #bc9458
      font-style: italic

    .keyword, .selector-tag
      color: #c26230

    .string, .number, .regexp, .variable, .template-variable
      color: #a5c261

    .subst
      color: #519f50

    .tag, .name
      color: #e8bf6a

    .type
      color: #da4939

    .symbol, .bullet, .built_in, .builtin-name, .attr, .link
      color: #6d9cbe

    .params
      color: #d0d0ff

    .attribute
      color: #cda869

    .meta
      color: #9b859d

    .title, .section
      color: #ffc66d

    .addition
      display: inline-block
      width: 100%
      background-color: #144212
      color: #e6e1dc

    .deletion
      display: inline-block
      width: 100%
      background-color: #600
      color: #e6e1dc

    .selector-class
      color: #9b703f

    .selector-id
      color: #8b98ab

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

    .link
      text-decoration: underline

```

# source/css/_highlight/rainbow.styl

```styl
/*
   
   Style with support for rainbow parens
   
*/
.highlight
  background: #474949
  color: #d1d9e1

  .code
    .comment, .quote
      color: #969896
      font-style: italic

    .keyword, .selector-tag, .literal, .type, .addition
      color: #cc99cc

    .number, .selector-attr, .selector-pseudo
      color: #f99157

    .string, .doctag, .regexp
      color: #8abeb7

    .title, .name, .section, .built_in
      color: #b5bd68

    .variable, .template-variable, .selector-id, .class .title
      color: #ffcc66

    .section, .name, .strong
      font-weight: bold

    .symbol, .bullet, .subst, .meta, .link
      color: #f99157

    .deletion
      color: #dc322f

    .formula
      background: #eee8d5

    .attr, .attribute
      color: #81a2be

    .emphasis
      font-style: italic

```

# source/css/_highlight/school-book.png

This is a binary file of the type: Image

# source/css/_highlight/school-book.styl

```styl
/*

School Book style from goldblog.com.ua (c) Zaripov Yura <yur4ik7@ukr.net>

*/

.highlight
    background:#f6f6ae url(./school-book.png)
    border-top: solid 2px #d2e8b9
    border-bottom: solid 1px #d2e8b9
    .code
        .keyword,
        .selector-tag,
        .literal
            color:#005599
            font-weight:bold

        .highlight,
        .subst
            color: #3e5915

        .string,
        .title,
        .section,
        .type,
        .symbol,
        .bullet,
        .attribute,
        .built_in,
        .builtin-name,
        .addition,
        .variable,
        .template-tag,
        .template-variable,
        .link
            color: #2c009f

        .comment,
        .quote,
        .deletion,
        .meta
            color: #e60415

        .keyword,
        .selector-tag,
        .literal,
        .doctag,
        .title,
        .section,
        .type,
        .name,
        .selector-id,
        .strong
            font-weight: bold

        .emphasis
            font-style: italic

```

# source/css/_highlight/solarized-dark.styl

```styl
/*
   
   Orginal Style from ethanschoonover.com/solarized (c) Jeremy Hull <sourdrums@gmail.com>
   
*/
.highlight
  background: #002b36
  color: #839496

  .code
    .comment, .quote
      color: #586e75

    /* Solarized Green */
    .keyword, .selector-tag, .addition
      color: #859900

    /* Solarized Cyan */
    .number, .string, .meta .meta-string, .literal, .doctag, .regexp
      color: #2aa198

    /* Solarized Blue */
    .title, .section, .name, .selector-id, .selector-class
      color: #268bd2

    /* Solarized Yellow */
    .attribute, .attr, .variable, .template-variable, .class .title, .type
      color: #b58900

    /* Solarized Orange */
    .symbol, .bullet, .subst, .meta, .meta .keyword, .selector-attr, .selector-pseudo, .link
      color: #cb4b16

    /* Solarized Red */
    .built_in, .deletion
      color: #dc322f

    .formula
      background: #073642

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/solarized-light.styl

```styl
/*

Orginal Style from ethanschoonover.com/solarized (c) Jeremy Hull <sourdrums@gmail.com>

*/

.highlight
    color: #657b83
    background: #fdf6e3
    .code
        .comment,
        .quote
            color: #93a1a1

        /* Solarized Green */
        .keyword,
        .selector-tag,
        .addition
            color: #859900

        /* Solarized Cyan */
        .number,
        .string,
        .meta .meta-string,
        .literal,
        .doctag,
        .regexp
            color: #2aa198

        /* Solarized Blue */
        .title,
        .section,
        .name,
        .selector-id,
        .selector-class
            color: #268bd2

        /* Solarized Yellow */
        .attribute,
        .attr,
        .variable,
        .template-variable,
        .class .title,
        .type
            color: #b58900

        /* Solarized Orange */
        .symbol,
        .bullet,
        .subst,
        .meta,
        .meta .keyword,
        .selector-attr,
        .selector-pseudo,
        .link
            color: #cb4b16

        /* Solarized Red */
        .built_in,
        .deletion
            color: #dc322f

        .formula
            background: #eee8d5

        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/sunburst.styl

```styl
/*
   
   Sunburst-like style (c) Vasily Polovnyov <vast@whiteants.net>
   
*/
.highlight
  background: #000
  color: #f8f8f8

  .code
    .comment, .quote
      color: #aeaeae
      font-style: italic

    .keyword, .selector-tag, .type
      color: #e28964

    .string
      color: #65b042

    .subst
      color: #daefa3

    .regexp, .link
      color: #e9c062

    .title, .section, .tag, .name
      color: #89bdff

    .class .title, .doctag
      text-decoration: underline

    .symbol, .bullet, .number
      color: #3387cc

    .params, .variable, .template-variable
      color: #3e87e3

    .attribute
      color: #cda869

    .meta
      color: #8996a8

    .formula
      background-color: #0e2231
      color: #f8f8f8
      font-style: italic

    .addition
      background-color: #253b22
      color: #f8f8f8

    .deletion
      background-color: #420e09
      color: #f8f8f8

    .selector-class
      color: #9b703f

    .selector-id
      color: #8b98ab

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/tomorrow-night-blue.styl

```styl
/* Tomorrow Night Blue Theme */
/* http://jmblog.github.com/color-themes-for-google-code-highlightjs */
/* Original theme - https://github.com/chriskempson/tomorrow-theme */
/* http://jmblog.github.com/color-themes-for-google-code-highlightjs */
.highlight
  background: #002451
  color: white

  .code
    /* Tomorrow Comment */
    .comment, .quote
      color: #7285b7

    /* Tomorrow Red */
    .variable, .template-variable, .tag, .name, .selector-id, .selector-class, .regexp, .deletion
      color: #ff9da4

    /* Tomorrow Orange */
    .number, .built_in, .builtin-name, .literal, .type, .params, .meta, .link
      color: #ffc58f

    /* Tomorrow Yellow */
    .attribute
      color: #ffeead

    /* Tomorrow Green */
    .string, .symbol, .bullet, .addition
      color: #d1f1a9

    /* Tomorrow Blue */
    .title, .section
      color: #bbdaff

    /* Tomorrow Purple */
    .keyword, .selector-tag
      color: #ebbbff

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/tomorrow-night-bright.styl

```styl
/* Tomorrow Night Bright Theme */
/* Original theme - https://github.com/chriskempson/tomorrow-theme */
/* http://jmblog.github.com/color-themes-for-google-code-highlightjs */
.highlight
  background: black
  color: #eaeaea

  .code
    /* Tomorrow Comment */
    .comment, .quote
      color: #969896

    /* Tomorrow Red */
    .variable, .template-variable, .tag, .name, .selector-id, .selector-class, .regexp, .deletion
      color: #d54e53

    /* Tomorrow Orange */
    .number, .built_in, .builtin-name, .literal, .type, .params, .meta, .link
      color: #e78c45

    /* Tomorrow Yellow */
    .attribute
      color: #e7c547

    /* Tomorrow Green */
    .string, .symbol, .bullet, .addition
      color: #b9ca4a

    /* Tomorrow Blue */
    .title, .section
      color: #7aa6da

    /* Tomorrow Purple */
    .keyword, .selector-tag
      color: #c397d8

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/tomorrow-night-eighties.styl

```styl
/* Tomorrow Night Eighties Theme */
/* Original theme - https://github.com/chriskempson/tomorrow-theme */
/* http://jmblog.github.com/color-themes-for-google-code-highlightjs */
.highlight
  background: #2d2d2d
  color: #cccccc

  .code
    /* Tomorrow Comment */
    .comment, .quote
      color: #999999

    /* Tomorrow Red */
    .variable, .template-variable, .tag, .name, .selector-id, .selector-class, .regexp, .deletion
      color: #f2777a

    /* Tomorrow Orange */
    .number, .built_in, .builtin-name, .literal, .type, .params, .meta, .link
      color: #f99157

    /* Tomorrow Yellow */
    .attribute
      color: #ffcc66

    /* Tomorrow Green */
    .string, .symbol, .bullet, .addition
      color: #99cc99

    /* Tomorrow Blue */
    .title, .section
      color: #6699cc

    /* Tomorrow Purple */
    .keyword, .selector-tag
      color: #cc99cc

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/tomorrow-night.styl

```styl
/* Original theme - https://github.com/chriskempson/tomorrow-theme */
/* http://jmblog.github.com/color-themes-for-google-code-highlightjs */
.highlight
  background: #1d1f21
  color: #c5c8c6

  .code
    /* Tomorrow Comment */
    .comment, .quote
      color: #969896

    /* Tomorrow Red */
    .variable, .template-variable, .tag, .name, .selector-id, .selector-class, .regexp, .deletion
      color: #cc6666

    /* Tomorrow Orange */
    .number, .built_in, .builtin-name, .literal, .type, .params, .meta, .link
      color: #de935f

    /* Tomorrow Yellow */
    .attribute
      color: #f0c674

    /* Tomorrow Green */
    .string, .symbol, .bullet, .addition
      color: #b5bd68

    /* Tomorrow Blue */
    .title, .section
      color: #81a2be

    /* Tomorrow Purple */
    .keyword, .selector-tag
      color: #b294bb

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_highlight/tomorrow.styl

```styl
.highlight
    color: #4d4d4c
    background: white
    .code
        /* Tomorrow Comment */
        .comment,
        .quote
            color: #8e908c

        /* Tomorrow Red */
        .variable,
        .template-variable,
        .tag,
        .name,
        .selector-id,
        .selector-class,
        .regexp,
        .deletion
            color: #c82829

        /* Tomorrow Orange */
        .number,
        .built_in,
        .builtin-name,
        .literal,
        .type,
        .params,
        .meta,
        .link
            color: #f5871f

        /* Tomorrow Yellow */
        .attribute
            color: #eab700

        /* Tomorrow Green */
        .string,
        .symbol,
        .bullet,
        .addition
            color: #718c00

        /* Tomorrow Blue */
        .title,
        .section
            color: #4271ae

        /* Tomorrow Purple */
        .keyword,
        .selector-tag
            color: #8959a8
        .emphasis
            font-style: italic

        .strong
            font-weight: bold
```

# source/css/_highlight/vs.styl

```styl
/*

Visual Studio-like style based on original C# coloring by Jason Diamond <jason@diamond.name>

*/
.highlight
    display: block
    overflow-x: auto
    padding: 0.5em
    background: white
    color: black
    .code
        .comment,
        .quote,
        .variable
            color: #008000

        .keyword,
        .selector-tag,
        .built_in,
        .name,
        .tag
            color: #00f

        .string,
        .title,
        .section,
        .attribute,
        .literal,
        .template-tag,
        .template-variable,
        .type,
        .addition
            color: #a31515

        .deletion,
        .selector-attr,
        .selector-pseudo,
        .meta
            color: #2b91af

        .doctag
            color: #808080

        .attr
            color: #f00

        .symbol,
        .bullet,
        .link
            color: #00b0e8


        .emphasis
            font-style: italic

        .strong
            font-weight: bold

```

# source/css/_highlight/xcode.styl

```styl
/*

XCode style (c) Angel Garcia <angelgarcia.mail@gmail.com>

*/

.highlight
    color: black
    background: #fff
    .code
        .comment,
        .quote
            color: #006a00

        .keyword,
        .selector-tag,
        .literal
            color: #aa0d91

        .name
            color: #008

        .variable,
        .template-variable
            color: #660

        .string
            color: #c41a16

        .regexp,
        .link
            color: #080

        .title,
        .tag,
        .symbol,
        .bullet,
        .number,
        .meta
            color: #1c00cf

        .section,
        .class .title,
        .type,
        .attr,
        .built_in,
        .builtin-name,
        .params
            color: #5c2699

        .attribute,
        .subst
            color: #000

        .formula
            background-color: #eee
            font-style: italic

        .addition
            background-color: #baeeba

        .deletion
            background-color: #ffc8bd

        .selector-id,
        .selector-class
            color: #9b703f

        .doctag,
        .strong
            font-weight: bold

        .emphasis
            font-style: italic

```

# source/css/_highlight/zenburn.styl

```styl
/*
   
   Zenburn style from voldmar.ru (c) Vladimir Epifanov <voldmar@voldmar.ru>
   based on dark.css by Ivan Sagalaev
   
*/
.highlight
  background: #3f3f3f
  color: #dcdcdc

  .code
    .keyword, .selector-tag, .tag
      color: #e3ceab

    .template-tag
      color: #dcdcdc

    .number
      color: #8cd0d3

    .variable, .template-variable, .attribute
      color: #efdcbc

    .literal
      color: #efefaf

    .subst
      color: #8f8f8f

    .title, .name, .selector-id, .selector-class, .section, .type
      color: #efef8f

    .symbol, .bullet, .link
      color: #dca3a3

    .deletion, .string, .built_in, .builtin-name
      color: #cc9393

    .addition, .comment, .quote, .meta
      color: #7f9f7f

    .emphasis
      font-style: italic

    .strong
      font-weight: bold

```

# source/css/_mixins.styl

```styl
antialias()
  -moz-osx-font-smoothing: grayscale
  -webkit-font-smoothing: antialiased

hyphens($value)
  hyphens: $value
  -moz-hyphens: $value
  -ms-hyphens: $value
  -webkit-hyphens: $value

underline($size, $color)
  background-image: linear-gradient(transparent, transparent $size, $color $size, $color)
  background-position: bottom
  background-size: 100% 6px
  background-repeat: repeat-x

no-select()
  user-select: none
  -khtml-user-select: none
  -o-user-select: none
  -moz-user-select: none
  -webkit-user-select: none

```

# source/css/_partial/archive.styl

```styl
#archive
  .post-year
    list-style-type: none

  .post-list
    padding: 0

    .post-item
      margin-bottom: 1rem
      margin-left: 0
      list-style-type: none

      .meta
        display: block
        margin-right: 16px
        min-width: 100px
        color: $color-meta
        font-size: 14px

  @media (min-width: 480px)
    .post-list
      .post-item
        display: flex
        margin-bottom: 5px
        margin-left: 1rem

        .meta
          text-align: left

```

# source/css/_partial/article.styl

```styl
article
  header
    .posttitle
      margin-top: 0
      margin-bottom: 0
      text-transform: none
      font-size: 1.5em
      line-height: 1.25

    .meta
      margin-top: 0
      margin-bottom: 1rem

    .meta *
      color: $color-accent-3
      font-size: .85rem

    .author
      text-transform: uppercase
      letter-spacing: .01em
      font-weight: 700

    .postdate
      display: inline

  .content
    h2:before
      position: absolute
      top: -4px
      left: -1rem
      color: $color-accent-1
      content: "#"
      font-weight: bold
      font-size: 1.2rem

    img
    video
      display: block
      margin: auto
      max-width: 100%
      height: auto

    /* http://webdesignerwall.com/tutorials/css-elastic-videos */
    .video-container
      position: relative
      overflow: hidden
      padding-top: (9 / 16 * 100)% // 16:9 ratio
      height: 0

      iframe, object, embed
        position: absolute
        top: 0
        left: 0
        margin-top: 0
        width: 100%
        height: 100%

    blockquote
      margin: 1rem 10px
      padding: .5em 10px
      background: inherit
      color: $color-quote
      quotes: "\201C" "\201D" "\2018" "\2019"
      font-weight: bold

      p
        margin: 0

      &:before
        margin-right: .25em
        color: $color-quote
        content: "\201C"
        vertical-align: -.4em
        font-size: 2em
        line-height: .1em

      footer
        margin: line-height 0
        color: $color-meta
        font-size: 12px

        a
          background-image: linear-gradient(transparent, transparent 5px, $color-meta 5px, $color-meta)
          color: $color-meta

        a:hover
          background-image: linear-gradient(transparent, transparent 4px, lighten($color-meta, 20%) 4px, lighten($color-meta, 20%))
          color: lighten($color-meta, 20%)

        cite
          &:before
            padding: 0 .5em
            content: "—"

    .pullquote
      margin: 0
      width: 45%
      text-align: left

      &.left
        margin-right: 1em
        margin-left: .5em

      &.right
        margin-right: .5em
        margin-left: 1em

    .caption
      position: relative
      display: block
      margin-top: .5em
      color: $color-meta
      text-align: center
      font-size: .9em

.posttitle
  text-transform: none
  font-size: 1.5em
  line-height: 1.25

.article-tag
  .tag-link
    &:before
      content: "#"
    underline(10px, $color-link)

.article-category
  .category-link
    underline(10px, $color-link)

@media (min-width: 480px)
  .article-tag,
  .article-category
    display: inline

    &:before
      content: "|"

```

# source/css/_partial/categories.styl

```styl
#categories
  .category-list-title
    color: $color-meta
  .category-list
    .category-list-item
      .category-list-count
        color: $color-meta
      .category-list-count:before
        content: " ("
      .category-list-count:after
        content: ")"

```

# source/css/_partial/comments.styl

```styl
.blog-post-comments
  margin-top: 4rem

```

# source/css/_partial/footer.styl

```styl
#footer
  position: absolute
  bottom: 0
  margin-bottom: 10px
  width: 100%
  color: $color-meta
  vertical-align: top
  text-align: center
  font-size: 12px

  ul
    margin: 0
    padding: 0
    list-style: none

  li
    display: inline-block
    margin-right: 15px
    border-right: 1px solid
    border-color: $color-border
    vertical-align: middle

    a
      margin-right: 15px

  li:last-child
    margin-right: 0
    border-right: 0

    a
      margin-right: 0

  a
    color: $color-meta
    text-decoration: underline
    background-image: none

  a:hover
    color: lighten($color-meta, 20%)

  .footer-left
    height: 20px
    vertical-align: middle
    line-height: 20px

@media (min-width: 39rem)
  #footer
    display: flex
    flex-flow: row wrap
    justify-content: space-between
    align-items: center
    align-content: center
    margin-bottom: 20px

    .footer-left
      align-self: flex-start
      margin-right: 20px

    .footer-right
      align-self: flex-end

```

# source/css/_partial/header.styl

```styl
#header
  margin: 0 auto 2rem
  width: 100%

  h1, .h1
    margin-top: 0
    margin-bottom: 0
    color: $color-text
    letter-spacing: .01em
    font-weight: 700
    font-style: normal
    font-size: 1.5rem
    line-height: 2rem

    antialias()

  a
    background: none
    color: inherit
    text-decoration: none

  #logo
    display: inline-block
    float: left
    margin-right: 20px
    width: $logo-width
    height: $logo-height
    border-radius: 5px
    background-size: $logo-width $logo-height
    background-repeat: no-repeat
    if $logo-grayout
      filter: grayscale(100%)
      -webkit-filter: grayscale(100%)

  #nav
    color: $color-accent-1
    letter-spacing: .01em
    font-weight: 200
    font-style: normal
    font-size: .8rem

    ul
      margin: 0
      padding: 0
      list-style-type: none
      line-height: 15px

      a
        margin-right: 15px
        color: $color-accent-1

      a:hover
        underline(5px, $color-accent-1)

      li
        display: inline-block
        margin-right: 15px
        border-right: 1px dotted
        border-color: $color-accent-1
        vertical-align: middle

      .icon
        display: none

      li:last-child
        margin-right: 0
        border-right: 0

        a
          margin-right: 0

if $logo-grayout
  #header:hover
    #logo
      filter: none
      -webkit-filter: none

@media screen and (max-width: 480px)
  #header #title
    display: table
    margin-right: 5rem
    min-height: $logo-height
    h1
      display: table-cell
      vertical-align: middle

  #header #nav
    ul
      a:hover
        background: none

      li
        display: none
        border-right: 0

      li.icon
        position: absolute
        top: 77px
        right: 1rem
        display: inline-block
        text-align: center

    ul.responsive
      li
        display: block
    
    ul 
      a[aria-label="Menu"]
        display: inline-block
        min-width: 48px
        min-height: 48px

    li:not(:first-child)
      padding-top: 1rem
      padding-left: $logo-width + 20px
      font-size: 1rem

```

# source/css/_partial/index.styl

```styl
.post-list
  padding: 0

  .post-item
    margin-bottom: 1rem
    margin-left: 0
    list-style-type: none

    .meta
      display: block
      margin-right: 16px
      min-width: 100px
      color: $color-meta
      font-size: 14px

@media (min-width: 480px)
  .post-list
    .post-item
      display: flex
      margin-bottom: 5px

      .meta
        text-align: left

.project-list
  padding: 0
  list-style: none

  .project-item
    margin-bottom: 5px
    p
      display: inline

```

# source/css/_partial/pagination.styl

```styl
.pagination
  display: inline-block
  margin-top: 2rem
  width: 100%
  text-align: center

  .page-number
    color: $color-text
    font-size: .8rem

  a
    padding: 4px 6px
    border-radius: 5px
    // background-color: $color-accent-1
    background-image: none
    color: $color-text
    text-decoration: none

  a:hover
    background-image: none

  a:hover:not(.active)
    color: $color-accent-2

```

# source/css/_partial/post/actions_desktop.styl

```styl
#header-post
  position: fixed
  top: 2rem
  right: 0
  display: inline-block
  float: right
  z-index: 100

  a
    background: none
    color: inherit
    text-decoration: none

  a.icon
    background: none

    &:hover
      color: $color-link

  ol
    list-style-type: none

  ul
    display: inline-block
    margin: 0
    padding: 0
    list-style-type: none

    li
      display: inline-block
      margin-right: 15px
      vertical-align: middle

    li:last-child
      margin-right: 0

  #menu-icon
    float: right
    margin-right: 2rem
    margin-left: 15px

    &:hover
      color: $color-accent-1

  #menu-icon-tablet
    float: right
    margin-right: 2rem
    margin-left: 15px

    &:hover
      color: $color-accent-1

  #top-icon-tablet
    position: fixed
    right: 2rem
    bottom: 2rem
    margin-right: 2rem
    margin-left: 15px

    &:hover
      color: $color-accent-1

  .active
    color: $color-accent-1

  #menu
    display: none
    margin-right: 2rem

  #nav
    color: $color-accent-1
    letter-spacing: .01em
    font-weight: 200
    font-style: normal
    font-size: .8rem

    ul
      line-height: 15px

      a
        margin-right: 15px
        color: $color-accent-1

      a:hover
        underline(5px, $color-accent-1)

      li
        border-right: 1px dotted $color-accent-1

      li:last-child
        margin-right: 0
        border-right: 0

        a
          margin-right: 0

  #actions
    float: right
    margin-top: 2rem
    margin-right: 2rem
    width: 100%
    text-align: right

    ul
      display: block

    .info
      display: block
      font-style: italic

  #share
    clear: both
    padding-top: 1rem
    padding-right: 2rem
    text-align: right

    li
      display: block
      margin: 0

  #toc
    float: right
    clear: both
    overflow: auto
    margin-top: 1rem
    padding-right: 2rem
    max-width: 20em
    max-height: calc(95vh - 7rem)
    text-align: right

    a:hover
      color: $color-link

    .toc-level-1 > .toc-link
      display: none

    .toc-level-2
      color: $color-text
      font-size: .8rem

      &:before
        color: $color-accent-1
        content: "#"

    .toc-level-3
      color: $color-meta
      font-size: .7rem

    .toc-level-4
      color: darken($color-meta, 20%)
      font-size: .4rem

    .toc-level-5
      display: none

    .toc-level-6
      display: none

    .toc-number
      display: none

// smartphone + phapblet
@media screen and (max-width: 500px)
  #header-post
    display: none

@media screen and (max-width: 900px)
  #header-post
    #menu-icon
      display: none

    #actions
      display: none

@media screen and (max-width: 1199px)
  #header-post
    #toc
      display: none

@media screen and (min-width: 900px)
  #header-post
    #menu-icon-tablet
      display: none !important

    #top-icon-tablet
      display: none !important

@media screen and (min-width: 1199px)
  #header-post
    #actions
      width: auto

      ul
        display: inline-block
        float: right

      .info
        display: inline
        float: left
        margin-right: 2rem
        font-style: italic

@media print 
  #header-post
    display: none
  #footer-post-container
    display: none

```

# source/css/_partial/post/actions_mobile.styl

```styl
#footer-post
  position: fixed
  right: 0
  bottom: 0
  left: 0
  z-index: 5000000
  width: 100%
  border-top: 1px solid $color-border
  background: $color-footer-mobile-1
  transition: opacity .2s

  a
    background: none
    color: inherit
    text-decoration: none

  a.icon
    background: none

    &:hover
      color: $color-link

  #nav-footer
    padding-right: 1rem
    padding-left: 1rem
    background: $color-footer-mobile-2
    text-align: center

    a
      color: $color-accent-1
      font-size: 1em

    a:hover
      underline(5px, $color-accent-1)

    ul
      display: table
      margin: 0
      padding: 0
      width: 100%
      list-style-type: none

      li
        display: inline-table
        padding: 10px
        width: 20%
        vertical-align: middle

  #actions-footer
    overflow: auto
    margin-top: 1rem
    margin-bottom: 1rem
    padding-right: 1rem
    padding-left: 1rem
    width: 100%
    text-align: center
    white-space: nowrap

    a
      display: inline-block
      padding-left: 1rem
      color: $color-accent-1

  #share-footer
    padding-right: 1rem
    padding-left: 1rem
    background: $color-footer-mobile-2
    text-align: center

    ul
      display: table
      margin: 0
      padding: 0
      width: 100%
      list-style-type: none

      li
        display: inline-table
        padding: 10px
        width: 20%
        vertical-align: middle

  #toc-footer
    clear: both
    padding-top: 1rem
    padding-bottom: 1rem
    background: $color-footer-mobile-2
    text-align: left

    ol
      margin: 0
      padding-left: 20px
      list-style-type: none

      li
        line-height: 30px

    a:hover
      color: $color-link

    .toc-level-1 > .toc-link
      display: none

    .toc-level-2
      color: $color-text
      font-size: .8rem

      &:before
        color: $color-accent-1
        content: "#"

    .toc-level-3
      color: $color-meta
      font-size: .7rem
      line-height: 15px

    .toc-level-4
      display: none

    .toc-level-5
      display: none

    .toc-level-6
      display: none

    .toc-number
      display: none

@media screen and (min-width: 500px)
  #footer-post-container
    display: none

```

# source/css/_partial/search.styl

```styl
.search-input
  padding: 4px 7px
  width: 100%
  outline: none
  border: solid 1px $color-accent-3
  border-radius: 5px
  background-color: $color-background
  color: $color-text
  font-size: 1.2rem
  -webkit-border-radius: 5px
  -moz-border-radius: 5px

  &:focus
    border: solid 1px $color-accent-1

#search-result
  ul.search-result-list
    padding: 0
    list-style-type: none

  li
    margin: 2em auto

  a.search-result-title
    background-image: none
    color: $color-text
    text-transform: capitalize
    font-weight: bold
    line-height: 1.2

  p.search-result
    overflow: hidden
    margin: .4em auto
    max-height: 13em
    text-align: justify
    font-size: .8em

  em.search-keyword
    border-bottom: 1px dashed $color-link
    color: $color-link
    font-weight: bold

.search-no-result
  display: none
  padding-bottom: .5em
  color: $color-text

```

# source/css/_partial/tags.styl

```styl
#tag-cloud
  .tag-cloud-title
    color: $color-meta
  .tag-cloud-tags
    clear: both
    text-align: center
    a
      display: inline-block
      margin: 10px

```

# source/css/_partial/tooltip.styl

```styl
// ref: https://github.com/primer/primer/blob/master/modules/primer-tooltips/lib/tooltips.scss
.tooltipped
  position: relative
  
// This is the tooltip bubble
.tooltipped::after
  position: absolute
  z-index: 1000000
  display: none
  padding: .2em .5em
  -webkit-font-smoothing: subpixel-antialiased
  color: $color-background
  font-display: swap // @stylint ignore
  font-weight: 400
  font-size: $font-size * 0.8
  font-family: $font-family-body
  line-height: $line-height
  text-rendering: geometricPrecision
  text-align: center
  word-wrap: break-word
  white-space: pre
  content: attr(aria-label)
  background: $color-text
  border-radius: 3px
  opacity: 0
  
// This is the tooltip arrow
.tooltipped::before
  position: absolute
  z-index: 1000001
  display: none
  width: 0
  height: 0
  color: $color-text
  pointer-events: none
  content: ''
  border: 6px solid transparent
  opacity: 0
  
// delay animation for tooltip
@keyframes tooltip-appear
  from
    opacity: 0
  to
    opacity: 1
    
// This will indicate when we'll activate the tooltip
.tooltipped:hover,
.tooltipped:active,
.tooltipped:focus
  &::before,
  &::after
    display: inline-block
    text-decoration: none
    animation-name: tooltip-appear
    animation-duration: 0.1s
    animation-fill-mode: forwards
    animation-timing-function: ease-in
    
// Tooltipped south
.tooltipped-s,
.tooltipped-sw
  &::after
    top: 100%
    right: 50%
    margin-top: 6px
  &::before
    top: auto
    right: 50%
    bottom: -7px
    margin-right: -6px
    border-bottom-color: $color-text
.tooltipped-sw::after
  margin-right: -16px
  
// Move the tooltip body to the center of the object.
.tooltipped-s::after
  transform: translateX(50%)
```

# source/css/_util.styl

```styl
/* Basscss */
.inline
  display: inline

.block
  display: block

.inline-block
  display: inline-block

.table
  display: table

.table-cell
  display: table-cell

.overflow-hidden
  overflow: hidden

.overflow-scroll
  overflow: scroll

.overflow-auto
  overflow: auto

.clearfix:before, .clearfix:after
  display: table
  content: " "

.clearfix:after
  clear: both

.left
  float: left

.right
  float: right

.fit
  max-width: 100%

.truncate
  display: inline-block
  overflow: hidden
  text-overflow: ellipsis
  white-space: nowrap

.max-width-1
  max-width: 24rem

.max-width-2
  max-width: 32rem

.max-width-3
  max-width: 48rem

.max-width-4
  max-width: 64rem

.border-box
  box-sizing: border-box

.m0
  margin: 0

.mt0
  margin-top: 0

.mr0
  margin-right: 0

.mb0
  margin-bottom: 0

.ml0
  margin-left: 0

.mx0
  margin-right: 0
  margin-left: 0

.my0
  margin-top: 0
  margin-bottom: 0

.m1
  margin: .5rem

.mt1
  margin-top: .5rem

.mr1
  margin-right: .5rem

.mb1
  margin-bottom: .5rem

.ml1
  margin-left: .5rem

.mx1
  margin-right: .5rem
  margin-left: .5rem

.my1
  margin-top: .5rem
  margin-bottom: .5rem

.m2
  margin: 1rem

.mt2
  margin-top: 1rem

.mr2
  margin-right: 1rem

.mb2
  margin-bottom: 1rem

.ml2
  margin-left: 1rem

.mx2
  margin-right: 1rem
  margin-left: 1rem

.my2
  margin-top: 1rem
  margin-bottom: 1rem

.m3
  margin: 2rem

.mt3
  margin-top: 2rem

.mr3
  margin-right: 2rem

.mb3
  margin-bottom: 2rem

.ml3
  margin-left: 2rem

.mx3
  margin-right: 2rem
  margin-left: 2rem

.my3
  margin-top: 2rem
  margin-bottom: 2rem

.m4
  margin: 4rem

.mt4
  margin-top: 4rem

.mr4
  margin-right: 4rem

.mb4
  margin-bottom: 4rem

.ml4
  margin-left: 4rem

.mx4
  margin-right: 4rem
  margin-left: 4rem

.my4
  margin-top: 4rem
  margin-bottom: 4rem

.mxn1
  margin-right: -.5rem
  margin-left: -.5rem

.mxn2
  margin-right: -1rem
  margin-left: -1rem

.mxn3
  margin-right: -2rem
  margin-left: -2rem

.mxn4
  margin-right: -4rem
  margin-left: -4rem

.ml-auto
  margin-left: auto

.mr-auto
  margin-right: auto

.mx-auto
  margin-right: auto
  margin-left: auto

.p0
  padding: 0

.pt0
  padding-top: 0

.pr0
  padding-right: 0

.pb0
  padding-bottom: 0

.pl0
  padding-left: 0

.px0
  padding-right: 0
  padding-left: 0

.py0
  padding-top: 0
  padding-bottom: 0

.p1
  padding: .5rem

.pt1
  padding-top: .5rem

.pr1
  padding-right: .5rem

.pb1
  padding-bottom: .5rem

.pl1
  padding-left: .5rem

.py1
  padding-top: .5rem
  padding-bottom: .5rem

.px1
  padding-right: .5rem
  padding-left: .5rem

.p2
  padding: 1rem

.pt2
  padding-top: 1rem

.pr2
  padding-right: 1rem

.pb2
  padding-bottom: 1rem

.pl2
  padding-left: 1rem

.py2
  padding-top: 1rem
  padding-bottom: 1rem

.px2
  padding-right: 1rem
  padding-left: 1rem

.p3
  padding: 2rem

.pt3
  padding-top: 2rem

.pr3
  padding-right: 2rem

.pb3
  padding-bottom: 2rem

.pl3
  padding-left: 2rem

.py3
  padding-top: 2rem
  padding-bottom: 2rem

.px3
  padding-right: 2rem
  padding-left: 2rem

.p4
  padding: 4rem

.pt4
  padding-top: 4rem

.pr4
  padding-right: 4rem

.pb4
  padding-bottom: 4rem

.pl4
  padding-left: 4rem

.py4
  padding-top: 4rem
  padding-bottom: 4rem

.px4
  padding-right: 4rem
  padding-left: 4rem

```

# source/css/_variables.styl

```styl
// Fonts
$font-family-body = "Menlo", "Meslo LG", monospace
$font-family-mono = "Menlo", "Meslo LG", monospace
$font-size = 14px
$line-height = 1.725
$page-width = 0rem + (hexo-config("page_width") || 39)
// Logo
$logo-width = 0px + (hexo-config("logo.width") || 0)
$logo-height = 0px + (hexo-config("logo.height") || 0)
$logo-grayout = hexo-config("logo.grayout") || false
// Colors
$colors = hexo-config("colorscheme") || "dark"

```

# source/css/rtl.styl

```styl
@font-face
  font-family: Vazir
  src: url('../lib/vazir-font/Vazir.eot')
  src: url('../lib/vazir-font/Vazir.eot?#iefix') format('embedded-opentype'),
       url('../lib/vazir-font/Vazir.woff2') format('woff2'),
       url('../lib/vazir-font/Vazir.woff') format('woff'),
       url('../lib/vazir-font/Vazir.ttf') format('truetype')
  font-weight: normal

@font-face
  font-family: Vazir
  src: url('../lib/vazir-font/Vazir-Bold.eot')
  src: url('../lib/vazir-font/Vazir-Bold.eot?#iefix') format('embedded-opentype'),
       url('../lib/vazir-font/Vazir-Bold.woff2') format('woff2'),
       url('../lib/vazir-font/Vazir-Bold.woff') format('woff'),
       url('../lib/vazir-font/Vazir-Bold.ttf') format('truetype')
  font-weight: bold

@font-face
  font-family: Vazir
  src: url('../lib/vazir-font/Vazir-Light.eot')
  src: url('../lib/vazir-font/Vazir-Light.eot?#iefix') format('embedded-opentype'),
       url('../lib/vazir-font/Vazir-Light.woff2') format('woff2'),
       url('../lib/vazir-font/Vazir-Light.woff') format('woff'),
       url('../lib/vazir-font/Vazir-Light.ttf') format('truetype')
  font-weight: 300

.rtl
  font-family: Vazir, sans-serif
  direction: rtl

  #nav
    li
      margin-right: 0px !important // @stylint ignore
      padding-left: 15px
      border-right: 0px !important // @stylint ignore
      border-left: 1px dotted

    li:last-child
      margin-right: 15px !important // @stylint ignore
      border-left: 0 !important // @stylint ignore

  #header
    #logo
      float: right
      margin-right: 0
      margin-left: 20px

  #footer
    li
      margin-right: 0px
      padding-left: 15px
      border-right: 0px
      border-left: 1px dotted

    li:last-child
      margin-right: 15px !important // @stylint ignore
      border-left: 0 !important // @stylint ignore

    #logo
      float: right

  article
    .content
      h2:before
        right: -1rem

  .post-list
    .post-item
      .meta
        margin-left: 16px
        margin-right: inherit
        
@media screen and (min-width: 480px)
  .rtl
    .post-list
      .post-item
        .meta
          text-align: left
 
@media screen and (max-width: 480px)
  .rtl
    #header
      #title
        margin-left: 5rem
        margin-right: 0

      #nav
        ul
          li
            left: 1rem
            right: auto
            border: 0
```

# source/css/style.styl

```styl
@import "_variables"
@import "_colors/" + $colors
@import "_util"
@import "_mixins"
@import "_extend"
@import "_fonts"

global-reset()

*, *:before, *:after
  box-sizing: border-box

/* Scroll bar */
/* For Firefox */
*
  scrollbar-color: $color-scrollbar transparent

/* For Chrome, Edge, and Safari */
*::-webkit-scrollbar
  width: 8px
  height: 6px

*::-webkit-scrollbar-track
  background: transparent

*::-webkit-scrollbar-thumb
  background-color: $color-scrollbar
  border-radius: 6px

*::-webkit-scrollbar-thumb:hover
  background-color: darken($color-scrollbar, 20%)

*::-webkit-scrollbar-thumb:active
  background-color: darken($color-scrollbar, 30%)

html
  margin: 0
  padding: 0
  height: 100%
  border-top: 2px solid $color-text
  -webkit-text-size-adjust: 100%
  -ms-text-size-adjust: 100%

body
  margin: 0
  height: 100%
  background-color: $color-background
  color: $color-text
  font-weight: 400
  font-size: $font-size
  font-family: $font-family-body
  line-height: $line-height
  text-rendering: geometricPrecision

  antialias()

  @extend $base-style

.content
  position: relative
  display: flex
  flex-direction: column
  min-height: 100%
  overflow-wrap: break-word

  p
    hyphens(auto)

  code
    hyphens(manual)

  a
    color: $color-text
    text-decoration: none

    underline(5px, $color-text)

    &:hover
      background-image: linear-gradient(transparent, transparent 4px, $color-link 4px, $color-link)

  a.icon
    background: none

    &:hover
      color: $color-link

  h1 a, .h1 a, h2 a, h3 a, h4 a, h5 a, h6 a
    background: none
    color: inherit
    text-decoration: none

  h1 a:hover, .h1 a:hover, h2 a:hover, h3 a:hover, h4 a:hover, h5 a:hover, h6 a:hover
    underline(6px, $color-link)

  h6
    a
      background: none
      color: inherit
      text-decoration: none

  h6
    a:hover
      underline(6px, $color-link)

@media (min-width: 540px)
  .image-wrap
    flex-direction: row
    margin-bottom: 2rem

    .image-block
      flex: 1 0 35%
      margin-right: 2rem

    p
      flex: 1 0 65%

.max-width
  max-width: $page-width

@media (max-width: 480px)
  // smaller margins at smaller screen widths
  .px3
    padding-right: 1rem
    padding-left: 1rem

  .my4
    margin-top: 2rem
    margin-bottom: 2rem

@media (min-width: 480px)
  p
    text-align: justify

@import "_partial/header"
@import "_partial/post/actions_desktop"
@import "_partial/post/actions_mobile"
@import "_partial/index"
@import "_partial/article"
@import "_partial/archive"
@import "_partial/comments"
@import "_partial/footer"
@import "_partial/pagination"
@import "_partial/search"
@import "_partial/tags"
@import "_partial/tooltip"
@import "_partial/categories"
// Code
@import "_highlight/" + $highlight

pre
  overflow-x: auto
  padding: 10px 15px
  padding-bottom: 0
  border: 1px dotted $color-border
  border-radius: 4px
  font-size: 13px
  font-family: $font-family-mono
  line-height: 22px
  -webkit-border-radius: 4px

  code
    display: block
    padding: 0
    border: none

code
  padding: 0 5px
  border: 1px dotted $color-border
  border-radius: 2px
  -webkit-border-radius: 2px

.highlight
  overflow-x: auto
  margin: 1rem 0
  padding: 10px 15px
  border-radius: 4px
  background: $color-background-code
  font-family: $font-family-mono
  // color: $color-accent-3
  -webkit-border-radius: 4px

  figcaption
    margin: -5px 0 5px
    color: $color-meta-code
    font-size: .9em
    transform: scale(1)

    a
      float: right
      color: $color-meta-code
      font-style: italic
      font-size: .8em

      underline(10px, $color-link)

    a:hover
      color: lighten($color-meta-code, 20%)

    &:before, content: ""
      display: table

    &:after
      clear: both

  &:hover 
    .btn-copy
      opacity: 1

  .btn-copy
    font-size: 1.2rem
    position: absolute
    right: 20px
    opacity: 0
    transition: opacity 0.2s ease-in
    &:hover
      color: $color-accent-1

  pre
    margin: 0
    padding: 0
    border: none
    background: none

  table
    width: auto

  td.gutter
    text-align: right
    opacity: .2

  .line
    height: 22px

#header-post #actions
  direction: ltr !important

```

# source/images/apple-touch-icon.png

This is a binary file of the type: Image

# source/images/favicon-192x192.png

This is a binary file of the type: Image

# source/images/favicon.ico

This is a binary file of the type: Binary

# source/images/logo.png

This is a binary file of the type: Image

# source/js/main.js

```js
/**
 * Sets up Justified Gallery.
 */
if (!!$.prototype.justifiedGallery) {
  var options = {
    rowHeight: 140,
    margins: 4,
    lastRow: "justify"
  };
  $(".article-gallery").justifiedGallery(options);
}

$(document).ready(function() {

  /**
   * Shows the responsive navigation menu on mobile.
   */
  $("#header > #nav > ul > .icon").click(function() {
    $("#header > #nav > ul").toggleClass("responsive");
  });


  /**
   * Controls the different versions of  the menu in blog post articles 
   * for Desktop, tablet and mobile.
   */
  if ($(".post").length) {
    var menu = $("#menu");
    var nav = $("#menu > #nav");
    var menuIcon = $("#menu-icon, #menu-icon-tablet");

    /**
     * Display the menu on hi-res laptops and desktops.
     */
    if ($(document).width() >= 1440) {
      menu.show();
      menuIcon.addClass("active");
    }

    /**
     * Display the menu if the menu icon is clicked.
     */
    menuIcon.click(function() {
      if (menu.is(":hidden")) {
        menu.show();
        menuIcon.addClass("active");
      } else {
        menu.hide();
        menuIcon.removeClass("active");
      }
      return false;
    });

    /**
     * Add a scroll listener to the menu to hide/show the navigation links.
     */
    if (menu.length) {
      $(window).on("scroll", function() {
        var topDistance = menu.offset().top;

        // hide only the navigation links on desktop
        if (!nav.is(":visible") && topDistance < 50) {
          nav.show();
        } else if (nav.is(":visible") && topDistance > 100) {
          nav.hide();
        }

        // on tablet, hide the navigation icon as well and show a "scroll to top
        // icon" instead
        if ( ! $( "#menu-icon" ).is(":visible") && topDistance < 50 ) {
          $("#menu-icon-tablet").show();
          $("#top-icon-tablet").hide();
        } else if (! $( "#menu-icon" ).is(":visible") && topDistance > 100) {
          $("#menu-icon-tablet").hide();
          $("#top-icon-tablet").show();
        }
      });
    }

    /**
     * Show mobile navigation menu after scrolling upwards,
     * hide it again after scrolling downwards.
     */
    if ($( "#footer-post").length) {
      var lastScrollTop = 0;
      $(window).on("scroll", function() {
        var topDistance = $(window).scrollTop();

        if (topDistance > lastScrollTop){
          // downscroll -> show menu
          $("#footer-post").hide();
        } else {
          // upscroll -> hide menu
          $("#footer-post").show();
        }
        lastScrollTop = topDistance;

        // close all submenu"s on scroll
        $("#nav-footer").hide();
        $("#toc-footer").hide();
        $("#share-footer").hide();

        // show a "navigation" icon when close to the top of the page, 
        // otherwise show a "scroll to the top" icon
        if (topDistance < 50) {
          $("#actions-footer > #top").hide();
        } else if (topDistance > 100) {
          $("#actions-footer > #top").show();
        }
      });
    }
  }
});

```

# source/js/search.js

```js
// A local search script with the help of
// [hexo-generator-search](https://github.com/PaicHyperionDev/hexo-generator-search)
// Copyright (C) 2015
// Joseph Pan <http://github.com/wzpan>
// Shuhao Mao <http://github.com/maoshuhao>
// This library is free software; you can redistribute it and/or modify
// it under the terms of the GNU Lesser General Public License as
// published by the Free Software Foundation; either version 2.1 of the
// License, or (at your option) any later version.
//
// This library is distributed in the hope that it will be useful, but
// WITHOUT ANY WARRANTY; without even the implied warranty of
// MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
// Lesser General Public License for more details.
//
// You should have received a copy of the GNU Lesser General Public
// License along with this library; if not, write to the Free Software
// Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA
// 02110-1301 USA
//
// Modified by:
// Pieter Robberechts <http://github.com/probberechts>

/*exported searchFunc*/
var searchFunc = function(path, searchId, contentId) {

  function stripHtml(html) {
    html = html.replace(/<style([\s\S]*?)<\/style>/gi, "");
    html = html.replace(/<script([\s\S]*?)<\/script>/gi, "");
    html = html.replace(/<figure([\s\S]*?)<\/figure>/gi, "");
    html = html.replace(/<\/div>/ig, "\n");
    html = html.replace(/<\/li>/ig, "\n");
    html = html.replace(/<li>/ig, "  *  ");
    html = html.replace(/<\/ul>/ig, "\n");
    html = html.replace(/<\/p>/ig, "\n");
    html = html.replace(/<br\s*[\/]?>/gi, "\n");
    html = html.replace(/<[^>]+>/ig, "");
    return html;
  }

  function getAllCombinations(keywords) {
    var i, j, result = [];

    for (i = 0; i < keywords.length; i++) {
        for (j = i + 1; j < keywords.length + 1; j++) {
            result.push(keywords.slice(i, j).join(" "));
        }
    }
    return result;
  }

  $.ajax({
    url: path,
    dataType: "xml",
    success: function(xmlResponse) {
      // get the contents from search data
      var datas = $("entry", xmlResponse).map(function() {
        return {
          title: $("title", this).text(),
          content: $("content", this).text(),
          url: $("link", this).attr("href")
        };
      }).get();

      var $input = document.getElementById(searchId);
      if (!$input) { return; }
      var $resultContent = document.getElementById(contentId);

      $input.addEventListener("input", function(){
        var resultList = [];
        var keywords = getAllCombinations(this.value.trim().toLowerCase().split(" "))
          .sort(function(a,b) { return b.split(" ").length - a.split(" ").length; });
        $resultContent.innerHTML = "";
        if (this.value.trim().length <= 0) {
          return;
        }
        // perform local searching
        datas.forEach(function(data) {
          var matches = 0;
          if (!data.title || data.title.trim() === "") {
            data.title = "Untitled";
          }
          var dataTitle = data.title.trim().toLowerCase();
          var dataTitleLowerCase = dataTitle.toLowerCase();
          var dataContent = stripHtml(data.content.trim());
          var dataContentLowerCase = dataContent.toLowerCase();
          var dataUrl = data.url;
          var indexTitle = -1;
          var indexContent = -1;
          var firstOccur = -1;
          // only match artiles with not empty contents
          if (dataContent !== "") {
            keywords.forEach(function(keyword) {
              indexTitle = dataTitleLowerCase.indexOf(keyword);
              indexContent = dataContentLowerCase.indexOf(keyword);

              if( indexTitle >= 0 || indexContent >= 0 ){
                matches += 1;
                if (indexContent < 0) {
                  indexContent = 0;
                }
                if (firstOccur < 0) {
                  firstOccur = indexContent;
                }
              }
            });
          }
          // show search results
          if (matches > 0) {
            var searchResult = {};
            searchResult.rank = matches;
            searchResult.str = "<li><a href='"+ dataUrl +"' class='search-result-title'>"+ dataTitle +"</a>";
            if (firstOccur >= 0) {
              // cut out 100 characters
              var start = firstOccur - 20;
              var end = firstOccur + 80;

              if(start < 0){
                start = 0;
              }

              if(start == 0){
                end = 100;
              }

              if(end > dataContent.length){
                end = dataContent.length;
              }

              var matchContent = dataContent.substring(start, end);

              // highlight all keywords
              var regS = new RegExp(keywords.join("|"), "gi");
              matchContent = matchContent.replace(regS, function(keyword) {
                return "<em class=\"search-keyword\">"+keyword+"</em>";
              });

              searchResult.str += "<p class=\"search-result\">" + matchContent +"...</p>";
            }
            searchResult.str += "</li>";
            resultList.push(searchResult);
          }
        });
        if (resultList.length) {
          resultList.sort(function(a, b) {
              return b.rank - a.rank;
          });
          var result ="<ul class=\"search-result-list\">";
          for (var i = 0; i < resultList.length; i++) {
            result += resultList[i].str;
          }
          result += "</ul>";
          $resultContent.innerHTML = result;
        }
      });
    }
  });
};

```

# source/lib/clipboard/clipboard.min.js

```js
/*!
 * clipboard.js v2.0.11
 * https://clipboardjs.com/
 *
 * Licensed MIT © Zeno Rocha
 */
!function(t,e){"object"==typeof exports&&"object"==typeof module?module.exports=e():"function"==typeof define&&define.amd?define([],e):"object"==typeof exports?exports.ClipboardJS=e():t.ClipboardJS=e()}(this,function(){return n={686:function(t,e,n){"use strict";n.d(e,{default:function(){return b}});var e=n(279),i=n.n(e),e=n(370),u=n.n(e),e=n(817),r=n.n(e);function c(t){try{return document.execCommand(t)}catch(t){return}}var a=function(t){t=r()(t);return c("cut"),t};function o(t,e){var n,o,t=(n=t,o="rtl"===document.documentElement.getAttribute("dir"),(t=document.createElement("textarea")).style.fontSize="12pt",t.style.border="0",t.style.padding="0",t.style.margin="0",t.style.position="absolute",t.style[o?"right":"left"]="-9999px",o=window.pageYOffset||document.documentElement.scrollTop,t.style.top="".concat(o,"px"),t.setAttribute("readonly",""),t.value=n,t);return e.container.appendChild(t),e=r()(t),c("copy"),t.remove(),e}var f=function(t){var e=1<arguments.length&&void 0!==arguments[1]?arguments[1]:{container:document.body},n="";return"string"==typeof t?n=o(t,e):t instanceof HTMLInputElement&&!["text","search","url","tel","password"].includes(null==t?void 0:t.type)?n=o(t.value,e):(n=r()(t),c("copy")),n};function l(t){return(l="function"==typeof Symbol&&"symbol"==typeof Symbol.iterator?function(t){return typeof t}:function(t){return t&&"function"==typeof Symbol&&t.constructor===Symbol&&t!==Symbol.prototype?"symbol":typeof t})(t)}var s=function(){var t=0<arguments.length&&void 0!==arguments[0]?arguments[0]:{},e=t.action,n=void 0===e?"copy":e,o=t.container,e=t.target,t=t.text;if("copy"!==n&&"cut"!==n)throw new Error('Invalid "action" value, use either "copy" or "cut"');if(void 0!==e){if(!e||"object"!==l(e)||1!==e.nodeType)throw new Error('Invalid "target" value, use a valid Element');if("copy"===n&&e.hasAttribute("disabled"))throw new Error('Invalid "target" attribute. Please use "readonly" instead of "disabled" attribute');if("cut"===n&&(e.hasAttribute("readonly")||e.hasAttribute("disabled")))throw new Error('Invalid "target" attribute. You can\'t cut text from elements with "readonly" or "disabled" attributes')}return t?f(t,{container:o}):e?"cut"===n?a(e):f(e,{container:o}):void 0};function p(t){return(p="function"==typeof Symbol&&"symbol"==typeof Symbol.iterator?function(t){return typeof t}:function(t){return t&&"function"==typeof Symbol&&t.constructor===Symbol&&t!==Symbol.prototype?"symbol":typeof t})(t)}function d(t,e){for(var n=0;n<e.length;n++){var o=e[n];o.enumerable=o.enumerable||!1,o.configurable=!0,"value"in o&&(o.writable=!0),Object.defineProperty(t,o.key,o)}}function y(t,e){return(y=Object.setPrototypeOf||function(t,e){return t.__proto__=e,t})(t,e)}function h(n){var o=function(){if("undefined"==typeof Reflect||!Reflect.construct)return!1;if(Reflect.construct.sham)return!1;if("function"==typeof Proxy)return!0;try{return Date.prototype.toString.call(Reflect.construct(Date,[],function(){})),!0}catch(t){return!1}}();return function(){var t,e=v(n);return t=o?(t=v(this).constructor,Reflect.construct(e,arguments,t)):e.apply(this,arguments),e=this,!(t=t)||"object"!==p(t)&&"function"!=typeof t?function(t){if(void 0!==t)return t;throw new ReferenceError("this hasn't been initialised - super() hasn't been called")}(e):t}}function v(t){return(v=Object.setPrototypeOf?Object.getPrototypeOf:function(t){return t.__proto__||Object.getPrototypeOf(t)})(t)}function m(t,e){t="data-clipboard-".concat(t);if(e.hasAttribute(t))return e.getAttribute(t)}var b=function(){!function(t,e){if("function"!=typeof e&&null!==e)throw new TypeError("Super expression must either be null or a function");t.prototype=Object.create(e&&e.prototype,{constructor:{value:t,writable:!0,configurable:!0}}),e&&y(t,e)}(r,i());var t,e,n,o=h(r);function r(t,e){var n;return function(t){if(!(t instanceof r))throw new TypeError("Cannot call a class as a function")}(this),(n=o.call(this)).resolveOptions(e),n.listenClick(t),n}return t=r,n=[{key:"copy",value:function(t){var e=1<arguments.length&&void 0!==arguments[1]?arguments[1]:{container:document.body};return f(t,e)}},{key:"cut",value:function(t){return a(t)}},{key:"isSupported",value:function(){var t=0<arguments.length&&void 0!==arguments[0]?arguments[0]:["copy","cut"],t="string"==typeof t?[t]:t,e=!!document.queryCommandSupported;return t.forEach(function(t){e=e&&!!document.queryCommandSupported(t)}),e}}],(e=[{key:"resolveOptions",value:function(){var t=0<arguments.length&&void 0!==arguments[0]?arguments[0]:{};this.action="function"==typeof t.action?t.action:this.defaultAction,this.target="function"==typeof t.target?t.target:this.defaultTarget,this.text="function"==typeof t.text?t.text:this.defaultText,this.container="object"===p(t.container)?t.container:document.body}},{key:"listenClick",value:function(t){var e=this;this.listener=u()(t,"click",function(t){return e.onClick(t)})}},{key:"onClick",value:function(t){var e=t.delegateTarget||t.currentTarget,n=this.action(e)||"copy",t=s({action:n,container:this.container,target:this.target(e),text:this.text(e)});this.emit(t?"success":"error",{action:n,text:t,trigger:e,clearSelection:function(){e&&e.focus(),window.getSelection().removeAllRanges()}})}},{key:"defaultAction",value:function(t){return m("action",t)}},{key:"defaultTarget",value:function(t){t=m("target",t);if(t)return document.querySelector(t)}},{key:"defaultText",value:function(t){return m("text",t)}},{key:"destroy",value:function(){this.listener.destroy()}}])&&d(t.prototype,e),n&&d(t,n),r}()},828:function(t){var e;"undefined"==typeof Element||Element.prototype.matches||((e=Element.prototype).matches=e.matchesSelector||e.mozMatchesSelector||e.msMatchesSelector||e.oMatchesSelector||e.webkitMatchesSelector),t.exports=function(t,e){for(;t&&9!==t.nodeType;){if("function"==typeof t.matches&&t.matches(e))return t;t=t.parentNode}}},438:function(t,e,n){var u=n(828);function i(t,e,n,o,r){var i=function(e,n,t,o){return function(t){t.delegateTarget=u(t.target,n),t.delegateTarget&&o.call(e,t)}}.apply(this,arguments);return t.addEventListener(n,i,r),{destroy:function(){t.removeEventListener(n,i,r)}}}t.exports=function(t,e,n,o,r){return"function"==typeof t.addEventListener?i.apply(null,arguments):"function"==typeof n?i.bind(null,document).apply(null,arguments):("string"==typeof t&&(t=document.querySelectorAll(t)),Array.prototype.map.call(t,function(t){return i(t,e,n,o,r)}))}},879:function(t,n){n.node=function(t){return void 0!==t&&t instanceof HTMLElement&&1===t.nodeType},n.nodeList=function(t){var e=Object.prototype.toString.call(t);return void 0!==t&&("[object NodeList]"===e||"[object HTMLCollection]"===e)&&"length"in t&&(0===t.length||n.node(t[0]))},n.string=function(t){return"string"==typeof t||t instanceof String},n.fn=function(t){return"[object Function]"===Object.prototype.toString.call(t)}},370:function(t,e,n){var f=n(879),l=n(438);t.exports=function(t,e,n){if(!t&&!e&&!n)throw new Error("Missing required arguments");if(!f.string(e))throw new TypeError("Second argument must be a String");if(!f.fn(n))throw new TypeError("Third argument must be a Function");if(f.node(t))return c=e,a=n,(u=t).addEventListener(c,a),{destroy:function(){u.removeEventListener(c,a)}};if(f.nodeList(t))return o=t,r=e,i=n,Array.prototype.forEach.call(o,function(t){t.addEventListener(r,i)}),{destroy:function(){Array.prototype.forEach.call(o,function(t){t.removeEventListener(r,i)})}};if(f.string(t))return t=t,e=e,n=n,l(document.body,t,e,n);throw new TypeError("First argument must be a String, HTMLElement, HTMLCollection, or NodeList");var o,r,i,u,c,a}},817:function(t){t.exports=function(t){var e,n="SELECT"===t.nodeName?(t.focus(),t.value):"INPUT"===t.nodeName||"TEXTAREA"===t.nodeName?((e=t.hasAttribute("readonly"))||t.setAttribute("readonly",""),t.select(),t.setSelectionRange(0,t.value.length),e||t.removeAttribute("readonly"),t.value):(t.hasAttribute("contenteditable")&&t.focus(),n=window.getSelection(),(e=document.createRange()).selectNodeContents(t),n.removeAllRanges(),n.addRange(e),n.toString());return n}},279:function(t){function e(){}e.prototype={on:function(t,e,n){var o=this.e||(this.e={});return(o[t]||(o[t]=[])).push({fn:e,ctx:n}),this},once:function(t,e,n){var o=this;function r(){o.off(t,r),e.apply(n,arguments)}return r._=e,this.on(t,r,n)},emit:function(t){for(var e=[].slice.call(arguments,1),n=((this.e||(this.e={}))[t]||[]).slice(),o=0,r=n.length;o<r;o++)n[o].fn.apply(n[o].ctx,e);return this},off:function(t,e){var n=this.e||(this.e={}),o=n[t],r=[];if(o&&e)for(var i=0,u=o.length;i<u;i++)o[i].fn!==e&&o[i].fn._!==e&&r.push(o[i]);return r.length?n[t]=r:delete n[t],this}},t.exports=e,t.exports.TinyEmitter=e}},r={},o.n=function(t){var e=t&&t.__esModule?function(){return t.default}:function(){return t};return o.d(e,{a:e}),e},o.d=function(t,e){for(var n in e)o.o(e,n)&&!o.o(t,n)&&Object.defineProperty(t,n,{enumerable:!0,get:e[n]})},o.o=function(t,e){return Object.prototype.hasOwnProperty.call(t,e)},o(686).default;function o(t){if(r[t])return r[t].exports;var e=r[t]={exports:{}};return n[t](e,e.exports,o),e.exports}var n,r});
```

# source/lib/font-awesome/css/all.min.css

```css
/*!
 * Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com
 * License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License)
 * Copyright 2023 Fonticons, Inc.
 */
.fa{font-family:var(--fa-style-family,"Font Awesome 6 Free");font-weight:var(--fa-style,900)}.fa,.fa-brands,.fa-classic,.fa-regular,.fa-sharp,.fa-solid,.fab,.far,.fas{-moz-osx-font-smoothing:grayscale;-webkit-font-smoothing:antialiased;display:var(--fa-display,inline-block);font-style:normal;font-variant:normal;line-height:1;text-rendering:auto}.fa-classic,.fa-regular,.fa-solid,.far,.fas{font-family:"Font Awesome 6 Free"}.fa-brands,.fab{font-family:"Font Awesome 6 Brands"}.fa-1x{font-size:1em}.fa-2x{font-size:2em}.fa-3x{font-size:3em}.fa-4x{font-size:4em}.fa-5x{font-size:5em}.fa-6x{font-size:6em}.fa-7x{font-size:7em}.fa-8x{font-size:8em}.fa-9x{font-size:9em}.fa-10x{font-size:10em}.fa-2xs{font-size:.625em;line-height:.1em;vertical-align:.225em}.fa-xs{font-size:.75em;line-height:.08333em;vertical-align:.125em}.fa-sm{font-size:.875em;line-height:.07143em;vertical-align:.05357em}.fa-lg{font-size:1.25em;line-height:.05em;vertical-align:-.075em}.fa-xl{font-size:1.5em;line-height:.04167em;vertical-align:-.125em}.fa-2xl{font-size:2em;line-height:.03125em;vertical-align:-.1875em}.fa-fw{text-align:center;width:1.25em}.fa-ul{list-style-type:none;margin-left:var(--fa-li-margin,2.5em);padding-left:0}.fa-ul>li{position:relative}.fa-li{left:calc(var(--fa-li-width, 2em)*-1);position:absolute;text-align:center;width:var(--fa-li-width,2em);line-height:inherit}.fa-border{border-radius:var(--fa-border-radius,.1em);border:var(--fa-border-width,.08em) var(--fa-border-style,solid) var(--fa-border-color,#eee);padding:var(--fa-border-padding,.2em .25em .15em)}.fa-pull-left{float:left;margin-right:var(--fa-pull-margin,.3em)}.fa-pull-right{float:right;margin-left:var(--fa-pull-margin,.3em)}.fa-beat{-webkit-animation-name:fa-beat;animation-name:fa-beat;-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,ease-in-out);animation-timing-function:var(--fa-animation-timing,ease-in-out)}.fa-bounce{-webkit-animation-name:fa-bounce;animation-name:fa-bounce;-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,cubic-bezier(.28,.84,.42,1));animation-timing-function:var(--fa-animation-timing,cubic-bezier(.28,.84,.42,1))}.fa-fade{-webkit-animation-name:fa-fade;animation-name:fa-fade;-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,cubic-bezier(.4,0,.6,1));animation-timing-function:var(--fa-animation-timing,cubic-bezier(.4,0,.6,1))}.fa-beat-fade,.fa-fade{-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s)}.fa-beat-fade{-webkit-animation-name:fa-beat-fade;animation-name:fa-beat-fade;-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,cubic-bezier(.4,0,.6,1));animation-timing-function:var(--fa-animation-timing,cubic-bezier(.4,0,.6,1))}.fa-flip{-webkit-animation-name:fa-flip;animation-name:fa-flip;-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,ease-in-out);animation-timing-function:var(--fa-animation-timing,ease-in-out)}.fa-shake{-webkit-animation-name:fa-shake;animation-name:fa-shake;-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,linear);animation-timing-function:var(--fa-animation-timing,linear)}.fa-shake,.fa-spin{-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal)}.fa-spin{-webkit-animation-name:fa-spin;animation-name:fa-spin;-webkit-animation-duration:var(--fa-animation-duration,2s);animation-duration:var(--fa-animation-duration,2s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,linear);animation-timing-function:var(--fa-animation-timing,linear)}.fa-spin-reverse{--fa-animation-direction:reverse}.fa-pulse,.fa-spin-pulse{-webkit-animation-name:fa-spin;animation-name:fa-spin;-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,steps(8));animation-timing-function:var(--fa-animation-timing,steps(8))}@media (prefers-reduced-motion:reduce){.fa-beat,.fa-beat-fade,.fa-bounce,.fa-fade,.fa-flip,.fa-pulse,.fa-shake,.fa-spin,.fa-spin-pulse{-webkit-animation-delay:-1ms;animation-delay:-1ms;-webkit-animation-duration:1ms;animation-duration:1ms;-webkit-animation-iteration-count:1;animation-iteration-count:1;-webkit-transition-delay:0s;transition-delay:0s;-webkit-transition-duration:0s;transition-duration:0s}}@-webkit-keyframes fa-beat{0%,90%{-webkit-transform:scale(1);transform:scale(1)}45%{-webkit-transform:scale(var(--fa-beat-scale,1.25));transform:scale(var(--fa-beat-scale,1.25))}}@keyframes fa-beat{0%,90%{-webkit-transform:scale(1);transform:scale(1)}45%{-webkit-transform:scale(var(--fa-beat-scale,1.25));transform:scale(var(--fa-beat-scale,1.25))}}@-webkit-keyframes fa-bounce{0%{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}10%{-webkit-transform:scale(var(--fa-bounce-start-scale-x,1.1),var(--fa-bounce-start-scale-y,.9)) translateY(0);transform:scale(var(--fa-bounce-start-scale-x,1.1),var(--fa-bounce-start-scale-y,.9)) translateY(0)}30%{-webkit-transform:scale(var(--fa-bounce-jump-scale-x,.9),var(--fa-bounce-jump-scale-y,1.1)) translateY(var(--fa-bounce-height,-.5em));transform:scale(var(--fa-bounce-jump-scale-x,.9),var(--fa-bounce-jump-scale-y,1.1)) translateY(var(--fa-bounce-height,-.5em))}50%{-webkit-transform:scale(var(--fa-bounce-land-scale-x,1.05),var(--fa-bounce-land-scale-y,.95)) translateY(0);transform:scale(var(--fa-bounce-land-scale-x,1.05),var(--fa-bounce-land-scale-y,.95)) translateY(0)}57%{-webkit-transform:scale(1) translateY(var(--fa-bounce-rebound,-.125em));transform:scale(1) translateY(var(--fa-bounce-rebound,-.125em))}64%{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}to{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}}@keyframes fa-bounce{0%{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}10%{-webkit-transform:scale(var(--fa-bounce-start-scale-x,1.1),var(--fa-bounce-start-scale-y,.9)) translateY(0);transform:scale(var(--fa-bounce-start-scale-x,1.1),var(--fa-bounce-start-scale-y,.9)) translateY(0)}30%{-webkit-transform:scale(var(--fa-bounce-jump-scale-x,.9),var(--fa-bounce-jump-scale-y,1.1)) translateY(var(--fa-bounce-height,-.5em));transform:scale(var(--fa-bounce-jump-scale-x,.9),var(--fa-bounce-jump-scale-y,1.1)) translateY(var(--fa-bounce-height,-.5em))}50%{-webkit-transform:scale(var(--fa-bounce-land-scale-x,1.05),var(--fa-bounce-land-scale-y,.95)) translateY(0);transform:scale(var(--fa-bounce-land-scale-x,1.05),var(--fa-bounce-land-scale-y,.95)) translateY(0)}57%{-webkit-transform:scale(1) translateY(var(--fa-bounce-rebound,-.125em));transform:scale(1) translateY(var(--fa-bounce-rebound,-.125em))}64%{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}to{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}}@-webkit-keyframes fa-fade{50%{opacity:var(--fa-fade-opacity,.4)}}@keyframes fa-fade{50%{opacity:var(--fa-fade-opacity,.4)}}@-webkit-keyframes fa-beat-fade{0%,to{opacity:var(--fa-beat-fade-opacity,.4);-webkit-transform:scale(1);transform:scale(1)}50%{opacity:1;-webkit-transform:scale(var(--fa-beat-fade-scale,1.125));transform:scale(var(--fa-beat-fade-scale,1.125))}}@keyframes fa-beat-fade{0%,to{opacity:var(--fa-beat-fade-opacity,.4);-webkit-transform:scale(1);transform:scale(1)}50%{opacity:1;-webkit-transform:scale(var(--fa-beat-fade-scale,1.125));transform:scale(var(--fa-beat-fade-scale,1.125))}}@-webkit-keyframes fa-flip{50%{-webkit-transform:rotate3d(var(--fa-flip-x,0),var(--fa-flip-y,1),var(--fa-flip-z,0),var(--fa-flip-angle,-180deg));transform:rotate3d(var(--fa-flip-x,0),var(--fa-flip-y,1),var(--fa-flip-z,0),var(--fa-flip-angle,-180deg))}}@keyframes fa-flip{50%{-webkit-transform:rotate3d(var(--fa-flip-x,0),var(--fa-flip-y,1),var(--fa-flip-z,0),var(--fa-flip-angle,-180deg));transform:rotate3d(var(--fa-flip-x,0),var(--fa-flip-y,1),var(--fa-flip-z,0),var(--fa-flip-angle,-180deg))}}@-webkit-keyframes fa-shake{0%{-webkit-transform:rotate(-15deg);transform:rotate(-15deg)}4%{-webkit-transform:rotate(15deg);transform:rotate(15deg)}8%,24%{-webkit-transform:rotate(-18deg);transform:rotate(-18deg)}12%,28%{-webkit-transform:rotate(18deg);transform:rotate(18deg)}16%{-webkit-transform:rotate(-22deg);transform:rotate(-22deg)}20%{-webkit-transform:rotate(22deg);transform:rotate(22deg)}32%{-webkit-transform:rotate(-12deg);transform:rotate(-12deg)}36%{-webkit-transform:rotate(12deg);transform:rotate(12deg)}40%,to{-webkit-transform:rotate(0deg);transform:rotate(0deg)}}@keyframes fa-shake{0%{-webkit-transform:rotate(-15deg);transform:rotate(-15deg)}4%{-webkit-transform:rotate(15deg);transform:rotate(15deg)}8%,24%{-webkit-transform:rotate(-18deg);transform:rotate(-18deg)}12%,28%{-webkit-transform:rotate(18deg);transform:rotate(18deg)}16%{-webkit-transform:rotate(-22deg);transform:rotate(-22deg)}20%{-webkit-transform:rotate(22deg);transform:rotate(22deg)}32%{-webkit-transform:rotate(-12deg);transform:rotate(-12deg)}36%{-webkit-transform:rotate(12deg);transform:rotate(12deg)}40%,to{-webkit-transform:rotate(0deg);transform:rotate(0deg)}}@-webkit-keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}@keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}.fa-rotate-90{-webkit-transform:rotate(90deg);transform:rotate(90deg)}.fa-rotate-180{-webkit-transform:rotate(180deg);transform:rotate(180deg)}.fa-rotate-270{-webkit-transform:rotate(270deg);transform:rotate(270deg)}.fa-flip-horizontal{-webkit-transform:scaleX(-1);transform:scaleX(-1)}.fa-flip-vertical{-webkit-transform:scaleY(-1);transform:scaleY(-1)}.fa-flip-both,.fa-flip-horizontal.fa-flip-vertical{-webkit-transform:scale(-1);transform:scale(-1)}.fa-rotate-by{-webkit-transform:rotate(var(--fa-rotate-angle,none));transform:rotate(var(--fa-rotate-angle,none))}.fa-stack{display:inline-block;height:2em;line-height:2em;position:relative;vertical-align:middle;width:2.5em}.fa-stack-1x,.fa-stack-2x{left:0;position:absolute;text-align:center;width:100%;z-index:var(--fa-stack-z-index,auto)}.fa-stack-1x{line-height:inherit}.fa-stack-2x{font-size:2em}.fa-inverse{color:var(--fa-inverse,#fff)}

.fa-0:before{content:"\30"}.fa-1:before{content:"\31"}.fa-2:before{content:"\32"}.fa-3:before{content:"\33"}.fa-4:before{content:"\34"}.fa-5:before{content:"\35"}.fa-6:before{content:"\36"}.fa-7:before{content:"\37"}.fa-8:before{content:"\38"}.fa-9:before{content:"\39"}.fa-fill-drip:before{content:"\f576"}.fa-arrows-to-circle:before{content:"\e4bd"}.fa-chevron-circle-right:before,.fa-circle-chevron-right:before{content:"\f138"}.fa-at:before{content:"\40"}.fa-trash-alt:before,.fa-trash-can:before{content:"\f2ed"}.fa-text-height:before{content:"\f034"}.fa-user-times:before,.fa-user-xmark:before{content:"\f235"}.fa-stethoscope:before{content:"\f0f1"}.fa-comment-alt:before,.fa-message:before{content:"\f27a"}.fa-info:before{content:"\f129"}.fa-compress-alt:before,.fa-down-left-and-up-right-to-center:before{content:"\f422"}.fa-explosion:before{content:"\e4e9"}.fa-file-alt:before,.fa-file-lines:before,.fa-file-text:before{content:"\f15c"}.fa-wave-square:before{content:"\f83e"}.fa-ring:before{content:"\f70b"}.fa-building-un:before{content:"\e4d9"}.fa-dice-three:before{content:"\f527"}.fa-calendar-alt:before,.fa-calendar-days:before{content:"\f073"}.fa-anchor-circle-check:before{content:"\e4aa"}.fa-building-circle-arrow-right:before{content:"\e4d1"}.fa-volleyball-ball:before,.fa-volleyball:before{content:"\f45f"}.fa-arrows-up-to-line:before{content:"\e4c2"}.fa-sort-desc:before,.fa-sort-down:before{content:"\f0dd"}.fa-circle-minus:before,.fa-minus-circle:before{content:"\f056"}.fa-door-open:before{content:"\f52b"}.fa-right-from-bracket:before,.fa-sign-out-alt:before{content:"\f2f5"}.fa-atom:before{content:"\f5d2"}.fa-soap:before{content:"\e06e"}.fa-heart-music-camera-bolt:before,.fa-icons:before{content:"\f86d"}.fa-microphone-alt-slash:before,.fa-microphone-lines-slash:before{content:"\f539"}.fa-bridge-circle-check:before{content:"\e4c9"}.fa-pump-medical:before{content:"\e06a"}.fa-fingerprint:before{content:"\f577"}.fa-hand-point-right:before{content:"\f0a4"}.fa-magnifying-glass-location:before,.fa-search-location:before{content:"\f689"}.fa-forward-step:before,.fa-step-forward:before{content:"\f051"}.fa-face-smile-beam:before,.fa-smile-beam:before{content:"\f5b8"}.fa-flag-checkered:before{content:"\f11e"}.fa-football-ball:before,.fa-football:before{content:"\f44e"}.fa-school-circle-exclamation:before{content:"\e56c"}.fa-crop:before{content:"\f125"}.fa-angle-double-down:before,.fa-angles-down:before{content:"\f103"}.fa-users-rectangle:before{content:"\e594"}.fa-people-roof:before{content:"\e537"}.fa-people-line:before{content:"\e534"}.fa-beer-mug-empty:before,.fa-beer:before{content:"\f0fc"}.fa-diagram-predecessor:before{content:"\e477"}.fa-arrow-up-long:before,.fa-long-arrow-up:before{content:"\f176"}.fa-burn:before,.fa-fire-flame-simple:before{content:"\f46a"}.fa-male:before,.fa-person:before{content:"\f183"}.fa-laptop:before{content:"\f109"}.fa-file-csv:before{content:"\f6dd"}.fa-menorah:before{content:"\f676"}.fa-truck-plane:before{content:"\e58f"}.fa-record-vinyl:before{content:"\f8d9"}.fa-face-grin-stars:before,.fa-grin-stars:before{content:"\f587"}.fa-bong:before{content:"\f55c"}.fa-pastafarianism:before,.fa-spaghetti-monster-flying:before{content:"\f67b"}.fa-arrow-down-up-across-line:before{content:"\e4af"}.fa-spoon:before,.fa-utensil-spoon:before{content:"\f2e5"}.fa-jar-wheat:before{content:"\e517"}.fa-envelopes-bulk:before,.fa-mail-bulk:before{content:"\f674"}.fa-file-circle-exclamation:before{content:"\e4eb"}.fa-circle-h:before,.fa-hospital-symbol:before{content:"\f47e"}.fa-pager:before{content:"\f815"}.fa-address-book:before,.fa-contact-book:before{content:"\f2b9"}.fa-strikethrough:before{content:"\f0cc"}.fa-k:before{content:"\4b"}.fa-landmark-flag:before{content:"\e51c"}.fa-pencil-alt:before,.fa-pencil:before{content:"\f303"}.fa-backward:before{content:"\f04a"}.fa-caret-right:before{content:"\f0da"}.fa-comments:before{content:"\f086"}.fa-file-clipboard:before,.fa-paste:before{content:"\f0ea"}.fa-code-pull-request:before{content:"\e13c"}.fa-clipboard-list:before{content:"\f46d"}.fa-truck-loading:before,.fa-truck-ramp-box:before{content:"\f4de"}.fa-user-check:before{content:"\f4fc"}.fa-vial-virus:before{content:"\e597"}.fa-sheet-plastic:before{content:"\e571"}.fa-blog:before{content:"\f781"}.fa-user-ninja:before{content:"\f504"}.fa-person-arrow-up-from-line:before{content:"\e539"}.fa-scroll-torah:before,.fa-torah:before{content:"\f6a0"}.fa-broom-ball:before,.fa-quidditch-broom-ball:before,.fa-quidditch:before{content:"\f458"}.fa-toggle-off:before{content:"\f204"}.fa-archive:before,.fa-box-archive:before{content:"\f187"}.fa-person-drowning:before{content:"\e545"}.fa-arrow-down-9-1:before,.fa-sort-numeric-desc:before,.fa-sort-numeric-down-alt:before{content:"\f886"}.fa-face-grin-tongue-squint:before,.fa-grin-tongue-squint:before{content:"\f58a"}.fa-spray-can:before{content:"\f5bd"}.fa-truck-monster:before{content:"\f63b"}.fa-w:before{content:"\57"}.fa-earth-africa:before,.fa-globe-africa:before{content:"\f57c"}.fa-rainbow:before{content:"\f75b"}.fa-circle-notch:before{content:"\f1ce"}.fa-tablet-alt:before,.fa-tablet-screen-button:before{content:"\f3fa"}.fa-paw:before{content:"\f1b0"}.fa-cloud:before{content:"\f0c2"}.fa-trowel-bricks:before{content:"\e58a"}.fa-face-flushed:before,.fa-flushed:before{content:"\f579"}.fa-hospital-user:before{content:"\f80d"}.fa-tent-arrow-left-right:before{content:"\e57f"}.fa-gavel:before,.fa-legal:before{content:"\f0e3"}.fa-binoculars:before{content:"\f1e5"}.fa-microphone-slash:before{content:"\f131"}.fa-box-tissue:before{content:"\e05b"}.fa-motorcycle:before{content:"\f21c"}.fa-bell-concierge:before,.fa-concierge-bell:before{content:"\f562"}.fa-pen-ruler:before,.fa-pencil-ruler:before{content:"\f5ae"}.fa-people-arrows-left-right:before,.fa-people-arrows:before{content:"\e068"}.fa-mars-and-venus-burst:before{content:"\e523"}.fa-caret-square-right:before,.fa-square-caret-right:before{content:"\f152"}.fa-cut:before,.fa-scissors:before{content:"\f0c4"}.fa-sun-plant-wilt:before{content:"\e57a"}.fa-toilets-portable:before{content:"\e584"}.fa-hockey-puck:before{content:"\f453"}.fa-table:before{content:"\f0ce"}.fa-magnifying-glass-arrow-right:before{content:"\e521"}.fa-digital-tachograph:before,.fa-tachograph-digital:before{content:"\f566"}.fa-users-slash:before{content:"\e073"}.fa-clover:before{content:"\e139"}.fa-mail-reply:before,.fa-reply:before{content:"\f3e5"}.fa-star-and-crescent:before{content:"\f699"}.fa-house-fire:before{content:"\e50c"}.fa-minus-square:before,.fa-square-minus:before{content:"\f146"}.fa-helicopter:before{content:"\f533"}.fa-compass:before{content:"\f14e"}.fa-caret-square-down:before,.fa-square-caret-down:before{content:"\f150"}.fa-file-circle-question:before{content:"\e4ef"}.fa-laptop-code:before{content:"\f5fc"}.fa-swatchbook:before{content:"\f5c3"}.fa-prescription-bottle:before{content:"\f485"}.fa-bars:before,.fa-navicon:before{content:"\f0c9"}.fa-people-group:before{content:"\e533"}.fa-hourglass-3:before,.fa-hourglass-end:before{content:"\f253"}.fa-heart-broken:before,.fa-heart-crack:before{content:"\f7a9"}.fa-external-link-square-alt:before,.fa-square-up-right:before{content:"\f360"}.fa-face-kiss-beam:before,.fa-kiss-beam:before{content:"\f597"}.fa-film:before{content:"\f008"}.fa-ruler-horizontal:before{content:"\f547"}.fa-people-robbery:before{content:"\e536"}.fa-lightbulb:before{content:"\f0eb"}.fa-caret-left:before{content:"\f0d9"}.fa-circle-exclamation:before,.fa-exclamation-circle:before{content:"\f06a"}.fa-school-circle-xmark:before{content:"\e56d"}.fa-arrow-right-from-bracket:before,.fa-sign-out:before{content:"\f08b"}.fa-chevron-circle-down:before,.fa-circle-chevron-down:before{content:"\f13a"}.fa-unlock-alt:before,.fa-unlock-keyhole:before{content:"\f13e"}.fa-cloud-showers-heavy:before{content:"\f740"}.fa-headphones-alt:before,.fa-headphones-simple:before{content:"\f58f"}.fa-sitemap:before{content:"\f0e8"}.fa-circle-dollar-to-slot:before,.fa-donate:before{content:"\f4b9"}.fa-memory:before{content:"\f538"}.fa-road-spikes:before{content:"\e568"}.fa-fire-burner:before{content:"\e4f1"}.fa-flag:before{content:"\f024"}.fa-hanukiah:before{content:"\f6e6"}.fa-feather:before{content:"\f52d"}.fa-volume-down:before,.fa-volume-low:before{content:"\f027"}.fa-comment-slash:before{content:"\f4b3"}.fa-cloud-sun-rain:before{content:"\f743"}.fa-compress:before{content:"\f066"}.fa-wheat-alt:before,.fa-wheat-awn:before{content:"\e2cd"}.fa-ankh:before{content:"\f644"}.fa-hands-holding-child:before{content:"\e4fa"}.fa-asterisk:before{content:"\2a"}.fa-check-square:before,.fa-square-check:before{content:"\f14a"}.fa-peseta-sign:before{content:"\e221"}.fa-header:before,.fa-heading:before{content:"\f1dc"}.fa-ghost:before{content:"\f6e2"}.fa-list-squares:before,.fa-list:before{content:"\f03a"}.fa-phone-square-alt:before,.fa-square-phone-flip:before{content:"\f87b"}.fa-cart-plus:before{content:"\f217"}.fa-gamepad:before{content:"\f11b"}.fa-circle-dot:before,.fa-dot-circle:before{content:"\f192"}.fa-dizzy:before,.fa-face-dizzy:before{content:"\f567"}.fa-egg:before{content:"\f7fb"}.fa-house-medical-circle-xmark:before{content:"\e513"}.fa-campground:before{content:"\f6bb"}.fa-folder-plus:before{content:"\f65e"}.fa-futbol-ball:before,.fa-futbol:before,.fa-soccer-ball:before{content:"\f1e3"}.fa-paint-brush:before,.fa-paintbrush:before{content:"\f1fc"}.fa-lock:before{content:"\f023"}.fa-gas-pump:before{content:"\f52f"}.fa-hot-tub-person:before,.fa-hot-tub:before{content:"\f593"}.fa-map-location:before,.fa-map-marked:before{content:"\f59f"}.fa-house-flood-water:before{content:"\e50e"}.fa-tree:before{content:"\f1bb"}.fa-bridge-lock:before{content:"\e4cc"}.fa-sack-dollar:before{content:"\f81d"}.fa-edit:before,.fa-pen-to-square:before{content:"\f044"}.fa-car-side:before{content:"\f5e4"}.fa-share-alt:before,.fa-share-nodes:before{content:"\f1e0"}.fa-heart-circle-minus:before{content:"\e4ff"}.fa-hourglass-2:before,.fa-hourglass-half:before{content:"\f252"}.fa-microscope:before{content:"\f610"}.fa-sink:before{content:"\e06d"}.fa-bag-shopping:before,.fa-shopping-bag:before{content:"\f290"}.fa-arrow-down-z-a:before,.fa-sort-alpha-desc:before,.fa-sort-alpha-down-alt:before{content:"\f881"}.fa-mitten:before{content:"\f7b5"}.fa-person-rays:before{content:"\e54d"}.fa-users:before{content:"\f0c0"}.fa-eye-slash:before{content:"\f070"}.fa-flask-vial:before{content:"\e4f3"}.fa-hand-paper:before,.fa-hand:before{content:"\f256"}.fa-om:before{content:"\f679"}.fa-worm:before{content:"\e599"}.fa-house-circle-xmark:before{content:"\e50b"}.fa-plug:before{content:"\f1e6"}.fa-chevron-up:before{content:"\f077"}.fa-hand-spock:before{content:"\f259"}.fa-stopwatch:before{content:"\f2f2"}.fa-face-kiss:before,.fa-kiss:before{content:"\f596"}.fa-bridge-circle-xmark:before{content:"\e4cb"}.fa-face-grin-tongue:before,.fa-grin-tongue:before{content:"\f589"}.fa-chess-bishop:before{content:"\f43a"}.fa-face-grin-wink:before,.fa-grin-wink:before{content:"\f58c"}.fa-deaf:before,.fa-deafness:before,.fa-ear-deaf:before,.fa-hard-of-hearing:before{content:"\f2a4"}.fa-road-circle-check:before{content:"\e564"}.fa-dice-five:before{content:"\f523"}.fa-rss-square:before,.fa-square-rss:before{content:"\f143"}.fa-land-mine-on:before{content:"\e51b"}.fa-i-cursor:before{content:"\f246"}.fa-stamp:before{content:"\f5bf"}.fa-stairs:before{content:"\e289"}.fa-i:before{content:"\49"}.fa-hryvnia-sign:before,.fa-hryvnia:before{content:"\f6f2"}.fa-pills:before{content:"\f484"}.fa-face-grin-wide:before,.fa-grin-alt:before{content:"\f581"}.fa-tooth:before{content:"\f5c9"}.fa-v:before{content:"\56"}.fa-bangladeshi-taka-sign:before{content:"\e2e6"}.fa-bicycle:before{content:"\f206"}.fa-rod-asclepius:before,.fa-rod-snake:before,.fa-staff-aesculapius:before,.fa-staff-snake:before{content:"\e579"}.fa-head-side-cough-slash:before{content:"\e062"}.fa-ambulance:before,.fa-truck-medical:before{content:"\f0f9"}.fa-wheat-awn-circle-exclamation:before{content:"\e598"}.fa-snowman:before{content:"\f7d0"}.fa-mortar-pestle:before{content:"\f5a7"}.fa-road-barrier:before{content:"\e562"}.fa-school:before{content:"\f549"}.fa-igloo:before{content:"\f7ae"}.fa-joint:before{content:"\f595"}.fa-angle-right:before{content:"\f105"}.fa-horse:before{content:"\f6f0"}.fa-q:before{content:"\51"}.fa-g:before{content:"\47"}.fa-notes-medical:before{content:"\f481"}.fa-temperature-2:before,.fa-temperature-half:before,.fa-thermometer-2:before,.fa-thermometer-half:before{content:"\f2c9"}.fa-dong-sign:before{content:"\e169"}.fa-capsules:before{content:"\f46b"}.fa-poo-bolt:before,.fa-poo-storm:before{content:"\f75a"}.fa-face-frown-open:before,.fa-frown-open:before{content:"\f57a"}.fa-hand-point-up:before{content:"\f0a6"}.fa-money-bill:before{content:"\f0d6"}.fa-bookmark:before{content:"\f02e"}.fa-align-justify:before{content:"\f039"}.fa-umbrella-beach:before{content:"\f5ca"}.fa-helmet-un:before{content:"\e503"}.fa-bullseye:before{content:"\f140"}.fa-bacon:before{content:"\f7e5"}.fa-hand-point-down:before{content:"\f0a7"}.fa-arrow-up-from-bracket:before{content:"\e09a"}.fa-folder-blank:before,.fa-folder:before{content:"\f07b"}.fa-file-medical-alt:before,.fa-file-waveform:before{content:"\f478"}.fa-radiation:before{content:"\f7b9"}.fa-chart-simple:before{content:"\e473"}.fa-mars-stroke:before{content:"\f229"}.fa-vial:before{content:"\f492"}.fa-dashboard:before,.fa-gauge-med:before,.fa-gauge:before,.fa-tachometer-alt-average:before{content:"\f624"}.fa-magic-wand-sparkles:before,.fa-wand-magic-sparkles:before{content:"\e2ca"}.fa-e:before{content:"\45"}.fa-pen-alt:before,.fa-pen-clip:before{content:"\f305"}.fa-bridge-circle-exclamation:before{content:"\e4ca"}.fa-user:before{content:"\f007"}.fa-school-circle-check:before{content:"\e56b"}.fa-dumpster:before{content:"\f793"}.fa-shuttle-van:before,.fa-van-shuttle:before{content:"\f5b6"}.fa-building-user:before{content:"\e4da"}.fa-caret-square-left:before,.fa-square-caret-left:before{content:"\f191"}.fa-highlighter:before{content:"\f591"}.fa-key:before{content:"\f084"}.fa-bullhorn:before{content:"\f0a1"}.fa-globe:before{content:"\f0ac"}.fa-synagogue:before{content:"\f69b"}.fa-person-half-dress:before{content:"\e548"}.fa-road-bridge:before{content:"\e563"}.fa-location-arrow:before{content:"\f124"}.fa-c:before{content:"\43"}.fa-tablet-button:before{content:"\f10a"}.fa-building-lock:before{content:"\e4d6"}.fa-pizza-slice:before{content:"\f818"}.fa-money-bill-wave:before{content:"\f53a"}.fa-area-chart:before,.fa-chart-area:before{content:"\f1fe"}.fa-house-flag:before{content:"\e50d"}.fa-person-circle-minus:before{content:"\e540"}.fa-ban:before,.fa-cancel:before{content:"\f05e"}.fa-camera-rotate:before{content:"\e0d8"}.fa-air-freshener:before,.fa-spray-can-sparkles:before{content:"\f5d0"}.fa-star:before{content:"\f005"}.fa-repeat:before{content:"\f363"}.fa-cross:before{content:"\f654"}.fa-box:before{content:"\f466"}.fa-venus-mars:before{content:"\f228"}.fa-arrow-pointer:before,.fa-mouse-pointer:before{content:"\f245"}.fa-expand-arrows-alt:before,.fa-maximize:before{content:"\f31e"}.fa-charging-station:before{content:"\f5e7"}.fa-shapes:before,.fa-triangle-circle-square:before{content:"\f61f"}.fa-random:before,.fa-shuffle:before{content:"\f074"}.fa-person-running:before,.fa-running:before{content:"\f70c"}.fa-mobile-retro:before{content:"\e527"}.fa-grip-lines-vertical:before{content:"\f7a5"}.fa-spider:before{content:"\f717"}.fa-hands-bound:before{content:"\e4f9"}.fa-file-invoice-dollar:before{content:"\f571"}.fa-plane-circle-exclamation:before{content:"\e556"}.fa-x-ray:before{content:"\f497"}.fa-spell-check:before{content:"\f891"}.fa-slash:before{content:"\f715"}.fa-computer-mouse:before,.fa-mouse:before{content:"\f8cc"}.fa-arrow-right-to-bracket:before,.fa-sign-in:before{content:"\f090"}.fa-shop-slash:before,.fa-store-alt-slash:before{content:"\e070"}.fa-server:before{content:"\f233"}.fa-virus-covid-slash:before{content:"\e4a9"}.fa-shop-lock:before{content:"\e4a5"}.fa-hourglass-1:before,.fa-hourglass-start:before{content:"\f251"}.fa-blender-phone:before{content:"\f6b6"}.fa-building-wheat:before{content:"\e4db"}.fa-person-breastfeeding:before{content:"\e53a"}.fa-right-to-bracket:before,.fa-sign-in-alt:before{content:"\f2f6"}.fa-venus:before{content:"\f221"}.fa-passport:before{content:"\f5ab"}.fa-heart-pulse:before,.fa-heartbeat:before{content:"\f21e"}.fa-people-carry-box:before,.fa-people-carry:before{content:"\f4ce"}.fa-temperature-high:before{content:"\f769"}.fa-microchip:before{content:"\f2db"}.fa-crown:before{content:"\f521"}.fa-weight-hanging:before{content:"\f5cd"}.fa-xmarks-lines:before{content:"\e59a"}.fa-file-prescription:before{content:"\f572"}.fa-weight-scale:before,.fa-weight:before{content:"\f496"}.fa-user-friends:before,.fa-user-group:before{content:"\f500"}.fa-arrow-up-a-z:before,.fa-sort-alpha-up:before{content:"\f15e"}.fa-chess-knight:before{content:"\f441"}.fa-face-laugh-squint:before,.fa-laugh-squint:before{content:"\f59b"}.fa-wheelchair:before{content:"\f193"}.fa-arrow-circle-up:before,.fa-circle-arrow-up:before{content:"\f0aa"}.fa-toggle-on:before{content:"\f205"}.fa-person-walking:before,.fa-walking:before{content:"\f554"}.fa-l:before{content:"\4c"}.fa-fire:before{content:"\f06d"}.fa-bed-pulse:before,.fa-procedures:before{content:"\f487"}.fa-shuttle-space:before,.fa-space-shuttle:before{content:"\f197"}.fa-face-laugh:before,.fa-laugh:before{content:"\f599"}.fa-folder-open:before{content:"\f07c"}.fa-heart-circle-plus:before{content:"\e500"}.fa-code-fork:before{content:"\e13b"}.fa-city:before{content:"\f64f"}.fa-microphone-alt:before,.fa-microphone-lines:before{content:"\f3c9"}.fa-pepper-hot:before{content:"\f816"}.fa-unlock:before{content:"\f09c"}.fa-colon-sign:before{content:"\e140"}.fa-headset:before{content:"\f590"}.fa-store-slash:before{content:"\e071"}.fa-road-circle-xmark:before{content:"\e566"}.fa-user-minus:before{content:"\f503"}.fa-mars-stroke-up:before,.fa-mars-stroke-v:before{content:"\f22a"}.fa-champagne-glasses:before,.fa-glass-cheers:before{content:"\f79f"}.fa-clipboard:before{content:"\f328"}.fa-house-circle-exclamation:before{content:"\e50a"}.fa-file-arrow-up:before,.fa-file-upload:before{content:"\f574"}.fa-wifi-3:before,.fa-wifi-strong:before,.fa-wifi:before{content:"\f1eb"}.fa-bath:before,.fa-bathtub:before{content:"\f2cd"}.fa-underline:before{content:"\f0cd"}.fa-user-edit:before,.fa-user-pen:before{content:"\f4ff"}.fa-signature:before{content:"\f5b7"}.fa-stroopwafel:before{content:"\f551"}.fa-bold:before{content:"\f032"}.fa-anchor-lock:before{content:"\e4ad"}.fa-building-ngo:before{content:"\e4d7"}.fa-manat-sign:before{content:"\e1d5"}.fa-not-equal:before{content:"\f53e"}.fa-border-style:before,.fa-border-top-left:before{content:"\f853"}.fa-map-location-dot:before,.fa-map-marked-alt:before{content:"\f5a0"}.fa-jedi:before{content:"\f669"}.fa-poll:before,.fa-square-poll-vertical:before{content:"\f681"}.fa-mug-hot:before{content:"\f7b6"}.fa-battery-car:before,.fa-car-battery:before{content:"\f5df"}.fa-gift:before{content:"\f06b"}.fa-dice-two:before{content:"\f528"}.fa-chess-queen:before{content:"\f445"}.fa-glasses:before{content:"\f530"}.fa-chess-board:before{content:"\f43c"}.fa-building-circle-check:before{content:"\e4d2"}.fa-person-chalkboard:before{content:"\e53d"}.fa-mars-stroke-h:before,.fa-mars-stroke-right:before{content:"\f22b"}.fa-hand-back-fist:before,.fa-hand-rock:before{content:"\f255"}.fa-caret-square-up:before,.fa-square-caret-up:before{content:"\f151"}.fa-cloud-showers-water:before{content:"\e4e4"}.fa-bar-chart:before,.fa-chart-bar:before{content:"\f080"}.fa-hands-bubbles:before,.fa-hands-wash:before{content:"\e05e"}.fa-less-than-equal:before{content:"\f537"}.fa-train:before{content:"\f238"}.fa-eye-low-vision:before,.fa-low-vision:before{content:"\f2a8"}.fa-crow:before{content:"\f520"}.fa-sailboat:before{content:"\e445"}.fa-window-restore:before{content:"\f2d2"}.fa-plus-square:before,.fa-square-plus:before{content:"\f0fe"}.fa-torii-gate:before{content:"\f6a1"}.fa-frog:before{content:"\f52e"}.fa-bucket:before{content:"\e4cf"}.fa-image:before{content:"\f03e"}.fa-microphone:before{content:"\f130"}.fa-cow:before{content:"\f6c8"}.fa-caret-up:before{content:"\f0d8"}.fa-screwdriver:before{content:"\f54a"}.fa-folder-closed:before{content:"\e185"}.fa-house-tsunami:before{content:"\e515"}.fa-square-nfi:before{content:"\e576"}.fa-arrow-up-from-ground-water:before{content:"\e4b5"}.fa-glass-martini-alt:before,.fa-martini-glass:before{content:"\f57b"}.fa-rotate-back:before,.fa-rotate-backward:before,.fa-rotate-left:before,.fa-undo-alt:before{content:"\f2ea"}.fa-columns:before,.fa-table-columns:before{content:"\f0db"}.fa-lemon:before{content:"\f094"}.fa-head-side-mask:before{content:"\e063"}.fa-handshake:before{content:"\f2b5"}.fa-gem:before{content:"\f3a5"}.fa-dolly-box:before,.fa-dolly:before{content:"\f472"}.fa-smoking:before{content:"\f48d"}.fa-compress-arrows-alt:before,.fa-minimize:before{content:"\f78c"}.fa-monument:before{content:"\f5a6"}.fa-snowplow:before{content:"\f7d2"}.fa-angle-double-right:before,.fa-angles-right:before{content:"\f101"}.fa-cannabis:before{content:"\f55f"}.fa-circle-play:before,.fa-play-circle:before{content:"\f144"}.fa-tablets:before{content:"\f490"}.fa-ethernet:before{content:"\f796"}.fa-eur:before,.fa-euro-sign:before,.fa-euro:before{content:"\f153"}.fa-chair:before{content:"\f6c0"}.fa-check-circle:before,.fa-circle-check:before{content:"\f058"}.fa-circle-stop:before,.fa-stop-circle:before{content:"\f28d"}.fa-compass-drafting:before,.fa-drafting-compass:before{content:"\f568"}.fa-plate-wheat:before{content:"\e55a"}.fa-icicles:before{content:"\f7ad"}.fa-person-shelter:before{content:"\e54f"}.fa-neuter:before{content:"\f22c"}.fa-id-badge:before{content:"\f2c1"}.fa-marker:before{content:"\f5a1"}.fa-face-laugh-beam:before,.fa-laugh-beam:before{content:"\f59a"}.fa-helicopter-symbol:before{content:"\e502"}.fa-universal-access:before{content:"\f29a"}.fa-chevron-circle-up:before,.fa-circle-chevron-up:before{content:"\f139"}.fa-lari-sign:before{content:"\e1c8"}.fa-volcano:before{content:"\f770"}.fa-person-walking-dashed-line-arrow-right:before{content:"\e553"}.fa-gbp:before,.fa-pound-sign:before,.fa-sterling-sign:before{content:"\f154"}.fa-viruses:before{content:"\e076"}.fa-square-person-confined:before{content:"\e577"}.fa-user-tie:before{content:"\f508"}.fa-arrow-down-long:before,.fa-long-arrow-down:before{content:"\f175"}.fa-tent-arrow-down-to-line:before{content:"\e57e"}.fa-certificate:before{content:"\f0a3"}.fa-mail-reply-all:before,.fa-reply-all:before{content:"\f122"}.fa-suitcase:before{content:"\f0f2"}.fa-person-skating:before,.fa-skating:before{content:"\f7c5"}.fa-filter-circle-dollar:before,.fa-funnel-dollar:before{content:"\f662"}.fa-camera-retro:before{content:"\f083"}.fa-arrow-circle-down:before,.fa-circle-arrow-down:before{content:"\f0ab"}.fa-arrow-right-to-file:before,.fa-file-import:before{content:"\f56f"}.fa-external-link-square:before,.fa-square-arrow-up-right:before{content:"\f14c"}.fa-box-open:before{content:"\f49e"}.fa-scroll:before{content:"\f70e"}.fa-spa:before{content:"\f5bb"}.fa-location-pin-lock:before{content:"\e51f"}.fa-pause:before{content:"\f04c"}.fa-hill-avalanche:before{content:"\e507"}.fa-temperature-0:before,.fa-temperature-empty:before,.fa-thermometer-0:before,.fa-thermometer-empty:before{content:"\f2cb"}.fa-bomb:before{content:"\f1e2"}.fa-registered:before{content:"\f25d"}.fa-address-card:before,.fa-contact-card:before,.fa-vcard:before{content:"\f2bb"}.fa-balance-scale-right:before,.fa-scale-unbalanced-flip:before{content:"\f516"}.fa-subscript:before{content:"\f12c"}.fa-diamond-turn-right:before,.fa-directions:before{content:"\f5eb"}.fa-burst:before{content:"\e4dc"}.fa-house-laptop:before,.fa-laptop-house:before{content:"\e066"}.fa-face-tired:before,.fa-tired:before{content:"\f5c8"}.fa-money-bills:before{content:"\e1f3"}.fa-smog:before{content:"\f75f"}.fa-crutch:before{content:"\f7f7"}.fa-cloud-arrow-up:before,.fa-cloud-upload-alt:before,.fa-cloud-upload:before{content:"\f0ee"}.fa-palette:before{content:"\f53f"}.fa-arrows-turn-right:before{content:"\e4c0"}.fa-vest:before{content:"\e085"}.fa-ferry:before{content:"\e4ea"}.fa-arrows-down-to-people:before{content:"\e4b9"}.fa-seedling:before,.fa-sprout:before{content:"\f4d8"}.fa-arrows-alt-h:before,.fa-left-right:before{content:"\f337"}.fa-boxes-packing:before{content:"\e4c7"}.fa-arrow-circle-left:before,.fa-circle-arrow-left:before{content:"\f0a8"}.fa-group-arrows-rotate:before{content:"\e4f6"}.fa-bowl-food:before{content:"\e4c6"}.fa-candy-cane:before{content:"\f786"}.fa-arrow-down-wide-short:before,.fa-sort-amount-asc:before,.fa-sort-amount-down:before{content:"\f160"}.fa-cloud-bolt:before,.fa-thunderstorm:before{content:"\f76c"}.fa-remove-format:before,.fa-text-slash:before{content:"\f87d"}.fa-face-smile-wink:before,.fa-smile-wink:before{content:"\f4da"}.fa-file-word:before{content:"\f1c2"}.fa-file-powerpoint:before{content:"\f1c4"}.fa-arrows-h:before,.fa-arrows-left-right:before{content:"\f07e"}.fa-house-lock:before{content:"\e510"}.fa-cloud-arrow-down:before,.fa-cloud-download-alt:before,.fa-cloud-download:before{content:"\f0ed"}.fa-children:before{content:"\e4e1"}.fa-blackboard:before,.fa-chalkboard:before{content:"\f51b"}.fa-user-alt-slash:before,.fa-user-large-slash:before{content:"\f4fa"}.fa-envelope-open:before{content:"\f2b6"}.fa-handshake-alt-slash:before,.fa-handshake-simple-slash:before{content:"\e05f"}.fa-mattress-pillow:before{content:"\e525"}.fa-guarani-sign:before{content:"\e19a"}.fa-arrows-rotate:before,.fa-refresh:before,.fa-sync:before{content:"\f021"}.fa-fire-extinguisher:before{content:"\f134"}.fa-cruzeiro-sign:before{content:"\e152"}.fa-greater-than-equal:before{content:"\f532"}.fa-shield-alt:before,.fa-shield-halved:before{content:"\f3ed"}.fa-atlas:before,.fa-book-atlas:before{content:"\f558"}.fa-virus:before{content:"\e074"}.fa-envelope-circle-check:before{content:"\e4e8"}.fa-layer-group:before{content:"\f5fd"}.fa-arrows-to-dot:before{content:"\e4be"}.fa-archway:before{content:"\f557"}.fa-heart-circle-check:before{content:"\e4fd"}.fa-house-chimney-crack:before,.fa-house-damage:before{content:"\f6f1"}.fa-file-archive:before,.fa-file-zipper:before{content:"\f1c6"}.fa-square:before{content:"\f0c8"}.fa-glass-martini:before,.fa-martini-glass-empty:before{content:"\f000"}.fa-couch:before{content:"\f4b8"}.fa-cedi-sign:before{content:"\e0df"}.fa-italic:before{content:"\f033"}.fa-church:before{content:"\f51d"}.fa-comments-dollar:before{content:"\f653"}.fa-democrat:before{content:"\f747"}.fa-z:before{content:"\5a"}.fa-person-skiing:before,.fa-skiing:before{content:"\f7c9"}.fa-road-lock:before{content:"\e567"}.fa-a:before{content:"\41"}.fa-temperature-arrow-down:before,.fa-temperature-down:before{content:"\e03f"}.fa-feather-alt:before,.fa-feather-pointed:before{content:"\f56b"}.fa-p:before{content:"\50"}.fa-snowflake:before{content:"\f2dc"}.fa-newspaper:before{content:"\f1ea"}.fa-ad:before,.fa-rectangle-ad:before{content:"\f641"}.fa-arrow-circle-right:before,.fa-circle-arrow-right:before{content:"\f0a9"}.fa-filter-circle-xmark:before{content:"\e17b"}.fa-locust:before{content:"\e520"}.fa-sort:before,.fa-unsorted:before{content:"\f0dc"}.fa-list-1-2:before,.fa-list-numeric:before,.fa-list-ol:before{content:"\f0cb"}.fa-person-dress-burst:before{content:"\e544"}.fa-money-check-alt:before,.fa-money-check-dollar:before{content:"\f53d"}.fa-vector-square:before{content:"\f5cb"}.fa-bread-slice:before{content:"\f7ec"}.fa-language:before{content:"\f1ab"}.fa-face-kiss-wink-heart:before,.fa-kiss-wink-heart:before{content:"\f598"}.fa-filter:before{content:"\f0b0"}.fa-question:before{content:"\3f"}.fa-file-signature:before{content:"\f573"}.fa-arrows-alt:before,.fa-up-down-left-right:before{content:"\f0b2"}.fa-house-chimney-user:before{content:"\e065"}.fa-hand-holding-heart:before{content:"\f4be"}.fa-puzzle-piece:before{content:"\f12e"}.fa-money-check:before{content:"\f53c"}.fa-star-half-alt:before,.fa-star-half-stroke:before{content:"\f5c0"}.fa-code:before{content:"\f121"}.fa-glass-whiskey:before,.fa-whiskey-glass:before{content:"\f7a0"}.fa-building-circle-exclamation:before{content:"\e4d3"}.fa-magnifying-glass-chart:before{content:"\e522"}.fa-arrow-up-right-from-square:before,.fa-external-link:before{content:"\f08e"}.fa-cubes-stacked:before{content:"\e4e6"}.fa-krw:before,.fa-won-sign:before,.fa-won:before{content:"\f159"}.fa-virus-covid:before{content:"\e4a8"}.fa-austral-sign:before{content:"\e0a9"}.fa-f:before{content:"\46"}.fa-leaf:before{content:"\f06c"}.fa-road:before{content:"\f018"}.fa-cab:before,.fa-taxi:before{content:"\f1ba"}.fa-person-circle-plus:before{content:"\e541"}.fa-chart-pie:before,.fa-pie-chart:before{content:"\f200"}.fa-bolt-lightning:before{content:"\e0b7"}.fa-sack-xmark:before{content:"\e56a"}.fa-file-excel:before{content:"\f1c3"}.fa-file-contract:before{content:"\f56c"}.fa-fish-fins:before{content:"\e4f2"}.fa-building-flag:before{content:"\e4d5"}.fa-face-grin-beam:before,.fa-grin-beam:before{content:"\f582"}.fa-object-ungroup:before{content:"\f248"}.fa-poop:before{content:"\f619"}.fa-location-pin:before,.fa-map-marker:before{content:"\f041"}.fa-kaaba:before{content:"\f66b"}.fa-toilet-paper:before{content:"\f71e"}.fa-hard-hat:before,.fa-hat-hard:before,.fa-helmet-safety:before{content:"\f807"}.fa-eject:before{content:"\f052"}.fa-arrow-alt-circle-right:before,.fa-circle-right:before{content:"\f35a"}.fa-plane-circle-check:before{content:"\e555"}.fa-face-rolling-eyes:before,.fa-meh-rolling-eyes:before{content:"\f5a5"}.fa-object-group:before{content:"\f247"}.fa-chart-line:before,.fa-line-chart:before{content:"\f201"}.fa-mask-ventilator:before{content:"\e524"}.fa-arrow-right:before{content:"\f061"}.fa-map-signs:before,.fa-signs-post:before{content:"\f277"}.fa-cash-register:before{content:"\f788"}.fa-person-circle-question:before{content:"\e542"}.fa-h:before{content:"\48"}.fa-tarp:before{content:"\e57b"}.fa-screwdriver-wrench:before,.fa-tools:before{content:"\f7d9"}.fa-arrows-to-eye:before{content:"\e4bf"}.fa-plug-circle-bolt:before{content:"\e55b"}.fa-heart:before{content:"\f004"}.fa-mars-and-venus:before{content:"\f224"}.fa-home-user:before,.fa-house-user:before{content:"\e1b0"}.fa-dumpster-fire:before{content:"\f794"}.fa-house-crack:before{content:"\e3b1"}.fa-cocktail:before,.fa-martini-glass-citrus:before{content:"\f561"}.fa-face-surprise:before,.fa-surprise:before{content:"\f5c2"}.fa-bottle-water:before{content:"\e4c5"}.fa-circle-pause:before,.fa-pause-circle:before{content:"\f28b"}.fa-toilet-paper-slash:before{content:"\e072"}.fa-apple-alt:before,.fa-apple-whole:before{content:"\f5d1"}.fa-kitchen-set:before{content:"\e51a"}.fa-r:before{content:"\52"}.fa-temperature-1:before,.fa-temperature-quarter:before,.fa-thermometer-1:before,.fa-thermometer-quarter:before{content:"\f2ca"}.fa-cube:before{content:"\f1b2"}.fa-bitcoin-sign:before{content:"\e0b4"}.fa-shield-dog:before{content:"\e573"}.fa-solar-panel:before{content:"\f5ba"}.fa-lock-open:before{content:"\f3c1"}.fa-elevator:before{content:"\e16d"}.fa-money-bill-transfer:before{content:"\e528"}.fa-money-bill-trend-up:before{content:"\e529"}.fa-house-flood-water-circle-arrow-right:before{content:"\e50f"}.fa-poll-h:before,.fa-square-poll-horizontal:before{content:"\f682"}.fa-circle:before{content:"\f111"}.fa-backward-fast:before,.fa-fast-backward:before{content:"\f049"}.fa-recycle:before{content:"\f1b8"}.fa-user-astronaut:before{content:"\f4fb"}.fa-plane-slash:before{content:"\e069"}.fa-trademark:before{content:"\f25c"}.fa-basketball-ball:before,.fa-basketball:before{content:"\f434"}.fa-satellite-dish:before{content:"\f7c0"}.fa-arrow-alt-circle-up:before,.fa-circle-up:before{content:"\f35b"}.fa-mobile-alt:before,.fa-mobile-screen-button:before{content:"\f3cd"}.fa-volume-high:before,.fa-volume-up:before{content:"\f028"}.fa-users-rays:before{content:"\e593"}.fa-wallet:before{content:"\f555"}.fa-clipboard-check:before{content:"\f46c"}.fa-file-audio:before{content:"\f1c7"}.fa-burger:before,.fa-hamburger:before{content:"\f805"}.fa-wrench:before{content:"\f0ad"}.fa-bugs:before{content:"\e4d0"}.fa-rupee-sign:before,.fa-rupee:before{content:"\f156"}.fa-file-image:before{content:"\f1c5"}.fa-circle-question:before,.fa-question-circle:before{content:"\f059"}.fa-plane-departure:before{content:"\f5b0"}.fa-handshake-slash:before{content:"\e060"}.fa-book-bookmark:before{content:"\e0bb"}.fa-code-branch:before{content:"\f126"}.fa-hat-cowboy:before{content:"\f8c0"}.fa-bridge:before{content:"\e4c8"}.fa-phone-alt:before,.fa-phone-flip:before{content:"\f879"}.fa-truck-front:before{content:"\e2b7"}.fa-cat:before{content:"\f6be"}.fa-anchor-circle-exclamation:before{content:"\e4ab"}.fa-truck-field:before{content:"\e58d"}.fa-route:before{content:"\f4d7"}.fa-clipboard-question:before{content:"\e4e3"}.fa-panorama:before{content:"\e209"}.fa-comment-medical:before{content:"\f7f5"}.fa-teeth-open:before{content:"\f62f"}.fa-file-circle-minus:before{content:"\e4ed"}.fa-tags:before{content:"\f02c"}.fa-wine-glass:before{content:"\f4e3"}.fa-fast-forward:before,.fa-forward-fast:before{content:"\f050"}.fa-face-meh-blank:before,.fa-meh-blank:before{content:"\f5a4"}.fa-parking:before,.fa-square-parking:before{content:"\f540"}.fa-house-signal:before{content:"\e012"}.fa-bars-progress:before,.fa-tasks-alt:before{content:"\f828"}.fa-faucet-drip:before{content:"\e006"}.fa-cart-flatbed:before,.fa-dolly-flatbed:before{content:"\f474"}.fa-ban-smoking:before,.fa-smoking-ban:before{content:"\f54d"}.fa-terminal:before{content:"\f120"}.fa-mobile-button:before{content:"\f10b"}.fa-house-medical-flag:before{content:"\e514"}.fa-basket-shopping:before,.fa-shopping-basket:before{content:"\f291"}.fa-tape:before{content:"\f4db"}.fa-bus-alt:before,.fa-bus-simple:before{content:"\f55e"}.fa-eye:before{content:"\f06e"}.fa-face-sad-cry:before,.fa-sad-cry:before{content:"\f5b3"}.fa-audio-description:before{content:"\f29e"}.fa-person-military-to-person:before{content:"\e54c"}.fa-file-shield:before{content:"\e4f0"}.fa-user-slash:before{content:"\f506"}.fa-pen:before{content:"\f304"}.fa-tower-observation:before{content:"\e586"}.fa-file-code:before{content:"\f1c9"}.fa-signal-5:before,.fa-signal-perfect:before,.fa-signal:before{content:"\f012"}.fa-bus:before{content:"\f207"}.fa-heart-circle-xmark:before{content:"\e501"}.fa-home-lg:before,.fa-house-chimney:before{content:"\e3af"}.fa-window-maximize:before{content:"\f2d0"}.fa-face-frown:before,.fa-frown:before{content:"\f119"}.fa-prescription:before{content:"\f5b1"}.fa-shop:before,.fa-store-alt:before{content:"\f54f"}.fa-floppy-disk:before,.fa-save:before{content:"\f0c7"}.fa-vihara:before{content:"\f6a7"}.fa-balance-scale-left:before,.fa-scale-unbalanced:before{content:"\f515"}.fa-sort-asc:before,.fa-sort-up:before{content:"\f0de"}.fa-comment-dots:before,.fa-commenting:before{content:"\f4ad"}.fa-plant-wilt:before{content:"\e5aa"}.fa-diamond:before{content:"\f219"}.fa-face-grin-squint:before,.fa-grin-squint:before{content:"\f585"}.fa-hand-holding-dollar:before,.fa-hand-holding-usd:before{content:"\f4c0"}.fa-bacterium:before{content:"\e05a"}.fa-hand-pointer:before{content:"\f25a"}.fa-drum-steelpan:before{content:"\f56a"}.fa-hand-scissors:before{content:"\f257"}.fa-hands-praying:before,.fa-praying-hands:before{content:"\f684"}.fa-arrow-right-rotate:before,.fa-arrow-rotate-forward:before,.fa-arrow-rotate-right:before,.fa-redo:before{content:"\f01e"}.fa-biohazard:before{content:"\f780"}.fa-location-crosshairs:before,.fa-location:before{content:"\f601"}.fa-mars-double:before{content:"\f227"}.fa-child-dress:before{content:"\e59c"}.fa-users-between-lines:before{content:"\e591"}.fa-lungs-virus:before{content:"\e067"}.fa-face-grin-tears:before,.fa-grin-tears:before{content:"\f588"}.fa-phone:before{content:"\f095"}.fa-calendar-times:before,.fa-calendar-xmark:before{content:"\f273"}.fa-child-reaching:before{content:"\e59d"}.fa-head-side-virus:before{content:"\e064"}.fa-user-cog:before,.fa-user-gear:before{content:"\f4fe"}.fa-arrow-up-1-9:before,.fa-sort-numeric-up:before{content:"\f163"}.fa-door-closed:before{content:"\f52a"}.fa-shield-virus:before{content:"\e06c"}.fa-dice-six:before{content:"\f526"}.fa-mosquito-net:before{content:"\e52c"}.fa-bridge-water:before{content:"\e4ce"}.fa-person-booth:before{content:"\f756"}.fa-text-width:before{content:"\f035"}.fa-hat-wizard:before{content:"\f6e8"}.fa-pen-fancy:before{content:"\f5ac"}.fa-digging:before,.fa-person-digging:before{content:"\f85e"}.fa-trash:before{content:"\f1f8"}.fa-gauge-simple-med:before,.fa-gauge-simple:before,.fa-tachometer-average:before{content:"\f629"}.fa-book-medical:before{content:"\f7e6"}.fa-poo:before{content:"\f2fe"}.fa-quote-right-alt:before,.fa-quote-right:before{content:"\f10e"}.fa-shirt:before,.fa-t-shirt:before,.fa-tshirt:before{content:"\f553"}.fa-cubes:before{content:"\f1b3"}.fa-divide:before{content:"\f529"}.fa-tenge-sign:before,.fa-tenge:before{content:"\f7d7"}.fa-headphones:before{content:"\f025"}.fa-hands-holding:before{content:"\f4c2"}.fa-hands-clapping:before{content:"\e1a8"}.fa-republican:before{content:"\f75e"}.fa-arrow-left:before{content:"\f060"}.fa-person-circle-xmark:before{content:"\e543"}.fa-ruler:before{content:"\f545"}.fa-align-left:before{content:"\f036"}.fa-dice-d6:before{content:"\f6d1"}.fa-restroom:before{content:"\f7bd"}.fa-j:before{content:"\4a"}.fa-users-viewfinder:before{content:"\e595"}.fa-file-video:before{content:"\f1c8"}.fa-external-link-alt:before,.fa-up-right-from-square:before{content:"\f35d"}.fa-table-cells:before,.fa-th:before{content:"\f00a"}.fa-file-pdf:before{content:"\f1c1"}.fa-bible:before,.fa-book-bible:before{content:"\f647"}.fa-o:before{content:"\4f"}.fa-medkit:before,.fa-suitcase-medical:before{content:"\f0fa"}.fa-user-secret:before{content:"\f21b"}.fa-otter:before{content:"\f700"}.fa-female:before,.fa-person-dress:before{content:"\f182"}.fa-comment-dollar:before{content:"\f651"}.fa-briefcase-clock:before,.fa-business-time:before{content:"\f64a"}.fa-table-cells-large:before,.fa-th-large:before{content:"\f009"}.fa-book-tanakh:before,.fa-tanakh:before{content:"\f827"}.fa-phone-volume:before,.fa-volume-control-phone:before{content:"\f2a0"}.fa-hat-cowboy-side:before{content:"\f8c1"}.fa-clipboard-user:before{content:"\f7f3"}.fa-child:before{content:"\f1ae"}.fa-lira-sign:before{content:"\f195"}.fa-satellite:before{content:"\f7bf"}.fa-plane-lock:before{content:"\e558"}.fa-tag:before{content:"\f02b"}.fa-comment:before{content:"\f075"}.fa-birthday-cake:before,.fa-cake-candles:before,.fa-cake:before{content:"\f1fd"}.fa-envelope:before{content:"\f0e0"}.fa-angle-double-up:before,.fa-angles-up:before{content:"\f102"}.fa-paperclip:before{content:"\f0c6"}.fa-arrow-right-to-city:before{content:"\e4b3"}.fa-ribbon:before{content:"\f4d6"}.fa-lungs:before{content:"\f604"}.fa-arrow-up-9-1:before,.fa-sort-numeric-up-alt:before{content:"\f887"}.fa-litecoin-sign:before{content:"\e1d3"}.fa-border-none:before{content:"\f850"}.fa-circle-nodes:before{content:"\e4e2"}.fa-parachute-box:before{content:"\f4cd"}.fa-indent:before{content:"\f03c"}.fa-truck-field-un:before{content:"\e58e"}.fa-hourglass-empty:before,.fa-hourglass:before{content:"\f254"}.fa-mountain:before{content:"\f6fc"}.fa-user-doctor:before,.fa-user-md:before{content:"\f0f0"}.fa-circle-info:before,.fa-info-circle:before{content:"\f05a"}.fa-cloud-meatball:before{content:"\f73b"}.fa-camera-alt:before,.fa-camera:before{content:"\f030"}.fa-square-virus:before{content:"\e578"}.fa-meteor:before{content:"\f753"}.fa-car-on:before{content:"\e4dd"}.fa-sleigh:before{content:"\f7cc"}.fa-arrow-down-1-9:before,.fa-sort-numeric-asc:before,.fa-sort-numeric-down:before{content:"\f162"}.fa-hand-holding-droplet:before,.fa-hand-holding-water:before{content:"\f4c1"}.fa-water:before{content:"\f773"}.fa-calendar-check:before{content:"\f274"}.fa-braille:before{content:"\f2a1"}.fa-prescription-bottle-alt:before,.fa-prescription-bottle-medical:before{content:"\f486"}.fa-landmark:before{content:"\f66f"}.fa-truck:before{content:"\f0d1"}.fa-crosshairs:before{content:"\f05b"}.fa-person-cane:before{content:"\e53c"}.fa-tent:before{content:"\e57d"}.fa-vest-patches:before{content:"\e086"}.fa-check-double:before{content:"\f560"}.fa-arrow-down-a-z:before,.fa-sort-alpha-asc:before,.fa-sort-alpha-down:before{content:"\f15d"}.fa-money-bill-wheat:before{content:"\e52a"}.fa-cookie:before{content:"\f563"}.fa-arrow-left-rotate:before,.fa-arrow-rotate-back:before,.fa-arrow-rotate-backward:before,.fa-arrow-rotate-left:before,.fa-undo:before{content:"\f0e2"}.fa-hard-drive:before,.fa-hdd:before{content:"\f0a0"}.fa-face-grin-squint-tears:before,.fa-grin-squint-tears:before{content:"\f586"}.fa-dumbbell:before{content:"\f44b"}.fa-list-alt:before,.fa-rectangle-list:before{content:"\f022"}.fa-tarp-droplet:before{content:"\e57c"}.fa-house-medical-circle-check:before{content:"\e511"}.fa-person-skiing-nordic:before,.fa-skiing-nordic:before{content:"\f7ca"}.fa-calendar-plus:before{content:"\f271"}.fa-plane-arrival:before{content:"\f5af"}.fa-arrow-alt-circle-left:before,.fa-circle-left:before{content:"\f359"}.fa-subway:before,.fa-train-subway:before{content:"\f239"}.fa-chart-gantt:before{content:"\e0e4"}.fa-indian-rupee-sign:before,.fa-indian-rupee:before,.fa-inr:before{content:"\e1bc"}.fa-crop-alt:before,.fa-crop-simple:before{content:"\f565"}.fa-money-bill-1:before,.fa-money-bill-alt:before{content:"\f3d1"}.fa-left-long:before,.fa-long-arrow-alt-left:before{content:"\f30a"}.fa-dna:before{content:"\f471"}.fa-virus-slash:before{content:"\e075"}.fa-minus:before,.fa-subtract:before{content:"\f068"}.fa-chess:before{content:"\f439"}.fa-arrow-left-long:before,.fa-long-arrow-left:before{content:"\f177"}.fa-plug-circle-check:before{content:"\e55c"}.fa-street-view:before{content:"\f21d"}.fa-franc-sign:before{content:"\e18f"}.fa-volume-off:before{content:"\f026"}.fa-american-sign-language-interpreting:before,.fa-asl-interpreting:before,.fa-hands-american-sign-language-interpreting:before,.fa-hands-asl-interpreting:before{content:"\f2a3"}.fa-cog:before,.fa-gear:before{content:"\f013"}.fa-droplet-slash:before,.fa-tint-slash:before{content:"\f5c7"}.fa-mosque:before{content:"\f678"}.fa-mosquito:before{content:"\e52b"}.fa-star-of-david:before{content:"\f69a"}.fa-person-military-rifle:before{content:"\e54b"}.fa-cart-shopping:before,.fa-shopping-cart:before{content:"\f07a"}.fa-vials:before{content:"\f493"}.fa-plug-circle-plus:before{content:"\e55f"}.fa-place-of-worship:before{content:"\f67f"}.fa-grip-vertical:before{content:"\f58e"}.fa-arrow-turn-up:before,.fa-level-up:before{content:"\f148"}.fa-u:before{content:"\55"}.fa-square-root-alt:before,.fa-square-root-variable:before{content:"\f698"}.fa-clock-four:before,.fa-clock:before{content:"\f017"}.fa-backward-step:before,.fa-step-backward:before{content:"\f048"}.fa-pallet:before{content:"\f482"}.fa-faucet:before{content:"\e005"}.fa-baseball-bat-ball:before{content:"\f432"}.fa-s:before{content:"\53"}.fa-timeline:before{content:"\e29c"}.fa-keyboard:before{content:"\f11c"}.fa-caret-down:before{content:"\f0d7"}.fa-clinic-medical:before,.fa-house-chimney-medical:before{content:"\f7f2"}.fa-temperature-3:before,.fa-temperature-three-quarters:before,.fa-thermometer-3:before,.fa-thermometer-three-quarters:before{content:"\f2c8"}.fa-mobile-android-alt:before,.fa-mobile-screen:before{content:"\f3cf"}.fa-plane-up:before{content:"\e22d"}.fa-piggy-bank:before{content:"\f4d3"}.fa-battery-3:before,.fa-battery-half:before{content:"\f242"}.fa-mountain-city:before{content:"\e52e"}.fa-coins:before{content:"\f51e"}.fa-khanda:before{content:"\f66d"}.fa-sliders-h:before,.fa-sliders:before{content:"\f1de"}.fa-folder-tree:before{content:"\f802"}.fa-network-wired:before{content:"\f6ff"}.fa-map-pin:before{content:"\f276"}.fa-hamsa:before{content:"\f665"}.fa-cent-sign:before{content:"\e3f5"}.fa-flask:before{content:"\f0c3"}.fa-person-pregnant:before{content:"\e31e"}.fa-wand-sparkles:before{content:"\f72b"}.fa-ellipsis-v:before,.fa-ellipsis-vertical:before{content:"\f142"}.fa-ticket:before{content:"\f145"}.fa-power-off:before{content:"\f011"}.fa-long-arrow-alt-right:before,.fa-right-long:before{content:"\f30b"}.fa-flag-usa:before{content:"\f74d"}.fa-laptop-file:before{content:"\e51d"}.fa-teletype:before,.fa-tty:before{content:"\f1e4"}.fa-diagram-next:before{content:"\e476"}.fa-person-rifle:before{content:"\e54e"}.fa-house-medical-circle-exclamation:before{content:"\e512"}.fa-closed-captioning:before{content:"\f20a"}.fa-hiking:before,.fa-person-hiking:before{content:"\f6ec"}.fa-venus-double:before{content:"\f226"}.fa-images:before{content:"\f302"}.fa-calculator:before{content:"\f1ec"}.fa-people-pulling:before{content:"\e535"}.fa-n:before{content:"\4e"}.fa-cable-car:before,.fa-tram:before{content:"\f7da"}.fa-cloud-rain:before{content:"\f73d"}.fa-building-circle-xmark:before{content:"\e4d4"}.fa-ship:before{content:"\f21a"}.fa-arrows-down-to-line:before{content:"\e4b8"}.fa-download:before{content:"\f019"}.fa-face-grin:before,.fa-grin:before{content:"\f580"}.fa-backspace:before,.fa-delete-left:before{content:"\f55a"}.fa-eye-dropper-empty:before,.fa-eye-dropper:before,.fa-eyedropper:before{content:"\f1fb"}.fa-file-circle-check:before{content:"\e5a0"}.fa-forward:before{content:"\f04e"}.fa-mobile-android:before,.fa-mobile-phone:before,.fa-mobile:before{content:"\f3ce"}.fa-face-meh:before,.fa-meh:before{content:"\f11a"}.fa-align-center:before{content:"\f037"}.fa-book-dead:before,.fa-book-skull:before{content:"\f6b7"}.fa-drivers-license:before,.fa-id-card:before{content:"\f2c2"}.fa-dedent:before,.fa-outdent:before{content:"\f03b"}.fa-heart-circle-exclamation:before{content:"\e4fe"}.fa-home-alt:before,.fa-home-lg-alt:before,.fa-home:before,.fa-house:before{content:"\f015"}.fa-calendar-week:before{content:"\f784"}.fa-laptop-medical:before{content:"\f812"}.fa-b:before{content:"\42"}.fa-file-medical:before{content:"\f477"}.fa-dice-one:before{content:"\f525"}.fa-kiwi-bird:before{content:"\f535"}.fa-arrow-right-arrow-left:before,.fa-exchange:before{content:"\f0ec"}.fa-redo-alt:before,.fa-rotate-forward:before,.fa-rotate-right:before{content:"\f2f9"}.fa-cutlery:before,.fa-utensils:before{content:"\f2e7"}.fa-arrow-up-wide-short:before,.fa-sort-amount-up:before{content:"\f161"}.fa-mill-sign:before{content:"\e1ed"}.fa-bowl-rice:before{content:"\e2eb"}.fa-skull:before{content:"\f54c"}.fa-broadcast-tower:before,.fa-tower-broadcast:before{content:"\f519"}.fa-truck-pickup:before{content:"\f63c"}.fa-long-arrow-alt-up:before,.fa-up-long:before{content:"\f30c"}.fa-stop:before{content:"\f04d"}.fa-code-merge:before{content:"\f387"}.fa-upload:before{content:"\f093"}.fa-hurricane:before{content:"\f751"}.fa-mound:before{content:"\e52d"}.fa-toilet-portable:before{content:"\e583"}.fa-compact-disc:before{content:"\f51f"}.fa-file-arrow-down:before,.fa-file-download:before{content:"\f56d"}.fa-caravan:before{content:"\f8ff"}.fa-shield-cat:before{content:"\e572"}.fa-bolt:before,.fa-zap:before{content:"\f0e7"}.fa-glass-water:before{content:"\e4f4"}.fa-oil-well:before{content:"\e532"}.fa-vault:before{content:"\e2c5"}.fa-mars:before{content:"\f222"}.fa-toilet:before{content:"\f7d8"}.fa-plane-circle-xmark:before{content:"\e557"}.fa-cny:before,.fa-jpy:before,.fa-rmb:before,.fa-yen-sign:before,.fa-yen:before{content:"\f157"}.fa-rouble:before,.fa-rub:before,.fa-ruble-sign:before,.fa-ruble:before{content:"\f158"}.fa-sun:before{content:"\f185"}.fa-guitar:before{content:"\f7a6"}.fa-face-laugh-wink:before,.fa-laugh-wink:before{content:"\f59c"}.fa-horse-head:before{content:"\f7ab"}.fa-bore-hole:before{content:"\e4c3"}.fa-industry:before{content:"\f275"}.fa-arrow-alt-circle-down:before,.fa-circle-down:before{content:"\f358"}.fa-arrows-turn-to-dots:before{content:"\e4c1"}.fa-florin-sign:before{content:"\e184"}.fa-arrow-down-short-wide:before,.fa-sort-amount-desc:before,.fa-sort-amount-down-alt:before{content:"\f884"}.fa-less-than:before{content:"\3c"}.fa-angle-down:before{content:"\f107"}.fa-car-tunnel:before{content:"\e4de"}.fa-head-side-cough:before{content:"\e061"}.fa-grip-lines:before{content:"\f7a4"}.fa-thumbs-down:before{content:"\f165"}.fa-user-lock:before{content:"\f502"}.fa-arrow-right-long:before,.fa-long-arrow-right:before{content:"\f178"}.fa-anchor-circle-xmark:before{content:"\e4ac"}.fa-ellipsis-h:before,.fa-ellipsis:before{content:"\f141"}.fa-chess-pawn:before{content:"\f443"}.fa-first-aid:before,.fa-kit-medical:before{content:"\f479"}.fa-person-through-window:before{content:"\e5a9"}.fa-toolbox:before{content:"\f552"}.fa-hands-holding-circle:before{content:"\e4fb"}.fa-bug:before{content:"\f188"}.fa-credit-card-alt:before,.fa-credit-card:before{content:"\f09d"}.fa-automobile:before,.fa-car:before{content:"\f1b9"}.fa-hand-holding-hand:before{content:"\e4f7"}.fa-book-open-reader:before,.fa-book-reader:before{content:"\f5da"}.fa-mountain-sun:before{content:"\e52f"}.fa-arrows-left-right-to-line:before{content:"\e4ba"}.fa-dice-d20:before{content:"\f6cf"}.fa-truck-droplet:before{content:"\e58c"}.fa-file-circle-xmark:before{content:"\e5a1"}.fa-temperature-arrow-up:before,.fa-temperature-up:before{content:"\e040"}.fa-medal:before{content:"\f5a2"}.fa-bed:before{content:"\f236"}.fa-h-square:before,.fa-square-h:before{content:"\f0fd"}.fa-podcast:before{content:"\f2ce"}.fa-temperature-4:before,.fa-temperature-full:before,.fa-thermometer-4:before,.fa-thermometer-full:before{content:"\f2c7"}.fa-bell:before{content:"\f0f3"}.fa-superscript:before{content:"\f12b"}.fa-plug-circle-xmark:before{content:"\e560"}.fa-star-of-life:before{content:"\f621"}.fa-phone-slash:before{content:"\f3dd"}.fa-paint-roller:before{content:"\f5aa"}.fa-hands-helping:before,.fa-handshake-angle:before{content:"\f4c4"}.fa-location-dot:before,.fa-map-marker-alt:before{content:"\f3c5"}.fa-file:before{content:"\f15b"}.fa-greater-than:before{content:"\3e"}.fa-person-swimming:before,.fa-swimmer:before{content:"\f5c4"}.fa-arrow-down:before{content:"\f063"}.fa-droplet:before,.fa-tint:before{content:"\f043"}.fa-eraser:before{content:"\f12d"}.fa-earth-america:before,.fa-earth-americas:before,.fa-earth:before,.fa-globe-americas:before{content:"\f57d"}.fa-person-burst:before{content:"\e53b"}.fa-dove:before{content:"\f4ba"}.fa-battery-0:before,.fa-battery-empty:before{content:"\f244"}.fa-socks:before{content:"\f696"}.fa-inbox:before{content:"\f01c"}.fa-section:before{content:"\e447"}.fa-gauge-high:before,.fa-tachometer-alt-fast:before,.fa-tachometer-alt:before{content:"\f625"}.fa-envelope-open-text:before{content:"\f658"}.fa-hospital-alt:before,.fa-hospital-wide:before,.fa-hospital:before{content:"\f0f8"}.fa-wine-bottle:before{content:"\f72f"}.fa-chess-rook:before{content:"\f447"}.fa-bars-staggered:before,.fa-reorder:before,.fa-stream:before{content:"\f550"}.fa-dharmachakra:before{content:"\f655"}.fa-hotdog:before{content:"\f80f"}.fa-blind:before,.fa-person-walking-with-cane:before{content:"\f29d"}.fa-drum:before{content:"\f569"}.fa-ice-cream:before{content:"\f810"}.fa-heart-circle-bolt:before{content:"\e4fc"}.fa-fax:before{content:"\f1ac"}.fa-paragraph:before{content:"\f1dd"}.fa-check-to-slot:before,.fa-vote-yea:before{content:"\f772"}.fa-star-half:before{content:"\f089"}.fa-boxes-alt:before,.fa-boxes-stacked:before,.fa-boxes:before{content:"\f468"}.fa-chain:before,.fa-link:before{content:"\f0c1"}.fa-assistive-listening-systems:before,.fa-ear-listen:before{content:"\f2a2"}.fa-tree-city:before{content:"\e587"}.fa-play:before{content:"\f04b"}.fa-font:before{content:"\f031"}.fa-rupiah-sign:before{content:"\e23d"}.fa-magnifying-glass:before,.fa-search:before{content:"\f002"}.fa-ping-pong-paddle-ball:before,.fa-table-tennis-paddle-ball:before,.fa-table-tennis:before{content:"\f45d"}.fa-diagnoses:before,.fa-person-dots-from-line:before{content:"\f470"}.fa-trash-can-arrow-up:before,.fa-trash-restore-alt:before{content:"\f82a"}.fa-naira-sign:before{content:"\e1f6"}.fa-cart-arrow-down:before{content:"\f218"}.fa-walkie-talkie:before{content:"\f8ef"}.fa-file-edit:before,.fa-file-pen:before{content:"\f31c"}.fa-receipt:before{content:"\f543"}.fa-pen-square:before,.fa-pencil-square:before,.fa-square-pen:before{content:"\f14b"}.fa-suitcase-rolling:before{content:"\f5c1"}.fa-person-circle-exclamation:before{content:"\e53f"}.fa-chevron-down:before{content:"\f078"}.fa-battery-5:before,.fa-battery-full:before,.fa-battery:before{content:"\f240"}.fa-skull-crossbones:before{content:"\f714"}.fa-code-compare:before{content:"\e13a"}.fa-list-dots:before,.fa-list-ul:before{content:"\f0ca"}.fa-school-lock:before{content:"\e56f"}.fa-tower-cell:before{content:"\e585"}.fa-down-long:before,.fa-long-arrow-alt-down:before{content:"\f309"}.fa-ranking-star:before{content:"\e561"}.fa-chess-king:before{content:"\f43f"}.fa-person-harassing:before{content:"\e549"}.fa-brazilian-real-sign:before{content:"\e46c"}.fa-landmark-alt:before,.fa-landmark-dome:before{content:"\f752"}.fa-arrow-up:before{content:"\f062"}.fa-television:before,.fa-tv-alt:before,.fa-tv:before{content:"\f26c"}.fa-shrimp:before{content:"\e448"}.fa-list-check:before,.fa-tasks:before{content:"\f0ae"}.fa-jug-detergent:before{content:"\e519"}.fa-circle-user:before,.fa-user-circle:before{content:"\f2bd"}.fa-user-shield:before{content:"\f505"}.fa-wind:before{content:"\f72e"}.fa-car-burst:before,.fa-car-crash:before{content:"\f5e1"}.fa-y:before{content:"\59"}.fa-person-snowboarding:before,.fa-snowboarding:before{content:"\f7ce"}.fa-shipping-fast:before,.fa-truck-fast:before{content:"\f48b"}.fa-fish:before{content:"\f578"}.fa-user-graduate:before{content:"\f501"}.fa-adjust:before,.fa-circle-half-stroke:before{content:"\f042"}.fa-clapperboard:before{content:"\e131"}.fa-circle-radiation:before,.fa-radiation-alt:before{content:"\f7ba"}.fa-baseball-ball:before,.fa-baseball:before{content:"\f433"}.fa-jet-fighter-up:before{content:"\e518"}.fa-diagram-project:before,.fa-project-diagram:before{content:"\f542"}.fa-copy:before{content:"\f0c5"}.fa-volume-mute:before,.fa-volume-times:before,.fa-volume-xmark:before{content:"\f6a9"}.fa-hand-sparkles:before{content:"\e05d"}.fa-grip-horizontal:before,.fa-grip:before{content:"\f58d"}.fa-share-from-square:before,.fa-share-square:before{content:"\f14d"}.fa-child-combatant:before,.fa-child-rifle:before{content:"\e4e0"}.fa-gun:before{content:"\e19b"}.fa-phone-square:before,.fa-square-phone:before{content:"\f098"}.fa-add:before,.fa-plus:before{content:"\2b"}.fa-expand:before{content:"\f065"}.fa-computer:before{content:"\e4e5"}.fa-close:before,.fa-multiply:before,.fa-remove:before,.fa-times:before,.fa-xmark:before{content:"\f00d"}.fa-arrows-up-down-left-right:before,.fa-arrows:before{content:"\f047"}.fa-chalkboard-teacher:before,.fa-chalkboard-user:before{content:"\f51c"}.fa-peso-sign:before{content:"\e222"}.fa-building-shield:before{content:"\e4d8"}.fa-baby:before{content:"\f77c"}.fa-users-line:before{content:"\e592"}.fa-quote-left-alt:before,.fa-quote-left:before{content:"\f10d"}.fa-tractor:before{content:"\f722"}.fa-trash-arrow-up:before,.fa-trash-restore:before{content:"\f829"}.fa-arrow-down-up-lock:before{content:"\e4b0"}.fa-lines-leaning:before{content:"\e51e"}.fa-ruler-combined:before{content:"\f546"}.fa-copyright:before{content:"\f1f9"}.fa-equals:before{content:"\3d"}.fa-blender:before{content:"\f517"}.fa-teeth:before{content:"\f62e"}.fa-ils:before,.fa-shekel-sign:before,.fa-shekel:before,.fa-sheqel-sign:before,.fa-sheqel:before{content:"\f20b"}.fa-map:before{content:"\f279"}.fa-rocket:before{content:"\f135"}.fa-photo-film:before,.fa-photo-video:before{content:"\f87c"}.fa-folder-minus:before{content:"\f65d"}.fa-store:before{content:"\f54e"}.fa-arrow-trend-up:before{content:"\e098"}.fa-plug-circle-minus:before{content:"\e55e"}.fa-sign-hanging:before,.fa-sign:before{content:"\f4d9"}.fa-bezier-curve:before{content:"\f55b"}.fa-bell-slash:before{content:"\f1f6"}.fa-tablet-android:before,.fa-tablet:before{content:"\f3fb"}.fa-school-flag:before{content:"\e56e"}.fa-fill:before{content:"\f575"}.fa-angle-up:before{content:"\f106"}.fa-drumstick-bite:before{content:"\f6d7"}.fa-holly-berry:before{content:"\f7aa"}.fa-chevron-left:before{content:"\f053"}.fa-bacteria:before{content:"\e059"}.fa-hand-lizard:before{content:"\f258"}.fa-notdef:before{content:"\e1fe"}.fa-disease:before{content:"\f7fa"}.fa-briefcase-medical:before{content:"\f469"}.fa-genderless:before{content:"\f22d"}.fa-chevron-right:before{content:"\f054"}.fa-retweet:before{content:"\f079"}.fa-car-alt:before,.fa-car-rear:before{content:"\f5de"}.fa-pump-soap:before{content:"\e06b"}.fa-video-slash:before{content:"\f4e2"}.fa-battery-2:before,.fa-battery-quarter:before{content:"\f243"}.fa-radio:before{content:"\f8d7"}.fa-baby-carriage:before,.fa-carriage-baby:before{content:"\f77d"}.fa-traffic-light:before{content:"\f637"}.fa-thermometer:before{content:"\f491"}.fa-vr-cardboard:before{content:"\f729"}.fa-hand-middle-finger:before{content:"\f806"}.fa-percent:before,.fa-percentage:before{content:"\25"}.fa-truck-moving:before{content:"\f4df"}.fa-glass-water-droplet:before{content:"\e4f5"}.fa-display:before{content:"\e163"}.fa-face-smile:before,.fa-smile:before{content:"\f118"}.fa-thumb-tack:before,.fa-thumbtack:before{content:"\f08d"}.fa-trophy:before{content:"\f091"}.fa-person-praying:before,.fa-pray:before{content:"\f683"}.fa-hammer:before{content:"\f6e3"}.fa-hand-peace:before{content:"\f25b"}.fa-rotate:before,.fa-sync-alt:before{content:"\f2f1"}.fa-spinner:before{content:"\f110"}.fa-robot:before{content:"\f544"}.fa-peace:before{content:"\f67c"}.fa-cogs:before,.fa-gears:before{content:"\f085"}.fa-warehouse:before{content:"\f494"}.fa-arrow-up-right-dots:before{content:"\e4b7"}.fa-splotch:before{content:"\f5bc"}.fa-face-grin-hearts:before,.fa-grin-hearts:before{content:"\f584"}.fa-dice-four:before{content:"\f524"}.fa-sim-card:before{content:"\f7c4"}.fa-transgender-alt:before,.fa-transgender:before{content:"\f225"}.fa-mercury:before{content:"\f223"}.fa-arrow-turn-down:before,.fa-level-down:before{content:"\f149"}.fa-person-falling-burst:before{content:"\e547"}.fa-award:before{content:"\f559"}.fa-ticket-alt:before,.fa-ticket-simple:before{content:"\f3ff"}.fa-building:before{content:"\f1ad"}.fa-angle-double-left:before,.fa-angles-left:before{content:"\f100"}.fa-qrcode:before{content:"\f029"}.fa-clock-rotate-left:before,.fa-history:before{content:"\f1da"}.fa-face-grin-beam-sweat:before,.fa-grin-beam-sweat:before{content:"\f583"}.fa-arrow-right-from-file:before,.fa-file-export:before{content:"\f56e"}.fa-shield-blank:before,.fa-shield:before{content:"\f132"}.fa-arrow-up-short-wide:before,.fa-sort-amount-up-alt:before{content:"\f885"}.fa-house-medical:before{content:"\e3b2"}.fa-golf-ball-tee:before,.fa-golf-ball:before{content:"\f450"}.fa-chevron-circle-left:before,.fa-circle-chevron-left:before{content:"\f137"}.fa-house-chimney-window:before{content:"\e00d"}.fa-pen-nib:before{content:"\f5ad"}.fa-tent-arrow-turn-left:before{content:"\e580"}.fa-tents:before{content:"\e582"}.fa-magic:before,.fa-wand-magic:before{content:"\f0d0"}.fa-dog:before{content:"\f6d3"}.fa-carrot:before{content:"\f787"}.fa-moon:before{content:"\f186"}.fa-wine-glass-alt:before,.fa-wine-glass-empty:before{content:"\f5ce"}.fa-cheese:before{content:"\f7ef"}.fa-yin-yang:before{content:"\f6ad"}.fa-music:before{content:"\f001"}.fa-code-commit:before{content:"\f386"}.fa-temperature-low:before{content:"\f76b"}.fa-biking:before,.fa-person-biking:before{content:"\f84a"}.fa-broom:before{content:"\f51a"}.fa-shield-heart:before{content:"\e574"}.fa-gopuram:before{content:"\f664"}.fa-earth-oceania:before,.fa-globe-oceania:before{content:"\e47b"}.fa-square-xmark:before,.fa-times-square:before,.fa-xmark-square:before{content:"\f2d3"}.fa-hashtag:before{content:"\23"}.fa-expand-alt:before,.fa-up-right-and-down-left-from-center:before{content:"\f424"}.fa-oil-can:before{content:"\f613"}.fa-t:before{content:"\54"}.fa-hippo:before{content:"\f6ed"}.fa-chart-column:before{content:"\e0e3"}.fa-infinity:before{content:"\f534"}.fa-vial-circle-check:before{content:"\e596"}.fa-person-arrow-down-to-line:before{content:"\e538"}.fa-voicemail:before{content:"\f897"}.fa-fan:before{content:"\f863"}.fa-person-walking-luggage:before{content:"\e554"}.fa-arrows-alt-v:before,.fa-up-down:before{content:"\f338"}.fa-cloud-moon-rain:before{content:"\f73c"}.fa-calendar:before{content:"\f133"}.fa-trailer:before{content:"\e041"}.fa-bahai:before,.fa-haykal:before{content:"\f666"}.fa-sd-card:before{content:"\f7c2"}.fa-dragon:before{content:"\f6d5"}.fa-shoe-prints:before{content:"\f54b"}.fa-circle-plus:before,.fa-plus-circle:before{content:"\f055"}.fa-face-grin-tongue-wink:before,.fa-grin-tongue-wink:before{content:"\f58b"}.fa-hand-holding:before{content:"\f4bd"}.fa-plug-circle-exclamation:before{content:"\e55d"}.fa-chain-broken:before,.fa-chain-slash:before,.fa-link-slash:before,.fa-unlink:before{content:"\f127"}.fa-clone:before{content:"\f24d"}.fa-person-walking-arrow-loop-left:before{content:"\e551"}.fa-arrow-up-z-a:before,.fa-sort-alpha-up-alt:before{content:"\f882"}.fa-fire-alt:before,.fa-fire-flame-curved:before{content:"\f7e4"}.fa-tornado:before{content:"\f76f"}.fa-file-circle-plus:before{content:"\e494"}.fa-book-quran:before,.fa-quran:before{content:"\f687"}.fa-anchor:before{content:"\f13d"}.fa-border-all:before{content:"\f84c"}.fa-angry:before,.fa-face-angry:before{content:"\f556"}.fa-cookie-bite:before{content:"\f564"}.fa-arrow-trend-down:before{content:"\e097"}.fa-feed:before,.fa-rss:before{content:"\f09e"}.fa-draw-polygon:before{content:"\f5ee"}.fa-balance-scale:before,.fa-scale-balanced:before{content:"\f24e"}.fa-gauge-simple-high:before,.fa-tachometer-fast:before,.fa-tachometer:before{content:"\f62a"}.fa-shower:before{content:"\f2cc"}.fa-desktop-alt:before,.fa-desktop:before{content:"\f390"}.fa-m:before{content:"\4d"}.fa-table-list:before,.fa-th-list:before{content:"\f00b"}.fa-comment-sms:before,.fa-sms:before{content:"\f7cd"}.fa-book:before{content:"\f02d"}.fa-user-plus:before{content:"\f234"}.fa-check:before{content:"\f00c"}.fa-battery-4:before,.fa-battery-three-quarters:before{content:"\f241"}.fa-house-circle-check:before{content:"\e509"}.fa-angle-left:before{content:"\f104"}.fa-diagram-successor:before{content:"\e47a"}.fa-truck-arrow-right:before{content:"\e58b"}.fa-arrows-split-up-and-left:before{content:"\e4bc"}.fa-fist-raised:before,.fa-hand-fist:before{content:"\f6de"}.fa-cloud-moon:before{content:"\f6c3"}.fa-briefcase:before{content:"\f0b1"}.fa-person-falling:before{content:"\e546"}.fa-image-portrait:before,.fa-portrait:before{content:"\f3e0"}.fa-user-tag:before{content:"\f507"}.fa-rug:before{content:"\e569"}.fa-earth-europe:before,.fa-globe-europe:before{content:"\f7a2"}.fa-cart-flatbed-suitcase:before,.fa-luggage-cart:before{content:"\f59d"}.fa-rectangle-times:before,.fa-rectangle-xmark:before,.fa-times-rectangle:before,.fa-window-close:before{content:"\f410"}.fa-baht-sign:before{content:"\e0ac"}.fa-book-open:before{content:"\f518"}.fa-book-journal-whills:before,.fa-journal-whills:before{content:"\f66a"}.fa-handcuffs:before{content:"\e4f8"}.fa-exclamation-triangle:before,.fa-triangle-exclamation:before,.fa-warning:before{content:"\f071"}.fa-database:before{content:"\f1c0"}.fa-arrow-turn-right:before,.fa-mail-forward:before,.fa-share:before{content:"\f064"}.fa-bottle-droplet:before{content:"\e4c4"}.fa-mask-face:before{content:"\e1d7"}.fa-hill-rockslide:before{content:"\e508"}.fa-exchange-alt:before,.fa-right-left:before{content:"\f362"}.fa-paper-plane:before{content:"\f1d8"}.fa-road-circle-exclamation:before{content:"\e565"}.fa-dungeon:before{content:"\f6d9"}.fa-align-right:before{content:"\f038"}.fa-money-bill-1-wave:before,.fa-money-bill-wave-alt:before{content:"\f53b"}.fa-life-ring:before{content:"\f1cd"}.fa-hands:before,.fa-sign-language:before,.fa-signing:before{content:"\f2a7"}.fa-calendar-day:before{content:"\f783"}.fa-ladder-water:before,.fa-swimming-pool:before,.fa-water-ladder:before{content:"\f5c5"}.fa-arrows-up-down:before,.fa-arrows-v:before{content:"\f07d"}.fa-face-grimace:before,.fa-grimace:before{content:"\f57f"}.fa-wheelchair-alt:before,.fa-wheelchair-move:before{content:"\e2ce"}.fa-level-down-alt:before,.fa-turn-down:before{content:"\f3be"}.fa-person-walking-arrow-right:before{content:"\e552"}.fa-envelope-square:before,.fa-square-envelope:before{content:"\f199"}.fa-dice:before{content:"\f522"}.fa-bowling-ball:before{content:"\f436"}.fa-brain:before{content:"\f5dc"}.fa-band-aid:before,.fa-bandage:before{content:"\f462"}.fa-calendar-minus:before{content:"\f272"}.fa-circle-xmark:before,.fa-times-circle:before,.fa-xmark-circle:before{content:"\f057"}.fa-gifts:before{content:"\f79c"}.fa-hotel:before{content:"\f594"}.fa-earth-asia:before,.fa-globe-asia:before{content:"\f57e"}.fa-id-card-alt:before,.fa-id-card-clip:before{content:"\f47f"}.fa-magnifying-glass-plus:before,.fa-search-plus:before{content:"\f00e"}.fa-thumbs-up:before{content:"\f164"}.fa-user-clock:before{content:"\f4fd"}.fa-allergies:before,.fa-hand-dots:before{content:"\f461"}.fa-file-invoice:before{content:"\f570"}.fa-window-minimize:before{content:"\f2d1"}.fa-coffee:before,.fa-mug-saucer:before{content:"\f0f4"}.fa-brush:before{content:"\f55d"}.fa-mask:before{content:"\f6fa"}.fa-magnifying-glass-minus:before,.fa-search-minus:before{content:"\f010"}.fa-ruler-vertical:before{content:"\f548"}.fa-user-alt:before,.fa-user-large:before{content:"\f406"}.fa-train-tram:before{content:"\e5b4"}.fa-user-nurse:before{content:"\f82f"}.fa-syringe:before{content:"\f48e"}.fa-cloud-sun:before{content:"\f6c4"}.fa-stopwatch-20:before{content:"\e06f"}.fa-square-full:before{content:"\f45c"}.fa-magnet:before{content:"\f076"}.fa-jar:before{content:"\e516"}.fa-note-sticky:before,.fa-sticky-note:before{content:"\f249"}.fa-bug-slash:before{content:"\e490"}.fa-arrow-up-from-water-pump:before{content:"\e4b6"}.fa-bone:before{content:"\f5d7"}.fa-user-injured:before{content:"\f728"}.fa-face-sad-tear:before,.fa-sad-tear:before{content:"\f5b4"}.fa-plane:before{content:"\f072"}.fa-tent-arrows-down:before{content:"\e581"}.fa-exclamation:before{content:"\21"}.fa-arrows-spin:before{content:"\e4bb"}.fa-print:before{content:"\f02f"}.fa-try:before,.fa-turkish-lira-sign:before,.fa-turkish-lira:before{content:"\e2bb"}.fa-dollar-sign:before,.fa-dollar:before,.fa-usd:before{content:"\24"}.fa-x:before{content:"\58"}.fa-magnifying-glass-dollar:before,.fa-search-dollar:before{content:"\f688"}.fa-users-cog:before,.fa-users-gear:before{content:"\f509"}.fa-person-military-pointing:before{content:"\e54a"}.fa-bank:before,.fa-building-columns:before,.fa-institution:before,.fa-museum:before,.fa-university:before{content:"\f19c"}.fa-umbrella:before{content:"\f0e9"}.fa-trowel:before{content:"\e589"}.fa-d:before{content:"\44"}.fa-stapler:before{content:"\e5af"}.fa-masks-theater:before,.fa-theater-masks:before{content:"\f630"}.fa-kip-sign:before{content:"\e1c4"}.fa-hand-point-left:before{content:"\f0a5"}.fa-handshake-alt:before,.fa-handshake-simple:before{content:"\f4c6"}.fa-fighter-jet:before,.fa-jet-fighter:before{content:"\f0fb"}.fa-share-alt-square:before,.fa-square-share-nodes:before{content:"\f1e1"}.fa-barcode:before{content:"\f02a"}.fa-plus-minus:before{content:"\e43c"}.fa-video-camera:before,.fa-video:before{content:"\f03d"}.fa-graduation-cap:before,.fa-mortar-board:before{content:"\f19d"}.fa-hand-holding-medical:before{content:"\e05c"}.fa-person-circle-check:before{content:"\e53e"}.fa-level-up-alt:before,.fa-turn-up:before{content:"\f3bf"}
.fa-sr-only,.fa-sr-only-focusable:not(:focus),.sr-only,.sr-only-focusable:not(:focus){position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border-width:0}:host,:root{--fa-style-family-brands:"Font Awesome 6 Brands";--fa-font-brands:normal 400 1em/1 "Font Awesome 6 Brands"}@font-face{font-family:"Font Awesome 6 Brands";font-style:normal;font-weight:400;font-display:block;src:url(../webfonts/fa-brands-400.woff2) format("woff2"),url(../webfonts/fa-brands-400.ttf) format("truetype")}.fa-brands,.fab{font-weight:400}.fa-monero:before{content:"\f3d0"}.fa-hooli:before{content:"\f427"}.fa-yelp:before{content:"\f1e9"}.fa-cc-visa:before{content:"\f1f0"}.fa-lastfm:before{content:"\f202"}.fa-shopware:before{content:"\f5b5"}.fa-creative-commons-nc:before{content:"\f4e8"}.fa-aws:before{content:"\f375"}.fa-redhat:before{content:"\f7bc"}.fa-yoast:before{content:"\f2b1"}.fa-cloudflare:before{content:"\e07d"}.fa-ups:before{content:"\f7e0"}.fa-wpexplorer:before{content:"\f2de"}.fa-dyalog:before{content:"\f399"}.fa-bity:before{content:"\f37a"}.fa-stackpath:before{content:"\f842"}.fa-buysellads:before{content:"\f20d"}.fa-first-order:before{content:"\f2b0"}.fa-modx:before{content:"\f285"}.fa-guilded:before{content:"\e07e"}.fa-vnv:before{content:"\f40b"}.fa-js-square:before,.fa-square-js:before{content:"\f3b9"}.fa-microsoft:before{content:"\f3ca"}.fa-qq:before{content:"\f1d6"}.fa-orcid:before{content:"\f8d2"}.fa-java:before{content:"\f4e4"}.fa-invision:before{content:"\f7b0"}.fa-creative-commons-pd-alt:before{content:"\f4ed"}.fa-centercode:before{content:"\f380"}.fa-glide-g:before{content:"\f2a6"}.fa-drupal:before{content:"\f1a9"}.fa-hire-a-helper:before{content:"\f3b0"}.fa-creative-commons-by:before{content:"\f4e7"}.fa-unity:before{content:"\e049"}.fa-whmcs:before{content:"\f40d"}.fa-rocketchat:before{content:"\f3e8"}.fa-vk:before{content:"\f189"}.fa-untappd:before{content:"\f405"}.fa-mailchimp:before{content:"\f59e"}.fa-css3-alt:before{content:"\f38b"}.fa-reddit-square:before,.fa-square-reddit:before{content:"\f1a2"}.fa-vimeo-v:before{content:"\f27d"}.fa-contao:before{content:"\f26d"}.fa-square-font-awesome:before{content:"\e5ad"}.fa-deskpro:before{content:"\f38f"}.fa-sistrix:before{content:"\f3ee"}.fa-instagram-square:before,.fa-square-instagram:before{content:"\e055"}.fa-battle-net:before{content:"\f835"}.fa-the-red-yeti:before{content:"\f69d"}.fa-hacker-news-square:before,.fa-square-hacker-news:before{content:"\f3af"}.fa-edge:before{content:"\f282"}.fa-napster:before{content:"\f3d2"}.fa-snapchat-square:before,.fa-square-snapchat:before{content:"\f2ad"}.fa-google-plus-g:before{content:"\f0d5"}.fa-artstation:before{content:"\f77a"}.fa-markdown:before{content:"\f60f"}.fa-sourcetree:before{content:"\f7d3"}.fa-google-plus:before{content:"\f2b3"}.fa-diaspora:before{content:"\f791"}.fa-foursquare:before{content:"\f180"}.fa-stack-overflow:before{content:"\f16c"}.fa-github-alt:before{content:"\f113"}.fa-phoenix-squadron:before{content:"\f511"}.fa-pagelines:before{content:"\f18c"}.fa-algolia:before{content:"\f36c"}.fa-red-river:before{content:"\f3e3"}.fa-creative-commons-sa:before{content:"\f4ef"}.fa-safari:before{content:"\f267"}.fa-google:before{content:"\f1a0"}.fa-font-awesome-alt:before,.fa-square-font-awesome-stroke:before{content:"\f35c"}.fa-atlassian:before{content:"\f77b"}.fa-linkedin-in:before{content:"\f0e1"}.fa-digital-ocean:before{content:"\f391"}.fa-nimblr:before{content:"\f5a8"}.fa-chromecast:before{content:"\f838"}.fa-evernote:before{content:"\f839"}.fa-hacker-news:before{content:"\f1d4"}.fa-creative-commons-sampling:before{content:"\f4f0"}.fa-adversal:before{content:"\f36a"}.fa-creative-commons:before{content:"\f25e"}.fa-watchman-monitoring:before{content:"\e087"}.fa-fonticons:before{content:"\f280"}.fa-weixin:before{content:"\f1d7"}.fa-shirtsinbulk:before{content:"\f214"}.fa-codepen:before{content:"\f1cb"}.fa-git-alt:before{content:"\f841"}.fa-lyft:before{content:"\f3c3"}.fa-rev:before{content:"\f5b2"}.fa-windows:before{content:"\f17a"}.fa-wizards-of-the-coast:before{content:"\f730"}.fa-square-viadeo:before,.fa-viadeo-square:before{content:"\f2aa"}.fa-meetup:before{content:"\f2e0"}.fa-centos:before{content:"\f789"}.fa-adn:before{content:"\f170"}.fa-cloudsmith:before{content:"\f384"}.fa-pied-piper-alt:before{content:"\f1a8"}.fa-dribbble-square:before,.fa-square-dribbble:before{content:"\f397"}.fa-codiepie:before{content:"\f284"}.fa-node:before{content:"\f419"}.fa-mix:before{content:"\f3cb"}.fa-steam:before{content:"\f1b6"}.fa-cc-apple-pay:before{content:"\f416"}.fa-scribd:before{content:"\f28a"}.fa-openid:before{content:"\f19b"}.fa-instalod:before{content:"\e081"}.fa-expeditedssl:before{content:"\f23e"}.fa-sellcast:before{content:"\f2da"}.fa-square-twitter:before,.fa-twitter-square:before{content:"\f081"}.fa-r-project:before{content:"\f4f7"}.fa-delicious:before{content:"\f1a5"}.fa-freebsd:before{content:"\f3a4"}.fa-vuejs:before{content:"\f41f"}.fa-accusoft:before{content:"\f369"}.fa-ioxhost:before{content:"\f208"}.fa-fonticons-fi:before{content:"\f3a2"}.fa-app-store:before{content:"\f36f"}.fa-cc-mastercard:before{content:"\f1f1"}.fa-itunes-note:before{content:"\f3b5"}.fa-golang:before{content:"\e40f"}.fa-kickstarter:before{content:"\f3bb"}.fa-grav:before{content:"\f2d6"}.fa-weibo:before{content:"\f18a"}.fa-uncharted:before{content:"\e084"}.fa-firstdraft:before{content:"\f3a1"}.fa-square-youtube:before,.fa-youtube-square:before{content:"\f431"}.fa-wikipedia-w:before{content:"\f266"}.fa-rendact:before,.fa-wpressr:before{content:"\f3e4"}.fa-angellist:before{content:"\f209"}.fa-galactic-republic:before{content:"\f50c"}.fa-nfc-directional:before{content:"\e530"}.fa-skype:before{content:"\f17e"}.fa-joget:before{content:"\f3b7"}.fa-fedora:before{content:"\f798"}.fa-stripe-s:before{content:"\f42a"}.fa-meta:before{content:"\e49b"}.fa-laravel:before{content:"\f3bd"}.fa-hotjar:before{content:"\f3b1"}.fa-bluetooth-b:before{content:"\f294"}.fa-sticker-mule:before{content:"\f3f7"}.fa-creative-commons-zero:before{content:"\f4f3"}.fa-hips:before{content:"\f452"}.fa-behance:before{content:"\f1b4"}.fa-reddit:before{content:"\f1a1"}.fa-discord:before{content:"\f392"}.fa-chrome:before{content:"\f268"}.fa-app-store-ios:before{content:"\f370"}.fa-cc-discover:before{content:"\f1f2"}.fa-wpbeginner:before{content:"\f297"}.fa-confluence:before{content:"\f78d"}.fa-mdb:before{content:"\f8ca"}.fa-dochub:before{content:"\f394"}.fa-accessible-icon:before{content:"\f368"}.fa-ebay:before{content:"\f4f4"}.fa-amazon:before{content:"\f270"}.fa-unsplash:before{content:"\e07c"}.fa-yarn:before{content:"\f7e3"}.fa-square-steam:before,.fa-steam-square:before{content:"\f1b7"}.fa-500px:before{content:"\f26e"}.fa-square-vimeo:before,.fa-vimeo-square:before{content:"\f194"}.fa-asymmetrik:before{content:"\f372"}.fa-font-awesome-flag:before,.fa-font-awesome-logo-full:before,.fa-font-awesome:before{content:"\f2b4"}.fa-gratipay:before{content:"\f184"}.fa-apple:before{content:"\f179"}.fa-hive:before{content:"\e07f"}.fa-gitkraken:before{content:"\f3a6"}.fa-keybase:before{content:"\f4f5"}.fa-apple-pay:before{content:"\f415"}.fa-padlet:before{content:"\e4a0"}.fa-amazon-pay:before{content:"\f42c"}.fa-github-square:before,.fa-square-github:before{content:"\f092"}.fa-stumbleupon:before{content:"\f1a4"}.fa-fedex:before{content:"\f797"}.fa-phoenix-framework:before{content:"\f3dc"}.fa-shopify:before{content:"\e057"}.fa-neos:before{content:"\f612"}.fa-hackerrank:before{content:"\f5f7"}.fa-researchgate:before{content:"\f4f8"}.fa-swift:before{content:"\f8e1"}.fa-angular:before{content:"\f420"}.fa-speakap:before{content:"\f3f3"}.fa-angrycreative:before{content:"\f36e"}.fa-y-combinator:before{content:"\f23b"}.fa-empire:before{content:"\f1d1"}.fa-envira:before{content:"\f299"}.fa-gitlab-square:before,.fa-square-gitlab:before{content:"\e5ae"}.fa-studiovinari:before{content:"\f3f8"}.fa-pied-piper:before{content:"\f2ae"}.fa-wordpress:before{content:"\f19a"}.fa-product-hunt:before{content:"\f288"}.fa-firefox:before{content:"\f269"}.fa-linode:before{content:"\f2b8"}.fa-goodreads:before{content:"\f3a8"}.fa-odnoklassniki-square:before,.fa-square-odnoklassniki:before{content:"\f264"}.fa-jsfiddle:before{content:"\f1cc"}.fa-sith:before{content:"\f512"}.fa-themeisle:before{content:"\f2b2"}.fa-page4:before{content:"\f3d7"}.fa-hashnode:before{content:"\e499"}.fa-react:before{content:"\f41b"}.fa-cc-paypal:before{content:"\f1f4"}.fa-squarespace:before{content:"\f5be"}.fa-cc-stripe:before{content:"\f1f5"}.fa-creative-commons-share:before{content:"\f4f2"}.fa-bitcoin:before{content:"\f379"}.fa-keycdn:before{content:"\f3ba"}.fa-opera:before{content:"\f26a"}.fa-itch-io:before{content:"\f83a"}.fa-umbraco:before{content:"\f8e8"}.fa-galactic-senate:before{content:"\f50d"}.fa-ubuntu:before{content:"\f7df"}.fa-draft2digital:before{content:"\f396"}.fa-stripe:before{content:"\f429"}.fa-houzz:before{content:"\f27c"}.fa-gg:before{content:"\f260"}.fa-dhl:before{content:"\f790"}.fa-pinterest-square:before,.fa-square-pinterest:before{content:"\f0d3"}.fa-xing:before{content:"\f168"}.fa-blackberry:before{content:"\f37b"}.fa-creative-commons-pd:before{content:"\f4ec"}.fa-playstation:before{content:"\f3df"}.fa-quinscape:before{content:"\f459"}.fa-less:before{content:"\f41d"}.fa-blogger-b:before{content:"\f37d"}.fa-opencart:before{content:"\f23d"}.fa-vine:before{content:"\f1ca"}.fa-paypal:before{content:"\f1ed"}.fa-gitlab:before{content:"\f296"}.fa-typo3:before{content:"\f42b"}.fa-reddit-alien:before{content:"\f281"}.fa-yahoo:before{content:"\f19e"}.fa-dailymotion:before{content:"\e052"}.fa-affiliatetheme:before{content:"\f36b"}.fa-pied-piper-pp:before{content:"\f1a7"}.fa-bootstrap:before{content:"\f836"}.fa-odnoklassniki:before{content:"\f263"}.fa-nfc-symbol:before{content:"\e531"}.fa-ethereum:before{content:"\f42e"}.fa-speaker-deck:before{content:"\f83c"}.fa-creative-commons-nc-eu:before{content:"\f4e9"}.fa-patreon:before{content:"\f3d9"}.fa-avianex:before{content:"\f374"}.fa-ello:before{content:"\f5f1"}.fa-gofore:before{content:"\f3a7"}.fa-bimobject:before{content:"\f378"}.fa-facebook-f:before{content:"\f39e"}.fa-google-plus-square:before,.fa-square-google-plus:before{content:"\f0d4"}.fa-mandalorian:before{content:"\f50f"}.fa-first-order-alt:before{content:"\f50a"}.fa-osi:before{content:"\f41a"}.fa-google-wallet:before{content:"\f1ee"}.fa-d-and-d-beyond:before{content:"\f6ca"}.fa-periscope:before{content:"\f3da"}.fa-fulcrum:before{content:"\f50b"}.fa-cloudscale:before{content:"\f383"}.fa-forumbee:before{content:"\f211"}.fa-mizuni:before{content:"\f3cc"}.fa-schlix:before{content:"\f3ea"}.fa-square-xing:before,.fa-xing-square:before{content:"\f169"}.fa-bandcamp:before{content:"\f2d5"}.fa-wpforms:before{content:"\f298"}.fa-cloudversify:before{content:"\f385"}.fa-usps:before{content:"\f7e1"}.fa-megaport:before{content:"\f5a3"}.fa-magento:before{content:"\f3c4"}.fa-spotify:before{content:"\f1bc"}.fa-optin-monster:before{content:"\f23c"}.fa-fly:before{content:"\f417"}.fa-aviato:before{content:"\f421"}.fa-itunes:before{content:"\f3b4"}.fa-cuttlefish:before{content:"\f38c"}.fa-blogger:before{content:"\f37c"}.fa-flickr:before{content:"\f16e"}.fa-viber:before{content:"\f409"}.fa-soundcloud:before{content:"\f1be"}.fa-digg:before{content:"\f1a6"}.fa-tencent-weibo:before{content:"\f1d5"}.fa-symfony:before{content:"\f83d"}.fa-maxcdn:before{content:"\f136"}.fa-etsy:before{content:"\f2d7"}.fa-facebook-messenger:before{content:"\f39f"}.fa-audible:before{content:"\f373"}.fa-think-peaks:before{content:"\f731"}.fa-bilibili:before{content:"\e3d9"}.fa-erlang:before{content:"\f39d"}.fa-cotton-bureau:before{content:"\f89e"}.fa-dashcube:before{content:"\f210"}.fa-42-group:before,.fa-innosoft:before{content:"\e080"}.fa-stack-exchange:before{content:"\f18d"}.fa-elementor:before{content:"\f430"}.fa-pied-piper-square:before,.fa-square-pied-piper:before{content:"\e01e"}.fa-creative-commons-nd:before{content:"\f4eb"}.fa-palfed:before{content:"\f3d8"}.fa-superpowers:before{content:"\f2dd"}.fa-resolving:before{content:"\f3e7"}.fa-xbox:before{content:"\f412"}.fa-searchengin:before{content:"\f3eb"}.fa-tiktok:before{content:"\e07b"}.fa-facebook-square:before,.fa-square-facebook:before{content:"\f082"}.fa-renren:before{content:"\f18b"}.fa-linux:before{content:"\f17c"}.fa-glide:before{content:"\f2a5"}.fa-linkedin:before{content:"\f08c"}.fa-hubspot:before{content:"\f3b2"}.fa-deploydog:before{content:"\f38e"}.fa-twitch:before{content:"\f1e8"}.fa-ravelry:before{content:"\f2d9"}.fa-mixer:before{content:"\e056"}.fa-lastfm-square:before,.fa-square-lastfm:before{content:"\f203"}.fa-vimeo:before{content:"\f40a"}.fa-mendeley:before{content:"\f7b3"}.fa-uniregistry:before{content:"\f404"}.fa-figma:before{content:"\f799"}.fa-creative-commons-remix:before{content:"\f4ee"}.fa-cc-amazon-pay:before{content:"\f42d"}.fa-dropbox:before{content:"\f16b"}.fa-instagram:before{content:"\f16d"}.fa-cmplid:before{content:"\e360"}.fa-facebook:before{content:"\f09a"}.fa-gripfire:before{content:"\f3ac"}.fa-jedi-order:before{content:"\f50e"}.fa-uikit:before{content:"\f403"}.fa-fort-awesome-alt:before{content:"\f3a3"}.fa-phabricator:before{content:"\f3db"}.fa-ussunnah:before{content:"\f407"}.fa-earlybirds:before{content:"\f39a"}.fa-trade-federation:before{content:"\f513"}.fa-autoprefixer:before{content:"\f41c"}.fa-whatsapp:before{content:"\f232"}.fa-slideshare:before{content:"\f1e7"}.fa-google-play:before{content:"\f3ab"}.fa-viadeo:before{content:"\f2a9"}.fa-line:before{content:"\f3c0"}.fa-google-drive:before{content:"\f3aa"}.fa-servicestack:before{content:"\f3ec"}.fa-simplybuilt:before{content:"\f215"}.fa-bitbucket:before{content:"\f171"}.fa-imdb:before{content:"\f2d8"}.fa-deezer:before{content:"\e077"}.fa-raspberry-pi:before{content:"\f7bb"}.fa-jira:before{content:"\f7b1"}.fa-docker:before{content:"\f395"}.fa-screenpal:before{content:"\e570"}.fa-bluetooth:before{content:"\f293"}.fa-gitter:before{content:"\f426"}.fa-d-and-d:before{content:"\f38d"}.fa-microblog:before{content:"\e01a"}.fa-cc-diners-club:before{content:"\f24c"}.fa-gg-circle:before{content:"\f261"}.fa-pied-piper-hat:before{content:"\f4e5"}.fa-kickstarter-k:before{content:"\f3bc"}.fa-yandex:before{content:"\f413"}.fa-readme:before{content:"\f4d5"}.fa-html5:before{content:"\f13b"}.fa-sellsy:before{content:"\f213"}.fa-sass:before{content:"\f41e"}.fa-wirsindhandwerk:before,.fa-wsh:before{content:"\e2d0"}.fa-buromobelexperte:before{content:"\f37f"}.fa-salesforce:before{content:"\f83b"}.fa-octopus-deploy:before{content:"\e082"}.fa-medapps:before{content:"\f3c6"}.fa-ns8:before{content:"\f3d5"}.fa-pinterest-p:before{content:"\f231"}.fa-apper:before{content:"\f371"}.fa-fort-awesome:before{content:"\f286"}.fa-waze:before{content:"\f83f"}.fa-cc-jcb:before{content:"\f24b"}.fa-snapchat-ghost:before,.fa-snapchat:before{content:"\f2ab"}.fa-fantasy-flight-games:before{content:"\f6dc"}.fa-rust:before{content:"\e07a"}.fa-wix:before{content:"\f5cf"}.fa-behance-square:before,.fa-square-behance:before{content:"\f1b5"}.fa-supple:before{content:"\f3f9"}.fa-rebel:before{content:"\f1d0"}.fa-css3:before{content:"\f13c"}.fa-staylinked:before{content:"\f3f5"}.fa-kaggle:before{content:"\f5fa"}.fa-space-awesome:before{content:"\e5ac"}.fa-deviantart:before{content:"\f1bd"}.fa-cpanel:before{content:"\f388"}.fa-goodreads-g:before{content:"\f3a9"}.fa-git-square:before,.fa-square-git:before{content:"\f1d2"}.fa-square-tumblr:before,.fa-tumblr-square:before{content:"\f174"}.fa-trello:before{content:"\f181"}.fa-creative-commons-nc-jp:before{content:"\f4ea"}.fa-get-pocket:before{content:"\f265"}.fa-perbyte:before{content:"\e083"}.fa-grunt:before{content:"\f3ad"}.fa-weebly:before{content:"\f5cc"}.fa-connectdevelop:before{content:"\f20e"}.fa-leanpub:before{content:"\f212"}.fa-black-tie:before{content:"\f27e"}.fa-themeco:before{content:"\f5c6"}.fa-python:before{content:"\f3e2"}.fa-android:before{content:"\f17b"}.fa-bots:before{content:"\e340"}.fa-free-code-camp:before{content:"\f2c5"}.fa-hornbill:before{content:"\f592"}.fa-js:before{content:"\f3b8"}.fa-ideal:before{content:"\e013"}.fa-git:before{content:"\f1d3"}.fa-dev:before{content:"\f6cc"}.fa-sketch:before{content:"\f7c6"}.fa-yandex-international:before{content:"\f414"}.fa-cc-amex:before{content:"\f1f3"}.fa-uber:before{content:"\f402"}.fa-github:before{content:"\f09b"}.fa-php:before{content:"\f457"}.fa-alipay:before{content:"\f642"}.fa-youtube:before{content:"\f167"}.fa-skyatlas:before{content:"\f216"}.fa-firefox-browser:before{content:"\e007"}.fa-replyd:before{content:"\f3e6"}.fa-suse:before{content:"\f7d6"}.fa-jenkins:before{content:"\f3b6"}.fa-twitter:before{content:"\f099"}.fa-rockrms:before{content:"\f3e9"}.fa-pinterest:before{content:"\f0d2"}.fa-buffer:before{content:"\f837"}.fa-npm:before{content:"\f3d4"}.fa-yammer:before{content:"\f840"}.fa-btc:before{content:"\f15a"}.fa-dribbble:before{content:"\f17d"}.fa-stumbleupon-circle:before{content:"\f1a3"}.fa-internet-explorer:before{content:"\f26b"}.fa-stubber:before{content:"\e5c7"}.fa-telegram-plane:before,.fa-telegram:before{content:"\f2c6"}.fa-old-republic:before{content:"\f510"}.fa-odysee:before{content:"\e5c6"}.fa-square-whatsapp:before,.fa-whatsapp-square:before{content:"\f40c"}.fa-node-js:before{content:"\f3d3"}.fa-edge-legacy:before{content:"\e078"}.fa-slack-hash:before,.fa-slack:before{content:"\f198"}.fa-medrt:before{content:"\f3c8"}.fa-usb:before{content:"\f287"}.fa-tumblr:before{content:"\f173"}.fa-vaadin:before{content:"\f408"}.fa-quora:before{content:"\f2c4"}.fa-reacteurope:before{content:"\f75d"}.fa-medium-m:before,.fa-medium:before{content:"\f23a"}.fa-amilia:before{content:"\f36d"}.fa-mixcloud:before{content:"\f289"}.fa-flipboard:before{content:"\f44d"}.fa-viacoin:before{content:"\f237"}.fa-critical-role:before{content:"\f6c9"}.fa-sitrox:before{content:"\e44a"}.fa-discourse:before{content:"\f393"}.fa-joomla:before{content:"\f1aa"}.fa-mastodon:before{content:"\f4f6"}.fa-airbnb:before{content:"\f834"}.fa-wolf-pack-battalion:before{content:"\f514"}.fa-buy-n-large:before{content:"\f8a6"}.fa-gulp:before{content:"\f3ae"}.fa-creative-commons-sampling-plus:before{content:"\f4f1"}.fa-strava:before{content:"\f428"}.fa-ember:before{content:"\f423"}.fa-canadian-maple-leaf:before{content:"\f785"}.fa-teamspeak:before{content:"\f4f9"}.fa-pushed:before{content:"\f3e1"}.fa-wordpress-simple:before{content:"\f411"}.fa-nutritionix:before{content:"\f3d6"}.fa-wodu:before{content:"\e088"}.fa-google-pay:before{content:"\e079"}.fa-intercom:before{content:"\f7af"}.fa-zhihu:before{content:"\f63f"}.fa-korvue:before{content:"\f42f"}.fa-pix:before{content:"\e43a"}.fa-steam-symbol:before{content:"\f3f6"}:host,:root{--fa-font-regular:normal 400 1em/1 "Font Awesome 6 Free"}@font-face{font-family:"Font Awesome 6 Free";font-style:normal;font-weight:400;font-display:block;src:url(../webfonts/fa-regular-400.woff2) format("woff2"),url(../webfonts/fa-regular-400.ttf) format("truetype")}.fa-regular,.far{font-weight:400}:host,:root{--fa-style-family-classic:"Font Awesome 6 Free";--fa-font-solid:normal 900 1em/1 "Font Awesome 6 Free"}@font-face{font-family:"Font Awesome 6 Free";font-style:normal;font-weight:900;font-display:block;src:url(../webfonts/fa-solid-900.woff2) format("woff2"),url(../webfonts/fa-solid-900.ttf) format("truetype")}.fa-solid,.fas{font-weight:900}@font-face{font-family:"Font Awesome 5 Brands";font-display:block;font-weight:400;src:url(../webfonts/fa-brands-400.woff2) format("woff2"),url(../webfonts/fa-brands-400.ttf) format("truetype")}@font-face{font-family:"Font Awesome 5 Free";font-display:block;font-weight:900;src:url(../webfonts/fa-solid-900.woff2) format("woff2"),url(../webfonts/fa-solid-900.ttf) format("truetype")}@font-face{font-family:"Font Awesome 5 Free";font-display:block;font-weight:400;src:url(../webfonts/fa-regular-400.woff2) format("woff2"),url(../webfonts/fa-regular-400.ttf) format("truetype")}@font-face{font-family:"FontAwesome";font-display:block;src:url(../webfonts/fa-solid-900.woff2) format("woff2"),url(../webfonts/fa-solid-900.ttf) format("truetype")}@font-face{font-family:"FontAwesome";font-display:block;src:url(../webfonts/fa-brands-400.woff2) format("woff2"),url(../webfonts/fa-brands-400.ttf) format("truetype")}@font-face{font-family:"FontAwesome";font-display:block;src:url(../webfonts/fa-regular-400.woff2) format("woff2"),url(../webfonts/fa-regular-400.ttf) format("truetype");unicode-range:u+f003,u+f006,u+f014,u+f016-f017,u+f01a-f01b,u+f01d,u+f022,u+f03e,u+f044,u+f046,u+f05c-f05d,u+f06e,u+f070,u+f087-f088,u+f08a,u+f094,u+f096-f097,u+f09d,u+f0a0,u+f0a2,u+f0a4-f0a7,u+f0c5,u+f0c7,u+f0e5-f0e6,u+f0eb,u+f0f6-f0f8,u+f10c,u+f114-f115,u+f118-f11a,u+f11c-f11d,u+f133,u+f147,u+f14e,u+f150-f152,u+f185-f186,u+f18e,u+f190-f192,u+f196,u+f1c1-f1c9,u+f1d9,u+f1db,u+f1e3,u+f1ea,u+f1f7,u+f1f9,u+f20a,u+f247-f248,u+f24a,u+f24d,u+f255-f25b,u+f25d,u+f271-f274,u+f278,u+f27b,u+f28c,u+f28e,u+f29c,u+f2b5,u+f2b7,u+f2ba,u+f2bc,u+f2be,u+f2c0-f2c1,u+f2c3,u+f2d0,u+f2d2,u+f2d4,u+f2dc}@font-face{font-family:"FontAwesome";font-display:block;src:url(../webfonts/fa-v4compatibility.woff2) format("woff2"),url(../webfonts/fa-v4compatibility.ttf) format("truetype");unicode-range:u+f041,u+f047,u+f065-f066,u+f07d-f07e,u+f080,u+f08b,u+f08e,u+f090,u+f09a,u+f0ac,u+f0ae,u+f0b2,u+f0d0,u+f0d6,u+f0e4,u+f0ec,u+f10a-f10b,u+f123,u+f13e,u+f148-f149,u+f14c,u+f156,u+f15e,u+f160-f161,u+f163,u+f175-f178,u+f195,u+f1f8,u+f219,u+f27a}
```

# source/lib/font-awesome/webfonts/fa-brands-400.ttf

This is a binary file of the type: Binary

# source/lib/font-awesome/webfonts/fa-brands-400.woff2

This is a binary file of the type: Binary

# source/lib/font-awesome/webfonts/fa-regular-400.ttf

This is a binary file of the type: Binary

# source/lib/font-awesome/webfonts/fa-regular-400.woff2

This is a binary file of the type: Binary

# source/lib/font-awesome/webfonts/fa-solid-900.ttf

This is a binary file of the type: Binary

# source/lib/font-awesome/webfonts/fa-solid-900.woff2

This is a binary file of the type: Binary

# source/lib/font-awesome/webfonts/fa-v4compatibility.ttf

This is a binary file of the type: Binary

# source/lib/font-awesome/webfonts/fa-v4compatibility.woff2

This is a binary file of the type: Binary

# source/lib/jquery/jquery.min.js

```js
/*! jQuery v3.6.4 | (c) OpenJS Foundation and other contributors | jquery.org/license */
!function(e,t){"use strict";"object"==typeof module&&"object"==typeof module.exports?module.exports=e.document?t(e,!0):function(e){if(!e.document)throw new Error("jQuery requires a window with a document");return t(e)}:t(e)}("undefined"!=typeof window?window:this,function(C,e){"use strict";var t=[],r=Object.getPrototypeOf,s=t.slice,g=t.flat?function(e){return t.flat.call(e)}:function(e){return t.concat.apply([],e)},u=t.push,i=t.indexOf,n={},o=n.toString,y=n.hasOwnProperty,a=y.toString,l=a.call(Object),v={},m=function(e){return"function"==typeof e&&"number"!=typeof e.nodeType&&"function"!=typeof e.item},x=function(e){return null!=e&&e===e.window},E=C.document,c={type:!0,src:!0,nonce:!0,noModule:!0};function b(e,t,n){var r,i,o=(n=n||E).createElement("script");if(o.text=e,t)for(r in c)(i=t[r]||t.getAttribute&&t.getAttribute(r))&&o.setAttribute(r,i);n.head.appendChild(o).parentNode.removeChild(o)}function w(e){return null==e?e+"":"object"==typeof e||"function"==typeof e?n[o.call(e)]||"object":typeof e}var f="3.6.4",S=function(e,t){return new S.fn.init(e,t)};function p(e){var t=!!e&&"length"in e&&e.length,n=w(e);return!m(e)&&!x(e)&&("array"===n||0===t||"number"==typeof t&&0<t&&t-1 in e)}S.fn=S.prototype={jquery:f,constructor:S,length:0,toArray:function(){return s.call(this)},get:function(e){return null==e?s.call(this):e<0?this[e+this.length]:this[e]},pushStack:function(e){var t=S.merge(this.constructor(),e);return t.prevObject=this,t},each:function(e){return S.each(this,e)},map:function(n){return this.pushStack(S.map(this,function(e,t){return n.call(e,t,e)}))},slice:function(){return this.pushStack(s.apply(this,arguments))},first:function(){return this.eq(0)},last:function(){return this.eq(-1)},even:function(){return this.pushStack(S.grep(this,function(e,t){return(t+1)%2}))},odd:function(){return this.pushStack(S.grep(this,function(e,t){return t%2}))},eq:function(e){var t=this.length,n=+e+(e<0?t:0);return this.pushStack(0<=n&&n<t?[this[n]]:[])},end:function(){return this.prevObject||this.constructor()},push:u,sort:t.sort,splice:t.splice},S.extend=S.fn.extend=function(){var e,t,n,r,i,o,a=arguments[0]||{},s=1,u=arguments.length,l=!1;for("boolean"==typeof a&&(l=a,a=arguments[s]||{},s++),"object"==typeof a||m(a)||(a={}),s===u&&(a=this,s--);s<u;s++)if(null!=(e=arguments[s]))for(t in e)r=e[t],"__proto__"!==t&&a!==r&&(l&&r&&(S.isPlainObject(r)||(i=Array.isArray(r)))?(n=a[t],o=i&&!Array.isArray(n)?[]:i||S.isPlainObject(n)?n:{},i=!1,a[t]=S.extend(l,o,r)):void 0!==r&&(a[t]=r));return a},S.extend({expando:"jQuery"+(f+Math.random()).replace(/\D/g,""),isReady:!0,error:function(e){throw new Error(e)},noop:function(){},isPlainObject:function(e){var t,n;return!(!e||"[object Object]"!==o.call(e))&&(!(t=r(e))||"function"==typeof(n=y.call(t,"constructor")&&t.constructor)&&a.call(n)===l)},isEmptyObject:function(e){var t;for(t in e)return!1;return!0},globalEval:function(e,t,n){b(e,{nonce:t&&t.nonce},n)},each:function(e,t){var n,r=0;if(p(e)){for(n=e.length;r<n;r++)if(!1===t.call(e[r],r,e[r]))break}else for(r in e)if(!1===t.call(e[r],r,e[r]))break;return e},makeArray:function(e,t){var n=t||[];return null!=e&&(p(Object(e))?S.merge(n,"string"==typeof e?[e]:e):u.call(n,e)),n},inArray:function(e,t,n){return null==t?-1:i.call(t,e,n)},merge:function(e,t){for(var n=+t.length,r=0,i=e.length;r<n;r++)e[i++]=t[r];return e.length=i,e},grep:function(e,t,n){for(var r=[],i=0,o=e.length,a=!n;i<o;i++)!t(e[i],i)!==a&&r.push(e[i]);return r},map:function(e,t,n){var r,i,o=0,a=[];if(p(e))for(r=e.length;o<r;o++)null!=(i=t(e[o],o,n))&&a.push(i);else for(o in e)null!=(i=t(e[o],o,n))&&a.push(i);return g(a)},guid:1,support:v}),"function"==typeof Symbol&&(S.fn[Symbol.iterator]=t[Symbol.iterator]),S.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "),function(e,t){n["[object "+t+"]"]=t.toLowerCase()});var d=function(n){var e,d,b,o,i,h,f,g,w,u,l,T,C,a,E,y,s,c,v,S="sizzle"+1*new Date,p=n.document,k=0,r=0,m=ue(),x=ue(),A=ue(),N=ue(),j=function(e,t){return e===t&&(l=!0),0},D={}.hasOwnProperty,t=[],q=t.pop,L=t.push,H=t.push,O=t.slice,P=function(e,t){for(var n=0,r=e.length;n<r;n++)if(e[n]===t)return n;return-1},R="checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",M="[\\x20\\t\\r\\n\\f]",I="(?:\\\\[\\da-fA-F]{1,6}"+M+"?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",W="\\["+M+"*("+I+")(?:"+M+"*([*^$|!~]?=)"+M+"*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|("+I+"))|)"+M+"*\\]",F=":("+I+")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|"+W+")*)|.*)\\)|)",$=new RegExp(M+"+","g"),B=new RegExp("^"+M+"+|((?:^|[^\\\\])(?:\\\\.)*)"+M+"+$","g"),_=new RegExp("^"+M+"*,"+M+"*"),z=new RegExp("^"+M+"*([>+~]|"+M+")"+M+"*"),U=new RegExp(M+"|>"),X=new RegExp(F),V=new RegExp("^"+I+"$"),G={ID:new RegExp("^#("+I+")"),CLASS:new RegExp("^\\.("+I+")"),TAG:new RegExp("^("+I+"|[*])"),ATTR:new RegExp("^"+W),PSEUDO:new RegExp("^"+F),CHILD:new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\("+M+"*(even|odd|(([+-]|)(\\d*)n|)"+M+"*(?:([+-]|)"+M+"*(\\d+)|))"+M+"*\\)|)","i"),bool:new RegExp("^(?:"+R+")$","i"),needsContext:new RegExp("^"+M+"*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\("+M+"*((?:-\\d)?\\d*)"+M+"*\\)|)(?=[^-]|$)","i")},Y=/HTML$/i,Q=/^(?:input|select|textarea|button)$/i,J=/^h\d$/i,K=/^[^{]+\{\s*\[native \w/,Z=/^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,ee=/[+~]/,te=new RegExp("\\\\[\\da-fA-F]{1,6}"+M+"?|\\\\([^\\r\\n\\f])","g"),ne=function(e,t){var n="0x"+e.slice(1)-65536;return t||(n<0?String.fromCharCode(n+65536):String.fromCharCode(n>>10|55296,1023&n|56320))},re=/([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,ie=function(e,t){return t?"\0"===e?"\ufffd":e.slice(0,-1)+"\\"+e.charCodeAt(e.length-1).toString(16)+" ":"\\"+e},oe=function(){T()},ae=be(function(e){return!0===e.disabled&&"fieldset"===e.nodeName.toLowerCase()},{dir:"parentNode",next:"legend"});try{H.apply(t=O.call(p.childNodes),p.childNodes),t[p.childNodes.length].nodeType}catch(e){H={apply:t.length?function(e,t){L.apply(e,O.call(t))}:function(e,t){var n=e.length,r=0;while(e[n++]=t[r++]);e.length=n-1}}}function se(t,e,n,r){var i,o,a,s,u,l,c,f=e&&e.ownerDocument,p=e?e.nodeType:9;if(n=n||[],"string"!=typeof t||!t||1!==p&&9!==p&&11!==p)return n;if(!r&&(T(e),e=e||C,E)){if(11!==p&&(u=Z.exec(t)))if(i=u[1]){if(9===p){if(!(a=e.getElementById(i)))return n;if(a.id===i)return n.push(a),n}else if(f&&(a=f.getElementById(i))&&v(e,a)&&a.id===i)return n.push(a),n}else{if(u[2])return H.apply(n,e.getElementsByTagName(t)),n;if((i=u[3])&&d.getElementsByClassName&&e.getElementsByClassName)return H.apply(n,e.getElementsByClassName(i)),n}if(d.qsa&&!N[t+" "]&&(!y||!y.test(t))&&(1!==p||"object"!==e.nodeName.toLowerCase())){if(c=t,f=e,1===p&&(U.test(t)||z.test(t))){(f=ee.test(t)&&ve(e.parentNode)||e)===e&&d.scope||((s=e.getAttribute("id"))?s=s.replace(re,ie):e.setAttribute("id",s=S)),o=(l=h(t)).length;while(o--)l[o]=(s?"#"+s:":scope")+" "+xe(l[o]);c=l.join(",")}try{return H.apply(n,f.querySelectorAll(c)),n}catch(e){N(t,!0)}finally{s===S&&e.removeAttribute("id")}}}return g(t.replace(B,"$1"),e,n,r)}function ue(){var r=[];return function e(t,n){return r.push(t+" ")>b.cacheLength&&delete e[r.shift()],e[t+" "]=n}}function le(e){return e[S]=!0,e}function ce(e){var t=C.createElement("fieldset");try{return!!e(t)}catch(e){return!1}finally{t.parentNode&&t.parentNode.removeChild(t),t=null}}function fe(e,t){var n=e.split("|"),r=n.length;while(r--)b.attrHandle[n[r]]=t}function pe(e,t){var n=t&&e,r=n&&1===e.nodeType&&1===t.nodeType&&e.sourceIndex-t.sourceIndex;if(r)return r;if(n)while(n=n.nextSibling)if(n===t)return-1;return e?1:-1}function de(t){return function(e){return"input"===e.nodeName.toLowerCase()&&e.type===t}}function he(n){return function(e){var t=e.nodeName.toLowerCase();return("input"===t||"button"===t)&&e.type===n}}function ge(t){return function(e){return"form"in e?e.parentNode&&!1===e.disabled?"label"in e?"label"in e.parentNode?e.parentNode.disabled===t:e.disabled===t:e.isDisabled===t||e.isDisabled!==!t&&ae(e)===t:e.disabled===t:"label"in e&&e.disabled===t}}function ye(a){return le(function(o){return o=+o,le(function(e,t){var n,r=a([],e.length,o),i=r.length;while(i--)e[n=r[i]]&&(e[n]=!(t[n]=e[n]))})})}function ve(e){return e&&"undefined"!=typeof e.getElementsByTagName&&e}for(e in d=se.support={},i=se.isXML=function(e){var t=e&&e.namespaceURI,n=e&&(e.ownerDocument||e).documentElement;return!Y.test(t||n&&n.nodeName||"HTML")},T=se.setDocument=function(e){var t,n,r=e?e.ownerDocument||e:p;return r!=C&&9===r.nodeType&&r.documentElement&&(a=(C=r).documentElement,E=!i(C),p!=C&&(n=C.defaultView)&&n.top!==n&&(n.addEventListener?n.addEventListener("unload",oe,!1):n.attachEvent&&n.attachEvent("onunload",oe)),d.scope=ce(function(e){return a.appendChild(e).appendChild(C.createElement("div")),"undefined"!=typeof e.querySelectorAll&&!e.querySelectorAll(":scope fieldset div").length}),d.cssHas=ce(function(){try{return C.querySelector(":has(*,:jqfake)"),!1}catch(e){return!0}}),d.attributes=ce(function(e){return e.className="i",!e.getAttribute("className")}),d.getElementsByTagName=ce(function(e){return e.appendChild(C.createComment("")),!e.getElementsByTagName("*").length}),d.getElementsByClassName=K.test(C.getElementsByClassName),d.getById=ce(function(e){return a.appendChild(e).id=S,!C.getElementsByName||!C.getElementsByName(S).length}),d.getById?(b.filter.ID=function(e){var t=e.replace(te,ne);return function(e){return e.getAttribute("id")===t}},b.find.ID=function(e,t){if("undefined"!=typeof t.getElementById&&E){var n=t.getElementById(e);return n?[n]:[]}}):(b.filter.ID=function(e){var n=e.replace(te,ne);return function(e){var t="undefined"!=typeof e.getAttributeNode&&e.getAttributeNode("id");return t&&t.value===n}},b.find.ID=function(e,t){if("undefined"!=typeof t.getElementById&&E){var n,r,i,o=t.getElementById(e);if(o){if((n=o.getAttributeNode("id"))&&n.value===e)return[o];i=t.getElementsByName(e),r=0;while(o=i[r++])if((n=o.getAttributeNode("id"))&&n.value===e)return[o]}return[]}}),b.find.TAG=d.getElementsByTagName?function(e,t){return"undefined"!=typeof t.getElementsByTagName?t.getElementsByTagName(e):d.qsa?t.querySelectorAll(e):void 0}:function(e,t){var n,r=[],i=0,o=t.getElementsByTagName(e);if("*"===e){while(n=o[i++])1===n.nodeType&&r.push(n);return r}return o},b.find.CLASS=d.getElementsByClassName&&function(e,t){if("undefined"!=typeof t.getElementsByClassName&&E)return t.getElementsByClassName(e)},s=[],y=[],(d.qsa=K.test(C.querySelectorAll))&&(ce(function(e){var t;a.appendChild(e).innerHTML="<a id='"+S+"'></a><select id='"+S+"-\r\\' msallowcapture=''><option selected=''></option></select>",e.querySelectorAll("[msallowcapture^='']").length&&y.push("[*^$]="+M+"*(?:''|\"\")"),e.querySelectorAll("[selected]").length||y.push("\\["+M+"*(?:value|"+R+")"),e.querySelectorAll("[id~="+S+"-]").length||y.push("~="),(t=C.createElement("input")).setAttribute("name",""),e.appendChild(t),e.querySelectorAll("[name='']").length||y.push("\\["+M+"*name"+M+"*="+M+"*(?:''|\"\")"),e.querySelectorAll(":checked").length||y.push(":checked"),e.querySelectorAll("a#"+S+"+*").length||y.push(".#.+[+~]"),e.querySelectorAll("\\\f"),y.push("[\\r\\n\\f]")}),ce(function(e){e.innerHTML="<a href='' disabled='disabled'></a><select disabled='disabled'><option/></select>";var t=C.createElement("input");t.setAttribute("type","hidden"),e.appendChild(t).setAttribute("name","D"),e.querySelectorAll("[name=d]").length&&y.push("name"+M+"*[*^$|!~]?="),2!==e.querySelectorAll(":enabled").length&&y.push(":enabled",":disabled"),a.appendChild(e).disabled=!0,2!==e.querySelectorAll(":disabled").length&&y.push(":enabled",":disabled"),e.querySelectorAll("*,:x"),y.push(",.*:")})),(d.matchesSelector=K.test(c=a.matches||a.webkitMatchesSelector||a.mozMatchesSelector||a.oMatchesSelector||a.msMatchesSelector))&&ce(function(e){d.disconnectedMatch=c.call(e,"*"),c.call(e,"[s!='']:x"),s.push("!=",F)}),d.cssHas||y.push(":has"),y=y.length&&new RegExp(y.join("|")),s=s.length&&new RegExp(s.join("|")),t=K.test(a.compareDocumentPosition),v=t||K.test(a.contains)?function(e,t){var n=9===e.nodeType&&e.documentElement||e,r=t&&t.parentNode;return e===r||!(!r||1!==r.nodeType||!(n.contains?n.contains(r):e.compareDocumentPosition&&16&e.compareDocumentPosition(r)))}:function(e,t){if(t)while(t=t.parentNode)if(t===e)return!0;return!1},j=t?function(e,t){if(e===t)return l=!0,0;var n=!e.compareDocumentPosition-!t.compareDocumentPosition;return n||(1&(n=(e.ownerDocument||e)==(t.ownerDocument||t)?e.compareDocumentPosition(t):1)||!d.sortDetached&&t.compareDocumentPosition(e)===n?e==C||e.ownerDocument==p&&v(p,e)?-1:t==C||t.ownerDocument==p&&v(p,t)?1:u?P(u,e)-P(u,t):0:4&n?-1:1)}:function(e,t){if(e===t)return l=!0,0;var n,r=0,i=e.parentNode,o=t.parentNode,a=[e],s=[t];if(!i||!o)return e==C?-1:t==C?1:i?-1:o?1:u?P(u,e)-P(u,t):0;if(i===o)return pe(e,t);n=e;while(n=n.parentNode)a.unshift(n);n=t;while(n=n.parentNode)s.unshift(n);while(a[r]===s[r])r++;return r?pe(a[r],s[r]):a[r]==p?-1:s[r]==p?1:0}),C},se.matches=function(e,t){return se(e,null,null,t)},se.matchesSelector=function(e,t){if(T(e),d.matchesSelector&&E&&!N[t+" "]&&(!s||!s.test(t))&&(!y||!y.test(t)))try{var n=c.call(e,t);if(n||d.disconnectedMatch||e.document&&11!==e.document.nodeType)return n}catch(e){N(t,!0)}return 0<se(t,C,null,[e]).length},se.contains=function(e,t){return(e.ownerDocument||e)!=C&&T(e),v(e,t)},se.attr=function(e,t){(e.ownerDocument||e)!=C&&T(e);var n=b.attrHandle[t.toLowerCase()],r=n&&D.call(b.attrHandle,t.toLowerCase())?n(e,t,!E):void 0;return void 0!==r?r:d.attributes||!E?e.getAttribute(t):(r=e.getAttributeNode(t))&&r.specified?r.value:null},se.escape=function(e){return(e+"").replace(re,ie)},se.error=function(e){throw new Error("Syntax error, unrecognized expression: "+e)},se.uniqueSort=function(e){var t,n=[],r=0,i=0;if(l=!d.detectDuplicates,u=!d.sortStable&&e.slice(0),e.sort(j),l){while(t=e[i++])t===e[i]&&(r=n.push(i));while(r--)e.splice(n[r],1)}return u=null,e},o=se.getText=function(e){var t,n="",r=0,i=e.nodeType;if(i){if(1===i||9===i||11===i){if("string"==typeof e.textContent)return e.textContent;for(e=e.firstChild;e;e=e.nextSibling)n+=o(e)}else if(3===i||4===i)return e.nodeValue}else while(t=e[r++])n+=o(t);return n},(b=se.selectors={cacheLength:50,createPseudo:le,match:G,attrHandle:{},find:{},relative:{">":{dir:"parentNode",first:!0}," ":{dir:"parentNode"},"+":{dir:"previousSibling",first:!0},"~":{dir:"previousSibling"}},preFilter:{ATTR:function(e){return e[1]=e[1].replace(te,ne),e[3]=(e[3]||e[4]||e[5]||"").replace(te,ne),"~="===e[2]&&(e[3]=" "+e[3]+" "),e.slice(0,4)},CHILD:function(e){return e[1]=e[1].toLowerCase(),"nth"===e[1].slice(0,3)?(e[3]||se.error(e[0]),e[4]=+(e[4]?e[5]+(e[6]||1):2*("even"===e[3]||"odd"===e[3])),e[5]=+(e[7]+e[8]||"odd"===e[3])):e[3]&&se.error(e[0]),e},PSEUDO:function(e){var t,n=!e[6]&&e[2];return G.CHILD.test(e[0])?null:(e[3]?e[2]=e[4]||e[5]||"":n&&X.test(n)&&(t=h(n,!0))&&(t=n.indexOf(")",n.length-t)-n.length)&&(e[0]=e[0].slice(0,t),e[2]=n.slice(0,t)),e.slice(0,3))}},filter:{TAG:function(e){var t=e.replace(te,ne).toLowerCase();return"*"===e?function(){return!0}:function(e){return e.nodeName&&e.nodeName.toLowerCase()===t}},CLASS:function(e){var t=m[e+" "];return t||(t=new RegExp("(^|"+M+")"+e+"("+M+"|$)"))&&m(e,function(e){return t.test("string"==typeof e.className&&e.className||"undefined"!=typeof e.getAttribute&&e.getAttribute("class")||"")})},ATTR:function(n,r,i){return function(e){var t=se.attr(e,n);return null==t?"!="===r:!r||(t+="","="===r?t===i:"!="===r?t!==i:"^="===r?i&&0===t.indexOf(i):"*="===r?i&&-1<t.indexOf(i):"$="===r?i&&t.slice(-i.length)===i:"~="===r?-1<(" "+t.replace($," ")+" ").indexOf(i):"|="===r&&(t===i||t.slice(0,i.length+1)===i+"-"))}},CHILD:function(h,e,t,g,y){var v="nth"!==h.slice(0,3),m="last"!==h.slice(-4),x="of-type"===e;return 1===g&&0===y?function(e){return!!e.parentNode}:function(e,t,n){var r,i,o,a,s,u,l=v!==m?"nextSibling":"previousSibling",c=e.parentNode,f=x&&e.nodeName.toLowerCase(),p=!n&&!x,d=!1;if(c){if(v){while(l){a=e;while(a=a[l])if(x?a.nodeName.toLowerCase()===f:1===a.nodeType)return!1;u=l="only"===h&&!u&&"nextSibling"}return!0}if(u=[m?c.firstChild:c.lastChild],m&&p){d=(s=(r=(i=(o=(a=c)[S]||(a[S]={}))[a.uniqueID]||(o[a.uniqueID]={}))[h]||[])[0]===k&&r[1])&&r[2],a=s&&c.childNodes[s];while(a=++s&&a&&a[l]||(d=s=0)||u.pop())if(1===a.nodeType&&++d&&a===e){i[h]=[k,s,d];break}}else if(p&&(d=s=(r=(i=(o=(a=e)[S]||(a[S]={}))[a.uniqueID]||(o[a.uniqueID]={}))[h]||[])[0]===k&&r[1]),!1===d)while(a=++s&&a&&a[l]||(d=s=0)||u.pop())if((x?a.nodeName.toLowerCase()===f:1===a.nodeType)&&++d&&(p&&((i=(o=a[S]||(a[S]={}))[a.uniqueID]||(o[a.uniqueID]={}))[h]=[k,d]),a===e))break;return(d-=y)===g||d%g==0&&0<=d/g}}},PSEUDO:function(e,o){var t,a=b.pseudos[e]||b.setFilters[e.toLowerCase()]||se.error("unsupported pseudo: "+e);return a[S]?a(o):1<a.length?(t=[e,e,"",o],b.setFilters.hasOwnProperty(e.toLowerCase())?le(function(e,t){var n,r=a(e,o),i=r.length;while(i--)e[n=P(e,r[i])]=!(t[n]=r[i])}):function(e){return a(e,0,t)}):a}},pseudos:{not:le(function(e){var r=[],i=[],s=f(e.replace(B,"$1"));return s[S]?le(function(e,t,n,r){var i,o=s(e,null,r,[]),a=e.length;while(a--)(i=o[a])&&(e[a]=!(t[a]=i))}):function(e,t,n){return r[0]=e,s(r,null,n,i),r[0]=null,!i.pop()}}),has:le(function(t){return function(e){return 0<se(t,e).length}}),contains:le(function(t){return t=t.replace(te,ne),function(e){return-1<(e.textContent||o(e)).indexOf(t)}}),lang:le(function(n){return V.test(n||"")||se.error("unsupported lang: "+n),n=n.replace(te,ne).toLowerCase(),function(e){var t;do{if(t=E?e.lang:e.getAttribute("xml:lang")||e.getAttribute("lang"))return(t=t.toLowerCase())===n||0===t.indexOf(n+"-")}while((e=e.parentNode)&&1===e.nodeType);return!1}}),target:function(e){var t=n.location&&n.location.hash;return t&&t.slice(1)===e.id},root:function(e){return e===a},focus:function(e){return e===C.activeElement&&(!C.hasFocus||C.hasFocus())&&!!(e.type||e.href||~e.tabIndex)},enabled:ge(!1),disabled:ge(!0),checked:function(e){var t=e.nodeName.toLowerCase();return"input"===t&&!!e.checked||"option"===t&&!!e.selected},selected:function(e){return e.parentNode&&e.parentNode.selectedIndex,!0===e.selected},empty:function(e){for(e=e.firstChild;e;e=e.nextSibling)if(e.nodeType<6)return!1;return!0},parent:function(e){return!b.pseudos.empty(e)},header:function(e){return J.test(e.nodeName)},input:function(e){return Q.test(e.nodeName)},button:function(e){var t=e.nodeName.toLowerCase();return"input"===t&&"button"===e.type||"button"===t},text:function(e){var t;return"input"===e.nodeName.toLowerCase()&&"text"===e.type&&(null==(t=e.getAttribute("type"))||"text"===t.toLowerCase())},first:ye(function(){return[0]}),last:ye(function(e,t){return[t-1]}),eq:ye(function(e,t,n){return[n<0?n+t:n]}),even:ye(function(e,t){for(var n=0;n<t;n+=2)e.push(n);return e}),odd:ye(function(e,t){for(var n=1;n<t;n+=2)e.push(n);return e}),lt:ye(function(e,t,n){for(var r=n<0?n+t:t<n?t:n;0<=--r;)e.push(r);return e}),gt:ye(function(e,t,n){for(var r=n<0?n+t:n;++r<t;)e.push(r);return e})}}).pseudos.nth=b.pseudos.eq,{radio:!0,checkbox:!0,file:!0,password:!0,image:!0})b.pseudos[e]=de(e);for(e in{submit:!0,reset:!0})b.pseudos[e]=he(e);function me(){}function xe(e){for(var t=0,n=e.length,r="";t<n;t++)r+=e[t].value;return r}function be(s,e,t){var u=e.dir,l=e.next,c=l||u,f=t&&"parentNode"===c,p=r++;return e.first?function(e,t,n){while(e=e[u])if(1===e.nodeType||f)return s(e,t,n);return!1}:function(e,t,n){var r,i,o,a=[k,p];if(n){while(e=e[u])if((1===e.nodeType||f)&&s(e,t,n))return!0}else while(e=e[u])if(1===e.nodeType||f)if(i=(o=e[S]||(e[S]={}))[e.uniqueID]||(o[e.uniqueID]={}),l&&l===e.nodeName.toLowerCase())e=e[u]||e;else{if((r=i[c])&&r[0]===k&&r[1]===p)return a[2]=r[2];if((i[c]=a)[2]=s(e,t,n))return!0}return!1}}function we(i){return 1<i.length?function(e,t,n){var r=i.length;while(r--)if(!i[r](e,t,n))return!1;return!0}:i[0]}function Te(e,t,n,r,i){for(var o,a=[],s=0,u=e.length,l=null!=t;s<u;s++)(o=e[s])&&(n&&!n(o,r,i)||(a.push(o),l&&t.push(s)));return a}function Ce(d,h,g,y,v,e){return y&&!y[S]&&(y=Ce(y)),v&&!v[S]&&(v=Ce(v,e)),le(function(e,t,n,r){var i,o,a,s=[],u=[],l=t.length,c=e||function(e,t,n){for(var r=0,i=t.length;r<i;r++)se(e,t[r],n);return n}(h||"*",n.nodeType?[n]:n,[]),f=!d||!e&&h?c:Te(c,s,d,n,r),p=g?v||(e?d:l||y)?[]:t:f;if(g&&g(f,p,n,r),y){i=Te(p,u),y(i,[],n,r),o=i.length;while(o--)(a=i[o])&&(p[u[o]]=!(f[u[o]]=a))}if(e){if(v||d){if(v){i=[],o=p.length;while(o--)(a=p[o])&&i.push(f[o]=a);v(null,p=[],i,r)}o=p.length;while(o--)(a=p[o])&&-1<(i=v?P(e,a):s[o])&&(e[i]=!(t[i]=a))}}else p=Te(p===t?p.splice(l,p.length):p),v?v(null,t,p,r):H.apply(t,p)})}function Ee(e){for(var i,t,n,r=e.length,o=b.relative[e[0].type],a=o||b.relative[" "],s=o?1:0,u=be(function(e){return e===i},a,!0),l=be(function(e){return-1<P(i,e)},a,!0),c=[function(e,t,n){var r=!o&&(n||t!==w)||((i=t).nodeType?u(e,t,n):l(e,t,n));return i=null,r}];s<r;s++)if(t=b.relative[e[s].type])c=[be(we(c),t)];else{if((t=b.filter[e[s].type].apply(null,e[s].matches))[S]){for(n=++s;n<r;n++)if(b.relative[e[n].type])break;return Ce(1<s&&we(c),1<s&&xe(e.slice(0,s-1).concat({value:" "===e[s-2].type?"*":""})).replace(B,"$1"),t,s<n&&Ee(e.slice(s,n)),n<r&&Ee(e=e.slice(n)),n<r&&xe(e))}c.push(t)}return we(c)}return me.prototype=b.filters=b.pseudos,b.setFilters=new me,h=se.tokenize=function(e,t){var n,r,i,o,a,s,u,l=x[e+" "];if(l)return t?0:l.slice(0);a=e,s=[],u=b.preFilter;while(a){for(o in n&&!(r=_.exec(a))||(r&&(a=a.slice(r[0].length)||a),s.push(i=[])),n=!1,(r=z.exec(a))&&(n=r.shift(),i.push({value:n,type:r[0].replace(B," ")}),a=a.slice(n.length)),b.filter)!(r=G[o].exec(a))||u[o]&&!(r=u[o](r))||(n=r.shift(),i.push({value:n,type:o,matches:r}),a=a.slice(n.length));if(!n)break}return t?a.length:a?se.error(e):x(e,s).slice(0)},f=se.compile=function(e,t){var n,y,v,m,x,r,i=[],o=[],a=A[e+" "];if(!a){t||(t=h(e)),n=t.length;while(n--)(a=Ee(t[n]))[S]?i.push(a):o.push(a);(a=A(e,(y=o,m=0<(v=i).length,x=0<y.length,r=function(e,t,n,r,i){var o,a,s,u=0,l="0",c=e&&[],f=[],p=w,d=e||x&&b.find.TAG("*",i),h=k+=null==p?1:Math.random()||.1,g=d.length;for(i&&(w=t==C||t||i);l!==g&&null!=(o=d[l]);l++){if(x&&o){a=0,t||o.ownerDocument==C||(T(o),n=!E);while(s=y[a++])if(s(o,t||C,n)){r.push(o);break}i&&(k=h)}m&&((o=!s&&o)&&u--,e&&c.push(o))}if(u+=l,m&&l!==u){a=0;while(s=v[a++])s(c,f,t,n);if(e){if(0<u)while(l--)c[l]||f[l]||(f[l]=q.call(r));f=Te(f)}H.apply(r,f),i&&!e&&0<f.length&&1<u+v.length&&se.uniqueSort(r)}return i&&(k=h,w=p),c},m?le(r):r))).selector=e}return a},g=se.select=function(e,t,n,r){var i,o,a,s,u,l="function"==typeof e&&e,c=!r&&h(e=l.selector||e);if(n=n||[],1===c.length){if(2<(o=c[0]=c[0].slice(0)).length&&"ID"===(a=o[0]).type&&9===t.nodeType&&E&&b.relative[o[1].type]){if(!(t=(b.find.ID(a.matches[0].replace(te,ne),t)||[])[0]))return n;l&&(t=t.parentNode),e=e.slice(o.shift().value.length)}i=G.needsContext.test(e)?0:o.length;while(i--){if(a=o[i],b.relative[s=a.type])break;if((u=b.find[s])&&(r=u(a.matches[0].replace(te,ne),ee.test(o[0].type)&&ve(t.parentNode)||t))){if(o.splice(i,1),!(e=r.length&&xe(o)))return H.apply(n,r),n;break}}}return(l||f(e,c))(r,t,!E,n,!t||ee.test(e)&&ve(t.parentNode)||t),n},d.sortStable=S.split("").sort(j).join("")===S,d.detectDuplicates=!!l,T(),d.sortDetached=ce(function(e){return 1&e.compareDocumentPosition(C.createElement("fieldset"))}),ce(function(e){return e.innerHTML="<a href='#'></a>","#"===e.firstChild.getAttribute("href")})||fe("type|href|height|width",function(e,t,n){if(!n)return e.getAttribute(t,"type"===t.toLowerCase()?1:2)}),d.attributes&&ce(function(e){return e.innerHTML="<input/>",e.firstChild.setAttribute("value",""),""===e.firstChild.getAttribute("value")})||fe("value",function(e,t,n){if(!n&&"input"===e.nodeName.toLowerCase())return e.defaultValue}),ce(function(e){return null==e.getAttribute("disabled")})||fe(R,function(e,t,n){var r;if(!n)return!0===e[t]?t.toLowerCase():(r=e.getAttributeNode(t))&&r.specified?r.value:null}),se}(C);S.find=d,S.expr=d.selectors,S.expr[":"]=S.expr.pseudos,S.uniqueSort=S.unique=d.uniqueSort,S.text=d.getText,S.isXMLDoc=d.isXML,S.contains=d.contains,S.escapeSelector=d.escape;var h=function(e,t,n){var r=[],i=void 0!==n;while((e=e[t])&&9!==e.nodeType)if(1===e.nodeType){if(i&&S(e).is(n))break;r.push(e)}return r},T=function(e,t){for(var n=[];e;e=e.nextSibling)1===e.nodeType&&e!==t&&n.push(e);return n},k=S.expr.match.needsContext;function A(e,t){return e.nodeName&&e.nodeName.toLowerCase()===t.toLowerCase()}var N=/^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;function j(e,n,r){return m(n)?S.grep(e,function(e,t){return!!n.call(e,t,e)!==r}):n.nodeType?S.grep(e,function(e){return e===n!==r}):"string"!=typeof n?S.grep(e,function(e){return-1<i.call(n,e)!==r}):S.filter(n,e,r)}S.filter=function(e,t,n){var r=t[0];return n&&(e=":not("+e+")"),1===t.length&&1===r.nodeType?S.find.matchesSelector(r,e)?[r]:[]:S.find.matches(e,S.grep(t,function(e){return 1===e.nodeType}))},S.fn.extend({find:function(e){var t,n,r=this.length,i=this;if("string"!=typeof e)return this.pushStack(S(e).filter(function(){for(t=0;t<r;t++)if(S.contains(i[t],this))return!0}));for(n=this.pushStack([]),t=0;t<r;t++)S.find(e,i[t],n);return 1<r?S.uniqueSort(n):n},filter:function(e){return this.pushStack(j(this,e||[],!1))},not:function(e){return this.pushStack(j(this,e||[],!0))},is:function(e){return!!j(this,"string"==typeof e&&k.test(e)?S(e):e||[],!1).length}});var D,q=/^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;(S.fn.init=function(e,t,n){var r,i;if(!e)return this;if(n=n||D,"string"==typeof e){if(!(r="<"===e[0]&&">"===e[e.length-1]&&3<=e.length?[null,e,null]:q.exec(e))||!r[1]&&t)return!t||t.jquery?(t||n).find(e):this.constructor(t).find(e);if(r[1]){if(t=t instanceof S?t[0]:t,S.merge(this,S.parseHTML(r[1],t&&t.nodeType?t.ownerDocument||t:E,!0)),N.test(r[1])&&S.isPlainObject(t))for(r in t)m(this[r])?this[r](t[r]):this.attr(r,t[r]);return this}return(i=E.getElementById(r[2]))&&(this[0]=i,this.length=1),this}return e.nodeType?(this[0]=e,this.length=1,this):m(e)?void 0!==n.ready?n.ready(e):e(S):S.makeArray(e,this)}).prototype=S.fn,D=S(E);var L=/^(?:parents|prev(?:Until|All))/,H={children:!0,contents:!0,next:!0,prev:!0};function O(e,t){while((e=e[t])&&1!==e.nodeType);return e}S.fn.extend({has:function(e){var t=S(e,this),n=t.length;return this.filter(function(){for(var e=0;e<n;e++)if(S.contains(this,t[e]))return!0})},closest:function(e,t){var n,r=0,i=this.length,o=[],a="string"!=typeof e&&S(e);if(!k.test(e))for(;r<i;r++)for(n=this[r];n&&n!==t;n=n.parentNode)if(n.nodeType<11&&(a?-1<a.index(n):1===n.nodeType&&S.find.matchesSelector(n,e))){o.push(n);break}return this.pushStack(1<o.length?S.uniqueSort(o):o)},index:function(e){return e?"string"==typeof e?i.call(S(e),this[0]):i.call(this,e.jquery?e[0]:e):this[0]&&this[0].parentNode?this.first().prevAll().length:-1},add:function(e,t){return this.pushStack(S.uniqueSort(S.merge(this.get(),S(e,t))))},addBack:function(e){return this.add(null==e?this.prevObject:this.prevObject.filter(e))}}),S.each({parent:function(e){var t=e.parentNode;return t&&11!==t.nodeType?t:null},parents:function(e){return h(e,"parentNode")},parentsUntil:function(e,t,n){return h(e,"parentNode",n)},next:function(e){return O(e,"nextSibling")},prev:function(e){return O(e,"previousSibling")},nextAll:function(e){return h(e,"nextSibling")},prevAll:function(e){return h(e,"previousSibling")},nextUntil:function(e,t,n){return h(e,"nextSibling",n)},prevUntil:function(e,t,n){return h(e,"previousSibling",n)},siblings:function(e){return T((e.parentNode||{}).firstChild,e)},children:function(e){return T(e.firstChild)},contents:function(e){return null!=e.contentDocument&&r(e.contentDocument)?e.contentDocument:(A(e,"template")&&(e=e.content||e),S.merge([],e.childNodes))}},function(r,i){S.fn[r]=function(e,t){var n=S.map(this,i,e);return"Until"!==r.slice(-5)&&(t=e),t&&"string"==typeof t&&(n=S.filter(t,n)),1<this.length&&(H[r]||S.uniqueSort(n),L.test(r)&&n.reverse()),this.pushStack(n)}});var P=/[^\x20\t\r\n\f]+/g;function R(e){return e}function M(e){throw e}function I(e,t,n,r){var i;try{e&&m(i=e.promise)?i.call(e).done(t).fail(n):e&&m(i=e.then)?i.call(e,t,n):t.apply(void 0,[e].slice(r))}catch(e){n.apply(void 0,[e])}}S.Callbacks=function(r){var e,n;r="string"==typeof r?(e=r,n={},S.each(e.match(P)||[],function(e,t){n[t]=!0}),n):S.extend({},r);var i,t,o,a,s=[],u=[],l=-1,c=function(){for(a=a||r.once,o=i=!0;u.length;l=-1){t=u.shift();while(++l<s.length)!1===s[l].apply(t[0],t[1])&&r.stopOnFalse&&(l=s.length,t=!1)}r.memory||(t=!1),i=!1,a&&(s=t?[]:"")},f={add:function(){return s&&(t&&!i&&(l=s.length-1,u.push(t)),function n(e){S.each(e,function(e,t){m(t)?r.unique&&f.has(t)||s.push(t):t&&t.length&&"string"!==w(t)&&n(t)})}(arguments),t&&!i&&c()),this},remove:function(){return S.each(arguments,function(e,t){var n;while(-1<(n=S.inArray(t,s,n)))s.splice(n,1),n<=l&&l--}),this},has:function(e){return e?-1<S.inArray(e,s):0<s.length},empty:function(){return s&&(s=[]),this},disable:function(){return a=u=[],s=t="",this},disabled:function(){return!s},lock:function(){return a=u=[],t||i||(s=t=""),this},locked:function(){return!!a},fireWith:function(e,t){return a||(t=[e,(t=t||[]).slice?t.slice():t],u.push(t),i||c()),this},fire:function(){return f.fireWith(this,arguments),this},fired:function(){return!!o}};return f},S.extend({Deferred:function(e){var o=[["notify","progress",S.Callbacks("memory"),S.Callbacks("memory"),2],["resolve","done",S.Callbacks("once memory"),S.Callbacks("once memory"),0,"resolved"],["reject","fail",S.Callbacks("once memory"),S.Callbacks("once memory"),1,"rejected"]],i="pending",a={state:function(){return i},always:function(){return s.done(arguments).fail(arguments),this},"catch":function(e){return a.then(null,e)},pipe:function(){var i=arguments;return S.Deferred(function(r){S.each(o,function(e,t){var n=m(i[t[4]])&&i[t[4]];s[t[1]](function(){var e=n&&n.apply(this,arguments);e&&m(e.promise)?e.promise().progress(r.notify).done(r.resolve).fail(r.reject):r[t[0]+"With"](this,n?[e]:arguments)})}),i=null}).promise()},then:function(t,n,r){var u=0;function l(i,o,a,s){return function(){var n=this,r=arguments,e=function(){var e,t;if(!(i<u)){if((e=a.apply(n,r))===o.promise())throw new TypeError("Thenable self-resolution");t=e&&("object"==typeof e||"function"==typeof e)&&e.then,m(t)?s?t.call(e,l(u,o,R,s),l(u,o,M,s)):(u++,t.call(e,l(u,o,R,s),l(u,o,M,s),l(u,o,R,o.notifyWith))):(a!==R&&(n=void 0,r=[e]),(s||o.resolveWith)(n,r))}},t=s?e:function(){try{e()}catch(e){S.Deferred.exceptionHook&&S.Deferred.exceptionHook(e,t.stackTrace),u<=i+1&&(a!==M&&(n=void 0,r=[e]),o.rejectWith(n,r))}};i?t():(S.Deferred.getStackHook&&(t.stackTrace=S.Deferred.getStackHook()),C.setTimeout(t))}}return S.Deferred(function(e){o[0][3].add(l(0,e,m(r)?r:R,e.notifyWith)),o[1][3].add(l(0,e,m(t)?t:R)),o[2][3].add(l(0,e,m(n)?n:M))}).promise()},promise:function(e){return null!=e?S.extend(e,a):a}},s={};return S.each(o,function(e,t){var n=t[2],r=t[5];a[t[1]]=n.add,r&&n.add(function(){i=r},o[3-e][2].disable,o[3-e][3].disable,o[0][2].lock,o[0][3].lock),n.add(t[3].fire),s[t[0]]=function(){return s[t[0]+"With"](this===s?void 0:this,arguments),this},s[t[0]+"With"]=n.fireWith}),a.promise(s),e&&e.call(s,s),s},when:function(e){var n=arguments.length,t=n,r=Array(t),i=s.call(arguments),o=S.Deferred(),a=function(t){return function(e){r[t]=this,i[t]=1<arguments.length?s.call(arguments):e,--n||o.resolveWith(r,i)}};if(n<=1&&(I(e,o.done(a(t)).resolve,o.reject,!n),"pending"===o.state()||m(i[t]&&i[t].then)))return o.then();while(t--)I(i[t],a(t),o.reject);return o.promise()}});var W=/^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;S.Deferred.exceptionHook=function(e,t){C.console&&C.console.warn&&e&&W.test(e.name)&&C.console.warn("jQuery.Deferred exception: "+e.message,e.stack,t)},S.readyException=function(e){C.setTimeout(function(){throw e})};var F=S.Deferred();function $(){E.removeEventListener("DOMContentLoaded",$),C.removeEventListener("load",$),S.ready()}S.fn.ready=function(e){return F.then(e)["catch"](function(e){S.readyException(e)}),this},S.extend({isReady:!1,readyWait:1,ready:function(e){(!0===e?--S.readyWait:S.isReady)||(S.isReady=!0)!==e&&0<--S.readyWait||F.resolveWith(E,[S])}}),S.ready.then=F.then,"complete"===E.readyState||"loading"!==E.readyState&&!E.documentElement.doScroll?C.setTimeout(S.ready):(E.addEventListener("DOMContentLoaded",$),C.addEventListener("load",$));var B=function(e,t,n,r,i,o,a){var s=0,u=e.length,l=null==n;if("object"===w(n))for(s in i=!0,n)B(e,t,s,n[s],!0,o,a);else if(void 0!==r&&(i=!0,m(r)||(a=!0),l&&(a?(t.call(e,r),t=null):(l=t,t=function(e,t,n){return l.call(S(e),n)})),t))for(;s<u;s++)t(e[s],n,a?r:r.call(e[s],s,t(e[s],n)));return i?e:l?t.call(e):u?t(e[0],n):o},_=/^-ms-/,z=/-([a-z])/g;function U(e,t){return t.toUpperCase()}function X(e){return e.replace(_,"ms-").replace(z,U)}var V=function(e){return 1===e.nodeType||9===e.nodeType||!+e.nodeType};function G(){this.expando=S.expando+G.uid++}G.uid=1,G.prototype={cache:function(e){var t=e[this.expando];return t||(t={},V(e)&&(e.nodeType?e[this.expando]=t:Object.defineProperty(e,this.expando,{value:t,configurable:!0}))),t},set:function(e,t,n){var r,i=this.cache(e);if("string"==typeof t)i[X(t)]=n;else for(r in t)i[X(r)]=t[r];return i},get:function(e,t){return void 0===t?this.cache(e):e[this.expando]&&e[this.expando][X(t)]},access:function(e,t,n){return void 0===t||t&&"string"==typeof t&&void 0===n?this.get(e,t):(this.set(e,t,n),void 0!==n?n:t)},remove:function(e,t){var n,r=e[this.expando];if(void 0!==r){if(void 0!==t){n=(t=Array.isArray(t)?t.map(X):(t=X(t))in r?[t]:t.match(P)||[]).length;while(n--)delete r[t[n]]}(void 0===t||S.isEmptyObject(r))&&(e.nodeType?e[this.expando]=void 0:delete e[this.expando])}},hasData:function(e){var t=e[this.expando];return void 0!==t&&!S.isEmptyObject(t)}};var Y=new G,Q=new G,J=/^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,K=/[A-Z]/g;function Z(e,t,n){var r,i;if(void 0===n&&1===e.nodeType)if(r="data-"+t.replace(K,"-$&").toLowerCase(),"string"==typeof(n=e.getAttribute(r))){try{n="true"===(i=n)||"false"!==i&&("null"===i?null:i===+i+""?+i:J.test(i)?JSON.parse(i):i)}catch(e){}Q.set(e,t,n)}else n=void 0;return n}S.extend({hasData:function(e){return Q.hasData(e)||Y.hasData(e)},data:function(e,t,n){return Q.access(e,t,n)},removeData:function(e,t){Q.remove(e,t)},_data:function(e,t,n){return Y.access(e,t,n)},_removeData:function(e,t){Y.remove(e,t)}}),S.fn.extend({data:function(n,e){var t,r,i,o=this[0],a=o&&o.attributes;if(void 0===n){if(this.length&&(i=Q.get(o),1===o.nodeType&&!Y.get(o,"hasDataAttrs"))){t=a.length;while(t--)a[t]&&0===(r=a[t].name).indexOf("data-")&&(r=X(r.slice(5)),Z(o,r,i[r]));Y.set(o,"hasDataAttrs",!0)}return i}return"object"==typeof n?this.each(function(){Q.set(this,n)}):B(this,function(e){var t;if(o&&void 0===e)return void 0!==(t=Q.get(o,n))?t:void 0!==(t=Z(o,n))?t:void 0;this.each(function(){Q.set(this,n,e)})},null,e,1<arguments.length,null,!0)},removeData:function(e){return this.each(function(){Q.remove(this,e)})}}),S.extend({queue:function(e,t,n){var r;if(e)return t=(t||"fx")+"queue",r=Y.get(e,t),n&&(!r||Array.isArray(n)?r=Y.access(e,t,S.makeArray(n)):r.push(n)),r||[]},dequeue:function(e,t){t=t||"fx";var n=S.queue(e,t),r=n.length,i=n.shift(),o=S._queueHooks(e,t);"inprogress"===i&&(i=n.shift(),r--),i&&("fx"===t&&n.unshift("inprogress"),delete o.stop,i.call(e,function(){S.dequeue(e,t)},o)),!r&&o&&o.empty.fire()},_queueHooks:function(e,t){var n=t+"queueHooks";return Y.get(e,n)||Y.access(e,n,{empty:S.Callbacks("once memory").add(function(){Y.remove(e,[t+"queue",n])})})}}),S.fn.extend({queue:function(t,n){var e=2;return"string"!=typeof t&&(n=t,t="fx",e--),arguments.length<e?S.queue(this[0],t):void 0===n?this:this.each(function(){var e=S.queue(this,t,n);S._queueHooks(this,t),"fx"===t&&"inprogress"!==e[0]&&S.dequeue(this,t)})},dequeue:function(e){return this.each(function(){S.dequeue(this,e)})},clearQueue:function(e){return this.queue(e||"fx",[])},promise:function(e,t){var n,r=1,i=S.Deferred(),o=this,a=this.length,s=function(){--r||i.resolveWith(o,[o])};"string"!=typeof e&&(t=e,e=void 0),e=e||"fx";while(a--)(n=Y.get(o[a],e+"queueHooks"))&&n.empty&&(r++,n.empty.add(s));return s(),i.promise(t)}});var ee=/[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,te=new RegExp("^(?:([+-])=|)("+ee+")([a-z%]*)$","i"),ne=["Top","Right","Bottom","Left"],re=E.documentElement,ie=function(e){return S.contains(e.ownerDocument,e)},oe={composed:!0};re.getRootNode&&(ie=function(e){return S.contains(e.ownerDocument,e)||e.getRootNode(oe)===e.ownerDocument});var ae=function(e,t){return"none"===(e=t||e).style.display||""===e.style.display&&ie(e)&&"none"===S.css(e,"display")};function se(e,t,n,r){var i,o,a=20,s=r?function(){return r.cur()}:function(){return S.css(e,t,"")},u=s(),l=n&&n[3]||(S.cssNumber[t]?"":"px"),c=e.nodeType&&(S.cssNumber[t]||"px"!==l&&+u)&&te.exec(S.css(e,t));if(c&&c[3]!==l){u/=2,l=l||c[3],c=+u||1;while(a--)S.style(e,t,c+l),(1-o)*(1-(o=s()/u||.5))<=0&&(a=0),c/=o;c*=2,S.style(e,t,c+l),n=n||[]}return n&&(c=+c||+u||0,i=n[1]?c+(n[1]+1)*n[2]:+n[2],r&&(r.unit=l,r.start=c,r.end=i)),i}var ue={};function le(e,t){for(var n,r,i,o,a,s,u,l=[],c=0,f=e.length;c<f;c++)(r=e[c]).style&&(n=r.style.display,t?("none"===n&&(l[c]=Y.get(r,"display")||null,l[c]||(r.style.display="")),""===r.style.display&&ae(r)&&(l[c]=(u=a=o=void 0,a=(i=r).ownerDocument,s=i.nodeName,(u=ue[s])||(o=a.body.appendChild(a.createElement(s)),u=S.css(o,"display"),o.parentNode.removeChild(o),"none"===u&&(u="block"),ue[s]=u)))):"none"!==n&&(l[c]="none",Y.set(r,"display",n)));for(c=0;c<f;c++)null!=l[c]&&(e[c].style.display=l[c]);return e}S.fn.extend({show:function(){return le(this,!0)},hide:function(){return le(this)},toggle:function(e){return"boolean"==typeof e?e?this.show():this.hide():this.each(function(){ae(this)?S(this).show():S(this).hide()})}});var ce,fe,pe=/^(?:checkbox|radio)$/i,de=/<([a-z][^\/\0>\x20\t\r\n\f]*)/i,he=/^$|^module$|\/(?:java|ecma)script/i;ce=E.createDocumentFragment().appendChild(E.createElement("div")),(fe=E.createElement("input")).setAttribute("type","radio"),fe.setAttribute("checked","checked"),fe.setAttribute("name","t"),ce.appendChild(fe),v.checkClone=ce.cloneNode(!0).cloneNode(!0).lastChild.checked,ce.innerHTML="<textarea>x</textarea>",v.noCloneChecked=!!ce.cloneNode(!0).lastChild.defaultValue,ce.innerHTML="<option></option>",v.option=!!ce.lastChild;var ge={thead:[1,"<table>","</table>"],col:[2,"<table><colgroup>","</colgroup></table>"],tr:[2,"<table><tbody>","</tbody></table>"],td:[3,"<table><tbody><tr>","</tr></tbody></table>"],_default:[0,"",""]};function ye(e,t){var n;return n="undefined"!=typeof e.getElementsByTagName?e.getElementsByTagName(t||"*"):"undefined"!=typeof e.querySelectorAll?e.querySelectorAll(t||"*"):[],void 0===t||t&&A(e,t)?S.merge([e],n):n}function ve(e,t){for(var n=0,r=e.length;n<r;n++)Y.set(e[n],"globalEval",!t||Y.get(t[n],"globalEval"))}ge.tbody=ge.tfoot=ge.colgroup=ge.caption=ge.thead,ge.th=ge.td,v.option||(ge.optgroup=ge.option=[1,"<select multiple='multiple'>","</select>"]);var me=/<|&#?\w+;/;function xe(e,t,n,r,i){for(var o,a,s,u,l,c,f=t.createDocumentFragment(),p=[],d=0,h=e.length;d<h;d++)if((o=e[d])||0===o)if("object"===w(o))S.merge(p,o.nodeType?[o]:o);else if(me.test(o)){a=a||f.appendChild(t.createElement("div")),s=(de.exec(o)||["",""])[1].toLowerCase(),u=ge[s]||ge._default,a.innerHTML=u[1]+S.htmlPrefilter(o)+u[2],c=u[0];while(c--)a=a.lastChild;S.merge(p,a.childNodes),(a=f.firstChild).textContent=""}else p.push(t.createTextNode(o));f.textContent="",d=0;while(o=p[d++])if(r&&-1<S.inArray(o,r))i&&i.push(o);else if(l=ie(o),a=ye(f.appendChild(o),"script"),l&&ve(a),n){c=0;while(o=a[c++])he.test(o.type||"")&&n.push(o)}return f}var be=/^([^.]*)(?:\.(.+)|)/;function we(){return!0}function Te(){return!1}function Ce(e,t){return e===function(){try{return E.activeElement}catch(e){}}()==("focus"===t)}function Ee(e,t,n,r,i,o){var a,s;if("object"==typeof t){for(s in"string"!=typeof n&&(r=r||n,n=void 0),t)Ee(e,s,n,r,t[s],o);return e}if(null==r&&null==i?(i=n,r=n=void 0):null==i&&("string"==typeof n?(i=r,r=void 0):(i=r,r=n,n=void 0)),!1===i)i=Te;else if(!i)return e;return 1===o&&(a=i,(i=function(e){return S().off(e),a.apply(this,arguments)}).guid=a.guid||(a.guid=S.guid++)),e.each(function(){S.event.add(this,t,i,r,n)})}function Se(e,i,o){o?(Y.set(e,i,!1),S.event.add(e,i,{namespace:!1,handler:function(e){var t,n,r=Y.get(this,i);if(1&e.isTrigger&&this[i]){if(r.length)(S.event.special[i]||{}).delegateType&&e.stopPropagation();else if(r=s.call(arguments),Y.set(this,i,r),t=o(this,i),this[i](),r!==(n=Y.get(this,i))||t?Y.set(this,i,!1):n={},r!==n)return e.stopImmediatePropagation(),e.preventDefault(),n&&n.value}else r.length&&(Y.set(this,i,{value:S.event.trigger(S.extend(r[0],S.Event.prototype),r.slice(1),this)}),e.stopImmediatePropagation())}})):void 0===Y.get(e,i)&&S.event.add(e,i,we)}S.event={global:{},add:function(t,e,n,r,i){var o,a,s,u,l,c,f,p,d,h,g,y=Y.get(t);if(V(t)){n.handler&&(n=(o=n).handler,i=o.selector),i&&S.find.matchesSelector(re,i),n.guid||(n.guid=S.guid++),(u=y.events)||(u=y.events=Object.create(null)),(a=y.handle)||(a=y.handle=function(e){return"undefined"!=typeof S&&S.event.triggered!==e.type?S.event.dispatch.apply(t,arguments):void 0}),l=(e=(e||"").match(P)||[""]).length;while(l--)d=g=(s=be.exec(e[l])||[])[1],h=(s[2]||"").split(".").sort(),d&&(f=S.event.special[d]||{},d=(i?f.delegateType:f.bindType)||d,f=S.event.special[d]||{},c=S.extend({type:d,origType:g,data:r,handler:n,guid:n.guid,selector:i,needsContext:i&&S.expr.match.needsContext.test(i),namespace:h.join(".")},o),(p=u[d])||((p=u[d]=[]).delegateCount=0,f.setup&&!1!==f.setup.call(t,r,h,a)||t.addEventListener&&t.addEventListener(d,a)),f.add&&(f.add.call(t,c),c.handler.guid||(c.handler.guid=n.guid)),i?p.splice(p.delegateCount++,0,c):p.push(c),S.event.global[d]=!0)}},remove:function(e,t,n,r,i){var o,a,s,u,l,c,f,p,d,h,g,y=Y.hasData(e)&&Y.get(e);if(y&&(u=y.events)){l=(t=(t||"").match(P)||[""]).length;while(l--)if(d=g=(s=be.exec(t[l])||[])[1],h=(s[2]||"").split(".").sort(),d){f=S.event.special[d]||{},p=u[d=(r?f.delegateType:f.bindType)||d]||[],s=s[2]&&new RegExp("(^|\\.)"+h.join("\\.(?:.*\\.|)")+"(\\.|$)"),a=o=p.length;while(o--)c=p[o],!i&&g!==c.origType||n&&n.guid!==c.guid||s&&!s.test(c.namespace)||r&&r!==c.selector&&("**"!==r||!c.selector)||(p.splice(o,1),c.selector&&p.delegateCount--,f.remove&&f.remove.call(e,c));a&&!p.length&&(f.teardown&&!1!==f.teardown.call(e,h,y.handle)||S.removeEvent(e,d,y.handle),delete u[d])}else for(d in u)S.event.remove(e,d+t[l],n,r,!0);S.isEmptyObject(u)&&Y.remove(e,"handle events")}},dispatch:function(e){var t,n,r,i,o,a,s=new Array(arguments.length),u=S.event.fix(e),l=(Y.get(this,"events")||Object.create(null))[u.type]||[],c=S.event.special[u.type]||{};for(s[0]=u,t=1;t<arguments.length;t++)s[t]=arguments[t];if(u.delegateTarget=this,!c.preDispatch||!1!==c.preDispatch.call(this,u)){a=S.event.handlers.call(this,u,l),t=0;while((i=a[t++])&&!u.isPropagationStopped()){u.currentTarget=i.elem,n=0;while((o=i.handlers[n++])&&!u.isImmediatePropagationStopped())u.rnamespace&&!1!==o.namespace&&!u.rnamespace.test(o.namespace)||(u.handleObj=o,u.data=o.data,void 0!==(r=((S.event.special[o.origType]||{}).handle||o.handler).apply(i.elem,s))&&!1===(u.result=r)&&(u.preventDefault(),u.stopPropagation()))}return c.postDispatch&&c.postDispatch.call(this,u),u.result}},handlers:function(e,t){var n,r,i,o,a,s=[],u=t.delegateCount,l=e.target;if(u&&l.nodeType&&!("click"===e.type&&1<=e.button))for(;l!==this;l=l.parentNode||this)if(1===l.nodeType&&("click"!==e.type||!0!==l.disabled)){for(o=[],a={},n=0;n<u;n++)void 0===a[i=(r=t[n]).selector+" "]&&(a[i]=r.needsContext?-1<S(i,this).index(l):S.find(i,this,null,[l]).length),a[i]&&o.push(r);o.length&&s.push({elem:l,handlers:o})}return l=this,u<t.length&&s.push({elem:l,handlers:t.slice(u)}),s},addProp:function(t,e){Object.defineProperty(S.Event.prototype,t,{enumerable:!0,configurable:!0,get:m(e)?function(){if(this.originalEvent)return e(this.originalEvent)}:function(){if(this.originalEvent)return this.originalEvent[t]},set:function(e){Object.defineProperty(this,t,{enumerable:!0,configurable:!0,writable:!0,value:e})}})},fix:function(e){return e[S.expando]?e:new S.Event(e)},special:{load:{noBubble:!0},click:{setup:function(e){var t=this||e;return pe.test(t.type)&&t.click&&A(t,"input")&&Se(t,"click",we),!1},trigger:function(e){var t=this||e;return pe.test(t.type)&&t.click&&A(t,"input")&&Se(t,"click"),!0},_default:function(e){var t=e.target;return pe.test(t.type)&&t.click&&A(t,"input")&&Y.get(t,"click")||A(t,"a")}},beforeunload:{postDispatch:function(e){void 0!==e.result&&e.originalEvent&&(e.originalEvent.returnValue=e.result)}}}},S.removeEvent=function(e,t,n){e.removeEventListener&&e.removeEventListener(t,n)},S.Event=function(e,t){if(!(this instanceof S.Event))return new S.Event(e,t);e&&e.type?(this.originalEvent=e,this.type=e.type,this.isDefaultPrevented=e.defaultPrevented||void 0===e.defaultPrevented&&!1===e.returnValue?we:Te,this.target=e.target&&3===e.target.nodeType?e.target.parentNode:e.target,this.currentTarget=e.currentTarget,this.relatedTarget=e.relatedTarget):this.type=e,t&&S.extend(this,t),this.timeStamp=e&&e.timeStamp||Date.now(),this[S.expando]=!0},S.Event.prototype={constructor:S.Event,isDefaultPrevented:Te,isPropagationStopped:Te,isImmediatePropagationStopped:Te,isSimulated:!1,preventDefault:function(){var e=this.originalEvent;this.isDefaultPrevented=we,e&&!this.isSimulated&&e.preventDefault()},stopPropagation:function(){var e=this.originalEvent;this.isPropagationStopped=we,e&&!this.isSimulated&&e.stopPropagation()},stopImmediatePropagation:function(){var e=this.originalEvent;this.isImmediatePropagationStopped=we,e&&!this.isSimulated&&e.stopImmediatePropagation(),this.stopPropagation()}},S.each({altKey:!0,bubbles:!0,cancelable:!0,changedTouches:!0,ctrlKey:!0,detail:!0,eventPhase:!0,metaKey:!0,pageX:!0,pageY:!0,shiftKey:!0,view:!0,"char":!0,code:!0,charCode:!0,key:!0,keyCode:!0,button:!0,buttons:!0,clientX:!0,clientY:!0,offsetX:!0,offsetY:!0,pointerId:!0,pointerType:!0,screenX:!0,screenY:!0,targetTouches:!0,toElement:!0,touches:!0,which:!0},S.event.addProp),S.each({focus:"focusin",blur:"focusout"},function(t,e){S.event.special[t]={setup:function(){return Se(this,t,Ce),!1},trigger:function(){return Se(this,t),!0},_default:function(e){return Y.get(e.target,t)},delegateType:e}}),S.each({mouseenter:"mouseover",mouseleave:"mouseout",pointerenter:"pointerover",pointerleave:"pointerout"},function(e,i){S.event.special[e]={delegateType:i,bindType:i,handle:function(e){var t,n=e.relatedTarget,r=e.handleObj;return n&&(n===this||S.contains(this,n))||(e.type=r.origType,t=r.handler.apply(this,arguments),e.type=i),t}}}),S.fn.extend({on:function(e,t,n,r){return Ee(this,e,t,n,r)},one:function(e,t,n,r){return Ee(this,e,t,n,r,1)},off:function(e,t,n){var r,i;if(e&&e.preventDefault&&e.handleObj)return r=e.handleObj,S(e.delegateTarget).off(r.namespace?r.origType+"."+r.namespace:r.origType,r.selector,r.handler),this;if("object"==typeof e){for(i in e)this.off(i,t,e[i]);return this}return!1!==t&&"function"!=typeof t||(n=t,t=void 0),!1===n&&(n=Te),this.each(function(){S.event.remove(this,e,n,t)})}});var ke=/<script|<style|<link/i,Ae=/checked\s*(?:[^=]|=\s*.checked.)/i,Ne=/^\s*<!\[CDATA\[|\]\]>\s*$/g;function je(e,t){return A(e,"table")&&A(11!==t.nodeType?t:t.firstChild,"tr")&&S(e).children("tbody")[0]||e}function De(e){return e.type=(null!==e.getAttribute("type"))+"/"+e.type,e}function qe(e){return"true/"===(e.type||"").slice(0,5)?e.type=e.type.slice(5):e.removeAttribute("type"),e}function Le(e,t){var n,r,i,o,a,s;if(1===t.nodeType){if(Y.hasData(e)&&(s=Y.get(e).events))for(i in Y.remove(t,"handle events"),s)for(n=0,r=s[i].length;n<r;n++)S.event.add(t,i,s[i][n]);Q.hasData(e)&&(o=Q.access(e),a=S.extend({},o),Q.set(t,a))}}function He(n,r,i,o){r=g(r);var e,t,a,s,u,l,c=0,f=n.length,p=f-1,d=r[0],h=m(d);if(h||1<f&&"string"==typeof d&&!v.checkClone&&Ae.test(d))return n.each(function(e){var t=n.eq(e);h&&(r[0]=d.call(this,e,t.html())),He(t,r,i,o)});if(f&&(t=(e=xe(r,n[0].ownerDocument,!1,n,o)).firstChild,1===e.childNodes.length&&(e=t),t||o)){for(s=(a=S.map(ye(e,"script"),De)).length;c<f;c++)u=e,c!==p&&(u=S.clone(u,!0,!0),s&&S.merge(a,ye(u,"script"))),i.call(n[c],u,c);if(s)for(l=a[a.length-1].ownerDocument,S.map(a,qe),c=0;c<s;c++)u=a[c],he.test(u.type||"")&&!Y.access(u,"globalEval")&&S.contains(l,u)&&(u.src&&"module"!==(u.type||"").toLowerCase()?S._evalUrl&&!u.noModule&&S._evalUrl(u.src,{nonce:u.nonce||u.getAttribute("nonce")},l):b(u.textContent.replace(Ne,""),u,l))}return n}function Oe(e,t,n){for(var r,i=t?S.filter(t,e):e,o=0;null!=(r=i[o]);o++)n||1!==r.nodeType||S.cleanData(ye(r)),r.parentNode&&(n&&ie(r)&&ve(ye(r,"script")),r.parentNode.removeChild(r));return e}S.extend({htmlPrefilter:function(e){return e},clone:function(e,t,n){var r,i,o,a,s,u,l,c=e.cloneNode(!0),f=ie(e);if(!(v.noCloneChecked||1!==e.nodeType&&11!==e.nodeType||S.isXMLDoc(e)))for(a=ye(c),r=0,i=(o=ye(e)).length;r<i;r++)s=o[r],u=a[r],void 0,"input"===(l=u.nodeName.toLowerCase())&&pe.test(s.type)?u.checked=s.checked:"input"!==l&&"textarea"!==l||(u.defaultValue=s.defaultValue);if(t)if(n)for(o=o||ye(e),a=a||ye(c),r=0,i=o.length;r<i;r++)Le(o[r],a[r]);else Le(e,c);return 0<(a=ye(c,"script")).length&&ve(a,!f&&ye(e,"script")),c},cleanData:function(e){for(var t,n,r,i=S.event.special,o=0;void 0!==(n=e[o]);o++)if(V(n)){if(t=n[Y.expando]){if(t.events)for(r in t.events)i[r]?S.event.remove(n,r):S.removeEvent(n,r,t.handle);n[Y.expando]=void 0}n[Q.expando]&&(n[Q.expando]=void 0)}}}),S.fn.extend({detach:function(e){return Oe(this,e,!0)},remove:function(e){return Oe(this,e)},text:function(e){return B(this,function(e){return void 0===e?S.text(this):this.empty().each(function(){1!==this.nodeType&&11!==this.nodeType&&9!==this.nodeType||(this.textContent=e)})},null,e,arguments.length)},append:function(){return He(this,arguments,function(e){1!==this.nodeType&&11!==this.nodeType&&9!==this.nodeType||je(this,e).appendChild(e)})},prepend:function(){return He(this,arguments,function(e){if(1===this.nodeType||11===this.nodeType||9===this.nodeType){var t=je(this,e);t.insertBefore(e,t.firstChild)}})},before:function(){return He(this,arguments,function(e){this.parentNode&&this.parentNode.insertBefore(e,this)})},after:function(){return He(this,arguments,function(e){this.parentNode&&this.parentNode.insertBefore(e,this.nextSibling)})},empty:function(){for(var e,t=0;null!=(e=this[t]);t++)1===e.nodeType&&(S.cleanData(ye(e,!1)),e.textContent="");return this},clone:function(e,t){return e=null!=e&&e,t=null==t?e:t,this.map(function(){return S.clone(this,e,t)})},html:function(e){return B(this,function(e){var t=this[0]||{},n=0,r=this.length;if(void 0===e&&1===t.nodeType)return t.innerHTML;if("string"==typeof e&&!ke.test(e)&&!ge[(de.exec(e)||["",""])[1].toLowerCase()]){e=S.htmlPrefilter(e);try{for(;n<r;n++)1===(t=this[n]||{}).nodeType&&(S.cleanData(ye(t,!1)),t.innerHTML=e);t=0}catch(e){}}t&&this.empty().append(e)},null,e,arguments.length)},replaceWith:function(){var n=[];return He(this,arguments,function(e){var t=this.parentNode;S.inArray(this,n)<0&&(S.cleanData(ye(this)),t&&t.replaceChild(e,this))},n)}}),S.each({appendTo:"append",prependTo:"prepend",insertBefore:"before",insertAfter:"after",replaceAll:"replaceWith"},function(e,a){S.fn[e]=function(e){for(var t,n=[],r=S(e),i=r.length-1,o=0;o<=i;o++)t=o===i?this:this.clone(!0),S(r[o])[a](t),u.apply(n,t.get());return this.pushStack(n)}});var Pe=new RegExp("^("+ee+")(?!px)[a-z%]+$","i"),Re=/^--/,Me=function(e){var t=e.ownerDocument.defaultView;return t&&t.opener||(t=C),t.getComputedStyle(e)},Ie=function(e,t,n){var r,i,o={};for(i in t)o[i]=e.style[i],e.style[i]=t[i];for(i in r=n.call(e),t)e.style[i]=o[i];return r},We=new RegExp(ne.join("|"),"i"),Fe="[\\x20\\t\\r\\n\\f]",$e=new RegExp("^"+Fe+"+|((?:^|[^\\\\])(?:\\\\.)*)"+Fe+"+$","g");function Be(e,t,n){var r,i,o,a,s=Re.test(t),u=e.style;return(n=n||Me(e))&&(a=n.getPropertyValue(t)||n[t],s&&a&&(a=a.replace($e,"$1")||void 0),""!==a||ie(e)||(a=S.style(e,t)),!v.pixelBoxStyles()&&Pe.test(a)&&We.test(t)&&(r=u.width,i=u.minWidth,o=u.maxWidth,u.minWidth=u.maxWidth=u.width=a,a=n.width,u.width=r,u.minWidth=i,u.maxWidth=o)),void 0!==a?a+"":a}function _e(e,t){return{get:function(){if(!e())return(this.get=t).apply(this,arguments);delete this.get}}}!function(){function e(){if(l){u.style.cssText="position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0",l.style.cssText="position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%",re.appendChild(u).appendChild(l);var e=C.getComputedStyle(l);n="1%"!==e.top,s=12===t(e.marginLeft),l.style.right="60%",o=36===t(e.right),r=36===t(e.width),l.style.position="absolute",i=12===t(l.offsetWidth/3),re.removeChild(u),l=null}}function t(e){return Math.round(parseFloat(e))}var n,r,i,o,a,s,u=E.createElement("div"),l=E.createElement("div");l.style&&(l.style.backgroundClip="content-box",l.cloneNode(!0).style.backgroundClip="",v.clearCloneStyle="content-box"===l.style.backgroundClip,S.extend(v,{boxSizingReliable:function(){return e(),r},pixelBoxStyles:function(){return e(),o},pixelPosition:function(){return e(),n},reliableMarginLeft:function(){return e(),s},scrollboxSize:function(){return e(),i},reliableTrDimensions:function(){var e,t,n,r;return null==a&&(e=E.createElement("table"),t=E.createElement("tr"),n=E.createElement("div"),e.style.cssText="position:absolute;left:-11111px;border-collapse:separate",t.style.cssText="border:1px solid",t.style.height="1px",n.style.height="9px",n.style.display="block",re.appendChild(e).appendChild(t).appendChild(n),r=C.getComputedStyle(t),a=parseInt(r.height,10)+parseInt(r.borderTopWidth,10)+parseInt(r.borderBottomWidth,10)===t.offsetHeight,re.removeChild(e)),a}}))}();var ze=["Webkit","Moz","ms"],Ue=E.createElement("div").style,Xe={};function Ve(e){var t=S.cssProps[e]||Xe[e];return t||(e in Ue?e:Xe[e]=function(e){var t=e[0].toUpperCase()+e.slice(1),n=ze.length;while(n--)if((e=ze[n]+t)in Ue)return e}(e)||e)}var Ge=/^(none|table(?!-c[ea]).+)/,Ye={position:"absolute",visibility:"hidden",display:"block"},Qe={letterSpacing:"0",fontWeight:"400"};function Je(e,t,n){var r=te.exec(t);return r?Math.max(0,r[2]-(n||0))+(r[3]||"px"):t}function Ke(e,t,n,r,i,o){var a="width"===t?1:0,s=0,u=0;if(n===(r?"border":"content"))return 0;for(;a<4;a+=2)"margin"===n&&(u+=S.css(e,n+ne[a],!0,i)),r?("content"===n&&(u-=S.css(e,"padding"+ne[a],!0,i)),"margin"!==n&&(u-=S.css(e,"border"+ne[a]+"Width",!0,i))):(u+=S.css(e,"padding"+ne[a],!0,i),"padding"!==n?u+=S.css(e,"border"+ne[a]+"Width",!0,i):s+=S.css(e,"border"+ne[a]+"Width",!0,i));return!r&&0<=o&&(u+=Math.max(0,Math.ceil(e["offset"+t[0].toUpperCase()+t.slice(1)]-o-u-s-.5))||0),u}function Ze(e,t,n){var r=Me(e),i=(!v.boxSizingReliable()||n)&&"border-box"===S.css(e,"boxSizing",!1,r),o=i,a=Be(e,t,r),s="offset"+t[0].toUpperCase()+t.slice(1);if(Pe.test(a)){if(!n)return a;a="auto"}return(!v.boxSizingReliable()&&i||!v.reliableTrDimensions()&&A(e,"tr")||"auto"===a||!parseFloat(a)&&"inline"===S.css(e,"display",!1,r))&&e.getClientRects().length&&(i="border-box"===S.css(e,"boxSizing",!1,r),(o=s in e)&&(a=e[s])),(a=parseFloat(a)||0)+Ke(e,t,n||(i?"border":"content"),o,r,a)+"px"}function et(e,t,n,r,i){return new et.prototype.init(e,t,n,r,i)}S.extend({cssHooks:{opacity:{get:function(e,t){if(t){var n=Be(e,"opacity");return""===n?"1":n}}}},cssNumber:{animationIterationCount:!0,columnCount:!0,fillOpacity:!0,flexGrow:!0,flexShrink:!0,fontWeight:!0,gridArea:!0,gridColumn:!0,gridColumnEnd:!0,gridColumnStart:!0,gridRow:!0,gridRowEnd:!0,gridRowStart:!0,lineHeight:!0,opacity:!0,order:!0,orphans:!0,widows:!0,zIndex:!0,zoom:!0},cssProps:{},style:function(e,t,n,r){if(e&&3!==e.nodeType&&8!==e.nodeType&&e.style){var i,o,a,s=X(t),u=Re.test(t),l=e.style;if(u||(t=Ve(s)),a=S.cssHooks[t]||S.cssHooks[s],void 0===n)return a&&"get"in a&&void 0!==(i=a.get(e,!1,r))?i:l[t];"string"===(o=typeof n)&&(i=te.exec(n))&&i[1]&&(n=se(e,t,i),o="number"),null!=n&&n==n&&("number"!==o||u||(n+=i&&i[3]||(S.cssNumber[s]?"":"px")),v.clearCloneStyle||""!==n||0!==t.indexOf("background")||(l[t]="inherit"),a&&"set"in a&&void 0===(n=a.set(e,n,r))||(u?l.setProperty(t,n):l[t]=n))}},css:function(e,t,n,r){var i,o,a,s=X(t);return Re.test(t)||(t=Ve(s)),(a=S.cssHooks[t]||S.cssHooks[s])&&"get"in a&&(i=a.get(e,!0,n)),void 0===i&&(i=Be(e,t,r)),"normal"===i&&t in Qe&&(i=Qe[t]),""===n||n?(o=parseFloat(i),!0===n||isFinite(o)?o||0:i):i}}),S.each(["height","width"],function(e,u){S.cssHooks[u]={get:function(e,t,n){if(t)return!Ge.test(S.css(e,"display"))||e.getClientRects().length&&e.getBoundingClientRect().width?Ze(e,u,n):Ie(e,Ye,function(){return Ze(e,u,n)})},set:function(e,t,n){var r,i=Me(e),o=!v.scrollboxSize()&&"absolute"===i.position,a=(o||n)&&"border-box"===S.css(e,"boxSizing",!1,i),s=n?Ke(e,u,n,a,i):0;return a&&o&&(s-=Math.ceil(e["offset"+u[0].toUpperCase()+u.slice(1)]-parseFloat(i[u])-Ke(e,u,"border",!1,i)-.5)),s&&(r=te.exec(t))&&"px"!==(r[3]||"px")&&(e.style[u]=t,t=S.css(e,u)),Je(0,t,s)}}}),S.cssHooks.marginLeft=_e(v.reliableMarginLeft,function(e,t){if(t)return(parseFloat(Be(e,"marginLeft"))||e.getBoundingClientRect().left-Ie(e,{marginLeft:0},function(){return e.getBoundingClientRect().left}))+"px"}),S.each({margin:"",padding:"",border:"Width"},function(i,o){S.cssHooks[i+o]={expand:function(e){for(var t=0,n={},r="string"==typeof e?e.split(" "):[e];t<4;t++)n[i+ne[t]+o]=r[t]||r[t-2]||r[0];return n}},"margin"!==i&&(S.cssHooks[i+o].set=Je)}),S.fn.extend({css:function(e,t){return B(this,function(e,t,n){var r,i,o={},a=0;if(Array.isArray(t)){for(r=Me(e),i=t.length;a<i;a++)o[t[a]]=S.css(e,t[a],!1,r);return o}return void 0!==n?S.style(e,t,n):S.css(e,t)},e,t,1<arguments.length)}}),((S.Tween=et).prototype={constructor:et,init:function(e,t,n,r,i,o){this.elem=e,this.prop=n,this.easing=i||S.easing._default,this.options=t,this.start=this.now=this.cur(),this.end=r,this.unit=o||(S.cssNumber[n]?"":"px")},cur:function(){var e=et.propHooks[this.prop];return e&&e.get?e.get(this):et.propHooks._default.get(this)},run:function(e){var t,n=et.propHooks[this.prop];return this.options.duration?this.pos=t=S.easing[this.easing](e,this.options.duration*e,0,1,this.options.duration):this.pos=t=e,this.now=(this.end-this.start)*t+this.start,this.options.step&&this.options.step.call(this.elem,this.now,this),n&&n.set?n.set(this):et.propHooks._default.set(this),this}}).init.prototype=et.prototype,(et.propHooks={_default:{get:function(e){var t;return 1!==e.elem.nodeType||null!=e.elem[e.prop]&&null==e.elem.style[e.prop]?e.elem[e.prop]:(t=S.css(e.elem,e.prop,""))&&"auto"!==t?t:0},set:function(e){S.fx.step[e.prop]?S.fx.step[e.prop](e):1!==e.elem.nodeType||!S.cssHooks[e.prop]&&null==e.elem.style[Ve(e.prop)]?e.elem[e.prop]=e.now:S.style(e.elem,e.prop,e.now+e.unit)}}}).scrollTop=et.propHooks.scrollLeft={set:function(e){e.elem.nodeType&&e.elem.parentNode&&(e.elem[e.prop]=e.now)}},S.easing={linear:function(e){return e},swing:function(e){return.5-Math.cos(e*Math.PI)/2},_default:"swing"},S.fx=et.prototype.init,S.fx.step={};var tt,nt,rt,it,ot=/^(?:toggle|show|hide)$/,at=/queueHooks$/;function st(){nt&&(!1===E.hidden&&C.requestAnimationFrame?C.requestAnimationFrame(st):C.setTimeout(st,S.fx.interval),S.fx.tick())}function ut(){return C.setTimeout(function(){tt=void 0}),tt=Date.now()}function lt(e,t){var n,r=0,i={height:e};for(t=t?1:0;r<4;r+=2-t)i["margin"+(n=ne[r])]=i["padding"+n]=e;return t&&(i.opacity=i.width=e),i}function ct(e,t,n){for(var r,i=(ft.tweeners[t]||[]).concat(ft.tweeners["*"]),o=0,a=i.length;o<a;o++)if(r=i[o].call(n,t,e))return r}function ft(o,e,t){var n,a,r=0,i=ft.prefilters.length,s=S.Deferred().always(function(){delete u.elem}),u=function(){if(a)return!1;for(var e=tt||ut(),t=Math.max(0,l.startTime+l.duration-e),n=1-(t/l.duration||0),r=0,i=l.tweens.length;r<i;r++)l.tweens[r].run(n);return s.notifyWith(o,[l,n,t]),n<1&&i?t:(i||s.notifyWith(o,[l,1,0]),s.resolveWith(o,[l]),!1)},l=s.promise({elem:o,props:S.extend({},e),opts:S.extend(!0,{specialEasing:{},easing:S.easing._default},t),originalProperties:e,originalOptions:t,startTime:tt||ut(),duration:t.duration,tweens:[],createTween:function(e,t){var n=S.Tween(o,l.opts,e,t,l.opts.specialEasing[e]||l.opts.easing);return l.tweens.push(n),n},stop:function(e){var t=0,n=e?l.tweens.length:0;if(a)return this;for(a=!0;t<n;t++)l.tweens[t].run(1);return e?(s.notifyWith(o,[l,1,0]),s.resolveWith(o,[l,e])):s.rejectWith(o,[l,e]),this}}),c=l.props;for(!function(e,t){var n,r,i,o,a;for(n in e)if(i=t[r=X(n)],o=e[n],Array.isArray(o)&&(i=o[1],o=e[n]=o[0]),n!==r&&(e[r]=o,delete e[n]),(a=S.cssHooks[r])&&"expand"in a)for(n in o=a.expand(o),delete e[r],o)n in e||(e[n]=o[n],t[n]=i);else t[r]=i}(c,l.opts.specialEasing);r<i;r++)if(n=ft.prefilters[r].call(l,o,c,l.opts))return m(n.stop)&&(S._queueHooks(l.elem,l.opts.queue).stop=n.stop.bind(n)),n;return S.map(c,ct,l),m(l.opts.start)&&l.opts.start.call(o,l),l.progress(l.opts.progress).done(l.opts.done,l.opts.complete).fail(l.opts.fail).always(l.opts.always),S.fx.timer(S.extend(u,{elem:o,anim:l,queue:l.opts.queue})),l}S.Animation=S.extend(ft,{tweeners:{"*":[function(e,t){var n=this.createTween(e,t);return se(n.elem,e,te.exec(t),n),n}]},tweener:function(e,t){m(e)?(t=e,e=["*"]):e=e.match(P);for(var n,r=0,i=e.length;r<i;r++)n=e[r],ft.tweeners[n]=ft.tweeners[n]||[],ft.tweeners[n].unshift(t)},prefilters:[function(e,t,n){var r,i,o,a,s,u,l,c,f="width"in t||"height"in t,p=this,d={},h=e.style,g=e.nodeType&&ae(e),y=Y.get(e,"fxshow");for(r in n.queue||(null==(a=S._queueHooks(e,"fx")).unqueued&&(a.unqueued=0,s=a.empty.fire,a.empty.fire=function(){a.unqueued||s()}),a.unqueued++,p.always(function(){p.always(function(){a.unqueued--,S.queue(e,"fx").length||a.empty.fire()})})),t)if(i=t[r],ot.test(i)){if(delete t[r],o=o||"toggle"===i,i===(g?"hide":"show")){if("show"!==i||!y||void 0===y[r])continue;g=!0}d[r]=y&&y[r]||S.style(e,r)}if((u=!S.isEmptyObject(t))||!S.isEmptyObject(d))for(r in f&&1===e.nodeType&&(n.overflow=[h.overflow,h.overflowX,h.overflowY],null==(l=y&&y.display)&&(l=Y.get(e,"display")),"none"===(c=S.css(e,"display"))&&(l?c=l:(le([e],!0),l=e.style.display||l,c=S.css(e,"display"),le([e]))),("inline"===c||"inline-block"===c&&null!=l)&&"none"===S.css(e,"float")&&(u||(p.done(function(){h.display=l}),null==l&&(c=h.display,l="none"===c?"":c)),h.display="inline-block")),n.overflow&&(h.overflow="hidden",p.always(function(){h.overflow=n.overflow[0],h.overflowX=n.overflow[1],h.overflowY=n.overflow[2]})),u=!1,d)u||(y?"hidden"in y&&(g=y.hidden):y=Y.access(e,"fxshow",{display:l}),o&&(y.hidden=!g),g&&le([e],!0),p.done(function(){for(r in g||le([e]),Y.remove(e,"fxshow"),d)S.style(e,r,d[r])})),u=ct(g?y[r]:0,r,p),r in y||(y[r]=u.start,g&&(u.end=u.start,u.start=0))}],prefilter:function(e,t){t?ft.prefilters.unshift(e):ft.prefilters.push(e)}}),S.speed=function(e,t,n){var r=e&&"object"==typeof e?S.extend({},e):{complete:n||!n&&t||m(e)&&e,duration:e,easing:n&&t||t&&!m(t)&&t};return S.fx.off?r.duration=0:"number"!=typeof r.duration&&(r.duration in S.fx.speeds?r.duration=S.fx.speeds[r.duration]:r.duration=S.fx.speeds._default),null!=r.queue&&!0!==r.queue||(r.queue="fx"),r.old=r.complete,r.complete=function(){m(r.old)&&r.old.call(this),r.queue&&S.dequeue(this,r.queue)},r},S.fn.extend({fadeTo:function(e,t,n,r){return this.filter(ae).css("opacity",0).show().end().animate({opacity:t},e,n,r)},animate:function(t,e,n,r){var i=S.isEmptyObject(t),o=S.speed(e,n,r),a=function(){var e=ft(this,S.extend({},t),o);(i||Y.get(this,"finish"))&&e.stop(!0)};return a.finish=a,i||!1===o.queue?this.each(a):this.queue(o.queue,a)},stop:function(i,e,o){var a=function(e){var t=e.stop;delete e.stop,t(o)};return"string"!=typeof i&&(o=e,e=i,i=void 0),e&&this.queue(i||"fx",[]),this.each(function(){var e=!0,t=null!=i&&i+"queueHooks",n=S.timers,r=Y.get(this);if(t)r[t]&&r[t].stop&&a(r[t]);else for(t in r)r[t]&&r[t].stop&&at.test(t)&&a(r[t]);for(t=n.length;t--;)n[t].elem!==this||null!=i&&n[t].queue!==i||(n[t].anim.stop(o),e=!1,n.splice(t,1));!e&&o||S.dequeue(this,i)})},finish:function(a){return!1!==a&&(a=a||"fx"),this.each(function(){var e,t=Y.get(this),n=t[a+"queue"],r=t[a+"queueHooks"],i=S.timers,o=n?n.length:0;for(t.finish=!0,S.queue(this,a,[]),r&&r.stop&&r.stop.call(this,!0),e=i.length;e--;)i[e].elem===this&&i[e].queue===a&&(i[e].anim.stop(!0),i.splice(e,1));for(e=0;e<o;e++)n[e]&&n[e].finish&&n[e].finish.call(this);delete t.finish})}}),S.each(["toggle","show","hide"],function(e,r){var i=S.fn[r];S.fn[r]=function(e,t,n){return null==e||"boolean"==typeof e?i.apply(this,arguments):this.animate(lt(r,!0),e,t,n)}}),S.each({slideDown:lt("show"),slideUp:lt("hide"),slideToggle:lt("toggle"),fadeIn:{opacity:"show"},fadeOut:{opacity:"hide"},fadeToggle:{opacity:"toggle"}},function(e,r){S.fn[e]=function(e,t,n){return this.animate(r,e,t,n)}}),S.timers=[],S.fx.tick=function(){var e,t=0,n=S.timers;for(tt=Date.now();t<n.length;t++)(e=n[t])()||n[t]!==e||n.splice(t--,1);n.length||S.fx.stop(),tt=void 0},S.fx.timer=function(e){S.timers.push(e),S.fx.start()},S.fx.interval=13,S.fx.start=function(){nt||(nt=!0,st())},S.fx.stop=function(){nt=null},S.fx.speeds={slow:600,fast:200,_default:400},S.fn.delay=function(r,e){return r=S.fx&&S.fx.speeds[r]||r,e=e||"fx",this.queue(e,function(e,t){var n=C.setTimeout(e,r);t.stop=function(){C.clearTimeout(n)}})},rt=E.createElement("input"),it=E.createElement("select").appendChild(E.createElement("option")),rt.type="checkbox",v.checkOn=""!==rt.value,v.optSelected=it.selected,(rt=E.createElement("input")).value="t",rt.type="radio",v.radioValue="t"===rt.value;var pt,dt=S.expr.attrHandle;S.fn.extend({attr:function(e,t){return B(this,S.attr,e,t,1<arguments.length)},removeAttr:function(e){return this.each(function(){S.removeAttr(this,e)})}}),S.extend({attr:function(e,t,n){var r,i,o=e.nodeType;if(3!==o&&8!==o&&2!==o)return"undefined"==typeof e.getAttribute?S.prop(e,t,n):(1===o&&S.isXMLDoc(e)||(i=S.attrHooks[t.toLowerCase()]||(S.expr.match.bool.test(t)?pt:void 0)),void 0!==n?null===n?void S.removeAttr(e,t):i&&"set"in i&&void 0!==(r=i.set(e,n,t))?r:(e.setAttribute(t,n+""),n):i&&"get"in i&&null!==(r=i.get(e,t))?r:null==(r=S.find.attr(e,t))?void 0:r)},attrHooks:{type:{set:function(e,t){if(!v.radioValue&&"radio"===t&&A(e,"input")){var n=e.value;return e.setAttribute("type",t),n&&(e.value=n),t}}}},removeAttr:function(e,t){var n,r=0,i=t&&t.match(P);if(i&&1===e.nodeType)while(n=i[r++])e.removeAttribute(n)}}),pt={set:function(e,t,n){return!1===t?S.removeAttr(e,n):e.setAttribute(n,n),n}},S.each(S.expr.match.bool.source.match(/\w+/g),function(e,t){var a=dt[t]||S.find.attr;dt[t]=function(e,t,n){var r,i,o=t.toLowerCase();return n||(i=dt[o],dt[o]=r,r=null!=a(e,t,n)?o:null,dt[o]=i),r}});var ht=/^(?:input|select|textarea|button)$/i,gt=/^(?:a|area)$/i;function yt(e){return(e.match(P)||[]).join(" ")}function vt(e){return e.getAttribute&&e.getAttribute("class")||""}function mt(e){return Array.isArray(e)?e:"string"==typeof e&&e.match(P)||[]}S.fn.extend({prop:function(e,t){return B(this,S.prop,e,t,1<arguments.length)},removeProp:function(e){return this.each(function(){delete this[S.propFix[e]||e]})}}),S.extend({prop:function(e,t,n){var r,i,o=e.nodeType;if(3!==o&&8!==o&&2!==o)return 1===o&&S.isXMLDoc(e)||(t=S.propFix[t]||t,i=S.propHooks[t]),void 0!==n?i&&"set"in i&&void 0!==(r=i.set(e,n,t))?r:e[t]=n:i&&"get"in i&&null!==(r=i.get(e,t))?r:e[t]},propHooks:{tabIndex:{get:function(e){var t=S.find.attr(e,"tabindex");return t?parseInt(t,10):ht.test(e.nodeName)||gt.test(e.nodeName)&&e.href?0:-1}}},propFix:{"for":"htmlFor","class":"className"}}),v.optSelected||(S.propHooks.selected={get:function(e){var t=e.parentNode;return t&&t.parentNode&&t.parentNode.selectedIndex,null},set:function(e){var t=e.parentNode;t&&(t.selectedIndex,t.parentNode&&t.parentNode.selectedIndex)}}),S.each(["tabIndex","readOnly","maxLength","cellSpacing","cellPadding","rowSpan","colSpan","useMap","frameBorder","contentEditable"],function(){S.propFix[this.toLowerCase()]=this}),S.fn.extend({addClass:function(t){var e,n,r,i,o,a;return m(t)?this.each(function(e){S(this).addClass(t.call(this,e,vt(this)))}):(e=mt(t)).length?this.each(function(){if(r=vt(this),n=1===this.nodeType&&" "+yt(r)+" "){for(o=0;o<e.length;o++)i=e[o],n.indexOf(" "+i+" ")<0&&(n+=i+" ");a=yt(n),r!==a&&this.setAttribute("class",a)}}):this},removeClass:function(t){var e,n,r,i,o,a;return m(t)?this.each(function(e){S(this).removeClass(t.call(this,e,vt(this)))}):arguments.length?(e=mt(t)).length?this.each(function(){if(r=vt(this),n=1===this.nodeType&&" "+yt(r)+" "){for(o=0;o<e.length;o++){i=e[o];while(-1<n.indexOf(" "+i+" "))n=n.replace(" "+i+" "," ")}a=yt(n),r!==a&&this.setAttribute("class",a)}}):this:this.attr("class","")},toggleClass:function(t,n){var e,r,i,o,a=typeof t,s="string"===a||Array.isArray(t);return m(t)?this.each(function(e){S(this).toggleClass(t.call(this,e,vt(this),n),n)}):"boolean"==typeof n&&s?n?this.addClass(t):this.removeClass(t):(e=mt(t),this.each(function(){if(s)for(o=S(this),i=0;i<e.length;i++)r=e[i],o.hasClass(r)?o.removeClass(r):o.addClass(r);else void 0!==t&&"boolean"!==a||((r=vt(this))&&Y.set(this,"__className__",r),this.setAttribute&&this.setAttribute("class",r||!1===t?"":Y.get(this,"__className__")||""))}))},hasClass:function(e){var t,n,r=0;t=" "+e+" ";while(n=this[r++])if(1===n.nodeType&&-1<(" "+yt(vt(n))+" ").indexOf(t))return!0;return!1}});var xt=/\r/g;S.fn.extend({val:function(n){var r,e,i,t=this[0];return arguments.length?(i=m(n),this.each(function(e){var t;1===this.nodeType&&(null==(t=i?n.call(this,e,S(this).val()):n)?t="":"number"==typeof t?t+="":Array.isArray(t)&&(t=S.map(t,function(e){return null==e?"":e+""})),(r=S.valHooks[this.type]||S.valHooks[this.nodeName.toLowerCase()])&&"set"in r&&void 0!==r.set(this,t,"value")||(this.value=t))})):t?(r=S.valHooks[t.type]||S.valHooks[t.nodeName.toLowerCase()])&&"get"in r&&void 0!==(e=r.get(t,"value"))?e:"string"==typeof(e=t.value)?e.replace(xt,""):null==e?"":e:void 0}}),S.extend({valHooks:{option:{get:function(e){var t=S.find.attr(e,"value");return null!=t?t:yt(S.text(e))}},select:{get:function(e){var t,n,r,i=e.options,o=e.selectedIndex,a="select-one"===e.type,s=a?null:[],u=a?o+1:i.length;for(r=o<0?u:a?o:0;r<u;r++)if(((n=i[r]).selected||r===o)&&!n.disabled&&(!n.parentNode.disabled||!A(n.parentNode,"optgroup"))){if(t=S(n).val(),a)return t;s.push(t)}return s},set:function(e,t){var n,r,i=e.options,o=S.makeArray(t),a=i.length;while(a--)((r=i[a]).selected=-1<S.inArray(S.valHooks.option.get(r),o))&&(n=!0);return n||(e.selectedIndex=-1),o}}}}),S.each(["radio","checkbox"],function(){S.valHooks[this]={set:function(e,t){if(Array.isArray(t))return e.checked=-1<S.inArray(S(e).val(),t)}},v.checkOn||(S.valHooks[this].get=function(e){return null===e.getAttribute("value")?"on":e.value})}),v.focusin="onfocusin"in C;var bt=/^(?:focusinfocus|focusoutblur)$/,wt=function(e){e.stopPropagation()};S.extend(S.event,{trigger:function(e,t,n,r){var i,o,a,s,u,l,c,f,p=[n||E],d=y.call(e,"type")?e.type:e,h=y.call(e,"namespace")?e.namespace.split("."):[];if(o=f=a=n=n||E,3!==n.nodeType&&8!==n.nodeType&&!bt.test(d+S.event.triggered)&&(-1<d.indexOf(".")&&(d=(h=d.split(".")).shift(),h.sort()),u=d.indexOf(":")<0&&"on"+d,(e=e[S.expando]?e:new S.Event(d,"object"==typeof e&&e)).isTrigger=r?2:3,e.namespace=h.join("."),e.rnamespace=e.namespace?new RegExp("(^|\\.)"+h.join("\\.(?:.*\\.|)")+"(\\.|$)"):null,e.result=void 0,e.target||(e.target=n),t=null==t?[e]:S.makeArray(t,[e]),c=S.event.special[d]||{},r||!c.trigger||!1!==c.trigger.apply(n,t))){if(!r&&!c.noBubble&&!x(n)){for(s=c.delegateType||d,bt.test(s+d)||(o=o.parentNode);o;o=o.parentNode)p.push(o),a=o;a===(n.ownerDocument||E)&&p.push(a.defaultView||a.parentWindow||C)}i=0;while((o=p[i++])&&!e.isPropagationStopped())f=o,e.type=1<i?s:c.bindType||d,(l=(Y.get(o,"events")||Object.create(null))[e.type]&&Y.get(o,"handle"))&&l.apply(o,t),(l=u&&o[u])&&l.apply&&V(o)&&(e.result=l.apply(o,t),!1===e.result&&e.preventDefault());return e.type=d,r||e.isDefaultPrevented()||c._default&&!1!==c._default.apply(p.pop(),t)||!V(n)||u&&m(n[d])&&!x(n)&&((a=n[u])&&(n[u]=null),S.event.triggered=d,e.isPropagationStopped()&&f.addEventListener(d,wt),n[d](),e.isPropagationStopped()&&f.removeEventListener(d,wt),S.event.triggered=void 0,a&&(n[u]=a)),e.result}},simulate:function(e,t,n){var r=S.extend(new S.Event,n,{type:e,isSimulated:!0});S.event.trigger(r,null,t)}}),S.fn.extend({trigger:function(e,t){return this.each(function(){S.event.trigger(e,t,this)})},triggerHandler:function(e,t){var n=this[0];if(n)return S.event.trigger(e,t,n,!0)}}),v.focusin||S.each({focus:"focusin",blur:"focusout"},function(n,r){var i=function(e){S.event.simulate(r,e.target,S.event.fix(e))};S.event.special[r]={setup:function(){var e=this.ownerDocument||this.document||this,t=Y.access(e,r);t||e.addEventListener(n,i,!0),Y.access(e,r,(t||0)+1)},teardown:function(){var e=this.ownerDocument||this.document||this,t=Y.access(e,r)-1;t?Y.access(e,r,t):(e.removeEventListener(n,i,!0),Y.remove(e,r))}}});var Tt=C.location,Ct={guid:Date.now()},Et=/\?/;S.parseXML=function(e){var t,n;if(!e||"string"!=typeof e)return null;try{t=(new C.DOMParser).parseFromString(e,"text/xml")}catch(e){}return n=t&&t.getElementsByTagName("parsererror")[0],t&&!n||S.error("Invalid XML: "+(n?S.map(n.childNodes,function(e){return e.textContent}).join("\n"):e)),t};var St=/\[\]$/,kt=/\r?\n/g,At=/^(?:submit|button|image|reset|file)$/i,Nt=/^(?:input|select|textarea|keygen)/i;function jt(n,e,r,i){var t;if(Array.isArray(e))S.each(e,function(e,t){r||St.test(n)?i(n,t):jt(n+"["+("object"==typeof t&&null!=t?e:"")+"]",t,r,i)});else if(r||"object"!==w(e))i(n,e);else for(t in e)jt(n+"["+t+"]",e[t],r,i)}S.param=function(e,t){var n,r=[],i=function(e,t){var n=m(t)?t():t;r[r.length]=encodeURIComponent(e)+"="+encodeURIComponent(null==n?"":n)};if(null==e)return"";if(Array.isArray(e)||e.jquery&&!S.isPlainObject(e))S.each(e,function(){i(this.name,this.value)});else for(n in e)jt(n,e[n],t,i);return r.join("&")},S.fn.extend({serialize:function(){return S.param(this.serializeArray())},serializeArray:function(){return this.map(function(){var e=S.prop(this,"elements");return e?S.makeArray(e):this}).filter(function(){var e=this.type;return this.name&&!S(this).is(":disabled")&&Nt.test(this.nodeName)&&!At.test(e)&&(this.checked||!pe.test(e))}).map(function(e,t){var n=S(this).val();return null==n?null:Array.isArray(n)?S.map(n,function(e){return{name:t.name,value:e.replace(kt,"\r\n")}}):{name:t.name,value:n.replace(kt,"\r\n")}}).get()}});var Dt=/%20/g,qt=/#.*$/,Lt=/([?&])_=[^&]*/,Ht=/^(.*?):[ \t]*([^\r\n]*)$/gm,Ot=/^(?:GET|HEAD)$/,Pt=/^\/\//,Rt={},Mt={},It="*/".concat("*"),Wt=E.createElement("a");function Ft(o){return function(e,t){"string"!=typeof e&&(t=e,e="*");var n,r=0,i=e.toLowerCase().match(P)||[];if(m(t))while(n=i[r++])"+"===n[0]?(n=n.slice(1)||"*",(o[n]=o[n]||[]).unshift(t)):(o[n]=o[n]||[]).push(t)}}function $t(t,i,o,a){var s={},u=t===Mt;function l(e){var r;return s[e]=!0,S.each(t[e]||[],function(e,t){var n=t(i,o,a);return"string"!=typeof n||u||s[n]?u?!(r=n):void 0:(i.dataTypes.unshift(n),l(n),!1)}),r}return l(i.dataTypes[0])||!s["*"]&&l("*")}function Bt(e,t){var n,r,i=S.ajaxSettings.flatOptions||{};for(n in t)void 0!==t[n]&&((i[n]?e:r||(r={}))[n]=t[n]);return r&&S.extend(!0,e,r),e}Wt.href=Tt.href,S.extend({active:0,lastModified:{},etag:{},ajaxSettings:{url:Tt.href,type:"GET",isLocal:/^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Tt.protocol),global:!0,processData:!0,async:!0,contentType:"application/x-www-form-urlencoded; charset=UTF-8",accepts:{"*":It,text:"text/plain",html:"text/html",xml:"application/xml, text/xml",json:"application/json, text/javascript"},contents:{xml:/\bxml\b/,html:/\bhtml/,json:/\bjson\b/},responseFields:{xml:"responseXML",text:"responseText",json:"responseJSON"},converters:{"* text":String,"text html":!0,"text json":JSON.parse,"text xml":S.parseXML},flatOptions:{url:!0,context:!0}},ajaxSetup:function(e,t){return t?Bt(Bt(e,S.ajaxSettings),t):Bt(S.ajaxSettings,e)},ajaxPrefilter:Ft(Rt),ajaxTransport:Ft(Mt),ajax:function(e,t){"object"==typeof e&&(t=e,e=void 0),t=t||{};var c,f,p,n,d,r,h,g,i,o,y=S.ajaxSetup({},t),v=y.context||y,m=y.context&&(v.nodeType||v.jquery)?S(v):S.event,x=S.Deferred(),b=S.Callbacks("once memory"),w=y.statusCode||{},a={},s={},u="canceled",T={readyState:0,getResponseHeader:function(e){var t;if(h){if(!n){n={};while(t=Ht.exec(p))n[t[1].toLowerCase()+" "]=(n[t[1].toLowerCase()+" "]||[]).concat(t[2])}t=n[e.toLowerCase()+" "]}return null==t?null:t.join(", ")},getAllResponseHeaders:function(){return h?p:null},setRequestHeader:function(e,t){return null==h&&(e=s[e.toLowerCase()]=s[e.toLowerCase()]||e,a[e]=t),this},overrideMimeType:function(e){return null==h&&(y.mimeType=e),this},statusCode:function(e){var t;if(e)if(h)T.always(e[T.status]);else for(t in e)w[t]=[w[t],e[t]];return this},abort:function(e){var t=e||u;return c&&c.abort(t),l(0,t),this}};if(x.promise(T),y.url=((e||y.url||Tt.href)+"").replace(Pt,Tt.protocol+"//"),y.type=t.method||t.type||y.method||y.type,y.dataTypes=(y.dataType||"*").toLowerCase().match(P)||[""],null==y.crossDomain){r=E.createElement("a");try{r.href=y.url,r.href=r.href,y.crossDomain=Wt.protocol+"//"+Wt.host!=r.protocol+"//"+r.host}catch(e){y.crossDomain=!0}}if(y.data&&y.processData&&"string"!=typeof y.data&&(y.data=S.param(y.data,y.traditional)),$t(Rt,y,t,T),h)return T;for(i in(g=S.event&&y.global)&&0==S.active++&&S.event.trigger("ajaxStart"),y.type=y.type.toUpperCase(),y.hasContent=!Ot.test(y.type),f=y.url.replace(qt,""),y.hasContent?y.data&&y.processData&&0===(y.contentType||"").indexOf("application/x-www-form-urlencoded")&&(y.data=y.data.replace(Dt,"+")):(o=y.url.slice(f.length),y.data&&(y.processData||"string"==typeof y.data)&&(f+=(Et.test(f)?"&":"?")+y.data,delete y.data),!1===y.cache&&(f=f.replace(Lt,"$1"),o=(Et.test(f)?"&":"?")+"_="+Ct.guid+++o),y.url=f+o),y.ifModified&&(S.lastModified[f]&&T.setRequestHeader("If-Modified-Since",S.lastModified[f]),S.etag[f]&&T.setRequestHeader("If-None-Match",S.etag[f])),(y.data&&y.hasContent&&!1!==y.contentType||t.contentType)&&T.setRequestHeader("Content-Type",y.contentType),T.setRequestHeader("Accept",y.dataTypes[0]&&y.accepts[y.dataTypes[0]]?y.accepts[y.dataTypes[0]]+("*"!==y.dataTypes[0]?", "+It+"; q=0.01":""):y.accepts["*"]),y.headers)T.setRequestHeader(i,y.headers[i]);if(y.beforeSend&&(!1===y.beforeSend.call(v,T,y)||h))return T.abort();if(u="abort",b.add(y.complete),T.done(y.success),T.fail(y.error),c=$t(Mt,y,t,T)){if(T.readyState=1,g&&m.trigger("ajaxSend",[T,y]),h)return T;y.async&&0<y.timeout&&(d=C.setTimeout(function(){T.abort("timeout")},y.timeout));try{h=!1,c.send(a,l)}catch(e){if(h)throw e;l(-1,e)}}else l(-1,"No Transport");function l(e,t,n,r){var i,o,a,s,u,l=t;h||(h=!0,d&&C.clearTimeout(d),c=void 0,p=r||"",T.readyState=0<e?4:0,i=200<=e&&e<300||304===e,n&&(s=function(e,t,n){var r,i,o,a,s=e.contents,u=e.dataTypes;while("*"===u[0])u.shift(),void 0===r&&(r=e.mimeType||t.getResponseHeader("Content-Type"));if(r)for(i in s)if(s[i]&&s[i].test(r)){u.unshift(i);break}if(u[0]in n)o=u[0];else{for(i in n){if(!u[0]||e.converters[i+" "+u[0]]){o=i;break}a||(a=i)}o=o||a}if(o)return o!==u[0]&&u.unshift(o),n[o]}(y,T,n)),!i&&-1<S.inArray("script",y.dataTypes)&&S.inArray("json",y.dataTypes)<0&&(y.converters["text script"]=function(){}),s=function(e,t,n,r){var i,o,a,s,u,l={},c=e.dataTypes.slice();if(c[1])for(a in e.converters)l[a.toLowerCase()]=e.converters[a];o=c.shift();while(o)if(e.responseFields[o]&&(n[e.responseFields[o]]=t),!u&&r&&e.dataFilter&&(t=e.dataFilter(t,e.dataType)),u=o,o=c.shift())if("*"===o)o=u;else if("*"!==u&&u!==o){if(!(a=l[u+" "+o]||l["* "+o]))for(i in l)if((s=i.split(" "))[1]===o&&(a=l[u+" "+s[0]]||l["* "+s[0]])){!0===a?a=l[i]:!0!==l[i]&&(o=s[0],c.unshift(s[1]));break}if(!0!==a)if(a&&e["throws"])t=a(t);else try{t=a(t)}catch(e){return{state:"parsererror",error:a?e:"No conversion from "+u+" to "+o}}}return{state:"success",data:t}}(y,s,T,i),i?(y.ifModified&&((u=T.getResponseHeader("Last-Modified"))&&(S.lastModified[f]=u),(u=T.getResponseHeader("etag"))&&(S.etag[f]=u)),204===e||"HEAD"===y.type?l="nocontent":304===e?l="notmodified":(l=s.state,o=s.data,i=!(a=s.error))):(a=l,!e&&l||(l="error",e<0&&(e=0))),T.status=e,T.statusText=(t||l)+"",i?x.resolveWith(v,[o,l,T]):x.rejectWith(v,[T,l,a]),T.statusCode(w),w=void 0,g&&m.trigger(i?"ajaxSuccess":"ajaxError",[T,y,i?o:a]),b.fireWith(v,[T,l]),g&&(m.trigger("ajaxComplete",[T,y]),--S.active||S.event.trigger("ajaxStop")))}return T},getJSON:function(e,t,n){return S.get(e,t,n,"json")},getScript:function(e,t){return S.get(e,void 0,t,"script")}}),S.each(["get","post"],function(e,i){S[i]=function(e,t,n,r){return m(t)&&(r=r||n,n=t,t=void 0),S.ajax(S.extend({url:e,type:i,dataType:r,data:t,success:n},S.isPlainObject(e)&&e))}}),S.ajaxPrefilter(function(e){var t;for(t in e.headers)"content-type"===t.toLowerCase()&&(e.contentType=e.headers[t]||"")}),S._evalUrl=function(e,t,n){return S.ajax({url:e,type:"GET",dataType:"script",cache:!0,async:!1,global:!1,converters:{"text script":function(){}},dataFilter:function(e){S.globalEval(e,t,n)}})},S.fn.extend({wrapAll:function(e){var t;return this[0]&&(m(e)&&(e=e.call(this[0])),t=S(e,this[0].ownerDocument).eq(0).clone(!0),this[0].parentNode&&t.insertBefore(this[0]),t.map(function(){var e=this;while(e.firstElementChild)e=e.firstElementChild;return e}).append(this)),this},wrapInner:function(n){return m(n)?this.each(function(e){S(this).wrapInner(n.call(this,e))}):this.each(function(){var e=S(this),t=e.contents();t.length?t.wrapAll(n):e.append(n)})},wrap:function(t){var n=m(t);return this.each(function(e){S(this).wrapAll(n?t.call(this,e):t)})},unwrap:function(e){return this.parent(e).not("body").each(function(){S(this).replaceWith(this.childNodes)}),this}}),S.expr.pseudos.hidden=function(e){return!S.expr.pseudos.visible(e)},S.expr.pseudos.visible=function(e){return!!(e.offsetWidth||e.offsetHeight||e.getClientRects().length)},S.ajaxSettings.xhr=function(){try{return new C.XMLHttpRequest}catch(e){}};var _t={0:200,1223:204},zt=S.ajaxSettings.xhr();v.cors=!!zt&&"withCredentials"in zt,v.ajax=zt=!!zt,S.ajaxTransport(function(i){var o,a;if(v.cors||zt&&!i.crossDomain)return{send:function(e,t){var n,r=i.xhr();if(r.open(i.type,i.url,i.async,i.username,i.password),i.xhrFields)for(n in i.xhrFields)r[n]=i.xhrFields[n];for(n in i.mimeType&&r.overrideMimeType&&r.overrideMimeType(i.mimeType),i.crossDomain||e["X-Requested-With"]||(e["X-Requested-With"]="XMLHttpRequest"),e)r.setRequestHeader(n,e[n]);o=function(e){return function(){o&&(o=a=r.onload=r.onerror=r.onabort=r.ontimeout=r.onreadystatechange=null,"abort"===e?r.abort():"error"===e?"number"!=typeof r.status?t(0,"error"):t(r.status,r.statusText):t(_t[r.status]||r.status,r.statusText,"text"!==(r.responseType||"text")||"string"!=typeof r.responseText?{binary:r.response}:{text:r.responseText},r.getAllResponseHeaders()))}},r.onload=o(),a=r.onerror=r.ontimeout=o("error"),void 0!==r.onabort?r.onabort=a:r.onreadystatechange=function(){4===r.readyState&&C.setTimeout(function(){o&&a()})},o=o("abort");try{r.send(i.hasContent&&i.data||null)}catch(e){if(o)throw e}},abort:function(){o&&o()}}}),S.ajaxPrefilter(function(e){e.crossDomain&&(e.contents.script=!1)}),S.ajaxSetup({accepts:{script:"text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"},contents:{script:/\b(?:java|ecma)script\b/},converters:{"text script":function(e){return S.globalEval(e),e}}}),S.ajaxPrefilter("script",function(e){void 0===e.cache&&(e.cache=!1),e.crossDomain&&(e.type="GET")}),S.ajaxTransport("script",function(n){var r,i;if(n.crossDomain||n.scriptAttrs)return{send:function(e,t){r=S("<script>").attr(n.scriptAttrs||{}).prop({charset:n.scriptCharset,src:n.url}).on("load error",i=function(e){r.remove(),i=null,e&&t("error"===e.type?404:200,e.type)}),E.head.appendChild(r[0])},abort:function(){i&&i()}}});var Ut,Xt=[],Vt=/(=)\?(?=&|$)|\?\?/;S.ajaxSetup({jsonp:"callback",jsonpCallback:function(){var e=Xt.pop()||S.expando+"_"+Ct.guid++;return this[e]=!0,e}}),S.ajaxPrefilter("json jsonp",function(e,t,n){var r,i,o,a=!1!==e.jsonp&&(Vt.test(e.url)?"url":"string"==typeof e.data&&0===(e.contentType||"").indexOf("application/x-www-form-urlencoded")&&Vt.test(e.data)&&"data");if(a||"jsonp"===e.dataTypes[0])return r=e.jsonpCallback=m(e.jsonpCallback)?e.jsonpCallback():e.jsonpCallback,a?e[a]=e[a].replace(Vt,"$1"+r):!1!==e.jsonp&&(e.url+=(Et.test(e.url)?"&":"?")+e.jsonp+"="+r),e.converters["script json"]=function(){return o||S.error(r+" was not called"),o[0]},e.dataTypes[0]="json",i=C[r],C[r]=function(){o=arguments},n.always(function(){void 0===i?S(C).removeProp(r):C[r]=i,e[r]&&(e.jsonpCallback=t.jsonpCallback,Xt.push(r)),o&&m(i)&&i(o[0]),o=i=void 0}),"script"}),v.createHTMLDocument=((Ut=E.implementation.createHTMLDocument("").body).innerHTML="<form></form><form></form>",2===Ut.childNodes.length),S.parseHTML=function(e,t,n){return"string"!=typeof e?[]:("boolean"==typeof t&&(n=t,t=!1),t||(v.createHTMLDocument?((r=(t=E.implementation.createHTMLDocument("")).createElement("base")).href=E.location.href,t.head.appendChild(r)):t=E),o=!n&&[],(i=N.exec(e))?[t.createElement(i[1])]:(i=xe([e],t,o),o&&o.length&&S(o).remove(),S.merge([],i.childNodes)));var r,i,o},S.fn.load=function(e,t,n){var r,i,o,a=this,s=e.indexOf(" ");return-1<s&&(r=yt(e.slice(s)),e=e.slice(0,s)),m(t)?(n=t,t=void 0):t&&"object"==typeof t&&(i="POST"),0<a.length&&S.ajax({url:e,type:i||"GET",dataType:"html",data:t}).done(function(e){o=arguments,a.html(r?S("<div>").append(S.parseHTML(e)).find(r):e)}).always(n&&function(e,t){a.each(function(){n.apply(this,o||[e.responseText,t,e])})}),this},S.expr.pseudos.animated=function(t){return S.grep(S.timers,function(e){return t===e.elem}).length},S.offset={setOffset:function(e,t,n){var r,i,o,a,s,u,l=S.css(e,"position"),c=S(e),f={};"static"===l&&(e.style.position="relative"),s=c.offset(),o=S.css(e,"top"),u=S.css(e,"left"),("absolute"===l||"fixed"===l)&&-1<(o+u).indexOf("auto")?(a=(r=c.position()).top,i=r.left):(a=parseFloat(o)||0,i=parseFloat(u)||0),m(t)&&(t=t.call(e,n,S.extend({},s))),null!=t.top&&(f.top=t.top-s.top+a),null!=t.left&&(f.left=t.left-s.left+i),"using"in t?t.using.call(e,f):c.css(f)}},S.fn.extend({offset:function(t){if(arguments.length)return void 0===t?this:this.each(function(e){S.offset.setOffset(this,t,e)});var e,n,r=this[0];return r?r.getClientRects().length?(e=r.getBoundingClientRect(),n=r.ownerDocument.defaultView,{top:e.top+n.pageYOffset,left:e.left+n.pageXOffset}):{top:0,left:0}:void 0},position:function(){if(this[0]){var e,t,n,r=this[0],i={top:0,left:0};if("fixed"===S.css(r,"position"))t=r.getBoundingClientRect();else{t=this.offset(),n=r.ownerDocument,e=r.offsetParent||n.documentElement;while(e&&(e===n.body||e===n.documentElement)&&"static"===S.css(e,"position"))e=e.parentNode;e&&e!==r&&1===e.nodeType&&((i=S(e).offset()).top+=S.css(e,"borderTopWidth",!0),i.left+=S.css(e,"borderLeftWidth",!0))}return{top:t.top-i.top-S.css(r,"marginTop",!0),left:t.left-i.left-S.css(r,"marginLeft",!0)}}},offsetParent:function(){return this.map(function(){var e=this.offsetParent;while(e&&"static"===S.css(e,"position"))e=e.offsetParent;return e||re})}}),S.each({scrollLeft:"pageXOffset",scrollTop:"pageYOffset"},function(t,i){var o="pageYOffset"===i;S.fn[t]=function(e){return B(this,function(e,t,n){var r;if(x(e)?r=e:9===e.nodeType&&(r=e.defaultView),void 0===n)return r?r[i]:e[t];r?r.scrollTo(o?r.pageXOffset:n,o?n:r.pageYOffset):e[t]=n},t,e,arguments.length)}}),S.each(["top","left"],function(e,n){S.cssHooks[n]=_e(v.pixelPosition,function(e,t){if(t)return t=Be(e,n),Pe.test(t)?S(e).position()[n]+"px":t})}),S.each({Height:"height",Width:"width"},function(a,s){S.each({padding:"inner"+a,content:s,"":"outer"+a},function(r,o){S.fn[o]=function(e,t){var n=arguments.length&&(r||"boolean"!=typeof e),i=r||(!0===e||!0===t?"margin":"border");return B(this,function(e,t,n){var r;return x(e)?0===o.indexOf("outer")?e["inner"+a]:e.document.documentElement["client"+a]:9===e.nodeType?(r=e.documentElement,Math.max(e.body["scroll"+a],r["scroll"+a],e.body["offset"+a],r["offset"+a],r["client"+a])):void 0===n?S.css(e,t,i):S.style(e,t,n,i)},s,n?e:void 0,n)}})}),S.each(["ajaxStart","ajaxStop","ajaxComplete","ajaxError","ajaxSuccess","ajaxSend"],function(e,t){S.fn[t]=function(e){return this.on(t,e)}}),S.fn.extend({bind:function(e,t,n){return this.on(e,null,t,n)},unbind:function(e,t){return this.off(e,null,t)},delegate:function(e,t,n,r){return this.on(t,e,n,r)},undelegate:function(e,t,n){return 1===arguments.length?this.off(e,"**"):this.off(t,e||"**",n)},hover:function(e,t){return this.mouseenter(e).mouseleave(t||e)}}),S.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "),function(e,n){S.fn[n]=function(e,t){return 0<arguments.length?this.on(n,null,e,t):this.trigger(n)}});var Gt=/^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;S.proxy=function(e,t){var n,r,i;if("string"==typeof t&&(n=e[t],t=e,e=n),m(e))return r=s.call(arguments,2),(i=function(){return e.apply(t||this,r.concat(s.call(arguments)))}).guid=e.guid=e.guid||S.guid++,i},S.holdReady=function(e){e?S.readyWait++:S.ready(!0)},S.isArray=Array.isArray,S.parseJSON=JSON.parse,S.nodeName=A,S.isFunction=m,S.isWindow=x,S.camelCase=X,S.type=w,S.now=Date.now,S.isNumeric=function(e){var t=S.type(e);return("number"===t||"string"===t)&&!isNaN(e-parseFloat(e))},S.trim=function(e){return null==e?"":(e+"").replace(Gt,"$1")},"function"==typeof define&&define.amd&&define("jquery",[],function(){return S});var Yt=C.jQuery,Qt=C.$;return S.noConflict=function(e){return C.$===S&&(C.$=Qt),e&&C.jQuery===S&&(C.jQuery=Yt),S},"undefined"==typeof e&&(C.jQuery=C.$=S),S});

```

# source/lib/justified-gallery/css/justifiedGallery.min.css

```css
/*!
 * justifiedGallery - v3.8.1
 * http://miromannino.github.io/Justified-Gallery/
 * Copyright (c) 2020 Miro Mannino
 * Licensed under the MIT license.
 */
.justified-gallery {
  width: 100%;
  position: relative;
  overflow: hidden;
}
.justified-gallery > a,
.justified-gallery > div,
.justified-gallery > figure {
  position: absolute;
  display: inline-block;
  overflow: hidden;
  /* background: #888888; To have gray placeholders while the gallery is loading with waitThumbnailsLoad = false */
  filter: "alpha(opacity=10)";
  opacity: 0.1;
  margin: 0;
  padding: 0;
}
.justified-gallery > a > img,
.justified-gallery > div > img,
.justified-gallery > figure > img,
.justified-gallery > a > a > img,
.justified-gallery > div > a > img,
.justified-gallery > figure > a > img,
.justified-gallery > a > svg,
.justified-gallery > div > svg,
.justified-gallery > figure > svg,
.justified-gallery > a > a > svg,
.justified-gallery > div > a > svg,
.justified-gallery > figure > a > svg {
  position: absolute;
  top: 50%;
  left: 50%;
  margin: 0;
  padding: 0;
  border: none;
  filter: "alpha(opacity=0)";
  opacity: 0;
}
.justified-gallery > a > .jg-caption,
.justified-gallery > div > .jg-caption,
.justified-gallery > figure > .jg-caption {
  display: none;
  position: absolute;
  bottom: 0;
  padding: 5px;
  background-color: #000000;
  left: 0;
  right: 0;
  margin: 0;
  color: white;
  font-size: 12px;
  font-weight: 300;
  font-family: sans-serif;
}
.justified-gallery > a > .jg-caption.jg-caption-visible,
.justified-gallery > div > .jg-caption.jg-caption-visible,
.justified-gallery > figure > .jg-caption.jg-caption-visible {
  display: initial;
  filter: "alpha(opacity=70)";
  opacity: 0.7;
  -webkit-transition: opacity 500ms ease-in;
  -moz-transition: opacity 500ms ease-in;
  -o-transition: opacity 500ms ease-in;
  transition: opacity 500ms ease-in;
}
.justified-gallery > .jg-entry-visible {
  filter: "alpha(opacity=100)";
  opacity: 1;
  background: none;
}
.justified-gallery > .jg-entry-visible > img,
.justified-gallery > .jg-entry-visible > a > img,
.justified-gallery > .jg-entry-visible > svg,
.justified-gallery > .jg-entry-visible > a > svg {
  filter: "alpha(opacity=100)";
  opacity: 1;
  -webkit-transition: opacity 500ms ease-in;
  -moz-transition: opacity 500ms ease-in;
  -o-transition: opacity 500ms ease-in;
  transition: opacity 500ms ease-in;
}
.justified-gallery > .jg-filtered {
  display: none;
}
.justified-gallery > .jg-spinner {
  position: absolute;
  bottom: 0;
  margin-left: -24px;
  padding: 10px 0 10px 0;
  left: 50%;
  filter: "alpha(opacity=100)";
  opacity: 1;
  overflow: initial;
}
.justified-gallery > .jg-spinner > span {
  display: inline-block;
  filter: "alpha(opacity=0)";
  opacity: 0;
  width: 8px;
  height: 8px;
  margin: 0 4px 0 4px;
  background-color: #000;
  border-radius: 6px;
}

```

# source/lib/justified-gallery/js/jquery.justifiedGallery.min.js

```js
/*!
 * justifiedGallery - v3.8.1
 * http://miromannino.github.io/Justified-Gallery/
 * Copyright (c) 2020 Miro Mannino
 * Licensed under the MIT license.
 */

!function(e){"function"==typeof define&&define.amd?define(["jquery"],e):"object"==typeof module&&module.exports?module.exports=function(t,i){return void 0===i&&(i="undefined"!=typeof window?require("jquery"):require("jquery")(t)),e(i),i}:e(jQuery)}(function(l){var r=function(t,i){this.settings=i,this.checkSettings(),this.imgAnalyzerTimeout=null,this.entries=null,this.buildingRow={entriesBuff:[],width:0,height:0,aspectRatio:0},this.lastFetchedEntry=null,this.lastAnalyzedIndex=-1,this.yield={every:2,flushed:0},this.border=0<=i.border?i.border:i.margins,this.maxRowHeight=this.retrieveMaxRowHeight(),this.suffixRanges=this.retrieveSuffixRanges(),this.offY=this.border,this.rows=0,this.spinner={phase:0,timeSlot:150,$el:l('<div class="jg-spinner"><span></span><span></span><span></span></div>'),intervalId:null},this.scrollBarOn=!1,this.checkWidthIntervalId=null,this.galleryWidth=t.width(),this.$gallery=t};r.prototype.getSuffix=function(t,i){var e,s;for(e=i<t?t:i,s=0;s<this.suffixRanges.length;s++)if(e<=this.suffixRanges[s])return this.settings.sizeRangeSuffixes[this.suffixRanges[s]];return this.settings.sizeRangeSuffixes[this.suffixRanges[s-1]]},r.prototype.removeSuffix=function(t,i){return t.substring(0,t.length-i.length)},r.prototype.endsWith=function(t,i){return-1!==t.indexOf(i,t.length-i.length)},r.prototype.getUsedSuffix=function(t){for(var i in this.settings.sizeRangeSuffixes)if(this.settings.sizeRangeSuffixes.hasOwnProperty(i)){if(0===this.settings.sizeRangeSuffixes[i].length)continue;if(this.endsWith(t,this.settings.sizeRangeSuffixes[i]))return this.settings.sizeRangeSuffixes[i]}return""},r.prototype.newSrc=function(t,i,e,s){var n;if(this.settings.thumbnailPath)n=this.settings.thumbnailPath(t,i,e,s);else{var r=t.match(this.settings.extension),o=null!==r?r[0]:"";n=t.replace(this.settings.extension,""),n=this.removeSuffix(n,this.getUsedSuffix(n)),n+=this.getSuffix(i,e)+o}return n},r.prototype.showImg=function(t,i){this.settings.cssAnimation?(t.addClass("jg-entry-visible"),i&&i()):(t.stop().fadeTo(this.settings.imagesAnimationDuration,1,i),t.find(this.settings.imgSelector).stop().fadeTo(this.settings.imagesAnimationDuration,1,i))},r.prototype.extractImgSrcFromImage=function(t){var i=t.data("safe-src"),e="data-safe-src";return void 0===i&&(i=t.attr("src"),e="src"),t.data("jg.originalSrc",i),t.data("jg.src",i),t.data("jg.originalSrcLoc",e),i},r.prototype.imgFromEntry=function(t){var i=t.find(this.settings.imgSelector);return 0===i.length?null:i},r.prototype.captionFromEntry=function(t){var i=t.find("> .jg-caption");return 0===i.length?null:i},r.prototype.displayEntry=function(t,i,e,s,n,r){t.width(s),t.height(r),t.css("top",e),t.css("left",i);var o=this.imgFromEntry(t);if(null!==o){o.css("width",s),o.css("height",n),o.css("margin-left",-s/2),o.css("margin-top",-n/2);var a=o.data("jg.src");if(a){a=this.newSrc(a,s,n,o[0]),o.one("error",function(){this.resetImgSrc(o)});var h=function(){o.attr("src",a)};"skipped"===t.data("jg.loaded")&&a?this.onImageEvent(a,function(){this.showImg(t,h),t.data("jg.loaded",!0)}.bind(this)):this.showImg(t,h)}}else this.showImg(t);this.displayEntryCaption(t)},r.prototype.displayEntryCaption=function(t){var i=this.imgFromEntry(t);if(null!==i&&this.settings.captions){var e=this.captionFromEntry(t);if(null===e){var s=i.attr("alt");this.isValidCaption(s)||(s=t.attr("title")),this.isValidCaption(s)&&(e=l('<div class="jg-caption">'+s+"</div>"),t.append(e),t.data("jg.createdCaption",!0))}null!==e&&(this.settings.cssAnimation||e.stop().fadeTo(0,this.settings.captionSettings.nonVisibleOpacity),this.addCaptionEventsHandlers(t))}else this.removeCaptionEventsHandlers(t)},r.prototype.isValidCaption=function(t){return void 0!==t&&0<t.length},r.prototype.onEntryMouseEnterForCaption=function(t){var i=this.captionFromEntry(l(t.currentTarget));this.settings.cssAnimation?i.addClass("jg-caption-visible").removeClass("jg-caption-hidden"):i.stop().fadeTo(this.settings.captionSettings.animationDuration,this.settings.captionSettings.visibleOpacity)},r.prototype.onEntryMouseLeaveForCaption=function(t){var i=this.captionFromEntry(l(t.currentTarget));this.settings.cssAnimation?i.removeClass("jg-caption-visible").removeClass("jg-caption-hidden"):i.stop().fadeTo(this.settings.captionSettings.animationDuration,this.settings.captionSettings.nonVisibleOpacity)},r.prototype.addCaptionEventsHandlers=function(t){var i=t.data("jg.captionMouseEvents");void 0===i&&(i={mouseenter:l.proxy(this.onEntryMouseEnterForCaption,this),mouseleave:l.proxy(this.onEntryMouseLeaveForCaption,this)},t.on("mouseenter",void 0,void 0,i.mouseenter),t.on("mouseleave",void 0,void 0,i.mouseleave),t.data("jg.captionMouseEvents",i))},r.prototype.removeCaptionEventsHandlers=function(t){var i=t.data("jg.captionMouseEvents");void 0!==i&&(t.off("mouseenter",void 0,i.mouseenter),t.off("mouseleave",void 0,i.mouseleave),t.removeData("jg.captionMouseEvents"))},r.prototype.clearBuildingRow=function(){this.buildingRow.entriesBuff=[],this.buildingRow.aspectRatio=0,this.buildingRow.width=0},r.prototype.prepareBuildingRow=function(t,i){var e,s,n,r,o,a=!0,h=0,g=this.galleryWidth-2*this.border-(this.buildingRow.entriesBuff.length-1)*this.settings.margins,l=g/this.buildingRow.aspectRatio,u=this.settings.rowHeight,d=this.buildingRow.width/g>this.settings.justifyThreshold;if(i||t&&"hide"===this.settings.lastRow&&!d){for(e=0;e<this.buildingRow.entriesBuff.length;e++)s=this.buildingRow.entriesBuff[e],this.settings.cssAnimation?s.removeClass("jg-entry-visible"):(s.stop().fadeTo(0,.1),s.find("> img, > a > img").fadeTo(0,0));return-1}for(t&&!d&&"justify"!==this.settings.lastRow&&"hide"!==this.settings.lastRow&&(a=!1,0<this.rows&&(a=(u=(this.offY-this.border-this.settings.margins*this.rows)/this.rows)*this.buildingRow.aspectRatio/g>this.settings.justifyThreshold)),e=0;e<this.buildingRow.entriesBuff.length;e++)n=(s=this.buildingRow.entriesBuff[e]).data("jg.width")/s.data("jg.height"),o=a?(r=e===this.buildingRow.entriesBuff.length-1?g:l*n,l):(r=u*n,u),g-=Math.round(r),s.data("jg.jwidth",Math.round(r)),s.data("jg.jheight",Math.ceil(o)),(0===e||o<h)&&(h=o);return this.buildingRow.height=h,a},r.prototype.flushRow=function(t,i){var e,s,n,r=this.settings,o=this.border;if(s=this.prepareBuildingRow(t,i),i||t&&"hide"===r.lastRow&&-1===s)this.clearBuildingRow();else{if(this.maxRowHeight&&this.maxRowHeight<this.buildingRow.height&&(this.buildingRow.height=this.maxRowHeight),t&&("center"===r.lastRow||"right"===r.lastRow)){var a=this.galleryWidth-2*this.border-(this.buildingRow.entriesBuff.length-1)*r.margins;for(n=0;n<this.buildingRow.entriesBuff.length;n++)a-=(e=this.buildingRow.entriesBuff[n]).data("jg.jwidth");"center"===r.lastRow?o+=Math.round(a/2):"right"===r.lastRow&&(o+=a)}var h=this.buildingRow.entriesBuff.length-1;for(n=0;n<=h;n++)e=this.buildingRow.entriesBuff[this.settings.rtl?h-n:n],this.displayEntry(e,o,this.offY,e.data("jg.jwidth"),e.data("jg.jheight"),this.buildingRow.height),o+=e.data("jg.jwidth")+r.margins;this.galleryHeightToSet=this.offY+this.buildingRow.height+this.border,this.setGalleryTempHeight(this.galleryHeightToSet+this.getSpinnerHeight()),(!t||this.buildingRow.height<=r.rowHeight&&s)&&(this.offY+=this.buildingRow.height+r.margins,this.rows+=1,this.clearBuildingRow(),this.settings.triggerEvent.call(this,"jg.rowflush"))}};var i=0;r.prototype.rememberGalleryHeight=function(){i=this.$gallery.height(),this.$gallery.height(i)},r.prototype.setGalleryTempHeight=function(t){i=Math.max(t,i),this.$gallery.height(i)},r.prototype.setGalleryFinalHeight=function(t){i=t,this.$gallery.height(t)},r.prototype.checkWidth=function(){this.checkWidthIntervalId=setInterval(l.proxy(function(){if(this.$gallery.is(":visible")){var t=parseFloat(this.$gallery.width());Math.abs(t-this.galleryWidth)>this.settings.refreshSensitivity&&(this.galleryWidth=t,this.rewind(),this.rememberGalleryHeight(),this.startImgAnalyzer(!0))}},this),this.settings.refreshTime)},r.prototype.isSpinnerActive=function(){return null!==this.spinner.intervalId},r.prototype.getSpinnerHeight=function(){return this.spinner.$el.innerHeight()},r.prototype.stopLoadingSpinnerAnimation=function(){clearInterval(this.spinner.intervalId),this.spinner.intervalId=null,this.setGalleryTempHeight(this.$gallery.height()-this.getSpinnerHeight()),this.spinner.$el.detach()},r.prototype.startLoadingSpinnerAnimation=function(){var t=this.spinner,i=t.$el.find("span");clearInterval(t.intervalId),this.$gallery.append(t.$el),this.setGalleryTempHeight(this.offY+this.buildingRow.height+this.getSpinnerHeight()),t.intervalId=setInterval(function(){t.phase<i.length?i.eq(t.phase).fadeTo(t.timeSlot,1):i.eq(t.phase-i.length).fadeTo(t.timeSlot,0),t.phase=(t.phase+1)%(2*i.length)},t.timeSlot)},r.prototype.rewind=function(){this.lastFetchedEntry=null,this.lastAnalyzedIndex=-1,this.offY=this.border,this.rows=0,this.clearBuildingRow()},r.prototype.getSelectorWithoutSpinner=function(){return this.settings.selector+", div:not(.jg-spinner)"},r.prototype.getAllEntries=function(){var t=this.getSelectorWithoutSpinner();return this.$gallery.children(t).toArray()},r.prototype.updateEntries=function(t){var i;if(t&&null!=this.lastFetchedEntry){var e=this.getSelectorWithoutSpinner();i=l(this.lastFetchedEntry).nextAll(e).toArray()}else this.entries=[],i=this.getAllEntries();return 0<i.length&&(l.isFunction(this.settings.sort)?i=this.sortArray(i):this.settings.randomize&&(i=this.shuffleArray(i)),this.lastFetchedEntry=i[i.length-1],this.settings.filter?i=this.filterArray(i):this.resetFilters(i)),this.entries=this.entries.concat(i),!0},r.prototype.insertToGallery=function(t){var i=this;l.each(t,function(){l(this).appendTo(i.$gallery)})},r.prototype.shuffleArray=function(t){var i,e,s;for(i=t.length-1;0<i;i--)e=Math.floor(Math.random()*(i+1)),s=t[i],t[i]=t[e],t[e]=s;return this.insertToGallery(t),t},r.prototype.sortArray=function(t){return t.sort(this.settings.sort),this.insertToGallery(t),t},r.prototype.resetFilters=function(t){for(var i=0;i<t.length;i++)l(t[i]).removeClass("jg-filtered")},r.prototype.filterArray=function(t){var e=this.settings;if("string"===l.type(e.filter))return t.filter(function(t){var i=l(t);return i.is(e.filter)?(i.removeClass("jg-filtered"),!0):(i.addClass("jg-filtered").removeClass("jg-visible"),!1)});if(l.isFunction(e.filter)){for(var i=t.filter(e.filter),s=0;s<t.length;s++)-1===i.indexOf(t[s])?l(t[s]).addClass("jg-filtered").removeClass("jg-visible"):l(t[s]).removeClass("jg-filtered");return i}},r.prototype.resetImgSrc=function(t){"src"===t.data("jg.originalSrcLoc")?t.attr("src",t.data("jg.originalSrc")):t.attr("src","")},r.prototype.destroy=function(){clearInterval(this.checkWidthIntervalId),this.stopImgAnalyzerStarter(),l.each(this.getAllEntries(),l.proxy(function(t,i){var e=l(i);e.css("width",""),e.css("height",""),e.css("top",""),e.css("left",""),e.data("jg.loaded",void 0),e.removeClass("jg-entry jg-filtered jg-entry-visible");var s=this.imgFromEntry(e);s&&(s.css("width",""),s.css("height",""),s.css("margin-left",""),s.css("margin-top",""),this.resetImgSrc(s),s.data("jg.originalSrc",void 0),s.data("jg.originalSrcLoc",void 0),s.data("jg.src",void 0)),this.removeCaptionEventsHandlers(e);var n=this.captionFromEntry(e);e.data("jg.createdCaption")?(e.data("jg.createdCaption",void 0),null!==n&&n.remove()):null!==n&&n.fadeTo(0,1)},this)),this.$gallery.css("height",""),this.$gallery.removeClass("justified-gallery"),this.$gallery.data("jg.controller",void 0),this.settings.triggerEvent.call(this,"jg.destroy")},r.prototype.analyzeImages=function(t){for(var i=this.lastAnalyzedIndex+1;i<this.entries.length;i++){var e=l(this.entries[i]);if(!0===e.data("jg.loaded")||"skipped"===e.data("jg.loaded")){var s=this.galleryWidth-2*this.border-(this.buildingRow.entriesBuff.length-1)*this.settings.margins,n=e.data("jg.width")/e.data("jg.height");if(this.buildingRow.entriesBuff.push(e),this.buildingRow.aspectRatio+=n,this.buildingRow.width+=n*this.settings.rowHeight,this.lastAnalyzedIndex=i,s/(this.buildingRow.aspectRatio+n)<this.settings.rowHeight&&(this.flushRow(!1,0<this.settings.maxRowsCount&&this.rows===this.settings.maxRowsCount),++this.yield.flushed>=this.yield.every))return void this.startImgAnalyzer(t)}else if("error"!==e.data("jg.loaded"))return}0<this.buildingRow.entriesBuff.length&&this.flushRow(!0,0<this.settings.maxRowsCount&&this.rows===this.settings.maxRowsCount),this.isSpinnerActive()&&this.stopLoadingSpinnerAnimation(),this.stopImgAnalyzerStarter(),this.setGalleryFinalHeight(this.galleryHeightToSet),this.settings.triggerEvent.call(this,t?"jg.resize":"jg.complete")},r.prototype.stopImgAnalyzerStarter=function(){this.yield.flushed=0,null!==this.imgAnalyzerTimeout&&(clearTimeout(this.imgAnalyzerTimeout),this.imgAnalyzerTimeout=null)},r.prototype.startImgAnalyzer=function(t){var i=this;this.stopImgAnalyzerStarter(),this.imgAnalyzerTimeout=setTimeout(function(){i.analyzeImages(t)},.001)},r.prototype.onImageEvent=function(t,i,e){if(i||e){var s=new Image,n=l(s);i&&n.one("load",function(){n.off("load error"),i(s)}),e&&n.one("error",function(){n.off("load error"),e(s)}),s.src=t}},r.prototype.init=function(){var a=!1,h=!1,g=this;l.each(this.entries,function(t,i){var e=l(i),s=g.imgFromEntry(e);if(e.addClass("jg-entry"),!0!==e.data("jg.loaded")&&"skipped"!==e.data("jg.loaded"))if(null!==g.settings.rel&&e.attr("rel",g.settings.rel),null!==g.settings.target&&e.attr("target",g.settings.target),null!==s){var n=g.extractImgSrcFromImage(s);if(!1===g.settings.waitThumbnailsLoad||!n){var r=parseFloat(s.attr("width")),o=parseFloat(s.attr("height"));if("svg"===s.prop("tagName")&&(r=parseFloat(s[0].getBBox().width),o=parseFloat(s[0].getBBox().height)),!isNaN(r)&&!isNaN(o))return e.data("jg.width",r),e.data("jg.height",o),e.data("jg.loaded","skipped"),h=!0,g.startImgAnalyzer(!1),!0}e.data("jg.loaded",!1),a=!0,g.isSpinnerActive()||g.startLoadingSpinnerAnimation(),g.onImageEvent(n,function(t){e.data("jg.width",t.width),e.data("jg.height",t.height),e.data("jg.loaded",!0),g.startImgAnalyzer(!1)},function(){e.data("jg.loaded","error"),g.startImgAnalyzer(!1)})}else e.data("jg.loaded",!0),e.data("jg.width",e.width()|parseFloat(e.css("width"))|1),e.data("jg.height",e.height()|parseFloat(e.css("height"))|1)}),a||h||this.startImgAnalyzer(!1),this.checkWidth()},r.prototype.checkOrConvertNumber=function(t,i){if("string"===l.type(t[i])&&(t[i]=parseFloat(t[i])),"number"!==l.type(t[i]))throw i+" must be a number";if(isNaN(t[i]))throw"invalid number for "+i},r.prototype.checkSizeRangesSuffixes=function(){if("object"!==l.type(this.settings.sizeRangeSuffixes))throw"sizeRangeSuffixes must be defined and must be an object";var t=[];for(var i in this.settings.sizeRangeSuffixes)this.settings.sizeRangeSuffixes.hasOwnProperty(i)&&t.push(i);for(var e={0:""},s=0;s<t.length;s++)if("string"===l.type(t[s]))try{e[parseInt(t[s].replace(/^[a-z]+/,""),10)]=this.settings.sizeRangeSuffixes[t[s]]}catch(t){throw"sizeRangeSuffixes keys must contains correct numbers ("+t+")"}else e[t[s]]=this.settings.sizeRangeSuffixes[t[s]];this.settings.sizeRangeSuffixes=e},r.prototype.retrieveMaxRowHeight=function(){var t=null,i=this.settings.rowHeight;if("string"===l.type(this.settings.maxRowHeight))t=this.settings.maxRowHeight.match(/^[0-9]+%$/)?i*parseFloat(this.settings.maxRowHeight.match(/^([0-9]+)%$/)[1])/100:parseFloat(this.settings.maxRowHeight);else{if("number"!==l.type(this.settings.maxRowHeight)){if(!1===this.settings.maxRowHeight||null==this.settings.maxRowHeight)return null;throw"maxRowHeight must be a number or a percentage"}t=this.settings.maxRowHeight}if(isNaN(t))throw"invalid number for maxRowHeight";return t<i&&(t=i),t},r.prototype.checkSettings=function(){this.checkSizeRangesSuffixes(),this.checkOrConvertNumber(this.settings,"rowHeight"),this.checkOrConvertNumber(this.settings,"margins"),this.checkOrConvertNumber(this.settings,"border"),this.checkOrConvertNumber(this.settings,"maxRowsCount");var t=["justify","nojustify","left","center","right","hide"];if(-1===t.indexOf(this.settings.lastRow))throw"lastRow must be one of: "+t.join(", ");if(this.checkOrConvertNumber(this.settings,"justifyThreshold"),this.settings.justifyThreshold<0||1<this.settings.justifyThreshold)throw"justifyThreshold must be in the interval [0,1]";if("boolean"!==l.type(this.settings.cssAnimation))throw"cssAnimation must be a boolean";if("boolean"!==l.type(this.settings.captions))throw"captions must be a boolean";if(this.checkOrConvertNumber(this.settings.captionSettings,"animationDuration"),this.checkOrConvertNumber(this.settings.captionSettings,"visibleOpacity"),this.settings.captionSettings.visibleOpacity<0||1<this.settings.captionSettings.visibleOpacity)throw"captionSettings.visibleOpacity must be in the interval [0, 1]";if(this.checkOrConvertNumber(this.settings.captionSettings,"nonVisibleOpacity"),this.settings.captionSettings.nonVisibleOpacity<0||1<this.settings.captionSettings.nonVisibleOpacity)throw"captionSettings.nonVisibleOpacity must be in the interval [0, 1]";if(this.checkOrConvertNumber(this.settings,"imagesAnimationDuration"),this.checkOrConvertNumber(this.settings,"refreshTime"),this.checkOrConvertNumber(this.settings,"refreshSensitivity"),"boolean"!==l.type(this.settings.randomize))throw"randomize must be a boolean";if("string"!==l.type(this.settings.selector))throw"selector must be a string";if(!1!==this.settings.sort&&!l.isFunction(this.settings.sort))throw"sort must be false or a comparison function";if(!1!==this.settings.filter&&!l.isFunction(this.settings.filter)&&"string"!==l.type(this.settings.filter))throw"filter must be false, a string or a filter function"},r.prototype.retrieveSuffixRanges=function(){var t=[];for(var i in this.settings.sizeRangeSuffixes)this.settings.sizeRangeSuffixes.hasOwnProperty(i)&&t.push(parseInt(i,10));return t.sort(function(t,i){return i<t?1:t<i?-1:0}),t},r.prototype.updateSettings=function(t){this.settings=l.extend({},this.settings,t),this.checkSettings(),this.border=0<=this.settings.border?this.settings.border:this.settings.margins,this.maxRowHeight=this.retrieveMaxRowHeight(),this.suffixRanges=this.retrieveSuffixRanges()},r.prototype.defaults={sizeRangeSuffixes:{},thumbnailPath:void 0,rowHeight:120,maxRowHeight:!1,maxRowsCount:0,margins:1,border:-1,lastRow:"nojustify",justifyThreshold:.9,waitThumbnailsLoad:!0,captions:!0,cssAnimation:!0,imagesAnimationDuration:500,captionSettings:{animationDuration:500,visibleOpacity:.7,nonVisibleOpacity:0},rel:null,target:null,extension:/\.[^.\\/]+$/,refreshTime:200,refreshSensitivity:0,randomize:!1,rtl:!1,sort:!1,filter:!1,selector:"a",imgSelector:"> img, > a > img, > svg, > a > svg",triggerEvent:function(t){this.$gallery.trigger(t)}},l.fn.justifiedGallery=function(n){return this.each(function(t,i){var e=l(i);e.addClass("justified-gallery");var s=e.data("jg.controller");if(void 0===s){if(null!=n&&"object"!==l.type(n)){if("destroy"===n)return;throw"The argument must be an object"}s=new r(e,l.extend({},r.prototype.defaults,n)),e.data("jg.controller",s)}else if("norewind"===n);else{if("destroy"===n)return void s.destroy();s.updateSettings(n),s.rewind()}s.updateEntries("norewind"===n)&&s.init()})}});
```

# source/lib/meslo-LG/MesloLGL-Bold.ttf

This is a binary file of the type: Binary

# source/lib/meslo-LG/MesloLGL-BoldItalic.ttf

This is a binary file of the type: Binary

# source/lib/meslo-LG/MesloLGL-Italic.ttf

This is a binary file of the type: Binary

# source/lib/meslo-LG/MesloLGL-Regular.ttf

This is a binary file of the type: Binary

# source/lib/meslo-LG/MesloLGM-Bold.ttf

This is a binary file of the type: Binary

# source/lib/meslo-LG/MesloLGM-BoldItalic.ttf

This is a binary file of the type: Binary

# source/lib/meslo-LG/MesloLGM-Italic.ttf

This is a binary file of the type: Binary

# source/lib/meslo-LG/MesloLGM-Regular.ttf

This is a binary file of the type: Binary

# source/lib/meslo-LG/MesloLGS-Bold.ttf

This is a binary file of the type: Binary

# source/lib/meslo-LG/MesloLGS-BoldItalic.ttf

This is a binary file of the type: Binary

# source/lib/meslo-LG/MesloLGS-Italic.ttf

This is a binary file of the type: Binary

# source/lib/meslo-LG/MesloLGS-Regular.ttf

This is a binary file of the type: Binary

# source/lib/vazir-font/font-face.css

```css
@font-face {
  font-family: Vazir;
  src: url('Vazir-Regular.eot');
  src: url('Vazir-Regular.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Regular.woff2') format('woff2'),
       url('Vazir-Regular.woff') format('woff'),
       url('Vazir-Regular.ttf') format('truetype');
  font-weight: normal;
  font-display:swap;
}

@font-face {
  font-family: Vazir;
  src: url('Vazir-Bold.eot');
  src: url('Vazir-Bold.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Bold.woff2') format('woff2'),
       url('Vazir-Bold.woff') format('woff'),
       url('Vazir-Bold.ttf') format('truetype');
  font-weight: bold;
  font-display:swap;
}

@font-face {
  font-family: Vazir;
  src: url('Vazir-Thin.eot');
  src: url('Vazir-Thin.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Thin.woff2') format('woff2'),
       url('Vazir-Thin.woff') format('woff'),
       url('Vazir-Thin.ttf') format('truetype');
  font-weight: 100;
  font-display:swap;
}

@font-face {
  font-family: Vazir;
  src: url('Vazir-Light.eot');
  src: url('Vazir-Light.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Light.woff2') format('woff2'),
       url('Vazir-Light.woff') format('woff'),
       url('Vazir-Light.ttf') format('truetype');
  font-weight: 300;
  font-display:swap;
}

@font-face {
  font-family: Vazir;
  src: url('Vazir-Medium.eot');
  src: url('Vazir-Medium.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Medium.woff2') format('woff2'),
       url('Vazir-Medium.woff') format('woff'),
       url('Vazir-Medium.ttf') format('truetype');
  font-weight: 500;
  font-display:swap;
}

@font-face {
  font-family: Vazir;
  src: url('Vazir-Black.eot');
  src: url('Vazir-Black.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Black.woff2') format('woff2'),
       url('Vazir-Black.woff') format('woff'),
       url('Vazir-Black.ttf') format('truetype');
  font-weight: 900;
  font-display:swap;
}
```

# source/lib/vazir-font/Vazir-Black.eot

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Black.ttf

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Black.woff

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Black.woff2

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Bold.eot

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Bold.ttf

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Bold.woff

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Bold.woff2

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Light.eot

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Light.ttf

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Light.woff

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Light.woff2

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Medium.eot

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Medium.ttf

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Medium.woff

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Medium.woff2

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Regular.eot

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Regular.ttf

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Regular.woff

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Regular.woff2

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Thin.eot

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Thin.ttf

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Thin.woff

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Thin.woff2

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Variable.eot

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Variable.ttf

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Variable.woff

This is a binary file of the type: Binary

# source/lib/vazir-font/Vazir-Variable.woff2

This is a binary file of the type: Binary


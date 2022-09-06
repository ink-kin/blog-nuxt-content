---
title: Создайте блог с Nuxt Content
description: 'Nuxt Content что это? Модуль Content — это безголовая CMS на основе файлов git, которая предоставляет мощные функции, когда речь идет о написании блогов, сайтов документации или просто добавлении контента на любой обычный веб-сайт.'
img: https://images.unsplash.com/reserve/LJIZlzHgQ7WPSh5KVTCB_Typewriter.jpg?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=60
alt: my first blog post
author: 
  name: Илья Клишин
  bio: Бизнесмен, Продюсер, Актёр, Преподаватель, Генеральный директор Communication Service Москва
  img: https://images.unsplash.com/photo-1533636721434-0e2d61030955?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2550&q=80
tags: 
  - nuxtjs content
  - 'создать сайт самостоятельно'
---

[Модуль контента](https://content.nuxtjs.org/) представляет собой безголовую CMS на основе файлов git, которая предоставляет мощные функции, когда речь идет о написании блогов, сайтов документации или просто добавлении контента на любой обычный веб-сайт. В этом посте мы рассмотрим большинство преимуществ этого модуля и узнаем, как мы можем создать с его помощью блог.

## Монтаж

Чтобы начать работу с модулем контента, нам сначала нужно установить модуль с помощью npm или yarn.

```
yarn add @nuxt/content
```

Затем мы можем добавить его в свойство нашего модуля внутри нашего файла nuxt.config.

```js[nuxt.config.js]
export default {
  modules: ['@nuxt/content']
}
```

::alert{type="warning"}
Если вы создали новый проект create-nuxt-app, вы можете добавить модуль содержимого, и поэтому он будет установлен для вас.
::

Модуль содержимого работает, читая файлы в нашем content/каталоге.

Но мы создадим articles/каталог, куда мы сможем добавлять статьи для нашего блога.

```
mkdir content/articles
```


## This is a heading
This is some more info
<div class="bg-blue-500 text-white p-4 mb-4">
  This is HTML inside markdown that has a class some classes
</div>

<info-box>
  <template #info-box>
    This is a vue component inside markdown using slots
  </template>
</info-box>

```js[nuxt.config.js]
export default {
  nuxt: "is the best"
}
```
```html[my-first-blog-post.md]
<p>code styling is easy</p>
```

### This is a sub heading
This is some more info

### This is another sub heading
This is some more info

## This is another heading
This is some more info

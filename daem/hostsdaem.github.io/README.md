::before ::after ссылка на них тоже распространяется, псевдоэлемент может быть только один

:hover::before есть, но fill не работает никак для after, before

.something:hover .somethingnd - дочерний элемент

.something:hover +.somethingnd - соседний элемент

::after background-img z-index -1 чтобы была сзади и не мешала или background url в родителе но тогда расплытие на дочерние распросраняется, у background есть слои картинки и цвета

pointer-events: none делает disabled на все action

либо button, либо link

**auth**

100vh растягивает на весь экран, не отдельный блок, для 100% ширины after

закидывать в url параметры можно только по действию

useSearchParams чекает url всегда и обновляет полученное значение через .get и рендерит страницу, изменение параметров не обновляет страницу, не делает переход потому что параметры не прописать в роутинге, set функция стирает прежднее

setSearchParams({ visits_all: "up" })

вот так не стирает

```tsx
;() => {
  searchParams.set("rooms", element)
  setSearchParams(searchParams)
}
```

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4918d19b-273c-4df2-b934-15b7e71b4aa5/Untitled.png)

NavLink параметры to="/news?\_page=1” path=”news” не видет для active

**matches, classList**

element.matches(”.класса”) есть ли такой класс у элемента

element.classList.remove(drop.show) удаляет класс, есть еще add, replace, contains, toggle

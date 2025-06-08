+++
title = 'I have a blog tab now !'
"blog/tags"=["Programming"]
date = "2025-06-07"
+++

I was curious if I could implement a CSS only system to handle tags on blog posts, and it turns out that I can ! 
It's quite simple once you learn about the `:has` CSS pseudo class, it allows you to check if a parent node contains something. Using this pseudo class allows us to model relationships between two distant elements in the DOM.

Basically, you define a structure like so :
```html
<div class="filters">
    <div>
        <input name="filter" id="tag1" type="radio"/>
        <label for="tag1"> Tag1 </label>
    </div>
    <div>
        <input name="filter" id="tag2" type="radio"/>
        <label for="tag2"> Tag2 </label>
    </div>
</div>

<div class="posts-container">
    <div class="post tag1"> Exemple 1 </div>
    <div class="post tag1 tag2"> Exemple 2 </div>
    <div class="post tag2"> Exemple 3 </div>
</div>
```

and the following CSS :
```css 
.post{
    display:none;
}

.filters:has(#tag1:checked) ~ .posts-container > .post.tag1,
.filters:has(#tag2:checked) ~ .posts-container > .post.tag2{
    display : flex;
}
```

We use the neighbour's selector `~` to access the corresponding tag class when the radio button is checked. 
Using Hugo, I can automatically create these lines to handle any number of tags !

I use this code inside a `blog_css.css` file that is then used as a Hugo partial :
```hugo
{{$terms := (where .Site.AllPages "Kind" "term")}}
{{$endIndex := (sub (len $terms) 1)}}

{{range $index, $element := $terms}}
.blog-filter-div:has(#{{.LinkTitle}}:checked)~ .blog-card-container > .blog-card.{{.LinkTitle}}{{if ne $index $endIndex}},{{end}}
{{end}}
{
        display:flex;
}
```

That was a fun project ! Maybe I will need a search bar at one point if I really use this functionality.

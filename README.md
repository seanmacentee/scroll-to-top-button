You need 3 things:

1. The jQuery
>      $(document).ready(function(){
>       $(window).scroll(function(){
>           if ($(this).scrollTop() > 100) {
>               $('.scrollUpButton').fadeIn();
>           } else {
>               $('.scrollUpButton').fadeOut();
>           }
>       });
>       $('.scrollUpButton').click(function(){
>           $("html, body").animate({ scrollTop: 0 }, 500);
>           return false;
>       });
>      });

2. The CSS
> .scrollUpButton {
>    display: none;
>    opacity: 0.6;
>    position: fixed;
>    bottom: 10px;
>    right: 10px;
>    display: none;
>    background: #000;
>    color: #fff;
>    font-size: 1.5em;
>    text-decoration: none;
>    padding: 5px 10px 5px 10px;
>  }
>  .scrollUpButton:hover {
>    text-decoration: none;
>    color: #fff;
>    opacity: 1;
>  }

3. The HTML
Add this somewhere before the closing body tag
`<a href="#" class="scrollUpButton">&#9650</a>`

Note that &#9650 is html character for an 'up arrow' shape (i'm just being lazy here, you could add an image or use a font icon either) 


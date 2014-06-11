### add fancybox image
`<a class="fancybox" rel="gallery1" href="https://<image>" title="">`

`![](https://<image>)`

`</a>`

### display images in rows
wrap block of images in

`<div class="cols <two, three, four>"> <images> </div>`

### setup comments

To set up Moot comments, do the following:

1. Go to: https://moot.it/ and create a new forum (near the bottom) and username for yourself.
2. Inside your new forum, create a discussion section that you'll use for comments (most people just name it "Posts").
3. Use a text editor to open the post.hbs file in this theme.
4. Find this code in that file:
	```
    <section id="comments">
        <a class="moot"
            title="{{title}}"
            href="https://moot.it/i/detox/posts:{{title}}">
            Comments for this blog entry
        </a>
    </section>
    ```
5. Replace "detox" with the name of the forum you created and "posts" with the name of the discussion section you created, like this:
	```
    href="https://moot.it/i/your-forumname/your-discusionsection:{{title}}"
    ```
Then you should be good to go!

For more information: 
- [https://moot.it/docs/embedding.html](https://moot.it/docs/embedding.html)
- [https://ghost.org/forum/plugins/605-blog-comments-discus/?page=2](https://ghost.org/forum/plugins/605-blog-comments-discus/?page=2)

## License

[MIT License](http://oswaldoacauan.mit-license.org/)
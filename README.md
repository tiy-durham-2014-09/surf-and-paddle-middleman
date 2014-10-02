## Surf and Paddle

Your goal is to replicate the [Surf and Paddle](surf-and-paddle.png) website
using Middleman to generate the page.

### Directions

1. Fork this repo.
2. Clone your forked repo to your local computer and change directories into your local repo.
3. Run `bundle install` on your command line.
4. Replace the content of `source/index.html.erb` and
   `source/stylesheets/all.css` with your content.
5. Make a pull request back to this repo.

Remember, run `bundle exec middleman` to preview your changes.

Once you have the site replicated, you should:

* Convert your CSS to Sass. (You should only have to rename your `.css` file
  to `.css.scss`.)
* Rebuild the page using Sass, Bourbon, and Neat. Specifically:
  * Replace your grids with Neat grids. Your column widths may vary from the
    ones in the original PNG. That is fine. Eyeball the ratio and decide for
    yourself.
* Turn your main page layout into a layout suitable for showing
  more posts like the one on the front page.
* Create 3 new pages _in Markdown_ (that is, with `.html.md` extensions) that
  use front-matter to populate the title, date, and author. These should
  use the new layout. Each page should have a different author.
* Set the author to a unique key (like `turing`) and pull their name,
  social links, and image from `data/authors.yml`. (You will need to download an
  image for each author and add that to their data in `authors.yml`.)
* Change your `index.html.erb` page to show all three of your other posts
  in descending order by date. Show:
    * The title -- which should be a link to the post
    * The author and date information
    * Either the first paragraph of the text or a truncated number of words
    * The buttons at the bottom of each post
* On your new `index.html.erb`, the sidebar author information should not
  show up, as you should have three different authors with posts on the page.
* __Bonus__: Use the `middleman-blog` extension to create a blog. Use that
  instead of the way we showed and aggregated posts in this homework.

Remember to use helpers to make your life easier and your templates nicer!

## Updating

In order to get the latest files (authors.yml), run the following on your command-line.

```sh
git origin add upstream https://github.com/tiy-durham-2014-09/surf-and-paddle-middleman.git
git pull upstream master
```

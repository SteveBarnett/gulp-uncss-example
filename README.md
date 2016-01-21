# gulp-uncss-example

A short example of how to use uncss with gulp.

[Uncss](https://github.com/giakki/uncss) removes unused CSS from your stylesheets. It's particularly powerful if you're using a framework like [Bootstrap](http://getbootstrap.com/) or [Foundation](http://foundation.zurb.com/): it can dramatically reduce the size of your CSS files.

## Usage

1. Install gulp globally:

```
$ npm install --global gulp
```

2. Install the dependencies (just `gulp-uncss` in this case) in `package.json`:

```
npm install
```

3. Run gulp:

```
$ gulp
```

The trimmed CSS file with be put in the `out` directory.

For the files included in this example, your trimmed CSS file should look like this:

```css
p {
  font: 1em sans-serif;
}

em {
  color: green;
}
```

The styles for `strong`, `header`, and `a` aren't applied in `index.html`, so uncss removes them from the `main.css` file.

## Updating

To use it on your own projects:

1. Make sure that the `src` array includes *all* your css files.
2. Update the `html` object to include *all* your views.

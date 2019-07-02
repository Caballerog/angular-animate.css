[Originally from carloscaballero.io blog](https://carloscaballero.io/angular-animate-css-in-only-5-steps).

[Animate.css](http://daneden.github.io/animate.css) is a cross-browser library of CSS animations. As easy to use as an easy thing.

In this post I am going to show you how to configure Animate.css to be used in angular in only 5-1 steps.

![Peek-2019-07-02-15-29](/content/images/2019/07/Peek-2019-07-02-15-29.gif)

# Step 1 (or 0). Init your project

If you are thinking about using animate.css in your angular project, you probably already have an initialized project. However, let's start with our project from scratch.

```
ng new angular-animate
cd angular-animate
```

# Step 2. Install `animate.css`

Install `animate.css`

```
  npm install animate.css
```

# Step 3. Include `animate.css`

There are several ways to include Animate.css in our project:

1. Open `angular.json` and insert a new entry into the styles array:

```
      "styles": [
            "node_modules/animate.css/animate.min.css",
            "styles.css",
       ],
```

2. Open `styles.scss` and insert a new entry into the file:

```
@import '~animate.css/animate.min';
```

# Step 4. Add animated CSS Class

Open your template's component and add the animated CSS class in any html elements:

```
<div style="text-align:center" class="animated flip infinite">
 content
</div>
<h2>Here are some links to help you start:</h2>
<ul class="animated fadeIn infinite">
 content
</ul>

<router-outlet></router-outlet>

```

# Step 5. Run your app!

Run your app:

```
ng serve
```

# More, More and More...

- [Animate.css](https://daneden.github.io/animate.css/)

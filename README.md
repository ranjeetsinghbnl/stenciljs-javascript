# Stencil component without a Framework

This is a step by step guide, how we can use a stencil component in a project without a JavaScript framework.
Integrating a Stencil component to a project without a JavaScript framework is straight forward.If you're using a simple HTML page, you can add your component via a script tag. 

## Similar guides
I have created another framework integration guide to use stencil components

* [Stencil components in Vue](https://github.com/ranjeetsinghbnl/stenciljs-vue)
* [Stencil components in React](https://github.com/ranjeetsinghbnl/stenciljs-react)
* [Stencil components in Angular](https://github.com/ranjeetsinghbnl/stenciljs-angular)
* [Stencil components in javascript](https://github.com/ranjeetsinghbnl/stenciljs-javascript)

This example use the stencil component from the following project
* [Product & Cart showcase example](https://github.com/ranjeetsinghbnl/product-mgmt-stenciljs)


## Using NPM package

For example, if we published a component to npm, we could load the component through unpkg like this:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <script src="https://unpkg.com/@ranjeetsinghbnl/product-mgmt-stenciljs@0.0.1/dist/product-mgmt/product-mgmt.js"></script>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" />
  <style>
      body {
          background-color: #f7f7f7;
          margin-top: 3em;
      }
  </style>
</head>
<body>
<div class="container-fluid">
      <div class="row">
          <div class="col-sm-7">
              <mf-product-view></mf-product-view>
          </div>
          <div class="col-sm-5">
              <mf-product-cart></mf-product-cart>
          </div>
      </div>
  </div>
</body>
</html>
```

For more details you can also check the official [integration guide](https://stenciljs.com/docs/javascript).
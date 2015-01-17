## Background & Objectives

A challenge to understand Bootstrap responsive grid system.


## Specs

Improve your page using Bootstrap grid to get [this final result](In this challenge, reproduce [this page](http://lewagon.github.io/bootstrap-challenges/02-bootstrap-grid/). You will have to use the grid at 3 places in your page:

- In the banner, make the header, text and button to fill 50% of the screen.
- In the section describing your service, use a nice responsive grid to position your 4 items.
- In the footer, use a 1/3-2/3 grid to position you footer social list (on the left) and disclaimer (on the right).

## Tips & Resources

- Alway code your grid **without content**, and insert your content in the `.col` as a second step.

```html
<!-- Example of pure grid design without content -->
<div class="container">
  <div class="row">
    <div class="col-xs-12 col-sm-6"></div>
    <div class="col-xs-12 col-sm-6"></div>
    <div class="col-xs-12 col-sm-6"></div>
    <div class="col-xs-12 col-sm-6"></div>
  </div>
</div>
```

- Always start writing your `.col` classes starting with the smallest resolution `xs` and asking yourself the proportion you want for this size (full screen (`.col-xs-12`)? half screen (`.col-xs-6`)? 25%-screen (`.col-xs-3`)?. Then move on to the next size (`sm`) and repeat this process, and so on and so on until you get to `lg`.

- Notice that you are not obliged to write all the `xs/sm/md/lg` classes. If you forgot one, the immediate preceding class applies. For instance a `<div class="col-xs-12 col-md-6">` will be full-screen from mobile to labtop, and then half-screen from labtop to larger screens (desktop).
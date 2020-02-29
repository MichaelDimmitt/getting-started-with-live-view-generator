## Lets try to make a live view generator
this repository will be a journal as I read through phoenix's installer/lib and installer/templates folders and try to make a rough draft of the live view phoenix generator.

Some pre-existing research that I have done lives in the following repositories:
https://github.com/MichaelDimmitt/live_view_app

## Docs:
The incredibly long readme that gives the live view 101:
https://hexdocs.pm/phoenix_live_view/Phoenix.LiveView.html

## Steps in order of difficulty
1) define some commands and their expected behavior.
    a. add live view into the project with no implementation but correct javascript.
    b. live view folder and with live view component to be added to a regular project.
    c. scaffold an entire live view project ... phx.new style. (hard)
```
Next, decide where you want to use your (LiveView)[https://hexdocs.pm/phoenix_live_view/Phoenix.LiveView.html].
    1) serve the LiveView directly from your router. (recommended)
    2) You can also live_render from any template.
    3) Or you can live_render your view from any controller.

Note: (Live EEx) or ~L sigil. They are similar to regular .eex templates except they
are designed to minimize the amount of data sent over the wire by splitting static 
and dynamic parts and tracking changes.
```

2) make a template folder and build templates that use application name. (example)[https://github.com/phoenixframework/phoenix/blob/master/installer/templates/phx_web/views/page_view.ex]

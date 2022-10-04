### About

This repo houses GTK3 bindings for the Neat language.

### Usage

1. Add a dependency to this repo to your package.json:
    ```
        "dependencies": {
            "gtk": "*"
        },
        "sources": {
            "gtk": "https://github.com/neat-lang/gtk"
        }
    ```
2. Import the library: `import gtk;`
3. Substitute functions as such:
    - `gtk_window_new("Hello World")` => `Window.new("Hello World")`
    - `gtk_window_set_title("Window")` => `Window.setTitle("Window")`
4. Connect signals as such:
    `connectSignal(widget, "name", &fun)` where fun is a nested function or method.
    Note that `fun` has to outlive the signal connection!

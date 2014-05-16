## Declarative Profiles

### Introduction
In Wombat Editor, an EditorProfile is something that allows an editor type to specify certain behavior for the editor core to follow.
Currently, it allows for 3 things:

1. A function to look at a file path and determine if the editor being defined is responsible for it, and if so return an instance of that EditorWidget.
2. A function to return an instance of NewFileMenu for the user to create a new file of the desired type.
3. New default paths to be added on the creation of a new project.

The purpose of the Declarative Profiles initiative is allow this system to handle modules written in QML and JavaScript.

### Specification


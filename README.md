# Quart Extension Repository Template
This repoistory is used as a template to build new Quart extensions using VS Code, Dev Containers, and Poetry.

## Project Required Changes

### quart_ext folder
There is currently a dummy quart extension package folder named *quart_ext* with an *__init__.py* file. This is just for testing the dev container with Poetry.
Please rename for your extension.

**Make sure you read the edits required under the Poetry section to see what you need to change in your *pyproject.toml* file for your quart extension package folder.**

### Poetry - pyproject.toml
There is already a pyproject.toml file created as part of this repository template. All you need to do is add your dependencies for your extension. Also, make sure you add your required development dependencies as well. Currently, only pytest and pytest-asyncio is include.

You will also need to change/edit the following in *pyproject.toml* file:

- tool.poetry
    - name: To match your extension name
    - version: To match the current version of your extension. 
    - description: The description of your extension. 
    - authors: The author(s) of your extension. 
    - license: The license you use. 
- tool.isort
    - known_first_party: You need to change *quart_ext* to match your package.
- tool.poetry.dependencies (As mentioned above.)
- tool.poetry.group.dependencies (As mentioned above.)

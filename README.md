# GitHub Workflows - Static Analysis

Reusable GitHub workflows to run static code analysis.


## Workflows

### Pylint

- [Project page](https://pypi.org/project/pylint/)
- **Description:** analyzes Python code without running it; checks for errors, enforces a coding standard, looks for code smells, and can make suggestions about how the code could be refactored
- **Example use:**

    ```yaml
    jobs:
        run-pylint:
            name: Run pylint
            uses: lizzieprader/gh_workflows_static_analysis/.github/workflows/pylint.yml@main
            with:
                python-version: 3.13
    ```

### Pycodestyle

- [Project page](https://pypi.org/project/pycodestyle/)
- **Description:** checks Python code against some of the style conventions in PEP 8
- **Example use:**

    ```yaml
    jobs:
        run-pycodestyle:
            name: Run pycodestyle
            uses: lizzieprader/gh_workflows_static_analysis/.github/workflows/pycodestyle.yml@main
            with:
                python-version: 3.13
    ```

### Pydocstyle

- [Project page](https://pypi.org/project/pydocstyle/)
- **Description:** checks compliance with Python docstring conventions
- **Example use:**

    ```yaml
    jobs:
        run-pydocstyle:
            name: Run pydocstyle
            uses: lizzieprader/gh_workflows_static_analysis/.github/workflows/pydocstyle.yml@main
            with:
                python-version: 3.13
    ```

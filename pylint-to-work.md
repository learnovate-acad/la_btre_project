# install pylint-django
pip install pylint-django

# Set Workspace Settings as

{
    "python.pythonPath": "venv/bin/python",
    "python.linting.pylintEnabled": true,
    "python.linting.flake8Enabled": false,
    "python.linting.enabled": true,
    "python.linting.lintOnSave": true,
}

### Do not add this in Workspace Settings 
    "python.linting.pylintArgs": [
        "--load-plugins=pylint_django",
        "--disable=all",
        "--enable=F,E,unreachable,duplicate-key,unnecessary-semicolon,global-variable-not-assigned,unused-variable,binary-op-exception,bad-format-string,anomalous-backslash-in-string,bad-open-mode"
    ],

# Create .pylintrc in base folder

load-plugins=pylint_django
disable=all
enable=F,E,unreachable,duplicate-key,unnecessary-semicolon,global-variable-not-assigned,unused-variable,binary-op-exception,bad-format-string,anomalous-backslash-in-string,bad-open-mode


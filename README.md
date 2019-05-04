# Upload gb-distributions package to Pypi.org
- OOP practices on class, inheritance and magic methods
- Steps and files needed to upload package to pypi.org

### Local Package
- `cd package_folder`
- `pip install .`
- `pip install --upgrade .`

### Put Code on PyPi
```
cd gb_distributions
python setup.py sdist
pip install twine

# commands to upload to the pypi test repository
twine upload --repository-url https://test.pypi.org/legacy/ dist/*
pip install --index-url https://test.pypi.org/simple/ gb-distributions

# command to upload to the pypi repository
twine upload dist/*
pip install gb-distributions
```

### Git commands
- [Set up new repo from local work directory](https://help.github.com/en/articles/adding-an-existing-project-to-github-using-the-command-line)

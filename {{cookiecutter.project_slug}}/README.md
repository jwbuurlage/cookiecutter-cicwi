{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%}
# {{ cookiecutter.project_name }}

{{ cookiecutter.project_short_description }}

{% if is_open_source %}
* Free software: {{ cookiecutter.open_source_license }}
* Documentation: [https://{{ cookiecutter.github_username }}.github.io/{{ cookiecutter.project_slug }}]
{% endif %}

## Getting Started

It takes a few steps to setup {{ cookiecutter.project_name }} on your
machine. We recommend installing
[Anaconda package manager](https://www.anaconda.com/download/) for
Python 3.

### Installing with conda

Simply install with:
```
conda install -c cicwi {{ cookiecutter.project_slug }}
```

### Installing from source

To install {{ cookiecutter.project_name }}, simply clone this GitHub
project. Go to the cloned directory and run PIP installer:
```
git clone https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug}}.git
cd {{ cookiecutter.project_slug }}
pip install -e .
```

### Running the examples

To learn more about the functionality of the package check out our
examples folder.

## Authors and contributors

* **{{ cookiecutter.full_name }} ** - *Initial work*

See also the list of [contributors](https://github.com/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/contributors) who participated in this project.

## How to contribute

Contributions are always welcome. Please submit pull requests against the `master` branch.

If you have any issues, questions, or remarks, then please open an issue on GitHub.

## License

This project is licensed under the {{ cookiecutter.open_source_license }} - see the [LICENSE.md](LICENSE.md) file for details.

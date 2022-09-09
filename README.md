# docs-template
This project is just a template of a Jekyll-theme for Github page. I slightly revised a theme I forked from Github to support some features for documentation such like mathjak or mermaid.
You just need to download the whole template in your project repo and then rename to `docs`; or start a new project from this repo (make Gihub page from /root).

`_config.yml` is the configuration file, parameters can be assigned from there if needed. All document should be put under folder `docs` and categorized by subfolders.
Only if you understand what you are doing, please do not modify any files/folders except for `index.md`, `docs`, and `_config.yml`

All document should be created by markdown and Jekyll will handle the rest of things for deploying to Github page. However, If any raw materials are jupyter notebooks, convert them to markdown first. 

```bash
$ jupyter nbconvert --to FORMAT notebook.ipynb
```
supported formats:
    - html
    - latex
    - pdf
    - webpdf
    - slides
    - markdown
    - rst
  
For converting multiple notebooks, create a list in a configuration file, say `mycfg.py`, containing the text:

```python
c = get_config()
c.NbConvertApp.notebooks = ["notebook1.ipynb", "notebook2.ipynb"]
and using the command:
```

```bash
$ jupyter nbconvert --config mycfg.py
```


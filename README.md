# documentation
sources for instructions/hints for the NIF practical session at SD-LLOD-17 (host by [Read The Docs](readthedocs.org))

# setting up local preview
Get required Python libs using `pip`:
    pip install -r requirements.txt

Build documentation once:

    cd docs
    make html

Preview with automatic reload on changes:

    cd docs
    sphinx-autobuild -a -r _build . _build_auto

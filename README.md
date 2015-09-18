Draft
=====

Create open-science template repositories with all the bells and whistles in an instant.

    pip install draft
    draft project-name apj

Wishlist
--------
- [ ] python code template (e.g., with encoding, __author__, etc)
- [ ] include a default python setup.py
- [ ] establish a virtualenv?
- [ ] Travis ready-to-run, perhaps even with a faux test
- [ ] Coveralls ready-to-run
- [ ] Folders for article/docs/code
- [ ] Script to make article
- [ ] Post commit hook to keep science article fresh (git hashes etc)
- [ ] Post commit hook to check for new version tags, run auto latex-diff
- [ ] LICENSE file
- [ ] README file (with badges?)
- [ ] REPRODUCEME file
- [ ] .gitignore default
- [ ] template files for different journals
- [ ] an extensive example journal file (e.g., with tables etc)
- [ ] function to upload data files to zenodo easily (does zenodo have an api?)
- [ ] Initialise the repo on GH?
- [ ] Trigger Travis, etc?
- [ ] Initiate RTD?
- [ ] Initiate GH wiki repo?
- [ ] Get travis to build manuscripts and upload difftex pdfs to the GH wiki?
- [ ] Some draft options/config file of what to turn on/off by default

Practicality Notes
------------------
- pip install draft 
- draft new needs to generate a lot of files
- draft MANIFEST could keep all the default files and draft new just copies over whatever is relevant, updating whatever text as required
- need functionality to interface with whatever APIs (GH, Travis ,etc?)
- use multiple post-commit hooks that each do their own thing (e.g. difftex'ing, git hashing, etc)
- need templates from different journals
- most default files (even things like LICENSE etc) need to be formattable so we can include things like %(name)s
- need something to configure default options (e.g., apj, travis+, gh+)
- need to be able to generate (e.g., default with edits):
    + licenses
    + articles?? [probably not bother]
    + setup.py
    + Coveralls
    + python code templates
    + rtd?
    + .travis.yml (post-file make'ing, posting diffs back to GH wiki? etc)
    + post-commit hook file
- need to be able to hook:
    + github
    + bitbucket?
    + travis
    + coveralls
    + rtd

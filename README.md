**ToDo -- Insert Zenodo badge**

# BIDS specification PDF releases

This repository exists to regularly release PDF versions of the BIDS specification.

The PDFs are accessible from the Zenodo record: **ToDo -- Insert Zenodo record**

The repository contains the following files:

1. `README.md` --> this file
1. `LICENSE` --> the license for the BIDS specification and all files in this repository
1. `bids-spec.pdf` --> the PDF version of the current (stable) release of the BIDS specification
1. `CITATION.cff` --> a file containing the metadata about the BIDS specification

The BIDS specification is developed in this repository: https://github.com/bids-standard/bids-specification

An HTML version of the BIDS specification is available here: https://bids-specification.readthedocs.io/en/stable/

You can find out more about BIDS on the website: https://bids.neuroimaging.io/

## Previous releases

The first release of this repository is version `1.9.0`.

Previous releases of the PDF version of the BIDS specification (versions `1.0.0` to `1.8.0`)
can be found in this Zenodo record: https://zenodo.org/doi/10.5281/zenodo.3686061

## Release instructions

This repository and these guidelines are mostly intended for BIDS maintainers.
Read more about the BIDS Maintainers Group in the BIDS Governance: https://bids.neuroimaging.io/governance.html#bids-maintainers-group

1. Follow the [release protocol](https://github.com/bids-standard/bids-specification/blob/master/Release_Protocol.md) in the bids-specification GitHub repository.
1. Once you have followed all steps of the protocol, you will have two files corresponding to their state at release time:
    1. A `CITATION.cff`
    1. A PDF version of the BIDS specification
1. Copy over these two files to the present repository, replacing the existing `CITATION.cff` and `BIDS_specification.pdf` files.
1. Commit and push the changes to https://github.com/bids-standard/bids-specification-pdf-releases, using a commit message like: `REL: version X.Y.Z`, where `X.Y.Z` is the current version.
1. Tag the commit: `git tag -a -m "X.Y.Z" X.Y.Z origin/main`, given that `origin` is the remote pointing to https://github.com/bids-standard/bids-specification-pdf-releases.
1. Push the tag: `git push --follow-tags`
1. Make a release from the GitHub web UI, based on the pushed tag. Use the the name of the tag (`X.Y.Z`) as the "Release title". You do not need to describe the release further.

The Zenodo webhook will then archive the release (see link to record above, or by clicking the badge).

If you want to edit the Zenodo settings, you need to have the credentials of the [bids-maintenance](https://github.com/bids-maintenance) GitHub user.
These credentials are available for all BIDS maintainers.
Log into GitHub with the `bids-maintenance` user, then navigate to https://zenodo.org/ and log in via GitHub.
You should be able to make all necessary changes there.

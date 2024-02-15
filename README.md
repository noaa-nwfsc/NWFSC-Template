# Instructions for including your repository in the noaa-nwfsc organization

## Collaborators

If you have collaborators on your repository who are not members of the NMFS GitHub Enterprise Cloud account, have them complete a [user request](https://sites.google.com/noaa.gov/nmfs-st-github-governance-team/github-users), if they cannot be a member of the NMFS account, contact an administrator to help you add them to your repository or to transfer in your repository with outside collaborators.

## For repositories migrated to noaa-nwfsc organization

1) Update your `README.md` file to include the disclaimer and an open access license (if repo is public). These are below.
2) Add a description and info on who created the content (otherwise the org managers will not know who to contact).
3) Add tags (far right side on repo) to help users find repositories. See the other repositories for examples.
4) Add the LICENSE file and edit for your content. Note LICENSE files are important for repositories that are public and that are "products" in some way. For example, data, code package, documentation, etc.
5) Add the file `.github/workflows/secretSCAN.yml`. This will check for token and keys that are accidentally committed to a repository.

## For new repositories in noaa-nwfsc organization

1) Add a description and info on who created the content to this `README.md` file (otherwise the org managers will not know who to contact).
2) Add tags (far right side on repo) to help users find repositories. See the other repositories for examples.
3) Confirm that the License (see License tab) is appropriate for the content in your repository. Note LICENSE files are important for repositories that are public and that are "products" in some way. For example, data, code package, documentation, etc.
4) Confirm that the file `.github/workflows/secretSCAN.yml` is in this repository. This will check for token and keys that are accidentally committed to a repository.
5) Once you have completed the first four steps, delete the instructions from this `README.md`.

# Disclaimer

This repository is a scientific product and is not official communication of the National Oceanic and Atmospheric Administration, or the United States Department of Commerce. All NOAA GitHub project content is provided on an "as is" basis and the user assumes responsibility for its use. Any claims against the Department of Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed by all applicable Federal law. Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by the Department of Commerce. The Department of Commerce seal and logo, or the seal and logo of a DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by DOC or the United States Government.


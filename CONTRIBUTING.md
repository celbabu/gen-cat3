# Contributing to GCI+ Catalogs

The following is a set of guidelines for contributing to GCI+ catalogs. These are mostly guidelines, not rules. Use your 
best judgment, and feel free to propose changes to this document in a pull request.

## What should I know before I get started?

The GCI+ ITE uses the *development* branch and the GCI+ production uses a specific version (e.g. gitlab tag) which provides 
an overall version for the software distribution. The `docker-compose.yml` files reference specific versions for docker images
which corresponds to specific release for the microservices in Gitlab (e.g. via tags).

The latest catalog folder is always the *development* version and the `upgrade_from` is typically set to `none`. 

See [Rancher](https://rancher.com/) for details on catalogs.

## How Can I Contribute?

In principle all changes should be made on the *development* branch and merged back to *master* when ready for release. A 
rebase should be performed on the *development* branch if changes are made to the *master* branch. 

Workflow for release :

1. Add changes to *development* branch
2. Copy latest catalog folder (e.g. 0/, 1/, etc.) to the next in the sequence

    ```
    $ cp -r 0/ 1/
    ```
    
    Should look like (`1/` will now be *development* catalog) :
    
    ```
    catalog/
    catalog/0/docker-compose.yml
    catalog/0/rancher-compose.yml
    catalog/1/docker-compose.yml
    catalog/1/rancher-compose.yml
    catalog/catalogIcon-gciplus.png
    catalog/config.yml
    catalog/README.md
    ```

3. Change versions in release folder (eg. `0/` in example) to specific release versions (and upgrade_from if applicable)
4. Commit and push changes to origin/development (Gitlab)
5. Checkout *master* branch
6. Merge changes from *development* to *master* branch
7. Commit and push changes to origin/master
8. Create tag (e.g in Gitlab) for overall release

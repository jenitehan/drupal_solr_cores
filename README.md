Creates Solr cores for Drupal 8 websites.

This Ansible role will create and configure Apache Solr cores as required for the [Search API Solr](https://www.drupal.org/project/search_api_solr) module.

Currently supports version 8.x-1.2 of the Search API Solr module.

This is loosely based on the [Apache Solr](https://github.com/geerlingguy/ansible-role-solr) role by [Jeff Geerling](https://www.jeffgeerling.com) and uses some of the same variables. It assumes you've set up Solr with that role, but can probably work if Solr was set up differently.

Set the drupal_solr_cores variable to add cores:

    drupal_solr_cores:
      - drupal1

Set the drupal_solr_version variable to copy files from the Search API Solr module according to your Solr version.

    drupal_solr_version: 6.x

See `defaults/main.yml` for all available variables.

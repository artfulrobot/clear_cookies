# Clear Cookies

This module provides a URL for your Drupal 7 website (`/clear-cookies`) which
clears various cookies.

The purpose is to provide an easy way for people to revoke consent for cookies,
e.g. may be considered helpful in fulfilling legal obligations under the EU GDPR.

Currently it only clears the following cookies:

- `consent-agreed` As set by [EU Cookie Compliance](https://www.drupal.org/project/eu_cookie_compliance) module.

- `_gat`, `_gid`, `_gaq` As set by Google Analytics.

You can use `destintation` as a query parameter to set the destination page (by
default it's the `<front>`), e.g.

    /clear-cookies?destination=privacy

Might redirect people to your privacy policy page (assuming it's URL path is
`privacy`).

## Roadmap

- It would be nice to have an admin interface to list which cookies to delete.


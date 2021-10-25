# Known issues

* URL can not correctly substitute catalog if it was originally provided in a fits file (as opposed to generating it from the image requested from the frontend) https://github.com/oda-hub/dispatcher-app/issues/265
* In rare cases (only one known so far, with catalog provided as file), URL provided in the email may not be processed correctly. In this case, some fields will be substituted, but other will not be. We expect to add a warning in such a case. https://github.com/oda-hub/frontend-astrooda/issues/98
* ISGRI LC is not enabled with OSA11.2-beta https://github.com/oda-hub/dispatcher-plugin-integral/issues/73

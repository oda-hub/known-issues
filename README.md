# Known issues in ODA 21.10.0002

## Frontend

* In rare cases (only one known so far, with catalog provided as file), URL provided in the email may not be processed correctly. In this case, some fields will be substituted, but other will not be. We expect to add a warning in such a case. https://github.com/oda-hub/frontend-astrooda/issues/98
* It is not possible to change the Xspec model in the Fit of spectra. However, spectra can be downloaded and fit with another package.
* If you submit a job and the error "Forbidden" appears, it means that you should logout and login again from the web interface.

## ISGRI

* In some cases, especially for large observations with many sources and noisy obserations, ISGRI mosaic produces too many sources and mosaic extraction (standard OSA, which is used internally) crashes. This leads to an `AnalysisException` error. 
  * *Suggested workaround*: request energy range will less noise (e.g. start from 25 keV and not from 20 keV).
  * *Suggested workaround*: provide custom catalog, based on ISDC Reference Catalog.

## JEM-X

* A source named "NEW SOURCE" will not be used in extracting JEM-X spectrum and light curves. It is necessary to name it differently.


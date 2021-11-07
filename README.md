# Known issues in ODA 21.11.0002

* In rare cases (only one known so far, with catalog provided as file), URL provided in the email may not be processed correctly. In this case, some fields will be substituted, but other will not be. We expect to add a warning in such a case. https://github.com/oda-hub/frontend-astrooda/issues/98
* It is not possible to change the Xspec model in the Fit of spectra. However, spectra can be downloaded and fit with another package.
* A source named "NEW SOURCE" will not be used in extracting JEM-X spectrum and light curves. It is necessary to name it differently.
* If you submit a job and the error "Forbidden" appears, it means that you should logout and login again from the web interface.

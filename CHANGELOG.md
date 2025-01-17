# Changelog

## 5.1.0 (4 October 2022)

### Feature
* **api:** Make pagination configurable ([`dd6615f`](https://github.com/adfinis/document-merge-service/commit/dd6615f14b81ec005b697bf43c58d3c74e8d3fe3))

## 5.0.6 (13 September 2022)

### Fix
* Also log unshare in formats-call / only test unshare in error-path ([`dd0f22c`](https://github.com/adfinis-sygroup/document-merge-service/commit/dd0f22c0e97139e9f5559da70683d20a6927fb5d))

## 5.0.5 (01 September 2022)

### Fix
* **validation:** Fix excel template validation ([`3c6149e`](https://github.com/adfinis-sygroup/document-merge-service/commit/3c6149e15a455539f544c61084a0e372cc74fa7b))

## 5.0.4 (29 August 2022)

### Fix
* Allow isolation of unoconv calls to be disabled (default) ([`74834f1`](https://github.com/adfinis-sygroup/document-merge-service/commit/74834f1c820eb258e53697ecd563f1ee353a5e66))
* Remove security restrictions to make unshare possible ([`5b10cff`](https://github.com/adfinis-sygroup/document-merge-service/commit/5b10cffac5bd365d02c16999748113747d6d36e9))

## 5.0.3 (23 August 2022)

Important: Be aware that the docker-container needs CAP_SYS_ADMIN since version 4.7.0

### Fix
* Log an error if unoconv or unshare fails ([`6e2f54a`](https://github.com/adfinis-sygroup/document-merge-service/commit/6e2f54ad961cdfb0052c0a03823121ccf53b68ae))

## 5.0.2 (22 August 2022)

### Fix
* Move temporary path to data directory
([`afce2ca`](https://github.com/adfinis-sygroup/document-merge-service/commit/afce2ca3429bf20d6c282fe5f8a1f1201fc278ee))

## 5.0.1 (9 August 2022)

### Fix
* **docker:** Fix docker uwsgi command ([`85892f6`](https://github.com/adfinis/document-merge-service/commit/85892f63005fe31b277ba8df623c8a0ec0f1b7ec))

## 5.0.0 (9 August 2022)

### Feature
* **license:** Switch license from MIT to GPL-3.0-or-later ([`47c1a84`](https://github.com/adfinis/document-merge-service/commit/47c1a843a9cda105d1640651a8231fbc4c18039f))

### Fix
* **python:** Use python v3.8 ([`920c0bd`](https://github.com/adfinis/document-merge-service/commit/920c0bd2c5c0dfe836b5b215a91691a4077fd63b))

### Breaking
* Drop support for Python v3.7. This should have been done in 29a49ee76b638f0a8fb7b189fb91e61c45d78bde which updated the python version to 3.10 which is too restrictive. We now guarantee support for python versions 3.7 to 3.10.  ([`920c0bd`](https://github.com/adfinis/document-merge-service/commit/920c0bd2c5c0dfe836b5b215a91691a4077fd63b))
* document-merge-service is now released under the GPL-3.0-or-later license.  ([`47c1a84`](https://github.com/adfinis/document-merge-service/commit/47c1a843a9cda105d1640651a8231fbc4c18039f))

## 4.7.0 (26 July 2022)

### Feature
* Isolate libreoffice instances ([`9e2db65`](https://github.com/adfinis/document-merge-service/commit/9e2db651a9804c787e7909baa415aa36e551007b))
* **engines:** Add basic excel validation ([`f396ae8`](https://github.com/adfinis/document-merge-service/commit/f396ae8879475d6c4aca29003f77965945da24fd))
* **engines:** Render all excel-sheets with thee same data ([`ca54651`](https://github.com/adfinis/document-merge-service/commit/ca54651ac85c5576fac5162ba1caaebff273f87b))
* **engines:** Test datastructures with excel templates ([`9a5c116`](https://github.com/adfinis/document-merge-service/commit/9a5c116c30c22957c9ee316c0c0f4baa9c3dba98))
* **engines:** Create template test ([`8c4cad1`](https://github.com/adfinis/document-merge-service/commit/8c4cad1273f35496080473f42ecb150a575b0a2e))
* **engines:** Fix code for new xlsx library ([`ca4a6a4`](https://github.com/adfinis/document-merge-service/commit/ca4a6a42dfb58196e7a819e1c9b2a4cd9b59dbe8))
* **engines:** Add xlsx template engine ([`e133c83`](https://github.com/adfinis/document-merge-service/commit/e133c834128916eb26ff7642e6eb31852406743c))

### Fix
* Cleanup thread pool ([`fec982e`](https://github.com/adfinis/document-merge-service/commit/fec982e25209b1088477f868bfa786f087d047bc))

## 4.6.2 (21 January 2022)

### Fix
* **cleanup:** Convert cleanup migration to command ([#467](https://github.com/adfinis/document-merge-service/issues/467)) ([`33052ee`](https://github.com/adfinis/document-merge-service/commit/33052eed48dc01a311aa57462d3a64595b74e743))
* **cleanup-migration:** Fail gracefully in new container ([`8a93339`](https://github.com/adfinis/document-merge-service/commit/8a93339be1218fe79579129483f238f17e67d2e9))

## 4.6.1

### Fix
* **api:** Do not crash in list view ([#458](https://github.com/adfinis/document-merge-service/issues/458)) ([`11b02fd`](https://github.com/adfinis/document-merge-service/commit/11b02fd58a6a0d38d10bb6a67da9999e11f0c07f))

## 4.6.0

### Feature
* Add config for deployment under specific URL prefix ([#456](https://github.com/adfinis/document-merge-service/issues/456)) ([`6801024`](https://github.com/adfinis/document-merge-service/commit/680102457b938b33b2ecbc314bcb1897644c519a))

### Fix
* **template:** Make template download url more stable ([`3438a53`](https://github.com/adfinis/document-merge-service/commit/3438a53efbd7bbe46cf3b38659e1bebc4cfe348b))
* **cleanup:** Delete old files when template is deleted or changed ([#445](https://github.com/adfinis/document-merge-service/issues/445)) ([`26c9570`](https://github.com/adfinis/document-merge-service/commit/26c9570e02dcc981ee523273a06137caa9bf8486))
* **jinja:** Autoescape data passed to template when merging ([#444](https://github.com/adfinis/document-merge-service/issues/444)) ([`2ac030e`](https://github.com/adfinis/document-merge-service/commit/2ac030e619899a55bc72440f55081258e1ab66ac))

### Documentation
* **readme:** Remove deprecated dependabot badge ([`4173a3b`](https://github.com/adfinis/document-merge-service/commit/4173a3bf6d26d02afd05fc3972492054e3476f5f))


## 4.5.0

### Feature
* Add meta-field to Template ([`27163e8`](https://github.com/adfinis/document-merge-service/commit/27163e8c5b2d1541566e4908ac88e55a3d5bc7b9))

### Fix
* Reduce number of uwsgi processes ([`46f950a`](https://github.com/adfinis/document-merge-service/commit/46f950a7a5ff6ca99c20941a5d1ec0a7cbd1bde0))
* Add uwsgi config suitable for production use ([`247c5df`](https://github.com/adfinis/document-merge-service/commit/247c5dfbc9e00e29a95b21f2646ad735368cdc21))
* **jinja:** Replace deprecated contextfilter with pass_context ([`3308cd1`](https://github.com/adfinis/document-merge-service/commit/3308cd11aac3332445053b1d9ac4564bb7034a06))

## 4.4.0

### Feature
* run subprocesses with timeout and cleanup forks
([`be092b4`](https://github.com/adfinis/document-merge-service/commit/be092b464d0120ce1d6e9bc8afdf4150cacd2710))

## 4.3.0

### Feature
* Allow disabling validation
([`f371b33`](https://github.com/adfinis/document-merge-service/commit/f371b339d7434b01b2a024308fc58f0806d8a287))

## 4.2.1

### Fix
* Fix using same image multiple times in template (35b7ffb9cff7e4577f505823449874361d1557a2)

## 4.2.0

### Feature
* Handle None for images (fd6f55d61e1877e0203d7ee4212641816119077c)

### Fix
* Dont crash when accessing undefined value in template (f2bb378dbb51a61d3d4e1f01afcf2b3efd831aba)


## 4.1.0
### Feature
* Support inline images for docx-template (37e42724c75a5f5c8ab60ee45a2fd64118cdf407)

### Fix
* Correctly validate image placeholders (9617bd71db90901ae0e18c513bc28bb3225b7857)
* Also add template to context in engine validation (639e9c27435873ca8680308684d799ea9da29d6a)


## 4.0.1

### Fix
* Don't reject templates with complex syntax (fb56a42aee82f9261596f7546f52f8b9930292de)


## 4.0.0

### Breaking
* Remove support for external unoconv listeners
  * `UNOCONV_SERVER` and `UNOCONV_PORT` are no longer supported configuration options. Please remove
	them from your configuration file.
  * By default an unoconv process gets launched within the container.

### Feature
* Check template for available placeholders (2ac9aeb95016665520bef53c7e3ac0310be9f84f)
* Allow to validate docx template on upload (de810446fbec2ffe610cda4f9cb12be34b5bdbb5)

### Fix
* Make sure port is always printed as string (dd8f34b93a9f3b279fa8e99b1b8ba3d8e1d582fb)

### Documentation
* Extended user guide (09f0393ec7fe40513fcd47473272a09cf0a294d3)


## 3.0.0

### Fix
* Revert automatic conversion, add filter instead (4e91c50a5938ab641a90cb84fabd56ff992c757c)

### Breaking
* Replace tfk-api-unoconv service with unoconv listener (f12f0a221b64fb22665ac4609e4f52e34ff767f2)
  * `UNOCONV_LOCAL` and `UNOCONV_URL` are no longer supported configuration options. Please remove
	them from your configuration file.
  * By default an unoconv listener gets launched within the container. To use a different listener
	you can specify `UNOCONV_SERVER` and `UNOCONV_PORT`.

* After gathering some practical experience with the new automatic "Listing"-conversion for
  multiline we noticed that this feature is a little bit too "clever" and breaks many advanced
  use-cases. (4e91c50a5938ab641a90cb84fabd56ff992c757c)

# SCA scanning results
## <a id='110'></a>1.1.0

### <a id='black-duck-ba'></a>Black Duck Binary Analysis (BDBA)

#### <a id='api-backend'></a>API backend

* Date: March 4, 2022
* Results: no known vulnerabilities

#### <a id='cli-sr'></a>CLI

* Date: March 8, 2022
* Results: no known vulnerabilities

### <a id='grype-sr'></a>Grype

Version: 0.33.1

#### <a id='api-backend-ci'></a>API Backend Container Image

* Date: March 7, 2022
* Results: No high or critical vulnerabilities. Multiple medium and low vulnerabilities. For more information, see the [API Backend Container Image v1.1.0 CycloneDX file content](api-backend-container-image-v1.1.0-grype-result.md).

#### <a id='api-backend-cr'></a>API Backend Code Repository

* Date: March 7, 2022
* Results: no known vulnerabilities

#### <a id='cli-cr'></a>CLI Repository

* Date: March 7, 2022
* Results: 2 high vulnerabilities: [CVE-2015-5237](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5237), [CVE-2021-22570](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-22570)

#### <a id='kube-rbac-proxy-ci'></a>Kube RBAC Proxy Container Image

* Date: March 7, 2022
* Results: 3 high vulnerabilities: [CVE-2022-21698](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-21698), [CVE-2015-5237](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5237), [CVE-2021-22570](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-22570)

#### <a id='postgres-database-ci'></a>Postgres Database Container Image

* Date: March 7, 2022
* Results: 1 high vulnerability in 3 different packages: [CVE-2022-24407](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-24407), and multiple medium and low vulnerabilities. For more information see the [Postgres Database Container Image v1.1.0 CycloneDX file content](postgres-database-image-v1.1.0-grype-result.md)

## <a id='102'></a>1.0.2

### <a id='black-duck-ba'></a>Black Duck Binary Analysis (BDBA)

#### <a id='api-backend'></a>API backend

* Date: January 31, 2022
* Results: no known vulnerabilities

#### <a id='cli-sr'></a>CLI

* Date: January 24, 2022
* Results: no known vulnerabilities

### <a id='grype-sr'></a>Grype

Version: 0.32.0

#### <a id='api-backend-ci'></a>API Backend Container Image

* Date: February 2, 2022
* Results: No high or critical vulnerabilities. Multiple medium and low vulnerabilities. For more information, see the [CycloneDX file content](cyclonedx-file-content.md).

#### <a id='api-backend-cr'></a>API Backend Code Repository

* Date: February 2, 2022
* Results: no known vulnerabilities

#### <a id='cli-cr'></a>CLI Code Repository

* Date: February 2, 2022
* Results: no known vulnerabilities

## <a id='100'></a>1.0.0
Date: November 26, 2021

### <a id='scan-type'></a>Scan Type:

Software Composition Analysis scanning

### <a id='source-scan'></a>Source of Scan:

* Black Duck Binary Analysis (BDBA)
* Grype

### <a id='version-source'></a>Version of Source:

* BDBA version 2021.9.0
* Grype version 0.25.1

### <a id='cves'></a>CVEs:

#### <a id='bdba'></a>BDBA

No vulnerabilities were found in the API backend and CLI binaries.

See BDBA reports:

- [API backend report](store-bdba-scan-2021-11-26.jpg)
- [CLI report](cli-bdba-scan-2021-11-26.jpg)

#### <a id='grype-cr'></a>Grype

No vulnerabilities were found through scanning the API back end sources, client lib, and CLI.

The following CVEs were found through scanning the API back end image:

```
NAME   INSTALLED        FIXED-IN  VULNERABILITY   SEVERITY   
libc6  2.27-3ubuntu1.4            CVE-2015-8985   Negligible  
libc6  2.27-3ubuntu1.4            CVE-2016-10739  Low         
libc6  2.27-3ubuntu1.4            CVE-2020-6096   Low         
libc6  2.27-3ubuntu1.4            CVE-2021-3326   Low         
libc6  2.27-3ubuntu1.4            CVE-2020-27618  Low         
libc6  2.27-3ubuntu1.4            CVE-2019-25013  Low         
libc6  2.27-3ubuntu1.4            CVE-2021-35942  Medium      
libc6  2.27-3ubuntu1.4            CVE-2021-33574  Low         
libc6  2.27-3ubuntu1.4            CVE-2021-38604  Medium      
libc6  2.27-3ubuntu1.4            CVE-2016-10228  Negligible  
libc6  2.27-3ubuntu1.4            CVE-2009-5155   Negligible  
```

No `high` or `critical` CVEs present.

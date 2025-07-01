# Oracle Weblogic CVE Check 

- **Affected Versions**:
  - WebLogic Server 10.3.6.0.0
  - WebLogic Server 12.1.3.0.0
  - WebLogic Server 12.2.1.3.0
  - WebLogic Server 12.2.1.4.0
  - WebLogic Server 14.1.1.0.0

**!Oudated versions are metioned are dangerous!**

A hacker can exploit the mentioned versions if running on a public IP. 
Please use this with care. 

## How to use :
You Will need nuclei !

https://github.com/projectdiscovery/nuclei

Check local nuclei install and verify template

```nuclei -t weblogic-cve-2019-2725.yaml -vv```

Out shows:

```[CVE-2019-2725] Oracle WebLogic Server wls9-async XML Deserialization RCE (CVE-2019-2725) (@psibot) [critical]```

## Scan as follow : 

To Use any of the templates with single target: 

```nuclei -t weblogic-cve-2019-2725.yaml -u https://*.*.*.*:7001```

To scan al list you would need the file with ip:port 

```nuclei -t weblogic-cve-2019-2725.yaml -l file.txt```

## CVE Checks are : 

Checks for:

```weblogic-cve-2019-2725.yaml - Oracle WebLogic Server wls9-async XML Deserialization RCE (CVE-2019-2725)```

```weblogic-cve-2019-2729.yaml - Oracle WebLogic Server wls-wsat Component Deserialization RCE (CVE-2019-2729)```

```weblogic-cve-2020-14882.yaml - Oracle WebLogic Server Authentication Bypass (CVE-2020-14882)```

```weblogic-cve-2020-2555.yaml - Oracle WebLogic Server T3 Protocol Deserialization RCE (CVE-2020-2555)```

```weblogic-cve-2021-2109.yaml - Oracle WebLogic Server RCE (CVE-2021-2109)```

```weblogic-cve-2022-21371.yaml - Oracle WebLogic Server RCE (CVE-2022-21371)```
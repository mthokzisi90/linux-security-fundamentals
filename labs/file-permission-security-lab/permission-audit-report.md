# Permission Audit Report: Fictional Customer Data File

## Executive Summary

A Linux file-permission review identified excessive read access on a fictional customer-data file.

The file initially used permission `644`, allowing the owner to read and write the file while allowing group members and other users to read it. This was unsuitable for data that should remain confidential.

The permission was corrected to `600`, limiting access to the file owner only.

## Finding Details

| Field | Details |
| --- | --- |
| File reviewed | `lab-data/customer_data.txt` |
| Data classification | Fictional sensitive customer data |
| Initial permission | `644` / `-rw-r--r--` |
| Security concern | Group and other users could read the file |
| Risk level | Medium — training scenario |
| Recommended permission | `600` / `-rw-------` |

## Evidence

Initial permission review:

```text
-rw-r--r-- customer_data.txt
```

The permission setting allowed unnecessary read access by users other than the owner.

## Remediation

The following command was used to apply least privilege:

```bash
chmod 600 customer_data.txt
```

## Verification

The file permissions were reviewed after remediation:

```text
-rw------- customer_data.txt
```

The corrected setting allows only the file owner to read and write the fictional sensitive data.

## Lessons Learned

- Sensitive files should be accessible only to authorised users.
- File permissions should be reviewed regularly.
- Least privilege reduces the risk of accidental or unauthorised data exposure.
- Security remediation should always be verified after changes are applied.

## Disclaimer

This report documents a fictional training scenario. No real customer data, systems, or accounts were accessed or modified.
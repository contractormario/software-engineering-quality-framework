# Security

## Context

* These notes are part of a broader set of [principles](../principles.md)
* TO DO: Further reading / training courses about security:
    * [OWASP top 10](https://owasp.org/www-project-top-ten/)
* TO DO: Reference to the Security Working Group (link to terms of reference?)

## Details

* Everything (including infrastructure) should be up to date.
* Application dependencies should be automatically scanned for vulnerabilities & license issues.
  * e.g. libraries, base container or VM images
  * Scan before deployment and periodically in live for components no longer receiving regular deployments
  * TO DO: guidance around setting team tolerances for warnings etc.
* Source code should be automatically scanned for secrets or other senstive data (see [everything as code](../patterns/everything-as-code.md) for details).
* Nobody should need access to production hosts, including:
    * Logging & monitoring should negate the need to manually inspect a production host.
    * Deployments are immutable, and all deployments are issued via delivery pipelines, negating the need to manually change a production host.
* Any access to production must be audited and granted using temporary "break glass" permissions.
* Access to environments, secrets & credentials, etc must use role based access control with minimum privileges.
* Use public resources as well as organisation policies, for example [OWASP Top 10](https://owasp.org/www-project-top-ten/).

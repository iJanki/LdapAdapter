**Ldap adapter that does not allow null passowrd (anonymous binding)**

Configure like any other ldap adapter.

services.yaml
```yaml
services:
    Symfony\Component\Ldap\Ldap:
        arguments: ['@Ijanki\Component\Ldap\Adapter\Adapter']
    Ijanki\Component\Ldap\Adapter\Adapter:
        arguments:
            - host: "ldaphost"
#              port: 389
#              encryption: tls
#              options:
#                  protocol_version: 3
#                  referrals: false

```
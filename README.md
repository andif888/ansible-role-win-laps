# ansible-role-win-laps

Role to install Windows Local Administrator Password Solution

## Table of content

- [Default Variables](#default-variables)
  - [win_laps_download_url](#win_laps_download_url)
  - [win_laps_download_validate_certs](#win_laps_download_validate_certs)
  - [win_laps_install_args](#win_laps_install_args)
  - [win_laps_install_product_id](#win_laps_install_product_id)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Default Variables

### win_laps_download_url

Download URL

#### Default value

```YAML
win_laps_download_url: https://download.microsoft.com/download/C/7/A/C7AAD914-A8A6-4904-88A1-29E657445D03/LAPS.x64.msi
```

### win_laps_download_validate_certs

If false, SSL certificates will not be validated.

#### Default value

```YAML
win_laps_download_validate_certs: true
```

### win_laps_install_args

Any arguments the installer needs to either installthe package. If the package is an MSI do not supply the /qn, /log or /norestart arguments.

#### Default value

```YAML
win_laps_install_args: ADDLOCAL=CSE ALLUSERS=1
```

### win_laps_install_product_id

The product id of the installed packaged. This is used for checking whether the product is already installed.

#### Default value

```YAML
win_laps_install_product_id: '{97E2CA7B-B657-4FF7-A6DB-30ECC73E1E28}'
```



## Dependencies

None.

## License

license (GPL-2.0-or-later, MIT, etc)

## Author

andif888

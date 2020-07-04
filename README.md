# Keybase Secret Management Extension for PowerShell

![PowerShell Gallery](https://img.shields.io/powershellgallery/dt/KeybaseSecretManagementExtension)

Secret Management Extension for [PowerShell Secrets Management](https://www.powershellgallery.com/packages/Microsoft.PowerShell.SecretsManagement/) using [Keybase](https://keybase.io/) KV store as a Vault.

Check out package in [PS Gallery](https://www.powershellgallery.com/packages/KeybaseSecretManagementExtension/).

```PowerShell
Install-Module -Name KeybaseSecretManagementExtension
```

Usage

```PowerShell
$SecretsVault = 'VaultName'
$VaultParameters = @{ 
    namespace = 'NamespaceName'
    team      = 'TeamName' # Optional
}

Register-SecretsVault -Name $SecretsVault -ModuleName 'KeybaseSecretManagementExtension' -VaultParameters $VaultParameters
```

## Secret type support

- [X] ByteArray
- [X] String
- [ ] SecureString
- [ ] PSCredential
- [X] Hashtable
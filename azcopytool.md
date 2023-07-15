AZCOPY TOOL
============

Source Account to Local
-----------------------
```
azcopy login --tenant-id <target-tenant-id>
```

```
azcopy login --tenant-id xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
```

```
azcopy copy "https://<source-storageaccount-name>.blob.core.windows.net/<source-container-name><sas-token>" "localpath" --recursive=true
```

Local to Destination Account
----------------------------
```
azcopy login --tenant-id <target-tenant-id>
```

```
azcopy login --tenant-id xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
```

```
azcopy copy "localpath" "https://<destination-storageaccount-name>.blob.core.windows.net/<destination-container-name><sas-token>" --recursive=true
```

Transfer the data from the source storage account to the destination storage account
---------------------------------------------------------------------------------------
```
azcopy copy "<source-url-with-sas-token>" "<destination-url-with-sas-token>" --recursive=true
```
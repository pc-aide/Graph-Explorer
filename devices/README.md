# devices

---

## Filter
|n|name|e.g.|O/P|
|-|----|----|---|
|1|isManaged|`https://graph.microsoft.com/beta/devices?$count=true&$filter=operatingSystem+eq+'Windows'+and+isManaged+eq+true`||
|2|detectedApps|`https://graph.microsoft.com/beta/deviceManagement/managedDevices/<managedDeviceID>/detectedApps`|

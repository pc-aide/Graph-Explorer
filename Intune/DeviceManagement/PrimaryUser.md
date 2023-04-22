# PrimaryUser

---

## All device
1. Method : Get
2. Version : v1.0
3. Query : `https://graph.microsoft.com/v1.0/deviceManagement/managedDevices?$select=id,deviceName`
4. O/P:
````json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#deviceManagement/managedDevices(id,deviceName)",
    "@odata.count": 10,
    "value": [
        {
            "id": "2202b3c0-6d14-41fe-ba16-abba8904b467",
            "deviceName": "DESKTOP-AJ2I2TB"
        },
        {
            "id": "7b125126-3070-4a19-9624-ec7bdd3a5a1c",
            "deviceName": "VT5HX7Z23"
        },
        {
            "id": "00d7ca56-c3ee-4d9a-8ffb-5aad97faae7d",
            "deviceName": "VTGXXXX333XXXXX"
        },
        {
            "id": "03fc1619-4029-4d63-bd7c-9b1d587c810b",
            "deviceName": "VTMJ06YQ52"
        },
        {
            "id": "ede1ef1e-8163-4645-a637-bac1ec802aac",
            "deviceName": "VTMJVHTXA"
        },
        {
            "id": "b488bca6-35e9-45c3-8523-f207fa108632",
            "deviceName": "VTPC02LMK0"
        },
        {
            "id": "ee4633a0-e0b6-4062-9655-e26d1d06280f",
            "deviceName": "VTPC03PK9M"
        },
        {
            "id": "233be163-ef6b-4456-bbdf-bf6e1c52090c",
            "deviceName": "VTPC08U64A"
        },
        {
            "id": "eae44cda-61f2-430e-ad80-6487e7a0cf9b",
            "deviceName": "VTPC0BSP6P"
        },
        {
            "id": "12d83524-99f5-4468-9833-je1ccedca075",
            "deviceName": "VTPC0SVZ9N"
        }
    ]
}
````

---

## PrimaryUser
1. Query : https://graph.microsoft.com/v1.0/deviceManagement/managedDevices/{id}/users
2. if not empty, so we have a primaryUser
3. else, we don't have a primaryUser for this device
4. O/P when is not empty :
````json
{

    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users",
    "value": [
        {
            "businessPhones": [],
            "displayName": "jessica, simpson",
            "givenName": null,
            "jobTitle": null,
            "mail": null,
            "mobilePhone": null,
            "officeLocation": null,
            "preferredLanguage": null,
            "surname": null,
            "userPrincipalName": "jessica.simpson@intunePracticeEdu.montreal.ca",
            "id": "1fe2cea5-5858-41b9-b935-01ef50ab706e"
        }
    ]
}
````

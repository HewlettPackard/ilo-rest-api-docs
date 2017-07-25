# Errata

## EthernetInterfaces for ComputerSystem
In iLO 5 1.10, the link (@odata.id) to the EthernetInterfacesCollection is in the wrong location in the ComputerSystem resource.  It should be a link directly from the root of the resoruce

```json
{
  "EthernetInterfaces": {
    "@odata.id": "<link>"
  }
}
```

In iLO 5 1.10 it is instead in the Hpe OEM sub-object:

```json
{
  "Oem": {
    "Hpe": {
      "EthernetInterfaces": {
        "@odata.id": "<link>"
      }
    }
  }
}
```

Future iLO 5 firmware will correct this by adding the additional corrected link.

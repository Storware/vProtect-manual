# oVirt UI Plugin

1. Download add-on from our FTP. Extract the provided archive on your oVirt manager.
2. In file `vprotect.json` edit lines in config part:
   * `vProtectURL` - URL to vProtect API
   * `username` - name of administrator in vProtect
   * `password` - administrator password in vProtect

**Example**:

```text
   {
      "name": "vprotect",
      "url": "plugin/vprotect/plugin.html",
      "resourcePath": "vprotect-resources",
      "lazyLoad": false,

      "config": {
          "vProtectURL": "http:///IP_address:8080/api",
          "username": "admin",
          "password": "vPr0tect"
       }
   }
```

1. Put `vprotect.json` file and `vprotect-resources` directory in the `/usr/share/ovirt-engine/ui-plugins` directory in the oVirt Engine.

![](https://github.com/backupmonster/storware-vprotect-manual/tree/31778b5e60e67956cc3fb965d118537bb2d2be7e/.gitbook/assets/rhv-ui-plugin.png)

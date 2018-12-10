# Color Correction

Download the color profile here:
https://www.notebookcheck.net/uploads/tx_nbc2/B140QAN02_0.icm

Load the color profile using the guide here: 
http://www.bartneck.de/2009/09/11/install-an-icc-color-profile-on-mac-os-x/

# HIDPI
The highest HIDPI resolution I can get to is 1472x828 using this override:

```
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
	<key>DisplayProductID</key>
	<integer>8246</integer>
	<key>DisplayProductName</key>
	<string>Lenovo</string>
	<key>DisplayVendorID</key>
	<integer>1711</integer>
	<key>scale-resolutions</key>
  	<array>
    		<data>AAAFwAAAAzw=</data>
    		<data>AAALgAAABngAAAABACAAAA==</data>
  	</array>
</dict>
</plist>
```

Copy this file to (make sure this file doesn't have any extension!):
`
/System/Library/Displays/Contents/Resources/Overrides/DisplayVendorID-6af/DisplayProductID-2036
`

Then use an app like to use the updated resolution:
https://github.com/avibrazil/RDM

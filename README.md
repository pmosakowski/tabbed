# Readme

This is a working fork of **tabbed** for my little experiments.
For the original visit [tabbed homepage at suckless.org](http://tools.suckless.org/tabbed/).

## List of 'improvements'

### Setting of WM\_NAME and \_NET\_WM\_NAME

This is for the keepassx auto-type feature, which uses window name to filter passwords. Modifications include setting of the **WM\_NAME** to **STRING** encoding and **\_NET\_WM\_NAME** to **UTF8_STRING** encoding. Originally both were set as **COMPUND\_TEXT** and keepassx failed to read it, failing silently.

My intention is to have these properties copied verbatim from the client window so tabbed doesn't need to touch them.

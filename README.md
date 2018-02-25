# rtl8814AU
Realtek 8814AU USB WiFi driver.

This is a temporary fork that merges updates from tpircher:devices and
the Ubuntu 17.10-specific work that HomerSp has done.

Once 18.04 comes out (and tpircher merges in the devices branch) we can
probably switch to using tpircher's master instead.

# DKMS support

From your src dir

````
sudo cp -R . /usr/src/rtl8814au-4.3.21
sudo dkms build -m rtl8814au -v 4.3.21
sudo dkms install -m rtl8814au -v 4.3.21
````

This should keep your 8814AU adapter working post kernel updates.

Ovpnctl
=======

This is a set of helper scripts to use small OpenVpn based vpn.


How to use
----------

Typical usage of Ovpnctl is listing and starting / stopping OpenVPN profiles.
Listing is done as follows:

```
ovpnctl list
```

And this print this kind of result:

```
  my-us-server
* my-iceland-server
  another-service
  work-vpn
```

This indicates that there are 4 valid OpenVPN profiles and the profile named
`my-iceland-server` is currently active.

It is possible to stop this profile by typing:

```
ovpnctl stop my-iceland-server
```

or to switch to another profile with:

```
ovpnctl start work-vpn
```


Dependencies
------------

Ovpnctl assumes the following dependencies are installed:

  * OpenVPN (client side)
  * Systemd

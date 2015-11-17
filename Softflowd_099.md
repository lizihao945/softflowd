# Softflowd 0.9.9 #

This release contains a number of bug fixes and some new features. It also welcomes Hitoshi Irino as a developer.

## Details ##

This release contains the following new features:

  * Add support for flow sampling, controlled by a new **-s** option (see softflowd(8) manpage for details)
  * Add compile-time **--chrootdir** option to specify alternate chroot directory.
  * Allow specification of input and output interface indices using a new **-i** option.
  * Introduce a freelist allocator for expiry and flow objects, faster than malloc

And the following bug fixes:

  * Correctly exit from mainloop when a signal is received
  * Fix logging from reduced-privileged child
  * Many manpage typo, consistency and formatting fixes
  * The _softflow statistics_ command now displays the time at which softflowd was started
  * Avoid spurious exit from mainloop while listening on "any" interface
  * Correct broken IPv6 Netflow v.9 flows
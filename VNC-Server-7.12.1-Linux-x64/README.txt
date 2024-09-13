VNC Server for Unix/Linux platforms
===================================

Run the vncinstall script to install VNC Server and associated
programs on any UNIX or Linux computer. Note this is the only way to install
VNC Server without administrative privileges, though not all modes and
features are subsequently available. See www.realvnc.com for more information.

Usage:
./vncinstall [<binary-dir>] [<doc-dir>]

To specify an alternative location for programs, specify <binary-dir>. To
specify an alternative location for man pages, specify <doc-dir>. Examine
the script for default locations.

SELinux
-------

VNC policy modules are registered automatically if SELinux is enabled when
VNC is installed or upgraded. If you enable SELinux afterwards, run
vncinitconfig -register-SELinux to register the VNC policy modules manually.

Note: the policy modules cannot be registered on versions of CentOS/RHEL
earlier than 5.0.

VNC policy modules are stored in /usr/share/selinux/packages/realvnc. If you
specified an alternative <binary-dir> for VNC, you will have to edit, build and
register the VNC policy modules manually.

To see how to use VNC once installed, consult the man pages.


Copyright (C) 2002 - 2017 RealVNC Limited. All rights reserved.

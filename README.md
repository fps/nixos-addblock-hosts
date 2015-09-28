# nixos-addblock-hosts
A nixos configuration file that you can import from configuration.nix to block common ad/tracker hosts

Download <code>hosts.nix</code> to <code>/etc/nixos/hosts.nix</code> and add it as import to your <code>/etc/nixos/configuration.nix</code> like this (example):

<pre>
# Edit this configuration file to define what should be installed on
# your system.  Help is available in the configuration.nix(5) man page
# and in the NixOS manual (accessible by running ‘nixos-help’).

{ config, pkgs, ... }:

{
  imports =
    [ # Include the results of the hardware scan.
      ./hardware-configuration.nix
      ./hosts.nix
    ];

...
</pre>

Also note this comment from the top of the original <code>hosts</code> file:

<pre>
# This hosts file is brought to you by Dan Pollock and can be found at
# http://someonewhocares.org/hosts/
# You are free to copy and distribute this file for non-commercial uses,
# as long the original URL and attribution is included. 
</pre>



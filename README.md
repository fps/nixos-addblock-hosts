# nixos-addblock-hosts
A nixos configuration file that you can import from configuration.nix to block common ad/tracker hosts

Download this file to /nixos/configuration/hosts.nix and add it as import to your configuration.nix like this (example):

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

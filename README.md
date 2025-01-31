# Camera Report for Synology Surveillance Station

Prepares a report of all enabled and connected cameras running in
*Synology Surveillance Station*. 

This report is designed to be printable as well as viewed on-screen. In the author's implementation, it has been used as a non-electronic reference
by building personnel.

## Prerequisites
- Synology DSM [Synology OS]
  - developed for DSM 6.2.4-25556 Update 8.
  - chance of it working on other DSM versions: unknown.
- Surveillance Station [Synology package]
  -   developed for Surveillance Station 9.22.9575
  -   chance of it working on other versions: unknown.
- Git [v2.48.1-34] [Commmunity package]
- Web Station [Synology package]
  - apache2 selected
  - PHP 7.4 selected
- Python 3.8+ [Synology package]
  - developed on 3.8.6
  - expected to run on 3.8+; <3.8 unknown

## Installing

The contents of this repository can be cloned into any directory writable by the user that will run it.  The simplest is to
clone directly to `/var/services/web/camreport/` The rest of the instructions will assume you did just that, except where noted.

## Running
- `ssh` into the server.
- `cd /var/services/web/`
- `python3 

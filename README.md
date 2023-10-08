# Quectel Timesync

## About

This tool allows for acquiring the current time from the cellular network for configuring the local clock.
Compared to NTP, this has the advantage of nut using up mobile traffic.

It takes avantage of the `AT+QLTS` command found on Quectel modems. This functionality depends on support
of the mobile network.


## Configuration

quectel-timesync supports UCI configuration.

## `enabled`

Determines if the tool should operate in daemon mode on system-start.

Valid values: `0` or `1`

## `path`

Path for the serial interface to use.

Example: `/dev/ttyUSB4`

## `interval`

Interval in seconds between syncronization attempts.

Minimum: `10`


## Supported Modems

 - Quectel EC25
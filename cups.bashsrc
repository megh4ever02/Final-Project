#!/bin/bash

LPSTAT = "/usr/bin/lpstat"
STATE-OK = 0
STATE_WARNING=1
STATE_CIRITICAL=3
STATE_UNKNOWN=3
STATE_DEPENDENT=4

if[ ! -x "$LPSTAT"]
then
	echo "UNKNOWN: $LPSTAT not found or is not executable by the nagios user"
exitstatus = $STATE_UNKNOWN
exit $exitstatus
fi

name = `basename $0`

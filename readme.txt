# Splunk TA for Kaspersky

*Install*
- Install both the TA in the search heads and indexers (or fowarders)
- Setup a TCP input pointed to index an (e.g. kaspersky) with the sourcetype kaspersky
- Configure Kaspersky Security Center to send logs to you splunk instance via syslog using the LEEF (Q1 Radar) option (other formats will be available in the future)

*Roadmap*
- Include extractions in case of CEF format being used
- Add missing event types for sourcetype renaming

*Feedback*
feedback+kaspersky_ta@devbusters.com


https://support.kaspersky.com/9323


# Docs

*Log types*
GNRL - General
KLNAG - Network Agent
KLAUD - Audit
KLPRCI -
KLSRV - Server Administration

*Event types*
GNRL_EV_ATTACK_DETECTED
GNRL_EV_DEVCTRL_DEV_PLUGGED
GNRL_EV_DEVCTRL_DEV_UNPLUGGED
GNRL_EV_LICENSE_EXPIRATION
GNRL_EV_OBJECT_BLOCKED
GNRL_EV_OBJECT_DELETED
GNRL_EV_OBJECT_NOTCURED
GNRL_EV_OBJECT_QUARANTINED
GNRL_EV_PASSWD_ARCHIVE_FOUND
GNRL_EV_SUSPICIOUS_OBJECT_FOUND
GNRL_EV_VIRUS_FOUND
KLAUD_EV_OBJECTMODIFY
KLAUD_EV_SERVERCONNECT
KLNAG_EV_DEVICE_ARRIVAL
KLNAG_EV_DEVICE_REMOVE
KLNAG_EV_INV_APP_INSTALLED
KLNAG_EV_INV_APP_UNINSTALLED
KLNAG_EV_PATCH_INSTALLED_SUCCESSFULLY
KLNAG_EV_PATCH_INSTALL_STARTING
KLPRCI_TaskState
KLSRV_EVENT_HOSTS_NEW_DETECTED
KLSRV_EVENT_HOSTS_NOT_VISIBLE
KLSRV_EV_MASTER_SRV_CONNECTED
KLSRV_EV_MASTER_SRV_DISCONNECTED
KLSRV_HOST_MOVED_WITH_RULE_EX
KLSRV_HOST_STATUS_CRITICAL
KLSRV_HOST_STATUS_WARNING
KLSRV_INVISIBLE_HOSTS_REMOVED
KLSRV_RUNTIME_ERROR
KLSRV_UPD_BASES_UPDATED

#Change Log

1.0.2
Added kaspersky:cef sourcetype
Added malware operations tags

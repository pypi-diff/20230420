# Comparing `tmp/mistapi-0.37.4.tar.gz` & `tmp/mistapi-0.37.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistapi-0.37.4.tar", last modified: Wed Apr 19 13:36:51 2023, max compression
+gzip compressed data, was "mistapi-0.37.6.tar", last modified: Thu Apr 20 13:58:35 2023, max compression
```

## Comparing `mistapi-0.37.4.tar` & `mistapi-0.37.6.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.089301 mistapi-0.37.4/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.37.4/LICENSE
--rw-r--r--   0 tmunzer    (502) staff       (20)    11332 2023-04-19 13:36:51.089395 mistapi-0.37.4/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)    10556 2023-02-22 14:11:31.000000 mistapi-0.37.4/README.md
--rw-r--r--   0 tmunzer    (502) staff       (20)      952 2023-04-19 13:22:50.000000 mistapi-0.37.4/pyproject.toml
--rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-04-19 13:36:51.089806 mistapi-0.37.4/setup.cfg
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.008642 mistapi-0.37.4/src/
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.016897 mistapi-0.37.4/src/mistapi/
--rw-r--r--   0 tmunzer    (502) staff       (20)     7162 2023-04-06 09:34:39.000000 mistapi-0.37.4/src/mistapi/__api_request.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-02-21 11:06:36.000000 mistapi-0.37.4/src/mistapi/__api_response.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    19300 2023-02-09 10:15:49.000000 mistapi-0.37.4/src/mistapi/__api_session.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2229 2023-02-13 15:54:52.000000 mistapi-0.37.4/src/mistapi/__logger.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.019083 mistapi-0.37.4/src/mistapi/__models/
--rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.37.4/src/mistapi/__models/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1514 2023-02-21 08:35:01.000000 mistapi-0.37.4/src/mistapi/__models/privilege.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2029 2023-02-09 11:01:08.000000 mistapi-0.37.4/src/mistapi/__pagination.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.019489 mistapi-0.37.4/src/mistapi/api/
--rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.019813 mistapi-0.37.4/src/mistapi/api/v1/
--rw-r--r--   0 tmunzer    (502) staff       (20)      869 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.024902 mistapi-0.37.4/src/mistapi/api/v1/const/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1133 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1041 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/alarm_defs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1193 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/ap_channels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1042 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/ap_led_status.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1035 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/applications.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1052 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/call_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1058 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/client_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1032 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/countries.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1383 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/default_gateway_config.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1058 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/device_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1036 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/device_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1068 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/insight_metrics.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1034 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/languages.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1058 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/mxedge_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1036 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/mxedge_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1036 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/const/traffic_types.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.025241 mistapi-0.37.4/src/mistapi/api/v1/installer/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.028205 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1157 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1167 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6483 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1158 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1148 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1145 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5928 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/sites.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.028902 mistapi-0.37.4/src/mistapi/api/v1/installer/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1149 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/installer/sites/optimize.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.029435 mistapi-0.37.4/src/mistapi/api/v1/invite/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/invite/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1080 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/invite/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.031188 mistapi-0.37.4/src/mistapi/api/v1/login/
--rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/login/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1117 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/login/login.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1126 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/login/lookup.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2609 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/login/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1136 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/login/two_factor.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.031829 mistapi-0.37.4/src/mistapi/api/v1/logout/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/logout/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      965 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/logout/logout.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.032395 mistapi-0.37.4/src/mistapi/api/v1/mobile/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/mobile/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1238 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/mobile/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.038356 mistapi-0.37.4/src/mistapi/api/v1/msps/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1060 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3136 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1231 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1724 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1186 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2648 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1861 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1809 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/logo.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2235 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/msps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3911 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/orggroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4501 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1641 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/search.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3243 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5146 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1921 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2175 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/msps/tickets.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.064808 mistapi-0.37.4/src/mistapi/api/v1/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)     3119 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2504 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6421 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6014 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3911 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3959 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/aptemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3987 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5316 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2325 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1690 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/cert.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1231 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    11362 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1217 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/clone.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1827 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/crl.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5994 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    17829 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4028 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4079 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5724 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2959 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5015 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2648 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4585 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/jsi.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2484 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3474 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1442 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3975 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/mxclusters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    13405 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3911 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/nacrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3863 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/nactags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4081 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/networktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1388 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/ocdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2956 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4548 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1133 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/pma.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3935 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/pskportals.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7181 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3959 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1297 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/sdkclients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6134 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/sdkinvites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3953 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/sdktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3950 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4038 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    12655 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3935 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7662 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4009 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/sitetemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6216 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3996 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    27680 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1728 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4686 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/templates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5874 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/tickets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1739 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/troubleshoot.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3795 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3887 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3521 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6882 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4481 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5136 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3911 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/orgs/wxtunnels.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.065807 mistapi-0.37.4/src/mistapi/api/v1/recover/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/recover/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1139 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/recover/recover.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1091 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/recover/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.066833 mistapi-0.37.4/src/mistapi/api/v1/register/
--rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/register/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1142 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/register/register.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1084 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/register/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.069559 mistapi-0.37.4/src/mistapi/api/v1/self/
--rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2251 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1476 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1996 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2090 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/self.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1047 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1818 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/two_factor.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1737 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/self/update.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.088054 mistapi-0.37.4/src/mistapi/api/v1/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)     2273 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8638 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2636 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/anomaly.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1111 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/apps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4015 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5358 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3897 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/beacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2337 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    17300 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2308 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/count.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    56692 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5018 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4058 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5997 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6547 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1138 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8520 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/location.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    13727 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4535 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1165 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1735 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4446 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/pcaps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6430 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5733 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/rfdiags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5702 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/rogues.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3790 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/rrm.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3941 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/rssizones.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5959 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2385 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3862 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/skyatp.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20752 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/sle.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1951 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    53181 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1688 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1886 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/synthetic_test.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4614 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/uisettings.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3917 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/vbeacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2220 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/visits.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4534 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3820 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6260 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4517 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5178 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3941 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/wxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3845 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/sites/zones.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.089026 mistapi-0.37.4/src/mistapi/api/v1/utils/
--rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/utils/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1053 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/utils/test_telstra.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1165 2023-04-19 13:22:50.000000 mistapi-0.37.4/src/mistapi/api/v1/utils/test_twilio.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8483 2023-02-09 10:30:57.000000 mistapi-0.37.4/src/mistapi/cli.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-19 13:36:51.018532 mistapi-0.37.4/src/mistapi.egg-info/
--rw-r--r--   0 tmunzer    (502) staff       (20)    11332 2023-04-19 13:36:50.000000 mistapi-0.37.4/src/mistapi.egg-info/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)     7303 2023-04-19 13:36:51.000000 mistapi-0.37.4/src/mistapi.egg-info/SOURCES.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-04-19 13:36:50.000000 mistapi-0.37.4/src/mistapi.egg-info/dependency_links.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)       48 2023-04-19 13:36:50.000000 mistapi-0.37.4/src/mistapi.egg-info/requires.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-04-19 13:36:50.000000 mistapi-0.37.4/src/mistapi.egg-info/top_level.txt
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.374282 mistapi-0.37.6/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.37.6/LICENSE
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11332 2023-04-20 13:58:35.374389 mistapi-0.37.6/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10556 2023-02-22 14:11:31.000000 mistapi-0.37.6/README.md
+-rw-r--r--   0 tmunzer    (502) staff       (20)      952 2023-04-20 13:58:24.000000 mistapi-0.37.6/pyproject.toml
+-rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-04-20 13:58:35.374779 mistapi-0.37.6/setup.cfg
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.268258 mistapi-0.37.6/src/
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.276484 mistapi-0.37.6/src/mistapi/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7909 2023-04-20 13:57:39.000000 mistapi-0.37.6/src/mistapi/__api_request.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-02-21 11:06:36.000000 mistapi-0.37.6/src/mistapi/__api_response.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    19300 2023-02-09 10:15:49.000000 mistapi-0.37.6/src/mistapi/__api_session.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-04-20 13:58:24.000000 mistapi-0.37.6/src/mistapi/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2229 2023-02-13 15:54:52.000000 mistapi-0.37.6/src/mistapi/__logger.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.278661 mistapi-0.37.6/src/mistapi/__models/
+-rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.37.6/src/mistapi/__models/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1514 2023-02-21 08:35:01.000000 mistapi-0.37.6/src/mistapi/__models/privilege.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2029 2023-02-09 11:01:08.000000 mistapi-0.37.6/src/mistapi/__pagination.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.279031 mistapi-0.37.6/src/mistapi/api/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.279358 mistapi-0.37.6/src/mistapi/api/v1/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      869 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.284268 mistapi-0.37.6/src/mistapi/api/v1/const/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1133 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1043 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/alarm_defs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1195 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/ap_channels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1044 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/ap_led_status.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1037 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1054 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/call_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1060 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/client_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1034 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/countries.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1383 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/default_gateway_config.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1060 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1038 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/device_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/insight_metrics.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1036 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/languages.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1060 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/mxedge_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1038 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/mxedge_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1038 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/const/traffic_types.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.284597 mistapi-0.37.6/src/mistapi/api/v1/installer/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/installer/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.287487 mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1159 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1159 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6282 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1160 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1150 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1147 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5905 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/sites.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.288193 mistapi-0.37.6/src/mistapi/api/v1/installer/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/installer/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1149 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/installer/sites/optimize.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.288737 mistapi-0.37.6/src/mistapi/api/v1/invite/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/invite/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1080 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/invite/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.290256 mistapi-0.37.6/src/mistapi/api/v1/login/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/login/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1117 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/login/login.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1126 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/login/lookup.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2609 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/login/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1136 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/login/two_factor.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.290818 mistapi-0.37.6/src/mistapi/api/v1/logout/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/logout/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      965 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/logout/logout.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.294490 mistapi-0.37.6/src/mistapi/api/v1/mobile/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/mobile/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1238 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/mobile/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.311212 mistapi-0.37.6/src/mistapi/api/v1/msps/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1060 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3138 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1231 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1724 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1186 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2648 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1863 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1809 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/logo.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2237 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/msps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3913 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/orggroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4503 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1641 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/search.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3245 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5148 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1925 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2177 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/msps/tickets.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.334902 mistapi-0.37.6/src/mistapi/api/v1/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3119 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2506 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6421 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6018 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3913 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3961 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3989 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5240 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2325 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1690 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/cert.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1231 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11362 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1217 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/clone.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1827 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/crl.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5996 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    17835 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4030 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4081 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5726 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2959 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5015 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2648 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4589 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/jsi.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2484 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3476 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1415 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3977 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/mxclusters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    13409 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3913 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3889 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/nacrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3865 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/nactags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3889 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4083 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1388 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/ocdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2956 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4550 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1135 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/pma.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3937 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/pskportals.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7105 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3961 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1297 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/sdkclients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6136 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/sdkinvites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3955 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/sdktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3952 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4040 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3889 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    12655 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3937 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7674 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4011 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3889 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6220 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3998 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    27686 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1728 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4688 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/templates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5798 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/tickets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1739 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/troubleshoot.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3797 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3889 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3521 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6681 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4483 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5138 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3913 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/orgs/wxtunnels.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.336010 mistapi-0.37.6/src/mistapi/api/v1/recover/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/recover/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1139 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/recover/recover.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1091 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/recover/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.337056 mistapi-0.37.6/src/mistapi/api/v1/register/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/register/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1142 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/register/register.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1084 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/register/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.339801 mistapi-0.37.6/src/mistapi/api/v1/self/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/self/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2253 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/self/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1478 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/self/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1996 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/self/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2090 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/self/self.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1049 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/self/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1818 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/self/two_factor.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1737 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/self/update.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.372695 mistapi-0.37.6/src/mistapi/api/v1/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2273 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8638 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2636 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/anomaly.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1113 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/apps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4017 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5282 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3899 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/beacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2337 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    17300 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2308 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/count.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    55793 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5018 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4054 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5999 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6551 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1138 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8520 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/location.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    13384 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4537 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1165 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1737 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4448 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/pcaps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6354 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5733 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/rfdiags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5702 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/rogues.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3790 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/rrm.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3943 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/rssizones.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5959 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2385 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3862 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/skyatp.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    20752 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/sle.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1951 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    53197 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1688 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1886 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/synthetic_test.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4614 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/uisettings.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3919 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/vbeacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2220 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/visits.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4536 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3820 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6059 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4519 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5180 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3943 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/wxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3847 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/sites/zones.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.373993 mistapi-0.37.6/src/mistapi/api/v1/utils/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/utils/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1053 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/utils/test_telstra.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1165 2023-04-20 13:58:25.000000 mistapi-0.37.6/src/mistapi/api/v1/utils/test_twilio.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8483 2023-02-09 10:30:57.000000 mistapi-0.37.6/src/mistapi/cli.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-04-20 13:58:35.277976 mistapi-0.37.6/src/mistapi.egg-info/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11332 2023-04-20 13:58:35.000000 mistapi-0.37.6/src/mistapi.egg-info/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7303 2023-04-20 13:58:35.000000 mistapi-0.37.6/src/mistapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-04-20 13:58:35.000000 mistapi-0.37.6/src/mistapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)       48 2023-04-20 13:58:35.000000 mistapi-0.37.6/src/mistapi.egg-info/requires.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-04-20 13:58:35.000000 mistapi-0.37.6/src/mistapi.egg-info/top_level.txt
```

### Comparing `mistapi-0.37.4/LICENSE` & `mistapi-0.37.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/PKG-INFO` & `mistapi-0.37.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.37.4
+Version: 0.37.6
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.37.4/README.md` & `mistapi-0.37.6/README.md`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/pyproject.toml` & `mistapi-0.37.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mistapi"
-version = "0.37.4"
+version = "0.37.6"
 authors = [{name="Thomas Munzer", email="tmunzer@juniper.net"}]
 description = "Python package to simplify the Mist System APIs usage"
 keywords = ["Mist", "Juniper", "API"]
 license = {text =  "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mistapi-0.37.4/src/mistapi/__api_request.py` & `mistapi-0.37.6/src/mistapi/__api_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 This module manages API requests with Mist Cloud. It is used to 
 * generate the URL based on the provided parameters
 * add the required HTTP Headers to the request
 * report error if any
 '''
 
 import requests
+import os
+import json
 from requests.exceptions import HTTPError
 from mistapi.__api_response import APIResponse
 from mistapi.__logger import logger
 
 
 class APIRequest:
 
@@ -73,14 +75,15 @@
             resp = self._session.get(url)
             resp.raise_for_status()
         except HTTPError as http_err:
             logger.error(f'HTTP error occurred: {http_err}')  # Python 3.6
             logger.error(f'HTTP error description: {resp.json()}')
         except Exception as err:
             logger.error(f'Other error occurred: {err}')  # Python 3.6
+            logger.error("Exception occurred", exc_info=True)
         finally:
             return APIResponse(url=url, response=resp)
 
     def mist_post(self, uri:str,  body:object=None) -> APIResponse:
         """
         POST HTTP Request
 
@@ -108,14 +111,15 @@
                 resp = self._session.post(url, json=body, headers=headers)
             resp.raise_for_status()
         except HTTPError as http_err:
             logger.error(f'HTTP error occurred: {http_err}')  # Python 3.6
             logger.error(f'HTTP error description: {resp.json()}')
         except Exception as err:
             logger.error(f'Other error occurred: {err}')  # Python 3.6
+            logger.error("Exception occurred", exc_info=True)
         finally: 
             return APIResponse(url=url, response=resp)
 
     def mist_put(self, uri:str, body:object=None) -> APIResponse:
         """
         PUT HTTP Request
 
@@ -143,14 +147,15 @@
                 resp = self._session.put(url, json=body, headers=headers)
             resp.raise_for_status()
         except HTTPError as http_err:
             logger.error(f'HTTP error occurred: {http_err}')  # Python 3.6
             logger.error(f'HTTP error description: {resp.json()}')
         except Exception as err:
             logger.error(f'Other error occurred: {err}')  # Python 3.6
+            logger.error("Exception occurred", exc_info=True)
         finally: 
             return APIResponse(url=url, response=resp)
 
     def mist_delete(self, uri:str, query:object=None) -> APIResponse:
         """
         DELETE HTTP Request
 
@@ -167,19 +172,20 @@
             logger.info(f"apirequest:sending DELETE request to {url}")
             resp = self._session.delete(url)
             resp.raise_for_status()
         except HTTPError as http_err:
             logger.error(f'HTTP error occurred: {http_err}')  # Python 3.6
         except Exception as err:
             logger.error(f'Other error occurred: {err}')  # Python 3.6
+            logger.error("Exception occurred", exc_info=True)
         else: 
             return APIResponse(url=url, response=resp)
 
 
-    def mist_post_file(self, uri:str, files=None) -> APIResponse:
+    def mist_post_file(self, uri:str, file:str="", csv:str="", body:dict={}) -> APIResponse:
         """
         POST HTTP Request
 
         PARAMS
         -----------
         :param str uri - HTTP URI (e.g. "/api/v1/self") 
         :param object body 
@@ -187,17 +193,22 @@
         RETURN
         -----------
         :return APIResponse
         """
         try:                 
             url = self._url(uri)
             logger.info(f"apirequest:sending POST request to {url}")
-            resp = self._session.post(url, files=files)
+            multipart_form_data = {}
+            if file: multipart_form_data["file"] = (os.path.basename(file), open(file, 'rb'), 'application/octet-stream')
+            if csv: multipart_form_data["csv"] = (os.path.basename(csv), open(file, 'rb'), 'application/octet-stream')
+            if body: multipart_form_data["json"] = (None, json.dumps(body), 'application/json')
+            resp = self._session.post(url, files=multipart_form_data)
             resp.raise_for_status()
         except HTTPError as http_err:
             logger.error(f'HTTP error occurred: {http_err}')  # Python 3.6
             logger.error(f'HTTP error description: {resp.json()}')
             return resp
         except Exception as err:
             logger.error(f'Other error occurred: {err}')  # Python 3.6
+            logger.error("Exception occurred", exc_info=True)
         else: 
             return APIResponse(url=url, response=resp)
```

### Comparing `mistapi-0.37.4/src/mistapi/__api_response.py` & `mistapi-0.37.6/src/mistapi/__api_response.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/__api_session.py` & `mistapi-0.37.6/src/mistapi/__api_session.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/__init__.py` & `mistapi-0.37.6/src/mistapi/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 '''
 
 from mistapi.__api_session import APISession
 from mistapi import api
 from mistapi import cli
 from mistapi.__pagination import get_next, get_all
 
-__version__ = "0.37.4"
+__version__ = "0.37.6"
 __author__ = "Thomas Munzer <tmunzer@juniper.net>"
```

### Comparing `mistapi-0.37.4/src/mistapi/__logger.py` & `mistapi-0.37.6/src/mistapi/__logger.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/__models/privilege.py` & `mistapi-0.37.6/src/mistapi/__models/privilege.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/__pagination.py` & `mistapi-0.37.6/src/mistapi/__pagination.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/__init__.py` & `mistapi-0.37.6/src/mistapi/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/__init__.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/alarm_defs.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/mxedge_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
+def listMxEdgeModels(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getAlarmDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listMxEdgeModels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/alarm_defs"
+    uri = f"/api/v1/const/mxedge_models"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/ap_channels.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/ap_channels.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getApChannels(mist_session:_APISession, country_code:str=None) -> _APIResponse:
+def listApChannels(mist_session:_APISession, country_code:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getApChannels
+    API doc: https://doc.mist-lab.fr/#operation/listApChannels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     QUERY PARAMS
     ------------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/ap_led_status.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/ap_led_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getApLedDefinition(mist_session:_APISession) -> _APIResponse:
+def listApLedDefinition(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getApLedDefinition
+    API doc: https://doc.mist-lab.fr/#operation/listApLedDefinition
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/applications.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/countries.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getApplications(mist_session:_APISession) -> _APIResponse:
+def listCountryCodes(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getApplications
+    API doc: https://doc.mist-lab.fr/#operation/listCountryCodes
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/applications"
+    uri = f"/api/v1/const/countries"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/call_events.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/client_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getCallEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+def listClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getCallEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listClientEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/call_events"
+    uri = f"/api/v1/const/client_events"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/client_events.py` & `mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/alarmtemplates.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+def listInstallerAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getClientEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listInstallerAlarmTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    :param str org_id        
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/client_events"
+    uri = f"/api/v1/installer/orgs/{org_id}/alarmtemplates"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/countries.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/alarm_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getCountryCodes(mist_session:_APISession) -> _APIResponse:
+def listAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getCountryCodes
+    API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/countries"
+    uri = f"/api/v1/const/alarm_defs"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/default_gateway_config.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/default_gateway_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getGetawayDefaultConfig(mist_session:_APISession, model:str=None, ha:str=None) -> _APIResponse:
+def getGatawayDefaultConfig(mist_session:_APISession, model:str=None, ha:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getGetawayDefaultConfig
+    API doc: https://doc.mist-lab.fr/#operation/getGatawayDefaultConfig
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     QUERY PARAMS
     ------------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/device_events.py` & `mistapi-0.37.6/src/mistapi/api/v1/self/subscriptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+def listAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getDeviceEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listAlarmSubscriptions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/device_events"
+    uri = f"/api/v1/self/subscriptions"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/device_models.py` & `mistapi-0.37.6/src/mistapi/api/v1/recover/recover.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,24 +9,27 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getDeviceModels(mist_session:_APISession) -> _APIResponse:
+def recoverPassword(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getDeviceModels
+    API doc: https://doc.mist-lab.fr/#operation/recoverPassword
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/device_models"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/recover"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/insight_metrics.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/insight_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteAvailableInsightMetrics(mist_session:_APISession) -> _APIResponse:
+def listSiteAvailableInsightMetrics(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteAvailableInsightMetrics
+    API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableInsightMetrics
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/languages.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/languages.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteLanguages(mist_session:_APISession) -> _APIResponse:
+def listSiteLanguages(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteLanguages
+    API doc: https://doc.mist-lab.fr/#operation/listSiteLanguages
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/mxedge_events.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/mxedge_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+def listMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMxEdgeEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listMxEdgeEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/mxedge_models.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/traffic_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMxEdgeModels(mist_session:_APISession) -> _APIResponse:
+def listTrafficTypes(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMxEdgeModels
+    API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/mxedge_models"
+    uri = f"/api/v1/const/traffic_types"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/const/traffic_types.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/pma.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getTrafficTypes(mist_session:_APISession) -> _APIResponse:
+def listOrgPmaDashboards(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getTrafficTypes
+    API doc: https://doc.mist-lab.fr/#operation/listOrgPmaDashboards
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    :param str org_id        
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/const/traffic_types"
+    uri = f"/api/v1/orgs/{org_id}/pma/dashboards"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/__init__.py` & `mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/alarmtemplates.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/inventory.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getInstallerAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getMspInventoryByMac(mist_session:_APISession, msp_id:str, device_mac:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getInstallerAlarmTemplates
+    API doc: https://doc.mist-lab.fr/#operation/getMspInventoryByMac
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str msp_id
+    :param str device_mac        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/alarmtemplates"
+    uri = f"/api/v1/msps/{msp_id}/inventory/{device_mac}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/deviceprofiles.py` & `mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/sitegroups.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getInstallerDeviceProfiles_WIP_(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listInstallerSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getInstallerDeviceProfiles_WIP_
+    API doc: https://doc.mist-lab.fr/#operation/listInstallerSiteGroups
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/deviceprofiles"
+    uri = f"/api/v1/installer/orgs/{org_id}/sitegroups"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/devices.py` & `mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/devices.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getInstallerListOfRenctlyClaimedDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listInstallerListOfRenctlyClaimedDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getInstallerListOfRenctlyClaimedDevices
+    API doc: https://doc.mist-lab.fr/#operation/listInstallerListOfRenctlyClaimedDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -170,34 +170,28 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}/{image_name}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def addInstallerDeviceImageFile(mist_session:_APISession, org_id:str, image_name:str, device_mac:str, file_path:str) -> _APIResponse:
+def addInstallerDeviceImageFile(mist_session:_APISession, org_id:str, image_name:str, device_mac:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/addInstallerDeviceImage
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str image_name
     :param str device_mac        
     
-    FILE PARAMS
-    -----------
-    :param str file_path - path to the file to upload
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}/{image_name}"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri)
+    return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/rftemplates.py` & `mistapi-0.37.6/src/mistapi/api/v1/mobile/verify.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,31 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getInstallerRfTemplatesNames(mist_session:_APISession, org_id:str) -> _APIResponse:
+def activateSdkInvite(mist_session:_APISession, secret:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getInstallerRfTemplatesNames
+    API doc: https://doc.mist-lab.fr/#operation/activateSdkInvite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
+    :param str secret        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/rftemplates"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/mobile/verify/{secret}"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/secpolicies.py` & `mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/secpolicies.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getInstallerSecPolicies
+    API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/sitegroups.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/troubleshoot.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,28 +9,41 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getInstallerSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
+def troubleshootOrgClient(mist_session:_APISession, org_id:str, mac:str=None, site_id:str=None, start:int=None, end:int=None, type:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getInstallerSiteGroups
+    API doc: https://doc.mist-lab.fr/#operation/troubleshootOrgClient
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
+    QUERY PARAMS
+    ------------
+    :param str mac - **required** when troubleshooting device
+    :param str site_id - **required** when troubleshooting site
+    :param int start
+    :param int end
+    :param str type(wireless, wired, wan) - when troubleshooting site, type of network to troubleshoot        
+    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/sitegroups"
-    query_params={}
+    uri = f"/api/v1/orgs/{org_id}/troubleshoot"
+    query_params={}
+    if mac: query_params["mac"]=mac
+    if site_id: query_params["site_id"]=site_id
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if type: query_params["type"]=type
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/installer/orgs/sites.py` & `mistapi-0.37.6/src/mistapi/api/v1/installer/orgs/sites.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getInstallerSites(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listInstallerSites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getInstallerSites
+    API doc: https://doc.mist-lab.fr/#operation/listInstallerSites
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -55,17 +55,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def getInstallerMaps(mist_session:_APISession, org_id:str, site_name:str) -> _APIResponse:
+def listInstallerMaps(mist_session:_APISession, org_id:str, site_name:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getInstallerMaps
+    API doc: https://doc.mist-lab.fr/#operation/listInstallerMaps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -77,15 +77,15 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}/maps"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def importInstallerMapFile(mist_session:_APISession, org_id:str, site_name:str, file_path:str, body:dict={}) -> _APIResponse:
+def importInstallerMapFile(mist_session:_APISession, org_id:str, site_name:str, file_path:str="", csv_path:str="", body:dict={}) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importInstallerMap
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
@@ -93,28 +93,24 @@
     -----------
     :param str org_id
     :param str site_name        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    FILE PARAMS
-    -----------
     :param str file_path - path to the file to upload
+    :param str csv_path - path to the csv file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}/maps/import"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files, body=body)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri, file=file_path, csv=csv_path, body=body)
+    return resp
 
 def deleteInstallerMap(mist_session:_APISession, org_id:str, site_name:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/deleteInstallerMap
     
     PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/installer/sites/optimize.py` & `mistapi-0.37.6/src/mistapi/api/v1/installer/sites/optimize.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/invite/verify.py` & `mistapi-0.37.6/src/mistapi/api/v1/invite/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/login/__init__.py` & `mistapi-0.37.6/src/mistapi/api/v1/login/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/login/login.py` & `mistapi-0.37.6/src/mistapi/api/v1/login/login.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/login/lookup.py` & `mistapi-0.37.6/src/mistapi/api/v1/login/lookup.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/login/oauth.py` & `mistapi-0.37.6/src/mistapi/api/v1/login/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/login/two_factor.py` & `mistapi-0.37.6/src/mistapi/api/v1/login/two_factor.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/logout/logout.py` & `mistapi-0.37.6/src/mistapi/api/v1/logout/logout.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/mobile/verify.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/licenses.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,31 +9,52 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def activateSdkInvite(mist_session:_APISession, secret:str, body:object) -> _APIResponse:
+def listMspLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/activateSdkInvite
+    API doc: https://doc.mist-lab.fr/#operation/listMspLicenses
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str secret        
+    :param str msp_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/msps/{msp_id}/licenses"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def moveOrDeleteMspLicenseToAnotherOrg(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/moveOrDeleteMspLicenseToAnotherOrg
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str msp_id        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/mobile/verify/{secret}"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/msps/{msp_id}/licenses"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/__init__.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/admins.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/admins.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMspAdmins(mist_session:_APISession, msp_id:str) -> _APIResponse:
+def listMspAdmins(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspAdmins
+    API doc: https://doc.mist-lab.fr/#operation/listMspAdmins
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/claim.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/insights.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/inventory.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/logo.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,29 +9,52 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMspInventoryByMac(mist_session:_APISession, msp_id:str, device_mac:str) -> _APIResponse:
+def deleteMspLogo(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspInventoryByMac
+    API doc: https://doc.mist-lab.fr/#operation/deleteMspLogo
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id
-    :param str device_mac        
+    :param str msp_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/inventory/{device_mac}"
+    uri = f"/api/v1/msps/{msp_id}/logo"
     query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def postMspLogo(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/postMspLogo
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str msp_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/msps/{msp_id}/logo"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/invites.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/licenses.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/sites.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,52 +9,73 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMspLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
+def getSiteInfo(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspLicenses
+    API doc: https://doc.mist-lab.fr/#operation/getSiteInfo
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id        
+    :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/licenses"
+    uri = f"/api/v1/sites/{site_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def moveOrDeleteMspLicenseToAnotherOrg(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
+def deleteSite(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/moveOrDeleteMspLicenseToAnotherOrg
+    API doc: https://doc.mist-lab.fr/#operation/deleteSite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id        
+    :param str site_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def updateSiteInfo(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteInfo
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/licenses"
+    uri = f"/api/v1/sites/{site_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/logo.py` & `mistapi-0.37.6/src/mistapi/api/v1/self/oauth.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,52 +9,57 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def deleteMspLogo(mist_session:_APISession, msp_id:str) -> _APIResponse:
+def getOAuth2UrlForLinking(mist_session:_APISession, provider:str, forward:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteMspLogo
+    API doc: https://doc.mist-lab.fr/#operation/getOAuth2UrlForLinking
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id        
+    :param str provider        
+    
+    QUERY PARAMS
+    ------------
+    :param str forward        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/logo"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/self/oauth/{provider}"
+    query_params={}
+    if forward: query_params["forward"]=forward
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def postMspLogo(mist_session:_APISession, msp_id:str, body:object) -> _APIResponse:
+def linkOAuth2MistAccount(mist_session:_APISession, provider:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/postMspLogo
+    API doc: https://doc.mist-lab.fr/#operation/linkOAuth2MistAccount
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str msp_id        
+    :param str provider        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/msps/{msp_id}/logo"
+    uri = f"/api/v1/self/oauth/{provider}"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/logs.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMspLogs(mist_session:_APISession, msp_id:str, org_id:str=None, admin_name:str=None, message:str=None) -> _APIResponse:
+def listMspLogs(mist_session:_APISession, msp_id:str, org_id:str=None, admin_name:str=None, message:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspLogs
+    API doc: https://doc.mist-lab.fr/#operation/listMspLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/msps.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/msps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/orggroups.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/orggroups.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMspOrgGroups(mist_session:_APISession, msp_id:str) -> _APIResponse:
+def listMspOrgGroups(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspOrgGroups
+    API doc: https://doc.mist-lab.fr/#operation/listMspOrgGroups
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/orgs.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/orgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMspOrgs(mist_session:_APISession, msp_id:str) -> _APIResponse:
+def listMspOrgs(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspOrgs
+    API doc: https://doc.mist-lab.fr/#operation/listMspOrgs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/search.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/search.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/ssoroles.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/ssoroles.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMspSsoRoles(mist_session:_APISession, msp_id:str) -> _APIResponse:
+def listMspSsoRoles(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspSsoRoles
+    API doc: https://doc.mist-lab.fr/#operation/listMspSsoRoles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/ssos.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,17 +101,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def getMspSsoLatestFailures(mist_session:_APISession, msp_id:str, sso_id:str) -> _APIResponse:
+def listMspSsoLatestFailures(mist_session:_APISession, msp_id:str, sso_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspSsoLatestFailures
+    API doc: https://doc.mist-lab.fr/#operation/listMspSsoLatestFailures
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/stats.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMspOrgLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
+def listMspOrgLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspOrgLicenses
+    API doc: https://doc.mist-lab.fr/#operation/listMspOrgLicenses
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -30,17 +30,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/stats/licenses"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getMspOrgStats(mist_session:_APISession, msp_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def listMspOrgStats(mist_session:_APISession, msp_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspOrgStats
+    API doc: https://doc.mist-lab.fr/#operation/listMspOrgStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/msps/tickets.py` & `mistapi-0.37.6/src/mistapi/api/v1/msps/tickets.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getMspTickets(mist_session:_APISession, msp_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def listMspTickets(mist_session:_APISession, msp_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspTickets
+    API doc: https://doc.mist-lab.fr/#operation/listMspTickets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/__init__.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/admins.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/admins.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgAdmins(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgAdmins(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgAdmins
+    API doc: https://doc.mist-lab.fr/#operation/listOrgAdmins
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/alarms.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/alarmtemplates.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/alarmtemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgAlarmTemplates
+    API doc: https://doc.mist-lab.fr/#operation/listOrgAlarmTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -54,17 +54,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgSuppressedAlarms(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgSuppressedAlarms(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSuppressedAlarms
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSuppressedAlarms
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/apitokens.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/apitokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgApiTokens(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgApiTokens(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgApiTokens
+    API doc: https://doc.mist-lab.fr/#operation/listOrgApiTokens
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/aptemplates.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/aptemplates.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgAptemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgAptemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgAptemplates
+    API doc: https://doc.mist-lab.fr/#operation/listOrgAptemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/assetfilters.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/assetfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgAssetFilters(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgAssetFilters(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgAssetFilters
+    API doc: https://doc.mist-lab.fr/#operation/listOrgAssetFilters
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/assets.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgAssets(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgAssets(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgAssets
+    API doc: https://doc.mist-lab.fr/#operation/listOrgAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -54,39 +54,37 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/assets"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def importOrgAssetsFile(mist_session:_APISession, org_id:str, file_path:str) -> _APIResponse:
+def importOrgAssetsFile(mist_session:_APISession, org_id:str, file_path:str="") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importOrgAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
-    FILE PARAMS
+    BODY PARAMS
     -----------
     :param str file_path - path to the file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/assets/import"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri, file=file_path)
+    return resp
 
 def importOrgAssets(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importOrgAssets
     
     PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/call.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/cert.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/cert.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/claim.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/clients.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/clone.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/clone.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/crl.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/crl.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/deviceprofiles.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/deviceprofiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap", limit:int=100, page:int=1) -> _APIResponse:
+def listOrgDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap", limit:int=100, page:int=1) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgDeviceProfiles
+    API doc: https://doc.mist-lab.fr/#operation/listOrgDeviceProfiles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/devices.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgDevices
+    API doc: https://doc.mist-lab.fr/#operation/listOrgDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -256,17 +256,17 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getOrgApsMacs(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgApsMacs(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgApsMacs
+    API doc: https://doc.mist-lab.fr/#operation/listOrgApsMacs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -349,17 +349,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getOrgMultiSitesDevicesUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgMultiSitesDevicesUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgMultiSitesDevicesUpgrades
+    API doc: https://doc.mist-lab.fr/#operation/listOrgMultiSitesDevicesUpgrades
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/evpn_topologies.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/evpn_topologies.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgEvpnTopologies(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgEvpnTopologies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgEvpnTopologies
+    API doc: https://doc.mist-lab.fr/#operation/listOrgEvpnTopologies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/gatewaytemplates.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/gatewaytemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgGatewayTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgGatewayTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgGatewayTemplates
+    API doc: https://doc.mist-lab.fr/#operation/listOrgGatewayTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/guests.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/guests.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgGuestAuthorizations(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgGuestAuthorizations(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgGuestAuthorizations
+    API doc: https://doc.mist-lab.fr/#operation/listOrgGuestAuthorizations
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/insights.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/inventory.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/invites.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/jsi.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/jsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgJsiDevices(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None, mac:str=None) -> _APIResponse:
+def listOrgJsiDevices(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None, mac:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgJsiDevices
+    API doc: https://doc.mist-lab.fr/#operation/listOrgJsiDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -110,17 +110,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgJsiPastPurchases(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None) -> _APIResponse:
+def listOrgJsiPastPurchases(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgJsiPastPurchases
+    API doc: https://doc.mist-lab.fr/#operation/listOrgJsiPastPurchases
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/licenses.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/logs.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
+def listOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgLogs
+    API doc: https://doc.mist-lab.fr/#operation/listOrgLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/maps.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/maps.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,36 +9,32 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def importOrgMapsFile(mist_session:_APISession, org_id:str, file_path:str, body:dict={}) -> _APIResponse:
+def importOrgMapsFile(mist_session:_APISession, org_id:str, file_path:str="", csv_path:str="", body:dict={}) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importOrgMaps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    FILE PARAMS
-    -----------
     :param str file_path - path to the file to upload
+    :param str csv_path - path to the csv file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/maps/import"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files, body=body)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri, file=file_path, csv=csv_path, body=body)
+    return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/mxclusters.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/mxclusters.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgMxEdgeClusters(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgMxEdgeClusters(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgMxEdgeClusters
+    API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeClusters
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/mxedges.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/mxedges.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgMxEdges(mist_session:_APISession, org_id:str, for_sites:str="any", limit:int=100, page:int=1) -> _APIResponse:
+def listOrgMxEdges(mist_session:_APISession, org_id:str, for_sites:str="any", limit:int=100, page:int=1) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgMxEdges
+    API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdges
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -135,17 +135,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/unassign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgMxEdgeUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgMxEdgeUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgMxEdgeUpgrades
+    API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeUpgrades
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/mxtunnels.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/mxtunnels.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgMxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgMxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgMxTunnels
+    API doc: https://doc.mist-lab.fr/#operation/listOrgMxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/nacrules.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/nacrules.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgNacRules(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgNacRules(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgNacRules
+    API doc: https://doc.mist-lab.fr/#operation/listOrgNacRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/nactags.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/nactags.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgNacTags(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgNacTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgNacTags
+    API doc: https://doc.mist-lab.fr/#operation/listOrgNacTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/networks.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/networks.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgNetworks(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgNetworks(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgNetworks
+    API doc: https://doc.mist-lab.fr/#operation/listOrgNetworks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/networktemplates.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/networktemplates.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgNetworkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgNetworkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgNetworkTemplates
+    API doc: https://doc.mist-lab.fr/#operation/listOrgNetworkTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/ocdevices.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/ocdevices.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/orgs.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/orgs.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/otherdevices.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/otherdevices.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgOtherDevices(mist_session:_APISession, org_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
+def listOrgOtherDevices(mist_session:_APISession, org_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgOtherDevices
+    API doc: https://doc.mist-lab.fr/#operation/listOrgOtherDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/pma.py` & `mistapi-0.37.6/src/mistapi/api/v1/self/two_factor.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,49 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgPmaDashboards(mist_session:_APISession, org_id:str) -> _APIResponse:
+def generateQrCodeForVerification(mist_session:_APISession, by:str="qrcode") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgPmaDashboards
+    API doc: https://doc.mist-lab.fr/#operation/generateQrCodeForVerification
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    :param str org_id        
+    QUERY PARAMS
+    ------------
+    :param str by(qrcode)        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/pma/dashboards"
-    query_params={}
+    uri = f"/api/v1/self/two_factor/token"
+    query_params={}
+    if by: query_params["by"]=by
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
+    
+def verifyTwoFactor(mist_session:_APISession, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/verifyTwoFactor
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/self/two_factor/verify"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/pskportals.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/pskportals.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgPskPortals(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgPskPortals(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgPskPortals
+    API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortals
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/psks.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/psks.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgPsks(mist_session:_APISession, org_id:str, name:str=None, ssid:str=None, role:str=None, page:int=1, limit:int=100) -> _APIResponse:
+def listOrgPsks(mist_session:_APISession, org_id:str, name:str=None, ssid:str=None, role:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgPsks
+    API doc: https://doc.mist-lab.fr/#operation/listOrgPsks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -91,39 +91,37 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/psks"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def importOrgPsksFile(mist_session:_APISession, org_id:str, file_path:str) -> _APIResponse:
+def importOrgPsksFile(mist_session:_APISession, org_id:str, file_path:str="") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importOrgPsks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id        
     
-    FILE PARAMS
+    BODY PARAMS
     -----------
     :param str file_path - path to the file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/psks/import"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri, file=file_path)
+    return resp
 
 def importOrgPsks(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importOrgPsks
     
     PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/rftemplates.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/rftemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgRfTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgRfTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgRfTemplates
+    API doc: https://doc.mist-lab.fr/#operation/listOrgRfTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/sdkclients.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/sdkclients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/sdkinvites.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/sdkinvites.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSdkInvites(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listSdkInvites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSdkInvites
+    API doc: https://doc.mist-lab.fr/#operation/listSdkInvites
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/sdktemplates.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/sdktemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSdkTemplates
+    API doc: https://doc.mist-lab.fr/#operation/listSdkTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/secpolicies.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/secpolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSecPolicies
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSecPolicies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/servicepolicies.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/servicepolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgServicePolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgServicePolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgServicePolicies
+    API doc: https://doc.mist-lab.fr/#operation/listOrgServicePolicies
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/services.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgServices(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgServices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgServices
+    API doc: https://doc.mist-lab.fr/#operation/listOrgServices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/setting.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/sitegroups.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/sitegroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSiteGroups
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSiteGroups
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/sites.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/sites.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgSites(mist_session:_APISession, org_id:str, limit:int=100, page:int=1) -> _APIResponse:
+def listOrgSites(mist_session:_APISession, org_id:str, limit:int=100, page:int=1) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSites
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSites
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -161,33 +161,32 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def importOrgMapToSiteFile(mist_session:_APISession, org_id:str, site_name:str, file_path:str) -> _APIResponse:
+def importOrgMapToSiteFile(mist_session:_APISession, org_id:str, site_name:str, file_path:str="", csv_path:str="") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importOrgMapToSite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str site_name        
     
-    FILE PARAMS
+    BODY PARAMS
     -----------
     :param str file_path - path to the file to upload
+    :param str csv_path - path to the csv file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/sites/{site_name}/maps/import"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri, file=file_path, csv=csv_path)
+    return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/sitetemplates.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/sitetemplates.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgSiteTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgSiteTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSiteTemplates
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSiteTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/ssoroles.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/ssoroles.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgSsoRoles(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgSsoRoles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSsoRoles
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSsoRoles
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/ssos.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/ssos.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgSsos(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgSsos(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSsos
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSsos
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -123,17 +123,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def getOrgSsoLatestFailures(mist_session:_APISession, org_id:str, sso_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def listOrgSsoLatestFailures(mist_session:_APISession, org_id:str, sso_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSsoLatestFailures
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSsoLatestFailures
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/ssr.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/ssr.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/128routers/register_cmd"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSsrUpgrades
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/stats.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getOrgAssetsStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def listOrgAssetsStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgAssetsStats
+    API doc: https://doc.mist-lab.fr/#operation/listOrgAssetsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -205,17 +205,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/stats/bgp_peers/search"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getOrgDevicesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", type:str="ap", status:str="all", site_id:str=None, mac:str=None, evpntopo_id:str=None, evpn_unused:str=None) -> _APIResponse:
+def listOrgDevicesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", type:str="ap", status:str="all", site_id:str=None, mac:str=None, evpntopo_id:str=None, evpn_unused:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgDevicesStats
+    API doc: https://doc.mist-lab.fr/#operation/listOrgDevicesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -251,17 +251,17 @@
     if site_id: query_params["site_id"]=site_id
     if mac: query_params["mac"]=mac
     if evpntopo_id: query_params["evpntopo_id"]=evpntopo_id
     if evpn_unused: query_params["evpn_unused"]=evpn_unused
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getOrgMxEdgesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", for_site:str="false") -> _APIResponse:
+def listOrgMxEdgesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", for_site:str="false") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgMxEdgesStats
+    API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/subscriptions.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/templates.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgTemplates
+    API doc: https://doc.mist-lab.fr/#operation/listOrgTemplates
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/tickets.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/tickets.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgTickets(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def listOrgTickets(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgTickets
+    API doc: https://doc.mist-lab.fr/#operation/listOrgTickets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -136,40 +136,38 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/tickets/{ticket_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def addOrgTicketCommentFile(mist_session:_APISession, org_id:str, ticket_id:str, file_path:str) -> _APIResponse:
+def addOrgTicketCommentFile(mist_session:_APISession, org_id:str, ticket_id:str, file_path:str="") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/addOrgTicketComment
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str ticket_id        
     
-    FILE PARAMS
+    BODY PARAMS
     -----------
     :param str file_path - path to the file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/tickets/{ticket_id}/comments"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri, file=file_path)
+    return resp
 
 def addOrgTicketComment(mist_session:_APISession, org_id:str, ticket_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/addOrgTicketComment
     
     PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/troubleshoot.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/mxtunnels.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,41 +9,28 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def troubleshootOrgClient(mist_session:_APISession, org_id:str, mac:str=None, site_id:str=None, start:int=None, end:int=None, type:str=None) -> _APIResponse:
+def preemptSitesMxTunnel(mist_session:_APISession, site_id:str, mxtunnel_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/troubleshootOrgClient
+    API doc: https://doc.mist-lab.fr/#operation/preemptSitesMxTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str org_id        
-    
-    QUERY PARAMS
-    ------------
-    :param str mac - **required** when troubleshooting device
-    :param str site_id - **required** when troubleshooting site
-    :param int start
-    :param int end
-    :param str type(wireless, wired, wan) - when troubleshooting site, type of network to troubleshoot        
+    :param str site_id
+    :param str mxtunnel_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/troubleshoot"
-    query_params={}
-    if mac: query_params["mac"]=mac
-    if site_id: query_params["site_id"]=site_id
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if type: query_params["type"]=type
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/mxtunnels/{mxtunnel_id}/preempt_aps"
+    resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/vpns.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/vpns.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgsVpns(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgsVpns(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgsVpns
+    API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/webhooks.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/webhooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgWebhooks(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgWebhooks(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWebhooks
+    API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/wired_clients.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/wlans.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/wlans.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgWlans(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgWlans(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWlans
+    API doc: https://doc.mist-lab.fr/#operation/listOrgWlans
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -171,40 +171,34 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}/portal_image"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def uploadOrgWlanPortalImageFile(mist_session:_APISession, org_id:str, wlan_id:str, file_path:str) -> _APIResponse:
+def uploadOrgWlanPortalImageFile(mist_session:_APISession, org_id:str, wlan_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/uploadOrgWlanPortalImage
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str org_id
     :param str wlan_id        
     
-    FILE PARAMS
-    -----------
-    :param str file_path - path to the file to upload
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}/portal_image"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri)
+    return resp
 
 def updateOrgWlanPortalTemplate(mist_session:_APISession, org_id:str, wlan_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/updateOrgWlanPortalTemplate
     
     PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/wxrules.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/wxrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgWxRules(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgWxRules(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWxRules
+    API doc: https://doc.mist-lab.fr/#operation/listOrgWxRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/wxtags.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/wxtags.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgWxTags(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgWxTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWxTags
+    API doc: https://doc.mist-lab.fr/#operation/listOrgWxTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/orgs/wxtunnels.py` & `mistapi-0.37.6/src/mistapi/api/v1/orgs/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOrgWxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgWxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWxTunnels
+    API doc: https://doc.mist-lab.fr/#operation/listOrgWxTunnels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/recover/recover.py` & `mistapi-0.37.6/src/mistapi/api/v1/register/register.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def recoverPassword(mist_session:_APISession, body:object) -> _APIResponse:
+def registerNewAdmin(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/recoverPassword
+    API doc: https://doc.mist-lab.fr/#operation/registerNewAdmin
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/recover"
+    uri = f"/api/v1/register"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/recover/verify.py` & `mistapi-0.37.6/src/mistapi/api/v1/recover/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/register/register.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/call_events.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,27 +9,24 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def registerNewAdmin(mist_session:_APISession, body:object) -> _APIResponse:
+def listCallEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/registerNewAdmin
+    API doc: https://doc.mist-lab.fr/#operation/listCallEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/register"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/const/call_events"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/register/verify.py` & `mistapi-0.37.6/src/mistapi/api/v1/register/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/self/__init__.py` & `mistapi-0.37.6/src/mistapi/api/v1/self/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/self/apitokens.py` & `mistapi-0.37.6/src/mistapi/api/v1/self/apitokens.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getApiTokens(mist_session:_APISession) -> _APIResponse:
+def listApiTokens(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getApiTokens
+    API doc: https://doc.mist-lab.fr/#operation/listApiTokens
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/self/logs.py` & `mistapi-0.37.6/src/mistapi/api/v1/self/logs.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSelfAuditLogs(mist_session:_APISession, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def listSelfAuditLogs(mist_session:_APISession, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSelfAuditLogs
+    API doc: https://doc.mist-lab.fr/#operation/listSelfAuditLogs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     QUERY PARAMS
     ------------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/self/oauth.py` & `mistapi-0.37.6/src/mistapi/api/v1/self/self.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,57 +9,61 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getOAuth2UrlForLinking(mist_session:_APISession, provider:str, forward:str=None) -> _APIResponse:
+def getSelf(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOAuth2UrlForLinking
+    API doc: https://doc.mist-lab.fr/#operation/getSelf
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    :param str provider        
-    
-    QUERY PARAMS
-    ------------
-    :param str forward        
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/oauth/{provider}"
-    query_params={}
-    if forward: query_params["forward"]=forward
+    uri = f"/api/v1/self"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def linkOAuth2MistAccount(mist_session:_APISession, provider:str, body:object) -> _APIResponse:
+def deleteSelf(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/linkOAuth2MistAccount
+    API doc: https://doc.mist-lab.fr/#operation/deleteSelf
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    :param str provider        
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/self"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def updateSelf(mist_session:_APISession, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateSelf
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/oauth/{provider}"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/self"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/self/self.py` & `mistapi-0.37.6/src/mistapi/api/v1/self/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,61 +9,48 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSelf(mist_session:_APISession) -> _APIResponse:
+def updateSelfEmail(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSelf
+    API doc: https://doc.mist-lab.fr/#operation/updateSelfEmail
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/self"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def deleteSelf(mist_session:_APISession) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSelf
-    
-    PARAMS
+    BODY PARAMS
     -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/self/update"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def updateSelf(mist_session:_APISession, body:object) -> _APIResponse:
+def verifySelfEmail(mist_session:_APISession, token:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSelf
+    API doc: https://doc.mist-lab.fr/#operation/verifySelfEmail
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    PATH PARAMS
+    -----------
+    :param str token        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/self/update/verify/{token}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/self/subscriptions.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/device_events.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
+def listDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getAlarmSubscriptions
+    API doc: https://doc.mist-lab.fr/#operation/listDeviceEventsDefinitions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/subscriptions"
+    uri = f"/api/v1/const/device_events"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/self/two_factor.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/ssr.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,49 +9,54 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def generateQrCodeForVerification(mist_session:_APISession, by:str="qrcode") -> _APIResponse:
+def getSiteSsrUpgrade(mist_session:_APISession, site_id:str, upgrade_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/generateQrCodeForVerification
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSsrUpgrade
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    QUERY PARAMS
-    ------------
-    :param str by(qrcode)        
+    PATH PARAMS
+    -----------
+    :param str site_id
+    :param str upgrade_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/two_factor/token"
-    query_params={}
-    if by: query_params["by"]=by
+    uri = f"/api/v1/sites/{site_id}/ssr/upgrade/{upgrade_id}"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def verifyTwoFactor(mist_session:_APISession, body:object) -> _APIResponse:
+def upgradeSiteSsr(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/verifyTwoFactor
+    API doc: https://doc.mist-lab.fr/#operation/upgradeSiteSsr
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    :param str site_id
+    :param str device_id        
+    
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/two_factor/verify"
+    uri = f"/api/v1/sites/{site_id}/ssr/{device_id}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/self/update.py` & `mistapi-0.37.6/src/mistapi/api/v1/utils/test_twilio.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,48 +9,27 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def updateSelfEmail(mist_session:_APISession, body:object) -> _APIResponse:
+def testSiteWlanTwilioSetup(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSelfEmail
+    API doc: https://doc.mist-lab.fr/#operation/testSiteWlanTwilioSetup
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/self/update"
+    uri = f"/api/v1/utils/test_twilio"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
-    
-def verifySelfEmail(mist_session:_APISession, token:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/verifySelfEmail
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str token        
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/self/update/verify/{token}"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/__init__.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/alarms.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/anomaly.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/anomaly.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/apps.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteApps
+    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/assetfilters.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/assetfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteAssetFilters(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteAssetFilters(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteAssetFilters
+    API doc: https://doc.mist-lab.fr/#operation/listSiteAssetFilters
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/assets.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteAssets(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteAssets(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteAssets
+    API doc: https://doc.mist-lab.fr/#operation/listSiteAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -54,39 +54,37 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/assets"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def importSiteAssetsFile(mist_session:_APISession, site_id:str, file_path:str) -> _APIResponse:
+def importSiteAssetsFile(mist_session:_APISession, site_id:str, file_path:str="") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importSiteAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
-    FILE PARAMS
+    BODY PARAMS
     -----------
     :param str file_path - path to the file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/assets/import"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri, file=file_path)
+    return resp
 
 def importSiteAssets(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importSiteAssets
     
     PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/beacons.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/beacons.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteBeacons
+    API doc: https://doc.mist-lab.fr/#operation/listSiteBeacons
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/call.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/clients.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/count.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/count.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/devices.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteDevices(mist_session:_APISession, site_id:str, type:str="ap", name:str=None, page:int=1, limit:int=100) -> _APIResponse:
+def listSiteDevices(mist_session:_APISession, site_id:str, type:str="ap", name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteDevices
+    API doc: https://doc.mist-lab.fr/#operation/listSiteDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -41,38 +41,14 @@
     if type: query_params["type"]=type
     if name: query_params["name"]=name
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteDevice(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteDevice
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id        
-    
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/devices"
-    resp = mist_session.mist_post(uri=uri, body=body)
-    return resp
-    
 def getSiteDeviceRadioChannels(mist_session:_APISession, site_id:str, country_code:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceRadioChannels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
@@ -663,17 +639,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/upgrade/{upgrade_id}/cancel"
     resp = mist_session.mist_post(uri=uri)
     return resp
     
-def getSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap") -> _APIResponse:
+def listSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteAvailableDeviceVersions
+    API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableDeviceVersions
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -1079,41 +1055,35 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/image{image_number}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def addSiteDeviceImageFile(mist_session:_APISession, site_id:str, device_id:str, image_number:int, file_path:str) -> _APIResponse:
+def addSiteDeviceImageFile(mist_session:_APISession, site_id:str, device_id:str, image_number:int) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/addSiteDeviceImage
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str device_id
     :param int image_number        
     
-    FILE PARAMS
-    -----------
-    :param str file_path - path to the file to upload
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/image{image_number}"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri)
+    return resp
 
 def getSiteDeviceIotPort(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceIotPort
     
     PARAMS
     -----------
@@ -1602,17 +1572,17 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteVirtualChassis(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
+def getSiteDeviceVirtualChassis(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteVirtualChassis
+    API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceVirtualChassis
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/events.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/evpn_topologies.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/evpn_topologies.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteEvpnTopologies(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteEvpnTopology(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteEvpnTopologies
+    API doc: https://doc.mist-lab.fr/#operation/getSiteEvpnTopology
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/guests.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/guests.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteAllGuestAuthorizations(mist_session:_APISession, site_id:str, wlan_id:str=None) -> _APIResponse:
+def listSiteAllGuestAuthorizations(mist_session:_APISession, site_id:str, wlan_id:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteAllGuestAuthorizations
+    API doc: https://doc.mist-lab.fr/#operation/listSiteAllGuestAuthorizations
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/insights.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/insights.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,17 +85,17 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteRogueAPs(mist_session:_APISession, site_id:str, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
+def listSiteRogueAPs(mist_session:_APISession, site_id:str, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteRogueAPs
+    API doc: https://doc.mist-lab.fr/#operation/listSiteRogueAPs
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -121,17 +121,17 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteRogueClients(mist_session:_APISession, site_id:str, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
+def listSiteRogueClients(mist_session:_APISession, site_id:str, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteRogueClients
+    API doc: https://doc.mist-lab.fr/#operation/listSiteRogueClients
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/licenses.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/location.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/location.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/maps.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/maps.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteMaps(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteMaps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteMaps
+    API doc: https://doc.mist-lab.fr/#operation/listSiteMaps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -54,43 +54,39 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def importSiteMapsFile(mist_session:_APISession, site_id:str, file_path:str, body:dict={}) -> _APIResponse:
+def importSiteMapsFile(mist_session:_APISession, site_id:str, file_path:str="", csv_path:str="", body:dict={}) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importSiteMaps
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    FILE PARAMS
-    -----------
     :param str file_path - path to the file to upload
+    :param str csv_path - path to the csv file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/import"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files, body=body)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri, file=file_path, csv=csv_path, body=body)
+    return resp
 
 def getSiteMap(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteMap
     
     PARAMS
     -----------
@@ -337,42 +333,36 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/{map_id}/image"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def addSiteMapImageFile(mist_session:_APISession, site_id:str, map_id:str, file_path:str) -> _APIResponse:
+def addSiteMapImageFile(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/addSiteMapImage
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str map_id        
     
-    FILE PARAMS
-    -----------
-    :param str file_path - path to the file to upload
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/{map_id}/image"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri)
+    return resp
 
-def replaceSiteMapImageFile(mist_session:_APISession, site_id:str, map_id:str, file_path:str, body:dict={}) -> _APIResponse:
+def replaceSiteMapImageFile(mist_session:_APISession, site_id:str, map_id:str, file_path:str="", body:dict={}) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/replaceSiteMapImage
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
@@ -380,28 +370,23 @@
     -----------
     :param str site_id
     :param str map_id        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    FILE PARAMS
-    -----------
     :param str file_path - path to the file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps/{map_id}/replace"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files, body=body)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri, file=file_path, body=body)
+    return resp
 
 def bulkAssignSiteApsToMap(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/bulkAssignSiteApsToMap
     
     PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/mxedges.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/mxedges.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteMxEdges(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteMxEdges(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteMxEdges
+    API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdges
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/mxtunnels.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/subscriptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,28 +9,48 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def preemptSitesMxTunnel(mist_session:_APISession, site_id:str, mxtunnel_id:str) -> _APIResponse:
+def UnsubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/preemptSitesMxTunnel
+    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSite
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    :param str site_id
-    :param str mxtunnel_id        
+    :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/mxtunnels/{mxtunnel_id}/preempt_aps"
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def SubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/SubscribeSite
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
     resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/otherdevices.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/otherdevices.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
+def listSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteOtherDevices
+    API doc: https://doc.mist-lab.fr/#operation/listSiteOtherDevices
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/pcaps.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/pcaps.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
+def listSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSitePacketCaptures
+    API doc: https://doc.mist-lab.fr/#operation/listSitePacketCaptures
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/psks.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/psks.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSitePsks(mist_session:_APISession, site_id:str, ssid:str=None, role:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
+def listSitePsks(mist_session:_APISession, site_id:str, ssid:str=None, role:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSitePsks
+    API doc: https://doc.mist-lab.fr/#operation/listSitePsks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -91,39 +91,37 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/psks"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def importSitePsksFile(mist_session:_APISession, site_id:str, file_path:str) -> _APIResponse:
+def importSitePsksFile(mist_session:_APISession, site_id:str, file_path:str="") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importSitePsks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
-    FILE PARAMS
+    BODY PARAMS
     -----------
     :param str file_path - path to the file to upload
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/psks/import"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri, file=file_path)
+    return resp
 
 def importSitePsks(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importSitePsks
     
     PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/rfdiags.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/rfdiags.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/rogues.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/rogues.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/rrm.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/rrm.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/rssizones.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/rssizones.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteRssiZones(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteRssiZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteRssiZones
+    API doc: https://doc.mist-lab.fr/#operation/listSiteRssiZones
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/setting.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/sites.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/synthetic_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,59 +9,38 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteInfo(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteSyntheticTestStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteInfo
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSyntheticTestStatus
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}"
+    uri = f"/api/v1/sites/{site_id}/synthetic_test"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSite(mist_session:_APISession, site_id:str) -> _APIResponse:
+def triggerSiteSyntheticTest(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSite
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id        
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
-    return resp
-    
-def updateSiteInfo(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteInfo
+    API doc: https://doc.mist-lab.fr/#operation/triggerSiteSyntheticTest
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -71,11 +50,11 @@
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/synthetic_test"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/skyatp.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/skyatp.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/sle.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/sle.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/ssr.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/wxtunnels.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,54 +9,121 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteSsrUpgrade(mist_session:_APISession, site_id:str, upgrade_id:str) -> _APIResponse:
+def listSiteWxTunnels(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteSsrUpgrade
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wxtunnels"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def createSiteWxTunnel(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/createSiteWxTunnel
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wxtunnels"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
+def getSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str upgrade_id        
+    :param str wxtunnel_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/ssr/upgrade/{upgrade_id}"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def upgradeSiteSsr(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
+def deleteSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/upgradeSiteSsr
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxTunnel
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str device_id        
+    :param str wxtunnel_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def updateSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxTunnel
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id
+    :param str wxtunnel_id        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/ssr/{device_id}/upgrade"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/stats.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,17 @@
     if distinct: query_params["distinct"]=distinct
     if device_mac: query_params["device_mac"]=device_mac
     if app: query_params["app"]=app
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteAssetsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def listSiteAssetsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteAssetsStats
+    API doc: https://doc.mist-lab.fr/#operation/listSiteAssetsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -212,17 +212,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteBeaconsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def listSiteBeaconsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteBeaconsStats
+    API doc: https://doc.mist-lab.fr/#operation/listSiteBeaconsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -363,17 +363,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteClientsStats(mist_session:_APISession, site_id:str, wired:bool=None) -> _APIResponse:
+def listSiteClientsStats(mist_session:_APISession, site_id:str, wired:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteClientsStats
+    API doc: https://doc.mist-lab.fr/#operation/listSiteClientsStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -416,17 +416,17 @@
     """
     uri = f"/api/v1/sites/{site_id}/stats/clients/{client_mac}"
     query_params={}
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteDevicesStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", type:str="ap", status:str="all") -> _APIResponse:
+def listSiteDevicesStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", type:str="ap", status:str="all") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteDevicesStats
+    API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -498,17 +498,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/devices/{device_id}/clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteDiscoveredAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def listSiteDiscoveredAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteDiscoveredAssets
+    API doc: https://doc.mist-lab.fr/#operation/listSiteDiscoveredAssets
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -810,17 +810,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/sdkclients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteUnconnectedClientStats(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
+def listSiteUnconnectedClientStats(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteUnconnectedClientStats
+    API doc: https://doc.mist-lab.fr/#operation/listSiteUnconnectedClientStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -832,17 +832,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/unconnected_clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteMxEdgesStats(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteMxEdgesStats(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteMxEdgesStats
+    API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdgesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -1312,17 +1312,17 @@
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteZonesStats(mist_session:_APISession, site_id:str, map_id:str=None) -> _APIResponse:
+def listSiteZonesStats(mist_session:_APISession, site_id:str, map_id:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteZonesStats
+    API doc: https://doc.mist-lab.fr/#operation/listSiteZonesStats
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/synthetic_test.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/wxrules.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteSyntheticTestStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteWxRules(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteSyntheticTestStatus
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/synthetic_test"
+    uri = f"/api/v1/sites/{site_id}/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def triggerSiteSyntheticTest(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteWxRule(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/triggerSiteSyntheticTest
+    API doc: https://doc.mist-lab.fr/#operation/createSiteWxRule
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -50,11 +50,101 @@
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/synthetic_test"
+    uri = f"/api/v1/sites/{site_id}/wxrules"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
+    
+def getSiteWxRulesDerived(mist_session:_APISession, site_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRulesDerived
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wxrules/derived"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def getSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRule
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id
+    :param str wxrules_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def deleteSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxRule
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id
+    :param str wxrules_id        
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def updateSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxRule
+    
+    PARAMS
+    -----------
+    :param APISession mist_session - mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    :param str site_id
+    :param str wxrules_id        
+    
+    BODY PARAMS
+    -----------
+    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    :return APIResponse - response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
+    return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/uisettings.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/uisettings.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/vbeacons.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/vbeacons.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteVBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteVBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteVBeacons
+    API doc: https://doc.mist-lab.fr/#operation/listSiteVBeacons
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/visits.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/visits.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/webhooks.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteWebhooks(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteWebhooks(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWebhooks
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWebhooks
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/wired_clients.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/wlans.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/wlans.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteWlans(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteWlans(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWlans
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWlans
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -149,40 +149,34 @@
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wlans/{wlan_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def uploadSiteWlanPortalImageFile(mist_session:_APISession, site_id:str, wlan_id:str, file_path:str) -> _APIResponse:
+def uploadSiteWlanPortalImageFile(mist_session:_APISession, site_id:str, wlan_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/uploadSiteWlanPortalImage
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
     :param str wlan_id        
     
-    FILE PARAMS
-    -----------
-    :param str file_path - path to the file to upload
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wlans/{wlan_id}/portal_image"
-    with open(file_path, "rb") as f:    
-        files = {"file": f.read()}
-        resp = mist_session.mist_post_file(uri=uri, files=files)
-        return resp
+    resp = mist_session.mist_post_file(uri=uri)
+    return resp
 
 def updateSiteWlanPortalTemplate(mist_session:_APISession, site_id:str, wlan_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/updateSiteWlanPortalTemplate
     
     PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/wxrules.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/zones.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteWxRules(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRules
+    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules"
+    uri = f"/api/v1/sites/{site_id}/zones"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteWxRule(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteZone(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/createSiteZone
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
@@ -50,101 +50,80 @@
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules"
+    uri = f"/api/v1/sites/{site_id}/zones"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteWxRulesDerived(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRulesDerived
-    
-    PARAMS
-    -----------
-    :param APISession mist_session - mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    :param str site_id        
-    
-    RETURN
-    -----------
-    :return APIResponse - response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/wxrules/derived"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def getSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/getSiteZone
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str wxrules_id        
+    :param str zone_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
+def deleteSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteZone
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str wxrules_id        
+    :param str zone_id        
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str, body:object) -> _APIResponse:
+def updateSiteZone(mist_session:_APISession, site_id:str, zone_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteZone
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     :param str site_id
-    :param str wxrules_id        
+    :param str zone_id        
     
     BODY PARAMS
     -----------
     :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/sites/wxtags.py` & `mistapi-0.37.6/src/mistapi/api/v1/sites/wxtags.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def getSiteWxTags(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteWxTags(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxTags
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
```

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/utils/test_telstra.py` & `mistapi-0.37.6/src/mistapi/api/v1/utils/test_telstra.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi/api/v1/utils/test_twilio.py` & `mistapi-0.37.6/src/mistapi/api/v1/const/device_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,27 +9,24 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 
-def testSiteWlanTwilioSetup(mist_session:_APISession, body:object) -> _APIResponse:
+def listDeviceModels(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/testSiteWlanTwilioSetup
+    API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
     
     PARAMS
     -----------
     :param APISession mist_session - mistapi session including authentication and Mist host information
     
-    BODY PARAMS
-    -----------
-    :param dict body - JSON object to send to Mist Cloud (see API doc above for more details)
-    
     RETURN
     -----------
     :return APIResponse - response from the API call
     """
-    uri = f"/api/v1/utils/test_twilio"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/const/device_models"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.37.4/src/mistapi/cli.py` & `mistapi-0.37.6/src/mistapi/cli.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.37.4/src/mistapi.egg-info/PKG-INFO` & `mistapi-0.37.6/src/mistapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.37.4
+Version: 0.37.6
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.37.4/src/mistapi.egg-info/SOURCES.txt` & `mistapi-0.37.6/src/mistapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/fittings-1.1.0.tar.gz` & `tmp/fittings-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fittings-1.1.0.tar", last modified: Wed Mar  9 12:23:48 2022, max compression
+gzip compressed data, was "dist/fittings-2.0.0.tar", last modified: Thu Apr 20 05:13:46 2023, max compression
```

## Comparing `fittings-1.1.0.tar` & `fittings-2.0.0.tar`

### file list

```diff
@@ -1,147 +1,150 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     5226 2022-03-09 12:23:48.000000 fittings-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35065 2022-03-09 12:23:38.000000 fittings-1.1.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/
--rw-rw-rw-   0 root         (0) root         (0)      964 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/auth_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/cogs/
--rw-rw-rw-   0 root         (0) root         (0)     8433 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/cogs/fittings.py
--rw-rw-rw-   0 root         (0) root         (0)    11699 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/templates/fittings/
--rw-rw-rw-   0 root         (0) root         (0)     2416 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/edit_fit.html
--rw-rw-rw-   0 root         (0) root         (0)    34682 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/view_fit.html
--rw-rw-rw-   0 root         (0) root         (0)     4366 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/view_all_categories.html
--rw-rw-rw-   0 root         (0) root         (0)     3559 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     5803 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/view_doctrine.html
--rw-rw-rw-   0 root         (0) root         (0)     3233 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/view_all_fits.html
--rw-rw-rw-   0 root         (0) root         (0)     6031 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/edit_category.html
--rw-rw-rw-   0 root         (0) root         (0)     6339 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/add_doctrine.html
--rw-rw-rw-   0 root         (0) root         (0)     3022 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/base.html
--rw-rw-rw-   0 root         (0) root         (0)     8161 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/view_category.html
--rw-rw-rw-   0 root         (0) root         (0)     2353 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/add_fit.html
--rw-rw-rw-   0 root         (0) root         (0)     5841 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/create_category.html
--rw-rw-rw-   0 root         (0) root         (0)     6776 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templates/fittings/edit_doctrine.html
--rw-rw-rw-   0 root         (0) root         (0)       68 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/static/fittings/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/static/fittings/img/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/
--rw-rw-rw-   0 root         (0) root         (0)     8580 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/7m.png
--rw-rw-rw-   0 root         (0) root         (0)     4956 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/4m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/0l.png
--rw-rw-rw-   0 root         (0) root         (0)     5888 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/5l.png
--rw-rw-rw-   0 root         (0) root         (0)    43642 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/tyrannis.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/h.png
--rw-rw-rw-   0 root         (0) root         (0)     7439 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/6m.png
--rw-rw-rw-   0 root         (0) root         (0)     7399 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/5s.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/r.png
--rw-rw-rw-   0 root         (0) root         (0)     4607 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/3h.png
--rw-rw-rw-   0 root         (0) root         (0)     3541 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/2h.png
--rw-rw-rw-   0 root         (0) root         (0)    16840 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/circle.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/l.png
--rw-rw-rw-   0 root         (0) root         (0)     4886 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/3r.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/m.png
--rw-rw-rw-   0 root         (0) root         (0)     2766 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/2m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/0r.png
--rw-rw-rw-   0 root         (0) root         (0)     3720 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/3m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/0m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/0s.png
--rw-rw-rw-   0 root         (0) root         (0)     6109 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/5h.png
--rw-rw-rw-   0 root         (0) root         (0)     4628 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/4l.png
--rw-rw-rw-   0 root         (0) root         (0)    33523 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/dustwheel.png
--rw-rw-rw-   0 root         (0) root         (0)     8972 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/8l.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/0h.png
--rw-rw-rw-   0 root         (0) root         (0)     9490 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/4s.png
--rw-rw-rw-   0 root         (0) root         (0)     6270 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/5m.png
--rw-rw-rw-   0 root         (0) root         (0)    38343 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/tyrannis_default.png
--rw-rw-rw-   0 root         (0) root         (0)    43560 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/tyrannis_blue.png
--rw-rw-rw-   0 root         (0) root         (0)      780 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/working.jpg
--rw-rw-rw-   0 root         (0) root         (0)     8067 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/7l.png
--rw-rw-rw-   0 root         (0) root         (0)     2512 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/1r.png
--rw-rw-rw-   0 root         (0) root         (0)     8879 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/noship.png
--rw-rw-rw-   0 root         (0) root         (0)     1976 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/1l.png
--rw-rw-rw-   0 root         (0) root         (0)     5309 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/4h.png
--rw-rw-rw-   0 root         (0) root         (0)     8288 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/7h.png
--rw-rw-rw-   0 root         (0) root         (0)     3523 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/3l.png
--rw-rw-rw-   0 root         (0) root         (0)     7203 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/6h.png
--rw-rw-rw-   0 root         (0) root         (0)     2590 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/1h.png
--rw-rw-rw-   0 root         (0) root         (0)     2025 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/1m.png
--rw-rw-rw-   0 root         (0) root         (0)    42868 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/tyrannis_revelations.png
--rw-rw-rw-   0 root         (0) root         (0)      195 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/blank.png
--rw-rw-rw-   0 root         (0) root         (0)     2570 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/2l.png
--rw-rw-rw-   0 root         (0) root         (0)     3497 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/2r.png
--rw-rw-rw-   0 root         (0) root         (0)     7014 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/6l.png
--rw-rw-rw-   0 root         (0) root         (0)      785 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/error.jpg
--rw-rw-rw-   0 root         (0) root         (0)    42833 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/tyrannis_darkred.png
--rw-rw-rw-   0 root         (0) root         (0)     9541 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/8m.png
--rw-rw-rw-   0 root         (0) root         (0)     9276 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/static/fittings/img/pannel/8h.png
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9416 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/models.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/tests.py
--rw-rw-rw-   0 root         (0) root         (0)     7475 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/managers.py
--rw-rw-rw-   0 root         (0) root         (0)    24776 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/views.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1328 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0005_unicategory.py
--rw-rw-rw-   0 root         (0) root         (0)      750 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0003_remove_type_description_not_null.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0008_auto_20200605_0736.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0014_serverversion.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0010_auto_20200718_2227.py
--rw-rw-rw-   0 root         (0) root         (0)     6132 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0011_auto_20200815_2022.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0012_typehistory.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0013_alter_doctrine_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0007_auto_20200605_0735.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0004_add_item_category_and_group.py
--rw-rw-rw-   0 root         (0) root         (0)      718 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0009_auto_20200605_2117.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0002_add_dgm_unique_constraints.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/migrations/0006_auto_20200605_0724.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      373 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10078 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      518 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/ru/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10229 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10085 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/fr_FR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/fr_FR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      337 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/fr_FR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10038 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      373 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/ja/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10078 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5900 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    12224 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/ko_KR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/locale/ko_KR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      337 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/ko_KR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10038 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)      569 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templatetags/filters.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1409 2022-03-09 12:23:38.000000 fittings-1.1.0/fittings/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-03-09 12:23:38.000000 fittings-1.1.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1572 2022-03-09 12:23:38.000000 fittings-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5226 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4736 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      130 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-09 12:23:48.000000 fittings-1.1.0/fittings.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)     4246 2022-03-09 12:23:38.000000 fittings-1.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-03-09 12:23:48.000000 fittings-1.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-04-20 05:13:46.000000 fittings-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35065 2023-04-20 05:13:35.000000 fittings-2.0.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/auth_hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/cogs/
+-rw-rw-rw-   0 root         (0) root         (0)     8433 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/cogs/fittings.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/templates/fittings/
+-rw-rw-rw-   0 root         (0) root         (0)     2417 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/edit_fit.html
+-rw-rw-rw-   0 root         (0) root         (0)    35170 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/view_fit.html
+-rw-rw-rw-   0 root         (0) root         (0)     4478 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/view_all_categories.html
+-rw-rw-rw-   0 root         (0) root         (0)     3666 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     6497 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/view_doctrine.html
+-rw-rw-rw-   0 root         (0) root         (0)     3345 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/view_all_fits.html
+-rw-rw-rw-   0 root         (0) root         (0)     6031 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/edit_category.html
+-rw-rw-rw-   0 root         (0) root         (0)     6365 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/add_doctrine.html
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     8161 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/view_category.html
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/add_fit.html
+-rw-rw-rw-   0 root         (0) root         (0)     6312 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/create_category.html
+-rw-rw-rw-   0 root         (0) root         (0)     6766 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templates/fittings/edit_doctrine.html
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/management/commands/fittings_preload_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/static/fittings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/static/fittings/img/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/
+-rw-rw-rw-   0 root         (0) root         (0)     8580 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/7m.png
+-rw-rw-rw-   0 root         (0) root         (0)     4956 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/4m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/0l.png
+-rw-rw-rw-   0 root         (0) root         (0)     5888 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/5l.png
+-rw-rw-rw-   0 root         (0) root         (0)    43642 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/h.png
+-rw-rw-rw-   0 root         (0) root         (0)     7439 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/6m.png
+-rw-rw-rw-   0 root         (0) root         (0)     7399 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/5s.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/r.png
+-rw-rw-rw-   0 root         (0) root         (0)     4607 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/3h.png
+-rw-rw-rw-   0 root         (0) root         (0)     3541 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/2h.png
+-rw-rw-rw-   0 root         (0) root         (0)    16840 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/circle.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/l.png
+-rw-rw-rw-   0 root         (0) root         (0)     4886 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/3r.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/m.png
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/2m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/0r.png
+-rw-rw-rw-   0 root         (0) root         (0)     3720 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/3m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/0m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/0s.png
+-rw-rw-rw-   0 root         (0) root         (0)     6109 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/5h.png
+-rw-rw-rw-   0 root         (0) root         (0)     4628 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/4l.png
+-rw-rw-rw-   0 root         (0) root         (0)    33523 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/dustwheel.png
+-rw-rw-rw-   0 root         (0) root         (0)     8972 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/8l.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/0h.png
+-rw-rw-rw-   0 root         (0) root         (0)     9490 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/4s.png
+-rw-rw-rw-   0 root         (0) root         (0)     6270 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/5m.png
+-rw-rw-rw-   0 root         (0) root         (0)    38343 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_default.png
+-rw-rw-rw-   0 root         (0) root         (0)    43560 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_blue.png
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/working.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     8067 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/7l.png
+-rw-rw-rw-   0 root         (0) root         (0)     2512 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/1r.png
+-rw-rw-rw-   0 root         (0) root         (0)     8879 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/noship.png
+-rw-rw-rw-   0 root         (0) root         (0)     1976 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/1l.png
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/4h.png
+-rw-rw-rw-   0 root         (0) root         (0)     8288 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/7h.png
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/3l.png
+-rw-rw-rw-   0 root         (0) root         (0)     7203 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/6h.png
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/1h.png
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/1m.png
+-rw-rw-rw-   0 root         (0) root         (0)    42868 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_revelations.png
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/blank.png
+-rw-rw-rw-   0 root         (0) root         (0)     2570 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/2l.png
+-rw-rw-rw-   0 root         (0) root         (0)     3497 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/2r.png
+-rw-rw-rw-   0 root         (0) root         (0)     7014 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/6l.png
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/error.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    42833 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_darkred.png
+-rw-rw-rw-   0 root         (0) root         (0)     9541 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/8m.png
+-rw-rw-rw-   0 root         (0) root         (0)     9276 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/static/fittings/img/pannel/8h.png
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6647 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)    24902 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/views.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0005_unicategory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      750 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0003_remove_type_description_not_null.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0008_auto_20200605_0736.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0014_serverversion.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0010_auto_20200718_2227.py
+-rw-rw-rw-   0 root         (0) root         (0)     6132 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0011_auto_20200815_2022.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0012_typehistory.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0013_alter_doctrine_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0007_auto_20200605_0735.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0004_add_item_category_and_group.py
+-rw-rw-rw-   0 root         (0) root         (0)      718 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0009_auto_20200605_2117.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0002_add_dgm_unique_constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/migrations/0006_auto_20200605_0724.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10078 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10229 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10085 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/fr_FR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/fr_FR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10038 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6341 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13534 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5900 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    12224 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/ko_KR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/locale/ko_KR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5263 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13034 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templatetags/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2023-04-20 05:13:35.000000 fittings-2.0.0/fittings/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-04-20 05:13:35.000000 fittings-2.0.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1645 2023-04-20 05:13:35.000000 fittings-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4857 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 05:13:46.000000 fittings-2.0.0/fittings.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)     4554 2023-04-20 05:13:35.000000 fittings-2.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-20 05:13:46.000000 fittings-2.0.0/setup.cfg
```

### Comparing `fittings-1.1.0/PKG-INFO` & `fittings-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: fittings
-Version: 1.1.0
+Version: 2.0.0
 Summary: A simple fittings and doctrine management application.
 Home-page: https://gitlab.com/colcrunch/fittings
 Author: Col Crunch
 Author-email: it-team@serin.space
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
@@ -105,37 +106,37 @@
 $ pip install fittings 
 ```
 
 ### 2. Configure AA settings
 
 Configure your AA settings (`local.py`) as follows:
 
-- Add `'fittings',` to `INSTALLED_APPS`
+- Add `'eveuniverse',` and `'fittings',` to `INSTALLED_APPS`
 - Add these line to the bottom of the settings file to have module name updates
 
-```python
-# Fittings Module
-CELERYBEAT_SCHEDULE['fittings_update_types'] = {
-    'task': 'fittings.tasks.verify_server_version_and_update_types',
-    'schedule': crontab(minute=0, hour='12'),
-}
-```
 ### 3. Finalize Install
 Run migrations and copy static files. 
 
 ```bash
 $ python manage.py migrate
 $ python manage.py collectstatic
 ```
 
 Restart your supervisor tasks.
 
 ### 4. Populate Types
-As of v1.0.0 there is no need to populate types from SDE. This will be done on the fly from
-ESI. 
+Now that fittings has transitioned to using [django-eveuniverse](https://gitlab.com/ErikKalkoken/django-eveuniverse) to handle static data this step is optional.
+
+You can choose to run the following command to preload the type information for most ships and modules in the game, or you can skip this step and let them be created on an as-needed basis.
+
+Keep in mind that running this command will take a while but will save you time later, if you do not run this command adding fits may take some time if they contain new types.
+
+```bash
+$ python manage.py fittings_preload_data
+```
 
 ## Updating
 To update your existing installation of Fittings first enable your virtual environment.
 
 Then run the following commands from your allianceauth project directory (the one that contains `manage.py`).
 
 ```bash
```

### Comparing `fittings-1.1.0/LICENSE` & `fittings-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/auth_hooks.py` & `fittings-2.0.0/fittings/auth_hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,13 +22,14 @@
     return FittingMenu()
 
 
 @hooks.register('url_hook')
 def register_url():
     return UrlHook(urls, 'fittings', '^fittings/')
 
+
 @hooks.register('discord_cogs_hook')
 def register_cogs():
     if FITTINGS_AADISCORDBOT_INTEGRATION is True:
         return ["fittings.cogs.fittings"]
     else:
         return [""]
```

### Comparing `fittings-1.1.0/fittings/cogs/fittings.py` & `fittings-2.0.0/fittings/cogs/fittings.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/tasks.py` & `fittings-2.0.0/fittings/tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 from allianceauth.services.hooks import get_extension_logger
 from celery import shared_task
+from eveuniverse.models import EveType, EveEntity
 
-from .models import Fitting, FittingItem, ServerVersion, Type, DogmaEffect, DogmaAttribute
+from .models import Fitting, FittingItem
 from .providers import esi
 
 logger = get_extension_logger(__name__)
 
 
 class EftParser:
     def __init__(self, eft_text):
@@ -118,15 +119,15 @@
                 types.append(_get_type(line.split(',')[0].strip()))
             else:
                 quantity = line.split()[-1]
                 if 'x' in quantity and quantity[1:].isdigit():
                     types.append(_get_type(line.split(quantity)[0].strip()))
                 else:
                     types.append(_get_type(line.strip()))
-        return all(_type is not None and _type.group.category_id == 18 for _type in types)
+        return all(_type is not None and _type.eve_group.eve_category.id == 18 for _type in types)
 
     def isFighterBay(self):
         types = []
         for line in self.lines:
             if line.startswith('['):
                 return False
             if ',' in line:
@@ -138,17 +139,21 @@
                 else:
                     types.append(_get_type(line.strip()))
         return all(_type is not None and _type.group.category_id == 87 for _type in types)
 
 
 def _get_type(type_name):
     try:
-        type_obj = Type.objects.get(type_name=type_name)
+        type_obj = EveType.objects.get(name=type_name)
     except:
-        type_obj = Type.objects.create_type(type_name)
+        # If the type is not already in the db, then we have to resolve type_id before we have eveuniverse
+        # create the object.
+        c = esi.client
+        type_id = c.Universe.post_universe_ids(names=[type_name]).result()['inventory_types'][0]["id"]
+        type_obj = EveType.objects.get_or_create_esi(id=type_id,enabled_sections=[EveType.Section.DOGMAS])
     return type_obj
 
 
 @shared_task()
 def create_fitting_item(fit, item):
     count = None
     quantity = None
@@ -205,26 +210,23 @@
     type_names = [x['name'] for x in parsed_eft['modules']]
     type_names += [x['name'] for x in parsed_eft['cargo']]
     type_names += [x['name'] for x in parsed_eft['drone_bay']]
     type_names += [x['name'] for x in parsed_eft['fighter_bay']]
     type_names = list(set(type_names))
 
     # Get a list of types missing from the db
-    types = Type.objects.filter(type_name__in=type_names).values_list('type_name', flat=True)
+    types = EveType.objects.filter(name__in=type_names).values_list('name', flat=True)
 
     missing = [x for x in type_names if x not in types]
 
     # Create missing types
-    _processes = []
-    with ThreadPoolExecutor(max_workers=50) as ex:  # Number of workers might need to be tweaked over time.
-        for name in missing:
-            _processes.append(ex.submit(Type.objects.create_type, name))
-
-    for item in as_completed(_processes):
-        _ = item.result()
+    ids = EveEntity.objects.fetch_by_names_esi(missing)\
+        .filter(category=EveEntity.CATEGORY_INVENTORY_TYPE)\
+        .values_list("id", flat=True)
+    _ = EveType.objects.bulk_get_or_create_esi(ids=ids)
 
     # Create the fitting items
     for module in parsed_eft['modules']:
         create_fitting_item(fit, module)
 
     for item in parsed_eft['cargo']:
         create_fitting_item(fit, item)
@@ -253,61 +255,7 @@
 
     fit.name = parsed_eft['name']
     fit.description = description
     fit.save()
 
     logger.info("Done updating fit " + fit_id)
 
-
-@shared_task
-def missing_group_type_fix():
-    logger.info("Started updating groups for preexisting types.")
-    type_used = FittingItem.objects.order_by('type_id').values_list('type_id', flat=True).distinct()
-    ship_type_used = Fitting.objects.order_by('ship_type_type_id').values_list('ship_type_type_id', flat=True).distinct()
-    joined_type = list(type_used) + list(ship_type_used)
-    da = DogmaAttribute.objects.exclude(type_id__in=joined_type).delete()
-    de = DogmaEffect.objects.exclude(type_id__in=joined_type).delete()
-    Type.objects.exclude(type_id__in=joined_type).delete()
-    # Grab all types with a null group field.
-    types = Type.objects.filter(group=None)
-
-    _processes = []
-    with ThreadPoolExecutor(max_workers=50) as ex:
-        for _type in types:
-            _processes.append(ex.submit(Type.objects.create_type_from_id, _type.type_id))
-
-    for item in as_completed(_processes):
-        _ = item.result()
-
-    logger.info("Done updating groups.")
-
-
-@shared_task
-def update_used_types():
-    logger.info("Started updating types for preexisting types used in fittings.")
-    fittingItem = FittingItem.objects.order_by('type_id').values_list('type_id', flat=True).distinct()
-    _processes = []
-    with ThreadPoolExecutor(max_workers=50) as ex:
-        for _fitting_item_type_id in fittingItem:
-            _processes.append(ex.submit(Type.objects.update_type_from_id, _fitting_item_type_id))
-
-    for item in as_completed(_processes):
-        _ = item.result()
-
-    logger.info("Done updating type.")
-
-@shared_task
-def verify_server_version_and_update_types():
-    logger.info("Looking up the current eve online server version")
-    currentServerVersion = ServerVersion.objects.all()    
-    if len(currentServerVersion) > 1:
-        raise Exception("Only one server version should be active")
-
-    c = esi.client
-    response = c.Status.get_status().result()
-    serverVersion = response.get("server_version")
-
-    if serverVersion is not None:
-        if len(currentServerVersion) == 0 or currentServerVersion[0].id != int(serverVersion):
-            ServerVersion.objects.all().delete()
-            ServerVersion.objects.create(id=serverVersion)
-            update_used_types.delay()
```

### Comparing `fittings-1.1.0/fittings/templates/fittings/edit_fit.html` & `fittings-2.0.0/fittings/templates/fittings/edit_fit.html`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                                     <textarea class="form-control" name="description" id="description" maxlength="500" rows="3">{{ fit.description }}</textarea>
                                 </div>
                             </div>
                             <br />
                             <div class="form-group" >
                                 <label for="eft" class="col-sm-2 control-label">{% translate "Fit" %}</label>
                                 <div class="col-sm-10" style="margin-top: 5px; margin-bottom: 5px;">
-                                    <textarea class="form-control" name="eft" id="eft" rows="5">{{ fit.eft }}</textarea>
+                                    <textarea class="form-control" name="eft" id="eft" rows="50">{{ fit.eft }}</textarea>
                                 </div>
                             </div>
                             <br />
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
```

### Comparing `fittings-1.1.0/fittings/templates/fittings/view_fit.html` & `fittings-2.0.0/fittings/templates/fittings/view_fit.html`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         <div class="modal-dialog" role="document">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                     <h4 class="modal-title" id="modalTitle">{{ fit.name }}</h4>
                 </div>
                 <div class="modal-body">
-                    <textarea style="width: 100%; height: 100%" rows="25" onclick="this.select()">{{ fit.eft }}</textarea>
+                    <textarea style="width: 100%; height: 100%" rows="25" onclick="this.select()" readonly>{{ fit.eft }}</textarea>
                 </div>
                 <div class="modal-footer">
                     <button type="button" class="btn btn-default" data-dismiss="modal">{% translate "Close" %}</button>
                 </div>
             </div>
         </div>
     </div>
@@ -66,19 +66,27 @@
                             {% for doctrine in doctrines %}
                             <li> <a href="{% url 'fittings:view_doctrine' doctrine.pk %}">{{ doctrine.name }}</a> </li>
                             {% endfor %}
                         </ul>
                     </dd>
                     {% if fit.created %}
                     <dt>{% translate "Created" %}</dt>
-                    <dd>{{ fit.created|date:'d M Y H:i:s' }}</dd>
+                        {% if LANGUAGE_CODE == 'ko' or LANGUAGE_CODE == 'ja' %}
+                            <dd>{{ fit.created|date:'Y-m-d / H:i:s' }}</dd>
+                        {% else %}
+                            <dd>{{ fit.created|date:'d M Y H:i:s' }}</dd>
+                        {% endif %}
                     {% endif %}
                     {% if fit.last_updated %}
                         <dt>{% translate "Last Updated" %}</dt>
-                        <dd>{{ fit.last_updated|date:'d M Y H:i:s' }}</dd>
+                        {% if LANGUAGE_CODE == 'ko' or LANGUAGE_CODE == 'ja' %}
+                            <dd>{{ fit.last_updated|date:'Y-m-d / H:i:s' }}</dd>
+                        {% else %}
+                            <dd>{{ fit.last_updated|date:'d M Y H:i:s' }}</dd>
+                        {% endif %}
                     {% endif %}
                 </dl>
             </div>
         </div>
     </div>
     <div class="col-md-9">
         <div class="panel panel-default">
@@ -156,15 +164,15 @@
                         </div>
                         <div class="col-sm-12 col-md-12">
                             <div class="panel panel-warning">
                                 <div class="panel-heading text-center">
                                     {% translate "Hull" %}
                                 </div>
                                 <div class="panel-body text-center">
-                                    {{ fit.ship_type.type_name }}
+                                    {{ fit.ship_type.name }}
                                 </div>
                                 <div class="panel-heading text-center">
                                     {% translate "Fitting Notes" %}
                                 </div>
                                 <div class="panel-body">
                                     <div class="well">
                                         <p style="white-space: pre-wrap; white-space: -moz-pre-wrap; white-space: -pre-wrap; white-space: -o-pre-wrap; word-wrap: break-word;">{{ fit.description|break_html_lines|striptags|urlize }}</p>
@@ -177,15 +185,15 @@
                 </div>
             </div>
 
             <div class="panel-heading">
               <h4 class="panel-title">
                 {% translate "Fit" %}
                   <div class="pull-right">
-                    <a href="{% url 'fittings:save_fit' fit.pk %}" class="btn btn-xs btn-success" style="margin-top: -2px;">Save to EVE</a>
+                    <a href="{% url 'fittings:save_fit' fit.pk %}" class="btn btn-xs btn-success" style="margin-top: -2px;">{% translate "Save to EVE" %}</a>
                     <button class='btn btn-xs btn-success' id="buyAllButton" style="margin-top: -2px;" data-clipboard-text="{{fit.ship_type.type_name}}&#10;{% if fitting.LoSlot0 %}{{fitting.LoSlot0.item_name}}&#10;{% endif %}{% if fitting.LoSlot1 %}{{fitting.LoSlot1.item_name}}&#10;{% endif %}{% if fitting.LoSlot2 %}{{fitting.LoSlot2.item_name}}&#10;{% endif %}{% if fitting.LoSlot3 %}{{fitting.LoSlot3.item_name}}&#10;{% endif %}{% if fitting.LoSlot4 %}{{fitting.LoSlot4.item_name}}&#10;{% endif %}{% if fitting.LoSlot5 %}{{fitting.LoSlot5.item_name}}&#10;{% endif %}{% if fitting.LoSlot6 %}{{fitting.LoSlot6.item_name}}&#10;{% endif %}{% if fitting.LoSlot7 %}{{fitting.LoSlot7.item_name}}&#10;{% endif %}{% if fitting.MedSlot0 %}{{fitting.MedSlot0.item_name}}&#10;{% endif %}{% if fitting.MedSlot1 %}{{fitting.MedSlot1.item_name}}&#10;{% endif %}{% if fitting.MedSlot2 %}{{fitting.MedSlot2.item_name}}&#10;{% endif %}{% if fitting.MedSlot3 %}{{fitting.MedSlot3.item_name}}&#10;{% endif %}{% if fitting.MedSlot4 %}{{fitting.MedSlot4.item_name}}&#10;{% endif %}{% if fitting.MedSlot5 %}{{fitting.MedSlot5.item_name}}&#10;{% endif %}{% if fitting.MedSlot6 %}{{fitting.MedSlot6.item_name}}&#10;{% endif %}{% if fitting.MedSlot7 %}{{fitting.MedSlot7.item_name}}&#10;{% endif %}{% if fitting.HiSlot0 %}{{fitting.HiSlot0.item_name}}&#10;{% endif %}{% if fitting.HiSlot1 %}{{fitting.HiSlot1.item_name}}&#10;{% endif %}{% if fitting.HiSlot2 %}{{fitting.HiSlot2.item_name}}&#10;{% endif %}{% if fitting.HiSlot3 %}{{fitting.HiSlot3.item_name}}&#10;{% endif %}{% if fitting.HiSlot4 %}{{fitting.HiSlot4.item_name}}&#10;{% endif %}{% if fitting.HiSlot5 %}{{fitting.HiSlot5.item_name}}&#10;{% endif %}{% if fitting.HiSlot6 %}{{fitting.HiSlot6.item_name}}&#10;{% endif %}{% if fitting.HiSlot7 %}{{fitting.HiSlot7.item_name}}&#10;{% endif %}{% if fitting.RigSlot0 %}{{fitting.RigSlot0.item_name}}&#10;{% endif %}{% if fitting.RigSlot1 %}{{fitting.RigSlot1.item_name}}&#10;{% endif %}{% if fitting.RigSlot2 %}{{fitting.RigSlot2.item_name}}&#10;{% endif %}{% if fitting.SubSystemSlot0 %}{{fitting.SubSystemSlot0.item_name}}&#10;{% endif %}{% if fitting.SubSystemSlot1 %}{{fitting.SubSystemSlot1.item_name}}&#10;{% endif %}{% if fitting.SubSystemSlot2 %}{{fitting.SubSystemSlot2.item_name}}&#10;{% endif %}{% if fitting.SubSystemSlot3 %}{{fitting.SubSystemSlot3.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot0 %}{{fitting.ServiceSlot0.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot1 %}{{fitting.ServiceSlot1.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot2 %}{{fitting.ServiceSlot2.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot3 %}{{fitting.ServiceSlot3.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot4 %}{{fitting.ServiceSlot4.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot5 %}{{fitting.ServiceSlot5.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot6 %}{{fitting.ServiceSlot6.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot7 %}{{fitting.ServiceSlot7.item_name}}&#10;{% endif %}{% if fitting.FighterTube0 %}{{fitting.FighterTube0.item_name}}&#10;{% endif %}{% if fitting.FighterTube1 %}{{fitting.FighterTube1.item_name}}&#10;{% endif %}{% if fitting.FighterTube2 %}{{fitting.FighterTube2.item_name}}&#10;{% endif %}{% if fitting.FighterTube3 %}{{fitting.FighterTube3.item_name}}&#10;{% endif %}{% if fitting.FighterTube4 %}{{fitting.FighterTube4.item_name}}&#10;{% endif %}{% for ammo in fitting.Cargo %}{{ammo.item_name}} x{{ammo.quantity}}&#10;{% endfor %}{% for fighter in fitting.FighterBay %}{{fighter.item_name}} x{{fighter.quantity}}&#10;{% endfor %}{% for drone in fitting.DroneBay %}{{drone.item_name}} x{{drone.quantity}}&#10;{% endfor %}">
                         {% translate "Copy Buy All" %}
                     </button>
 
                      <span data-toggle="modal" data-target="#eftModal">
                         <button class='btn btn-xs btn-success' id="copyEftButton" style="margin-top: -2px;" data-toggle="tooltip" data-placement="top" title="{% translate 'Copy Fit (EFT)' %}">{% translate "Copy Fit (EFT)" %}</button>
                     </span>
@@ -193,15 +201,15 @@
               </h4>
             </div>
 
             <div id="fitting">
               <div class="panel-body">
                 <ul class="list-group">
                     <li class="list-group-item list-group-item-warning">{% translate "Hull" %}</li>
-                    <li class="list-group-item"><img src="{{ fit.ship_type_type_id|type_render_url:32 }}" title="{{ fit.ship_type.type_name }}"> {{ fit.ship_type.type_name }}</li>
+                    <li class="list-group-item"><img src="{{ fit.ship_type_type_id|type_render_url:32 }}" title="{{ fit.ship_type.type_name }}"> {{ fit.ship_type.name }}</li>
                     {% if fitting.SubSystemSlot0 %}
                         <li class="list-group-item list-group-item-warning">{% translate "SubSystems" %}</li>
                         <li class="list-group-item"><img src="{{ fitting.SubSystemSlot0.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot0.item_name }}"> {{fitting.SubSystemSlot0.item_name}}</li>
                         <li class="list-group-item"><img src="{{ fitting.SubSystemSlot1.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot1.item_name }}"> {{fitting.SubSystemSlot1.item_name}}</li>
                         <li class="list-group-item"><img src="{{ fitting.SubSystemSlot2.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot2.item_name }}"> {{fitting.SubSystemSlot2.item_name}}</li>
                         <li class="list-group-item"><img src="{{ fitting.SubSystemSlot3.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot3.item_name }}"> {{fitting.SubSystemSlot3.item_name}}</li>
                     {% endif %}
```

#### html2text {}

```diff
@@ -79,22 +79,22 @@
 {% if fitting.SubSystemSlot3 %}[{
 { fitting.SubSystemSlot3.type_id|type_icon_url:32 }}]{% endif %}
 {% endif %}
 [{{ fit.ship_type_type_id|type_render_url:256 }}]
 **** {{fit.name}} ****
 {% for cat in cats %} {{cat.name}} {% endfor %}
 {% translate "Hull" %}
-{{ fit.ship_type.type_name }}
+{{ fit.ship_type.name }}
 {% translate "Fitting Notes" %}
 {{ fit.description|break_html_lines|striptags|urlize }}
 {% translate "Fit" %}
-Save_to_EVE  {% translate "Copy Buy All" %}   {% translate "Copy Fit (EFT)" %}
+{%_translate_"Save_to_EVE"_%}  {% translate "Copy Buy All" %}   {% translate
+"Copy Fit (EFT)" %}
     * {% translate "Hull" %}
-    * [{{ fit.ship_type_type_id|type_render_url:32 }}] {
-      { fit.ship_type.type_name }}
+    * [{{ fit.ship_type_type_id|type_render_url:32 }}] {{ fit.ship_type.name }}
     * {% if fitting.SubSystemSlot0 %}
     * {% translate "SubSystems" %}
     * [{{ fitting.SubSystemSlot0.type_id|type_icon_url:32 }}] {
       {fitting.SubSystemSlot0.item_name}}
     * [{{ fitting.SubSystemSlot1.type_id|type_icon_url:32 }}] {
       {fitting.SubSystemSlot1.item_name}}
     * [{{ fitting.SubSystemSlot2.type_id|type_icon_url:32 }}] {
```

### Comparing `fittings-1.1.0/fittings/templates/fittings/view_all_categories.html` & `fittings-2.0.0/fittings/templates/fittings/view_all_categories.html`

 * *Files 2% similar despite different names*

```diff
@@ -77,11 +77,13 @@
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
 {% endblock %}
 
 {% block extra_script %}
     $(document).ready(function(){
-        $('#fitTable').DataTable();
+        $('#fitTable').DataTable({
+            language: { url: '//cdn.datatables.net/plug-ins/1.12.1/i18n/{{ LANGUAGE_CODE }}.json' },
+        });
         $('[data-toggle="tooltip"]').tooltip();
     })
 {% endblock %}
```

### Comparing `fittings-1.1.0/fittings/templates/fittings/dashboard.html` & `fittings-2.0.0/fittings/templates/fittings/dashboard.html`

 * *Files 3% similar despite different names*

```diff
@@ -48,18 +48,18 @@
                                     <td> <a href="{% url 'fittings:view_doctrine' doc.pk %}"><img src="{{ doc.icon_url }}" class="img-circle" style="display: block; margin: auto;"/> </a></td>
                                     <td> <a href="{% url 'fittings:view_doctrine' doc.pk %}">{{ doc.name }}</a> </td>
                                     <td>
                                         {% for cat in doc.category.all %}
                                             <span class="label" style="background-color: {{cat.color}}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span>
                                         {% endfor %}
                                     </td>
-                                    <td> {{ doc.description }} </td>
+                                    <td> {{ doc.description|linebreaks }} </td>
                                     <td>
                                         {% for fitting in doc_dict|get_item:doc.pk %}
-                                            <img src="{{ fitting.ship_type_type_id|type_render_url:32 }}" class="img-circle" data-toggle="tooltip" data-placement="bottom" title="{{ fitting.ship_type.type_name }}"/>
+                                            <img src="{{ fitting.ship_type_type_id|type_render_url:32 }}" class="img-circle" data-toggle="tooltip" data-placement="bottom" title="{{ fitting.ship_type.name }}"/>
                                         {% endfor %}
                                     </td>
                                 </tr>
                             {% endfor %}
                         </tbody>
                     </table>
                 {% endif %}
@@ -71,12 +71,13 @@
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
 {% endblock %}
 
 {% block extra_script %}
     $(document).ready(function(){
         $('#docTable').DataTable({
+            language: { url: '//cdn.datatables.net/plug-ins/1.12.1/i18n/{{ LANGUAGE_CODE }}.json' },
             "order": [[ 1, "asc" ]],
         });
         $('[data-toggle="tooltip"]').tooltip();
     })
 {% endblock %}
```

### Comparing `fittings-1.1.0/fittings/templates/fittings/view_doctrine.html` & `fittings-2.0.0/fittings/templates/fittings/view_doctrine.html`

 * *Files 8% similar despite different names*

```diff
@@ -51,22 +51,30 @@
                         {% for cat in d_cats %}
                             <span class="label" style="background-color: {{cat.color}}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span>
                         {% endfor %}
                 </h5>
                 <hr />
                 <dl>
                     <dt>{% translate "Description" %}</dt>
-                    <dd>{{ doctrine.description|break_html_lines|striptags }}</dd>
+                    <dd><pre>{{ doctrine.description|break_html_lines|striptags }}</pre></dd>
                     {% if doctrine.created %}
                     <dt>{% translate "Created" %}</dt>
-                    <dd>{{ doctrine.created|date:'d M Y H:i:s' }}</dd>
+                        {% if LANGUAGE_CODE == 'ko' or LANGUAGE_CODE == 'ja' %}
+                            <dd>{{ doctrine.created|date:'Y-m-d / H:i:s' }}</dd>
+                        {% else %}
+                            <dd>{{ doctrine.created|date:'d M Y H:i:s' }}</dd>
+                        {% endif %}
                     {% endif %}
                     {% if doctrine.last_updated %}
                         <dt>{% translate "Last Updated" %}</dt>
-                        <dd>{{ doctrine.last_updated|date:'d M Y H:i:s' }}</dd>
+                        {% if LANGUAGE_CODE == 'ko' or LANGUAGE_CODE == 'ja' %}
+                            <dd>{{ doctrine.last_updated|date:'Y-m-d / H:i:s' }}</dd>
+                        {% else %}
+                            <dd>{{ doctrine.last_updated|date:'d M Y H:i:s' }}</dd>
+                        {% endif %}
                     {% endif %}
                 </dl>
             </div>
         </div>
     </div>
     <div class="col-md-9">
         <div class="panel panel-default">
@@ -105,11 +113,16 @@
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
 {% endblock %}
 
 {% block extra_script %}
      $(document).ready(function(){
-        $('#fitsTable').DataTable();
+        $('#fitsTable').DataTable({
+            language: { url: '//cdn.datatables.net/plug-ins/1.12.1/i18n/{{ LANGUAGE_CODE }}.json' },
+            paging: false,
+            searching: false,
+            order: [[1, 'asc']],
+        });
         $('[data-toggle="tooltip"]').tooltip();
     })
 {% endblock %}
```

### Comparing `fittings-1.1.0/fittings/templates/fittings/view_all_fits.html` & `fittings-2.0.0/fittings/templates/fittings/view_all_fits.html`

 * *Files 2% similar despite different names*

```diff
@@ -66,11 +66,13 @@
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
 {% endblock %}
 
 {% block extra_script %}
     $(document).ready(function(){
-        $('#fitTable').DataTable();
+        $('#fitTable').DataTable({
+            language: { url: '//cdn.datatables.net/plug-ins/1.12.1/i18n/{{ LANGUAGE_CODE }}.json' },
+        });
         $('[data-toggle="tooltip"]').tooltip();
     })
 {% endblock %}
```

### Comparing `fittings-1.1.0/fittings/templates/fittings/edit_category.html` & `fittings-2.0.0/fittings/templates/fittings/edit_category.html`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/templates/fittings/add_doctrine.html` & `fittings-2.0.0/fittings/templates/fittings/add_doctrine.html`

 * *Files 8% similar despite different names*

```diff
@@ -55,25 +55,25 @@
                                 </div>
                             </div>
                             <div class="form-group">
                                 <label for="fitSelect" class="col-sm-2 control-label">{% translate "Select Fits" %}</label>
                                 <div class="col-sm-10" style="margin-top: 5px; margin-bottom: 5px;">
                                     <select multiple="multiple" id="fitSelect" name="fitSelect">
                                         {% for fit in fittings %}
-                                            <option value="{{ fit.pk }}">{{ fit.name }} ({{fit.ship_type.type_name}})</option>
+                                            <option value="{{ fit.pk }}">{{ fit.name }} ({{fit.ship_type.name}})</option>
                                         {% endfor %}
                                     </select>
                                 </div>
                             </div>
                             <div class="form-group">
                                 <label for="iconSelect" class="col-sm-2 control-label">{% translate "Select Doctrine Icon" %}</label>
                                 <div class="col-sm-10">
                                     <select class="form-control" name="iconSelect" id="iconSelect" aria-describedby="helpBlock">
                                         {% for ship in ships %}
-                                            <option value="{{ ship.ship_type|type_render_url:64 }}">{{ship.ship_type__type_name}}</option>
+                                            <option value="{{ ship.ship_type|type_render_url:64 }}">{{ship.ship_type__name}}</option>
                                         {% endfor %}
                                     </select>
                                     <span id="helpBlock" class="help-block"> {% translate "If you do not see the ship type that you would like to use for the icon, add a fit that uses that ship type and try again." %}</span>
                                 </div>
                             </div>
                             <br />
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
@@ -88,16 +88,16 @@
 {% block extra_javascript %}
     <script src="https://cdnjs.cloudflare.com/ajax/libs/multi-select/0.9.12/js/jquery.multi-select.js" integrity="sha256-JU2QMhOvXGZtWxxkQTEgpVjdPHMYMuVYbYzNqfsioNw=" crossorigin="anonymous"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery.quicksearch/2.4.0/jquery.quicksearch.min.js" integrity="sha256-hD1kpQcVntR40eMx9uED+E4HAjD2OJkLIFcP6ukVd+g=" crossorigin="anonymous"></script>
 {% endblock %}
 
 {% block extra_script %}
     $('#fitSelect').multiSelect({
-          selectableHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='Search' style='margin-bottom: 3px;'>",
-          selectionHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='Search' style='margin-bottom: 3px;'>",
+          selectableHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='{% translate "Search" %}' style='margin-bottom: 3px;'>",
+          selectionHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='{% translate "Search" %}' style='margin-bottom: 3px;'>",
           afterInit: function(ms){
             var that = this,
                 $selectableSearch = that.$selectableUl.prev(),
                 $selectionSearch = that.$selectionUl.prev(),
                 selectableSearchString = '#'+that.$container.attr('id')+' .ms-elem-selectable:not(.ms-selected)',
                 selectionSearchString = '#'+that.$container.attr('id')+' .ms-elem-selection.ms-selected';
```

#### html2text {}

```diff
@@ -11,19 +11,19 @@
 {% translate "New Doctrine" %}
 {% csrf_token %}
 {% translate "Doctrine Name" %}
 [name                ]
 {% translate "Doctrine Description" %}
 {% translate "Select Fits" %}
 {% for fit in fittings %}
-{{ fit.name }} ({{fit.ship_type.type_name}})
+{{ fit.name }} ({{fit.ship_type.name}})
 {% endfor %}
 {% translate "Select Doctrine Icon" %}
 {% for ship in ships %}
-{{ship.ship_type__type_name}}
+{{ship.ship_type__name}}
 {% endfor %}
   {% translate "If you do not see the ship type that you would like to use for
 the icon, add a fit that uses that ship type and try again." %}
 
 {% translate "Submit" %}
 {% endblock %} {% block extra_javascript %}
  {% endblock %} {% block extra_script %} $('#fitSelect').multiSelect(
```

### Comparing `fittings-1.1.0/fittings/templates/fittings/base.html` & `fittings-2.0.0/fittings/templates/fittings/base.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% extends 'allianceauth/base.html' %}
 {% load i18n %}
+{% load navactive %}
 {% block extra_css %}
     <style>
         .flex-container {
             display: flex;
             flex-direction: row;
             height: 100%;
             align-items: center;
@@ -29,37 +30,40 @@
 {% block content %}
     <div class="col-lg-12">
         <br />
         <div class="col-lg-12 container">
             <nav class="navbar navbar-default">
                 <div class="container-fluid">
                     <div class="navbar-header">
-                        <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
+                        <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target=".fittings-menus-collapse" aria-expanded="false">
                             <span class="sr-only">{% translate "Toggle navigation" %}</span>
                             <span class="icon-bar"></span>
                             <span class="icon-bar"></span>
                             <span class="icon-bar"></span>
                         </button>
                         <a class="navbar-brand" href="{% url 'fittings:dashboard' %}">{% translate "Fittings and Doctrines" %}</a>
                     </div>
-                    <ul class="nav navbar-nav navbar-left">
-                            <li> <a href="{% url 'fittings:view_all_fits' %}">{% translate "View All Fits" %}</a></li>
-                            <li><a href="{% url 'fittings:view_all_categories' %}">{% translate "View All Categories" %}</a></li>
+                    <div class="collapse navbar-collapse fittings-menus-collapse">
+                    <ul class="nav navbar-nav">
+                            <li class="{% navactive request 'fittings:dashboard fittings:add_doctrine fittings:view_doctrine fittings:delete_doctrine fittings:edit_doctrine' %}"><a href="{% url 'fittings:dashboard' %}">{% translate "View All Doctrines" %}</a></li>
+                            <li class="{% navactive request 'fittings:add_fit fittings:view_all_fits fittings:view_fit fittings:delete_fit fittings:save_fit fittings:edit_fit' %}"><a href="{% url 'fittings:view_all_fits' %}">{% translate "View All Fits" %}</a></li>
+                            <li class="{% navactive request 'fittings:view_all_categories fittings:add_category fittings:view_category fittings:edit_category fittings:delete_category' %}"><a href="{% url 'fittings:view_all_categories' %}">{% translate "View All Categories" %}</a></li>
                     </ul>
                     {% if perms.fittings.manage %}
                         <div class="dropdown pull-right" style="margin-top: .8em;">
                             <button class="btn btn-success btn-sm dropdown-toggle" type="button" id="manageDrop" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                 <span class="fa fa-plus"></span>
                             </button>
                             <ul class="dropdown-menu" aria-labelledby="manageDrop">
                                 <li> <a href="{% url 'fittings:add_fit' %}">{% translate "Fitting" %}</a></li>
                                 <li> <a href="{% url 'fittings:add_doctrine' %}">{% translate "Doctrine" %}</a></li>
                                 <li> <a href="{% url 'fittings:add_category' %}">{% translate "Category" %}</a></li>
                             </ul>
                         </div>
                     {% endif %}
+                    </div>
                 </div>
             </nav>
             {% block fittings_block %}{% endblock %}
         </div>
     </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-{% extends 'allianceauth/base.html' %} {% load i18n %} {% block extra_css %}
+{% extends 'allianceauth/base.html' %} {% load i18n %} {% load navactive %} {%
+block extra_css %}
  {% include 'bundles/datatables-css.html' %} {% block more_css %}{%endblock%}
 {% endblock extra_css %} {% block content %}
 
  {% translate "Toggle navigation" %}     {%_translate_"Fittings_and_Doctrines"
 %}
+    * {%_translate_"View_All_Doctrines"_%}
     * {%_translate_"View_All_Fits"_%}
     * {%_translate_"View_All_Categories"_%}
 {% if perms.fittings.manage %}
 
     * {%_translate_"Fitting"_%}
     * {%_translate_"Doctrine"_%}
     * {%_translate_"Category"_%}
```

### Comparing `fittings-1.1.0/fittings/templates/fittings/view_category.html` & `fittings-2.0.0/fittings/templates/fittings/view_category.html`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/templates/fittings/add_fit.html` & `fittings-2.0.0/fittings/templates/fittings/add_fit.html`

 * *Files 3% similar despite different names*

```diff
@@ -28,17 +28,17 @@
                                 <label for="description" class="col-sm-2 control-label">{% translate "Description" %}</label>
                                 <div class="col-sm-10">
                                     <textarea class="form-control" name="description" id="description" maxlength="500" rows="3"></textarea>
                                 </div>
                             </div>
                             <br />
                             <div class="form-group" >
-                                <label for="eft" class="col-sm-2 control-label">Fit</label>
+                                <label for="eft" class="col-sm-2 control-label">{% translate "Fit" %}</label>
                                 <div class="col-sm-10" style="margin-top: 5px; margin-bottom: 5px;">
-                                    <textarea class="form-control" name="eft" id="eft" rows="5"></textarea>
+                                    <textarea class="form-control" name="eft" id="eft" rows="50"></textarea>
                                 </div>
                             </div>
                             <br />
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
```

### Comparing `fittings-1.1.0/fittings/templates/fittings/edit_doctrine.html` & `fittings-2.0.0/fittings/templates/fittings/edit_doctrine.html`

 * *Files 4% similar despite different names*

```diff
@@ -53,29 +53,29 @@
                                 </div>
                             </div>
                             <div class="form-group">
                                 <label for="fitSelect" class="col-sm-2 control-label">{% translate "Select Fits" %}</label>
                                 <div class="col-sm-10" style="margin-top: 5px; margin-bottom: 5px;">
                                     <select multiple="multiple" id="fitSelect" name="fitSelect">
                                         {% for fit in doc_fits %}
-                                            <option value="{{ fit.pk }}" selected>{{ fit.name }} ({{ fit.ship_type.type_name }})</option>
+                                            <option value="{{ fit.pk }}" selected>{{ fit.name }} ({{ fit.ship_type.name }})</option>
                                         {% endfor %}
                                         {% for fit in fits %}
                                             <option value="{{ fit.pk }}">{{ fit.name }} ({{fit.ship_type.type_name}})</option>
                                         {% endfor %}
                                     </select>
                                 </div>
                             </div>
                             <div class="form-group">
                                 <label for="iconSelect" class="col-sm-2 control-label">{% translate "Select Doctrine Icon" %}</label>
                                 <div class="col-sm-10">
                                     <select class="form-control" name="iconSelect" id="iconSelect" aria-describedby="helpBlock">
                                         <option value="{{ doctrine.icon_url }}" selected> {% translate "Current Icon" %} </option>
                                         {% for ship in ships %}
-                                            <option value="{{ ship.ship_type|type_render_url:64 }}">{{ship.ship_type__type_name}}</option>
+                                            <option value="{{ ship.ship_type|type_render_url:64 }}">{{ship.ship_type__name}}</option>
                                         {% endfor %}
                                     </select>
                                     <span id="helpBlock" class="help-block"> {% translate "If you do not see the ship type that you would like to use for the icon, add a fit that uses that ship type and try again." %}</span>
                                 </div>
                             </div>
                             <br />
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
```

#### html2text {}

```diff
@@ -12,21 +12,21 @@
 {% csrf_token %}
 {% translate "Doctrine Name" %}
 [{{ doctrine.name }} ]
 {% translate "Doctrine Description" %}
 {{ doctrine.description }}
 {% translate "Select Fits" %}
 {% for fit in doc_fits %}
-{{ fit.name }} ({{ fit.ship_type.type_name }})
+{{ fit.name }} ({{ fit.ship_type.name }})
 {% endfor %} {% for fit in fits %}
 {{ fit.name }} ({{fit.ship_type.type_name}})
 {% endfor %}
 {% translate "Select Doctrine Icon" %}
 {% for ship in ships %}
-{{ship.ship_type__type_name}}
+{{ship.ship_type__name}}
 {% endfor %}
   {% translate "If you do not see the ship type that you would like to use for
 the icon, add a fit that uses that ship type and try again." %}
 
 {% translate "Submit" %}
 {% endblock %} {% block extra_javascript %}
  {% endblock %} {% block extra_script %} $('#fitSelect').multiSelect(
```

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/7m.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/7m.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/4m.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/4m.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/0l.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/0l.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/5l.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/5l.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/tyrannis.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/h.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/h.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/6m.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/6m.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/5s.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/5s.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/r.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/r.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/3h.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/3h.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/2h.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/2h.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/circle.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/circle.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/l.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/l.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/3r.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/3r.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/m.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/m.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/2m.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/2m.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/0r.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/0r.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/3m.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/3m.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/0m.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/0m.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/0s.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/0s.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/5h.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/5h.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/4l.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/4l.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/dustwheel.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/dustwheel.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/8l.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/8l.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/0h.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/0h.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/4s.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/4s.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/5m.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/5m.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/tyrannis_default.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_default.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/tyrannis_blue.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_blue.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/working.jpg` & `fittings-2.0.0/fittings/static/fittings/img/pannel/working.jpg`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/7l.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/7l.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/1r.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/1r.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/noship.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/noship.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/1l.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/1l.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/4h.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/4h.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/7h.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/7h.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/3l.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/3l.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/6h.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/6h.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/1h.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/1h.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/1m.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/1m.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/tyrannis_revelations.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_revelations.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/2l.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/2l.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/2r.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/2r.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/6l.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/6l.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/error.jpg` & `fittings-2.0.0/fittings/static/fittings/img/pannel/error.jpg`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/tyrannis_darkred.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/tyrannis_darkred.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/8m.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/8m.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/static/fittings/img/pannel/8h.png` & `fittings-2.0.0/fittings/static/fittings/img/pannel/8h.png`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/models.py` & `fittings-2.0.0/fittings/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,127 +1,33 @@
 from django.contrib.auth.models import Group
 from django.db import models
 from django.db.models import Subquery, OuterRef
 from model_utils import Choices
 
-from .managers import TypeManager, DogmaAttributeManager, DogmaEffectManager, ItemCategoryManager, ItemGroupManager
-
-
-# Category Model
-class ItemCategory(models.Model):
-    category_id = models.IntegerField(primary_key=True)
-    name = models.CharField(max_length=250)
-    published = models.BooleanField(default=True)
-
-    objects = ItemCategoryManager()
-
-    class Meta:
-        default_permissions = ()
-
-
-# Group Model
-class ItemGroup(models.Model):
-    group_id = models.IntegerField(primary_key=True)
-    name = models.CharField(max_length=250)
-    category = models.ForeignKey(ItemCategory, on_delete=models.CASCADE)
-    published = models.BooleanField(default=True)
-
-    objects = ItemGroupManager()
-
-    class Meta:
-        default_permissions = ()
-
-
-# Type Model
-class Type(models.Model):
-    type_name = models.CharField(max_length=500)
-    type_id = models.BigIntegerField(primary_key=True)
-    # group_id = models.IntegerField()    # This is essentially a FK field.
-    group = models.ForeignKey(ItemGroup, on_delete=models.CASCADE, null=True)
-    published = models.BooleanField(default=False)
-    mass = models.FloatField(null=True)
-    capacity = models.FloatField(null=True)
-    description = models.CharField(max_length=5000, null=True)  # Not sure of the actual max.
-    volume = models.FloatField(null=True)
-    packaged_volume = models.FloatField(null=True)
-    portion_size = models.IntegerField(null=True)
-    radius = models.FloatField(null=True)
-    graphic_id = models.IntegerField(null=True)
-    icon_id = models.IntegerField(null=True)
-    market_group_id = models.IntegerField(null=True)
-
-    objects = TypeManager()
-
-    class Meta:
-        default_permissions = ()
-
-
-class TypeHistory(models.Model):
-    type_id = models.BigIntegerField()
-    type_name = models.CharField(max_length=500)
-
-    class Meta:
-        default_permissions = ()
-
-
-# Dogma Attribute
-class DogmaAttribute(models.Model):
-    # 12 - Low Slots | 13 - Med Slots | 14 - High Slots
-    # 1137 - Rig Slots | 1367 - Sub System Slots | 2056 - Service Slots
-    # 182 | 183 | 184 --- Req Skill 1/2/3
-    # 277 - Req. Skill 1 Lvl | 278 | 279 -- Req Skill 1/2 Lvl
-    # 1374 - HiSlotModifier | 1375 - MedSlotModifier | 1376 - RigSlotModifier
-    type = models.ForeignKey(Type, on_delete=models.DO_NOTHING, related_name='dogma_attributes')
-    attribute_id = models.IntegerField()
-    value = models.FloatField()
-
-    objects = DogmaAttributeManager()
-
-    class Meta:
-        default_permissions = ()
-        constraints = [
-            models.UniqueConstraint(fields=('attribute_id', 'type'), name='unique_type_and_attribute_id')
-        ]
-
-
-# Dogma Effect
-class DogmaEffect(models.Model):
-    # 11 - Low Power | 12 - High Power | 13 - Med Power
-    # 2663 - Rig Slot | 3772 - Subsystem | 6306 - Service Slot
-    type = models.ForeignKey(Type, on_delete=models.DO_NOTHING, related_name='dogma_effects')
-    effect_id = models.IntegerField()
-    is_default = models.BooleanField()
-
-    objects = DogmaEffectManager()
-
-    class Meta:
-        default_permissions = ()
-        constraints = [
-            models.UniqueConstraint(fields=('effect_id', 'type'), name='unique_type_and_effect_id')
-        ]
+from eveuniverse.models import EveType
 
 
 # Fitting
 class Fitting(models.Model):
     description = models.TextField(max_length=500)
     name = models.CharField(max_length=255, null=False)
-    ship_type = models.ForeignKey(Type, on_delete=models.DO_NOTHING)
+    ship_type = models.ForeignKey(EveType, to_field="id", on_delete=models.DO_NOTHING)
     ship_type_type_id = models.IntegerField()
     created = models.DateTimeField(auto_now_add=True, blank=True, null=True)
     last_updated = models.DateTimeField(auto_now=True, blank=True, null=True)
 
     def __str__(self):
-        return "{} ({})".format(self.ship_type.type_name, self.name)
+        return "{} ({})".format(self.ship_type.name, self.name)
 
     @property
     def eft(self):
-        types = Type.objects.filter(type_id=OuterRef('type_id'))
-        items = FittingItem.objects.filter(fit=self).annotate(item_name=Subquery(types.values('type_name')))
+        types = EveType.objects.filter(id=OuterRef('type_id'))
+        items = FittingItem.objects.filter(fit=self).annotate(item_name=Subquery(types.values('name')))
 
-        eft = '[' + self.ship_type.type_name + ', ' + self.name + ']\n\n'
+        eft = '[' + self.ship_type.name + ', ' + self.name + ']\n\n'
 
         temp = {'Cargo': [], 'FighterBay': [], 'DroneBay': []}
         
         slots = [
             {'key': 'LoSlot', 'range': 8},
             {'key': 'MedSlot', 'range': 8},
             {'key': 'HiSlot', 'range': 8},
@@ -172,28 +78,42 @@
         unique_together = (
             ('ship_type_type_id', 'name'),
         )
 
 
 # Fitting items
 class FittingItem(models.Model):
+    # Dogma Attribute Notes
+    # =====================
+    # 12 - Low Slots | 13 - Med Slots | 14 - High Slots
+    # 1137 - Rig Slots | 1367 - Sub System Slots | 2056 - Service Slots
+    # 182 | 183 | 184 --- Req Skill 1/2/3
+    # 277 - Req. Skill 1 Lvl | 278 | 279 -- Req Skill 1/2 Lvl
+    # 1374 - HiSlotModifier | 1375 - MedSlotModifier | 1376 - RigSlotModifier
+    # Dogma Effect Notes
+    # =====================
+    # 11 - Low Power | 12 - High Power | 13 - Med Power
+    # 2663 - Rig Slot | 3772 - Subsystem | 6306 - Service Slot
     fit = models.ForeignKey(Fitting, on_delete=models.CASCADE, related_name='items')
     _flag_enum = Choices('Cargo', 'DroneBay', 'FighterBay', 'HiSlot0', 'HiSlot1', 'HiSlot2',
                          'HiSlot3', 'HiSlot4', 'HiSlot5', 'HiSlot6', 'HiSlot7', 'Invalid',
                          'LoSlot0', 'LoSlot1', 'LoSlot2', 'LoSlot3', 'LoSlot4', 'LoSlot5',
                          'LoSlot6', 'LoSlot7', 'MedSlot0', 'MedSlot1', 'MedSlot2', 'MedSlot3',
                          'MedSlot4', 'MedSlot5', 'MedSlot6', 'MedSlot7', 'RigSlot0', 'RigSlot1',
                          'RigSlot2', 'ServiceSlot0', 'ServiceSlot1', 'ServiceSlot2', 'ServiceSlot3',
                          'ServiceSlot4', 'ServiceSlot5', 'ServiceSlot6', 'ServiceSlot7', 'SubSystemSlot0',
                          'SubSystemSlot1', 'SubSystemSlot2', 'SubSystemSlot3')
     flag = models.CharField(max_length=25, choices=_flag_enum, default='Invalid')
     quantity = models.IntegerField(default=1)
-    type_fk = models.ForeignKey(Type, on_delete=models.DO_NOTHING)
+    type_fk = models.ForeignKey(EveType, to_field="id", on_delete=models.DO_NOTHING)
     type_id = models.IntegerField()
 
+    def __str__(self):
+        return f'{self.type_fk.name} - {self.flag} ({self.fit.name})'
+
     class Meta:
         default_permissions = (())
 
 
 # Doctrine
 class Doctrine(models.Model):
     name = models.CharField(max_length=255, null=False)
@@ -232,20 +152,8 @@
 
     def __str__(self):
         return f"Category: {self.name}"
 
     class Meta:
         verbose_name = "Category"
         verbose_name_plural = "Categories"
-        default_permissions = (())
-
-
-# Unified Category
-class ServerVersion(models.Model):
-    id = models.BigIntegerField(primary_key=True)
-
-    def __str__(self):
-        return f"Server Version: {self.id}"
-
-    class Meta:
-        verbose_name = "ServerVersion"
-        default_permissions = (())
+        default_permissions = (())
```

### Comparing `fittings-1.1.0/fittings/admin.py` & `fittings-2.0.0/fittings/admin.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/views.py` & `fittings-2.0.0/fittings/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from django.contrib import messages
 from django.contrib.auth.models import Group
 from django.contrib.auth.decorators import login_required, permission_required
 from django.utils.translation import gettext as gt
 from django.db.models import Subquery, OuterRef, Count, Q, Prefetch, F
 from django.shortcuts import render, redirect
 from esi.decorators import token_required
+from eveuniverse.models import EveType
 from itertools import chain
 
-from .models import Doctrine, Fitting, Type, FittingItem, Category
+from .models import Doctrine, Fitting, FittingItem, Category
 from .providers import esi
 from .tasks import create_fit, update_fit
 
 logger = get_extension_logger(__name__)
 
 
 # Helper Function
@@ -130,41 +131,41 @@
     return docs
 
 
 def _build_slots(fit):
     ship = fit.ship_type
     attributes = (12, 13, 14, 1137, 1367, 2056)
 
-    t3c = ship.dogma_attributes.filter(attribute_id=1367).exists()
+    t3c = ship.dogma_attributes.filter(eve_dogma_attribute_id=1367).exists()
 
-    attributes = ship.dogma_attributes.filter(attribute_id__in=attributes)
+    attributes = ship.dogma_attributes.filter(eve_dogma_attribute_id__in=attributes)
 
     slots = {'low': 0, 'med': 0, 'high': 0}
     for attribute in attributes:
-        if attribute.attribute_id == 1367:
+        if attribute.eve_dogma_attribute_id == 1367:
             subAttbs = (1374, 1375, 1376)
             slots['sub'] = 4
             if t3c:
                 for item in FittingItem.objects.filter(fit=fit).exclude(flag='Cargo'):
-                    attbs = item.type_fk.dogma_attributes.filter(attribute_id__in=subAttbs)
+                    attbs = item.type_fk.dogma_attributes.filter(eve_dogma_attribute_id__in=subAttbs)
                     for attb in attbs:
-                        if attb.attribute_id == 1374:
+                        if attb.eve_dogma_attribute_id == 1374:
                             slots['high'] += int(attb.value)
-                        if attb.attribute_id == 1375:
+                        if attb.eve_dogma_attribute_id == 1375:
                             slots['med'] += int(attb.value)
-                        if attb.attribute_id == 1376:
+                        if attb.eve_dogma_attribute_id == 1376:
                             slots['low'] += int(attb.value)
 
-        elif attribute.attribute_id == 12:
+        elif attribute.eve_dogma_attribute_id == 12:
             slots['low'] += int(attribute.value)
-        elif attribute.attribute_id == 13:
+        elif attribute.eve_dogma_attribute_id == 13:
             slots['med'] += int(attribute.value)
-        elif attribute.attribute_id == 14:
+        elif attribute.eve_dogma_attribute_id == 14:
             slots['high'] += int(attribute.value)
-        elif attribute.attribute_id == 1137:
+        elif attribute.eve_dogma_attribute_id == 1137:
             slots['rig'] = int(attribute.value)
 
     return slots
 
 
 def _check_fit_access(request, fit_id: int) -> bool:
     fit = Fitting.objects.prefetch_related('category', 'doctrines', 'doctrines__category').get(pk=int(fit_id))
@@ -280,16 +281,16 @@
     access = _check_fit_access(request, fit_id)
 
     if not access:
         messages.warning(request, gt('You do not have access to that fit.'))
 
         return redirect('fittings:dashboard')
 
-    types = Type.objects.filter(type_id=OuterRef('type_id'))
-    items = FittingItem.objects.filter(fit=fit).annotate(item_name=Subquery(types.values('type_name')))
+    types = EveType.objects.filter(id=OuterRef('type_id'))
+    items = FittingItem.objects.filter(fit=fit).annotate(item_name=Subquery(types.values('name')))
 
     fittings = {'Cargo': [], 'FighterBay': [], 'DroneBay': []}
 
     for item in items:
         if item.flag == "Cargo":
             fittings['Cargo'].append(item)
         elif item.flag == "DroneBay":
@@ -336,15 +337,15 @@
         d = Doctrine(name=name, description=description, icon_url=icon_url)
         d.save()
         for fitting in fits:
             d.fittings.add(fitting)
         return redirect('fittings:dashboard')
 
     fits = Fitting.objects.all()
-    ships = Fitting.objects.order_by('ship_type').values('ship_type', 'ship_type__type_name')\
+    ships = Fitting.objects.order_by('ship_type').values('ship_type', 'ship_type__name')\
         .annotate(a=Count('ship_type'))
     ctx['fittings'] = fits
     ctx['ships'] = ships
     return render(request, 'fittings/add_doctrine.html', context=ctx)
 
 
 @permission_required('fittings.access_fittings')
@@ -448,15 +449,15 @@
         doctrine.icon_url = icon_url
         doctrine.save()
         doctrine.fittings.clear()
         for fit in fitSelect:
             doctrine.fittings.add(fit)
         return redirect('fittings:view_doctrine', doctrine_id)
 
-    ships = Fitting.objects.order_by('ship_type').values('ship_type', 'ship_type__type_name') \
+    ships = Fitting.objects.order_by('ship_type').values('ship_type', 'ship_type__name') \
         .annotate(a=Count('ship_type'))
     ctx['ships'] = ships
     ctx['doctrine'] = doctrine
     ctx['doc_fits'] = doctrine.fittings.all()
     ctx['fits'] = Fitting.objects.exclude(pk__in=ctx['doc_fits']).all()
     return render(request, 'fittings/edit_doctrine.html', context=ctx)
```

### Comparing `fittings-1.1.0/fittings/migrations/0005_unicategory.py` & `fittings-2.0.0/fittings/migrations/0005_unicategory.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py` & `fittings-2.0.0/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/migrations/0014_serverversion.py` & `fittings-2.0.0/fittings/migrations/0014_serverversion.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/migrations/0001_initial.py` & `fittings-2.0.0/fittings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/migrations/0011_auto_20200815_2022.py` & `fittings-2.0.0/fittings/migrations/0011_auto_20200815_2022.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/migrations/0012_typehistory.py` & `fittings-2.0.0/fittings/migrations/0012_typehistory.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/migrations/0007_auto_20200605_0735.py` & `fittings-2.0.0/fittings/migrations/0007_auto_20200605_0735.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/migrations/0004_add_item_category_and_group.py` & `fittings-2.0.0/fittings/migrations/0004_add_item_category_and_group.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/migrations/0009_auto_20200605_2117.py` & `fittings-2.0.0/fittings/migrations/0009_auto_20200605_2117.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/migrations/0002_add_dgm_unique_constraints.py` & `fittings-2.0.0/fittings/migrations/0002_add_dgm_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/locale/zh_Hans/LC_MESSAGES/django.po` & `fittings-2.0.0/fittings/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/locale/ru/LC_MESSAGES/django.mo` & `fittings-2.0.0/fittings/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/locale/ru/LC_MESSAGES/django.po` & `fittings-2.0.0/fittings/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/locale/es/LC_MESSAGES/django.po` & `fittings-2.0.0/fittings/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/locale/fr_FR/LC_MESSAGES/django.po` & `fittings-2.0.0/fittings/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/locale/de/LC_MESSAGES/django.mo` & `fittings-2.0.0/fittings/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/locale/de/LC_MESSAGES/django.po` & `fittings-2.0.0/fittings/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/templatetags/filters.py` & `fittings-2.0.0/fittings/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/fittings/urls.py` & `fittings-2.0.0/fittings/urls.py`

 * *Files identical despite different names*

### Comparing `fittings-1.1.0/setup.py` & `fittings-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 
 from fittings import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 install_requires = [
-    'allianceauth>=2.7.3',
+    'allianceauth>=3.0.0',
     'django-bootstrap-form',
     'django-model_utils>=3.1.1',
-    'django-esi>=2.0.0'
+    'django-esi>=2.0.0',
+    'django-eveuniverse>=0.18.0'
 ]
 
 testing_extras = [
 
 ]
 
 setup(
@@ -24,30 +25,31 @@
     author_email='it-team@serin.space',
     description='A simple fittings and doctrine management application.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=install_requires,
     extras_require={
         'testing': testing_extras,
-        ':python_version=="3.7"': ['typing'],
+        ':python_version=="3.8"': ['typing'],
     },
     python_requires='~=3.6',
     license='GPLv3',
     packages=find_packages(),
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
-        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
         'Intended Audience :: Developers',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
     url='https://gitlab.com/colcrunch/fittings',
     zip_safe=False,
     include_package_data=True,
```

### Comparing `fittings-1.1.0/fittings.egg-info/PKG-INFO` & `fittings-2.0.0/fittings.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: fittings
-Version: 1.1.0
+Version: 2.0.0
 Summary: A simple fittings and doctrine management application.
 Home-page: https://gitlab.com/colcrunch/fittings
 Author: Col Crunch
 Author-email: it-team@serin.space
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
@@ -105,37 +106,37 @@
 $ pip install fittings 
 ```
 
 ### 2. Configure AA settings
 
 Configure your AA settings (`local.py`) as follows:
 
-- Add `'fittings',` to `INSTALLED_APPS`
+- Add `'eveuniverse',` and `'fittings',` to `INSTALLED_APPS`
 - Add these line to the bottom of the settings file to have module name updates
 
-```python
-# Fittings Module
-CELERYBEAT_SCHEDULE['fittings_update_types'] = {
-    'task': 'fittings.tasks.verify_server_version_and_update_types',
-    'schedule': crontab(minute=0, hour='12'),
-}
-```
 ### 3. Finalize Install
 Run migrations and copy static files. 
 
 ```bash
 $ python manage.py migrate
 $ python manage.py collectstatic
 ```
 
 Restart your supervisor tasks.
 
 ### 4. Populate Types
-As of v1.0.0 there is no need to populate types from SDE. This will be done on the fly from
-ESI. 
+Now that fittings has transitioned to using [django-eveuniverse](https://gitlab.com/ErikKalkoken/django-eveuniverse) to handle static data this step is optional.
+
+You can choose to run the following command to preload the type information for most ships and modules in the game, or you can skip this step and let them be created on an as-needed basis.
+
+Keep in mind that running this command will take a while but will save you time later, if you do not run this command adding fits may take some time if they contain new types.
+
+```bash
+$ python manage.py fittings_preload_data
+```
 
 ## Updating
 To update your existing installation of Fittings first enable your virtual environment.
 
 Then run the following commands from your allianceauth project directory (the one that contains `manage.py`).
 
 ```bash
```

### Comparing `fittings-1.1.0/fittings.egg-info/SOURCES.txt` & `fittings-2.0.0/fittings.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 setup.py
 fittings/__init__.py
 fittings/admin.py
 fittings/app_settings.py
 fittings/apps.py
 fittings/auth_hooks.py
 fittings/forms.py
-fittings/managers.py
 fittings/models.py
 fittings/providers.py
 fittings/tasks.py
 fittings/tests.py
 fittings/urls.py
 fittings/views.py
 fittings.egg-info/PKG-INFO
@@ -33,14 +32,15 @@
 fittings/locale/ja/LC_MESSAGES/django.po
 fittings/locale/ko_KR/LC_MESSAGES/django.mo
 fittings/locale/ko_KR/LC_MESSAGES/django.po
 fittings/locale/ru/LC_MESSAGES/django.mo
 fittings/locale/ru/LC_MESSAGES/django.po
 fittings/locale/zh_Hans/LC_MESSAGES/django.mo
 fittings/locale/zh_Hans/LC_MESSAGES/django.po
+fittings/management/commands/fittings_preload_data.py
 fittings/migrations/0001_initial.py
 fittings/migrations/0002_add_dgm_unique_constraints.py
 fittings/migrations/0003_remove_type_description_not_null.py
 fittings/migrations/0004_add_item_category_and_group.py
 fittings/migrations/0005_unicategory.py
 fittings/migrations/0006_auto_20200605_0724.py
 fittings/migrations/0007_auto_20200605_0735.py
@@ -48,14 +48,15 @@
 fittings/migrations/0009_auto_20200605_2117.py
 fittings/migrations/0010_auto_20200718_2227.py
 fittings/migrations/0011_auto_20200815_2022.py
 fittings/migrations/0012_typehistory.py
 fittings/migrations/0013_alter_doctrine_description.py
 fittings/migrations/0014_serverversion.py
 fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py
+fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py
 fittings/migrations/__init__.py
 fittings/static/fittings/img/pannel/0h.png
 fittings/static/fittings/img/pannel/0l.png
 fittings/static/fittings/img/pannel/0m.png
 fittings/static/fittings/img/pannel/0r.png
 fittings/static/fittings/img/pannel/0s.png
 fittings/static/fittings/img/pannel/1h.png
```

### Comparing `fittings-1.1.0/README.md` & `fittings-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -78,37 +78,37 @@
 $ pip install fittings 
 ```
 
 ### 2. Configure AA settings
 
 Configure your AA settings (`local.py`) as follows:
 
-- Add `'fittings',` to `INSTALLED_APPS`
+- Add `'eveuniverse',` and `'fittings',` to `INSTALLED_APPS`
 - Add these line to the bottom of the settings file to have module name updates
 
-```python
-# Fittings Module
-CELERYBEAT_SCHEDULE['fittings_update_types'] = {
-    'task': 'fittings.tasks.verify_server_version_and_update_types',
-    'schedule': crontab(minute=0, hour='12'),
-}
-```
 ### 3. Finalize Install
 Run migrations and copy static files. 
 
 ```bash
 $ python manage.py migrate
 $ python manage.py collectstatic
 ```
 
 Restart your supervisor tasks.
 
 ### 4. Populate Types
-As of v1.0.0 there is no need to populate types from SDE. This will be done on the fly from
-ESI. 
+Now that fittings has transitioned to using [django-eveuniverse](https://gitlab.com/ErikKalkoken/django-eveuniverse) to handle static data this step is optional.
+
+You can choose to run the following command to preload the type information for most ships and modules in the game, or you can skip this step and let them be created on an as-needed basis.
+
+Keep in mind that running this command will take a while but will save you time later, if you do not run this command adding fits may take some time if they contain new types.
+
+```bash
+$ python manage.py fittings_preload_data
+```
 
 ## Updating
 To update your existing installation of Fittings first enable your virtual environment.
 
 Then run the following commands from your allianceauth project directory (the one that contains `manage.py`).
 
 ```bash
```


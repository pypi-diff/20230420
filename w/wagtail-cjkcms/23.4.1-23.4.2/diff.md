# Comparing `tmp/wagtail-cjkcms-23.4.1.tar.gz` & `tmp/wagtail-cjkcms-23.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-cjkcms-23.4.1.tar", last modified: Sun Apr 16 16:31:36 2023, max compression
+gzip compressed data, was "wagtail-cjkcms-23.4.2.tar", last modified: Thu Apr 20 08:09:53 2023, max compression
```

## Comparing `wagtail-cjkcms-23.4.1.tar` & `wagtail-cjkcms-23.4.2.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/
--rw-r--r--   0 grze      (1000) grze      (1000)     6374 2023-04-16 16:25:02.000000 wagtail-cjkcms-23.4.1/CHANGELOG.md
--rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/LICENSE
--rw-r--r--   0 grze      (1000) grze      (1000)      239 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/MANIFEST.in
--rw-r--r--   0 grze      (1000) grze      (1000)     2847 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     1688 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/README.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.874526 wagtail-cjkcms-23.4.1/cjkcms/
--rw-r--r--   0 grze      (1000) grze      (1000)      272 2023-04-16 16:23:34.000000 wagtail-cjkcms-23.4.1/cjkcms/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.874526 wagtail-cjkcms-23.4.1/cjkcms/api/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/api/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2832 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/api/mailchimp.py
--rw-r--r--   0 grze      (1000) grze      (1000)      173 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/apps.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.874526 wagtail-cjkcms-23.4.1/cjkcms/bin/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/bin/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5752 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/bin/cjkcms.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.874526 wagtail-cjkcms-23.4.1/cjkcms/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     3166 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/blocks/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)    10455 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/blocks/base_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     8476 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/blocks/content_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     9292 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/blocks/html_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3337 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/blocks/layout_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/blocks/searchable_html_block.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.874526 wagtail-cjkcms-23.4.1/cjkcms/draftail/
--rw-r--r--   0 grze      (1000) grze      (1000)      305 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/draftail/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3157 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/draftail/draftail_extensions.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5157 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/draftail/draftail_icons.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3191 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/fields.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.874526 wagtail-cjkcms-23.4.1/cjkcms/finders/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/finders/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2459 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/finders/oembed.py
--rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/forms.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1804 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/image_formats.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.854526 wagtail-cjkcms-23.4.1/cjkcms/management/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/management/commands/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/management/commands/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      453 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/management/commands/clear-embeds.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2565 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/management/commands/import-csv.py
--rw-r--r--   0 grze      (1000) grze      (1000)      952 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/management/commands/init-collections.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3560 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/management/commands/init-navbar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3820 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/management/commands/init-website.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/migrations/
--rw-r--r--   0 grze      (1000) grze      (1000)   216350 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0001_initial.py
--rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
--rw-r--r--   0 grze      (1000) grze      (1000)      668 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1027 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1709 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2886 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-04-16 16:02:39.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/models/
--rw-r--r--   0 grze      (1000) grze      (1000)      232 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/models/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      395 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/models/admin_sidebar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2356 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/models/cms_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6302 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/models/integration_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    19651 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/models/page_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    12522 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/models/snippet_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    18294 2023-04-16 16:01:13.000000 wagtail-cjkcms-23.4.1/cjkcms/models/wagtailsettings_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)      125 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/search_urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)     9215 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/settings.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.864526 wagtail-cjkcms-23.4.1/cjkcms/static/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.864526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/
--rw-r--r--   0 grze      (1000) grze      (1000)    93729 2023-04-03 17:02:22.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/bootstrap-icons.css
--rw-r--r--   0 grze      (1000) grze      (1000)    49971 2023-04-03 17:02:22.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/bootstrap-icons.json
--rw-r--r--   0 grze      (1000) grze      (1000)    55169 2023-04-03 17:02:22.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/fonts/
--rw-r--r--   0 grze      (1000) grze      (1000)   164360 2023-04-03 17:02:22.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
--rw-r--r--   0 grze      (1000) grze      (1000)   121340 2023-04-03 17:02:22.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/
--rw-r--r--   0 grze      (1000) grze      (1000)      846 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/cjkcms-admin.css
--rw-r--r--   0 grze      (1000) grze      (1000)     1039 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/cjkcms-editor.css
--rw-r--r--   0 grze      (1000) grze      (1000)     4375 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/cjkcms-front.css
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.864526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/avatars/
--rw-r--r--   0 grze      (1000) grze      (1000)      535 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/avatars/default.png
--rw-r--r--   0 grze      (1000) grze      (1000)      384 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/avatars/default.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/icons/
--rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/icons/quote.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/logos/
--rw-r--r--   0 grze      (1000) grze      (1000)     4166 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
--rw-r--r--   0 grze      (1000) grze      (1000)     4218 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/
--rw-r--r--   0 grze      (1000) grze      (1000)    47935 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)    31707 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)    38190 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.894526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/js/
--rw-r--r--   0 grze      (1000) grze      (1000)      444 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/js/cjkcms-editor.js
--rw-r--r--   0 grze      (1000) grze      (1000)     5780 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/js/cjkcms-front.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.894526 wagtail-cjkcms-23.4.1/cjkcms/static/cookieconsent/
--rw-r--r--   0 grze      (1000) grze      (1000)    18803 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cookieconsent/cookieconsent.css
--rw-r--r--   0 grze      (1000) grze      (1000)    18743 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cookieconsent/cookieconsent.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.894526 wagtail-cjkcms-23.4.1/cjkcms/templates/
--rw-r--r--   0 grze      (1000) grze      (1000)     4176 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/404.html
--rw-r--r--   0 grze      (1000) grze      (1000)     4802 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/500.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.894526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.904526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     1443 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/accordion_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      974 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/article_block_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1132 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)      188 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/base_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2505 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/base_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      740 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/button_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      746 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      856 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_blurb.html
--rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_foot.html
--rw-r--r--   0 grze      (1000) grze      (1000)      730 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_head.html
--rw-r--r--   0 grze      (1000) grze      (1000)      771 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html
--rw-r--r--   0 grze      (1000) grze      (1000)      990 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
--rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_img.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2618 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_landing1.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2758 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_landing2.html
--rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      450 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)      276 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2698 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/carousel_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      406 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/column_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/document_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/download_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      103 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/embed_video_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)       95 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/external_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      424 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/grid_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/h1_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/h2_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/h3_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      790 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/hero_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/image_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1400 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      627 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/image_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1020 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/modal_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      164 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/page_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      787 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      642 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
--rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)      956 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
--rw-r--r--   0 grze      (1000) grze      (1000)      397 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      610 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
--rw-r--r--   0 grze      (1000) grze      (1000)      300 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1065 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagepreview_form.html
--rw-r--r--   0 grze      (1000) grze      (1000)      244 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pricelist_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      513 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      353 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/quote_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      852 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
--rw-r--r--   0 grze      (1000) grze      (1000)      998 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
--rw-r--r--   0 grze      (1000) grze      (1000)      216 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)       91 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/rich_text_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1095 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/table_block.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.904526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/cookieconsent/
--rw-r--r--   0 grze      (1000) grze      (1000)     3672 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/cookieconsent/languages.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.904526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/
--rw-r--r--   0 grze      (1000) grze      (1000)      267 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/date.html
--rw-r--r--   0 grze      (1000) grze      (1000)      416 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/datetime.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.904526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/
--rw-r--r--   0 grze      (1000) grze      (1000)     9267 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
--rw-r--r--   0 grze      (1000) grze      (1000)     6469 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
--rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
--rw-r--r--   0 grze      (1000) grze      (1000)      264 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/time.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/
--rw-r--r--   0 grze      (1000) grze      (1000)      465 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/align-left.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/check-square-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/columns.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      359 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/desktop.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      571 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/font.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      292 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/google.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      813 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      666 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/hashtag.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      840 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/header.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/list-alt.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      459 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/map.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      448 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/newspaper-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      721 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      635 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/recycle.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      174 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/stop.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      505 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/th-large.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      762 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/universal-access.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      548 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/usd.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      225 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/window-maximize.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      199 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/window-minimize.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/
--rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
--rw-r--r--   0 grze      (1000) grze      (1000)      689 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      579 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/classifier_nav.html
--rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/codered_banner.html
--rw-r--r--   0 grze      (1000) grze      (1000)      268 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/form_honeypot.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1061 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/pagination.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/stream_forms/
--rw-r--r--   0 grze      (1000) grze      (1000)      532 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/
--rw-r--r--   0 grze      (1000) grze      (1000)     2002 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/article_index_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1705 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/article_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1018 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/article_page.search.html
--rw-r--r--   0 grze      (1000) grze      (1000)     7931 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/base.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/form_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      248 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/form_page_landing.html
--rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/home_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2610 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/search.html
--rw-r--r--   0 grze      (1000) grze      (1000)      582 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/search_result.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2462 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/stream_form_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      838 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/web_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      623 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/web_page_notitle.html
--rw-r--r--   0 grze      (1000) grze      (1000)      122 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/robots.txt
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/
--rw-r--r--   0 grze      (1000) grze      (1000)      430 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/footer.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2027 2023-04-16 16:13:17.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1196 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
--rw-r--r--   0 grze      (1000) grze      (1000)      836 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/lang_selector.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2586 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/navbar.html
--rw-r--r--   0 grze      (1000) grze      (1000)      386 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/navbar_search.html
--rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/tracking_g3.html
--rw-r--r--   0 grze      (1000) grze      (1000)      831 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/widgets/
--rw-r--r--   0 grze      (1000) grze      (1000)     1384 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.864526 wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/block_forms/
--rw-r--r--   0 grze      (1000) grze      (1000)      754 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
--rw-r--r--   0 grze      (1000) grze      (1000)      550 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/block_forms/struct.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/shared/
--rw-r--r--   0 grze      (1000) grze      (1000)      885 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/cjkcms/templatetags/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templatetags/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      327 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templatetags/auth_extras.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6684 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templatetags/cjkcms_tags.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4962 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templatetags/friendly_loader.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1127 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templatetags/gravatar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templatetags/txtutils_tags.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/cjkcms/tests/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4228 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_articlepages.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2629 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_gravatar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4639 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_search_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2665 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_settings.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3511 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_templatetags.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2678 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1522 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_webpage.py
--rw-r--r--   0 grze      (1000) grze      (1000)      506 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/utils.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4488 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/views.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6211 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/wagtail_hooks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1531 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/widgets.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/docs/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/docs/how-to/
--rw-r--r--   0 grze      (1000) grze      (1000)     1481 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/how-to/oembed_finder.md
--rw-r--r--   0 grze      (1000) grze      (1000)      537 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/index.md
--rw-r--r--   0 grze      (1000) grze      (1000)     5520 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/installation.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/docs/management_commands/
--rw-r--r--   0 grze      (1000) grze      (1000)      318 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/management_commands/clear-embeds.md
--rw-r--r--   0 grze      (1000) grze      (1000)      193 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/management_commands/index.md
--rw-r--r--   0 grze      (1000) grze      (1000)      420 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/management_commands/init-collections.md
--rw-r--r--   0 grze      (1000) grze      (1000)      936 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/quick-start.md
--rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/requirements.txt
--rw-r--r--   0 grze      (1000) grze      (1000)     1220 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/why-another-cms.md
--rw-r--r--   0 grze      (1000) grze      (1000)       93 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/pyproject.toml
--rw-r--r--   0 grze      (1000) grze      (1000)     1541 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/setup.cfg
--rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/setup.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/
--rw-r--r--   0 grze      (1000) grze      (1000)     2847 2023-04-16 16:31:36.000000 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     9351 2023-04-16 16:31:36.000000 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/SOURCES.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-04-16 16:31:36.000000 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/dependency_links.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       51 2023-04-16 16:31:36.000000 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/entry_points.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       79 2023-04-16 16:31:36.000000 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/requires.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-04-16 16:31:36.000000 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/top_level.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.799374 wagtail-cjkcms-23.4.2/
+-rw-r--r--   0 grze      (1000) grze      (1000)     6497 2023-04-20 08:06:11.000000 wagtail-cjkcms-23.4.2/CHANGELOG.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/LICENSE
+-rw-r--r--   0 grze      (1000) grze      (1000)      239 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/MANIFEST.in
+-rw-r--r--   0 grze      (1000) grze      (1000)     2847 2023-04-20 08:09:53.799374 wagtail-cjkcms-23.4.2/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)     1688 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.759374 wagtail-cjkcms-23.4.2/cjkcms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      272 2023-04-20 08:04:28.000000 wagtail-cjkcms-23.4.2/cjkcms/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.759374 wagtail-cjkcms-23.4.2/cjkcms/api/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/api/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2832 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/api/mailchimp.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      173 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/apps.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.759374 wagtail-cjkcms-23.4.2/cjkcms/bin/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/bin/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5752 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/bin/cjkcms.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.759374 wagtail-cjkcms-23.4.2/cjkcms/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     3166 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/blocks/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    10455 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/blocks/base_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     8476 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/blocks/content_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9292 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/blocks/html_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3337 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/blocks/layout_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/blocks/searchable_html_block.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.759374 wagtail-cjkcms-23.4.2/cjkcms/draftail/
+-rw-r--r--   0 grze      (1000) grze      (1000)      305 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/draftail/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3157 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/draftail/draftail_extensions.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5157 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/draftail/draftail_icons.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3191 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/fields.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.759374 wagtail-cjkcms-23.4.2/cjkcms/finders/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/finders/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2459 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/finders/oembed.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/forms.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1804 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/image_formats.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.749374 wagtail-cjkcms-23.4.2/cjkcms/management/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.769374 wagtail-cjkcms-23.4.2/cjkcms/management/commands/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/management/commands/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      453 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/management/commands/clear-embeds.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2565 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/management/commands/import-csv.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      952 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/management/commands/init-collections.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3560 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/management/commands/init-navbar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3820 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/management/commands/init-website.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.769374 wagtail-cjkcms-23.4.2/cjkcms/migrations/
+-rw-r--r--   0 grze      (1000) grze      (1000)   216350 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/migrations/0001_initial.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      668 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1027 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1709 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2886 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/migrations/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.769374 wagtail-cjkcms-23.4.2/cjkcms/models/
+-rw-r--r--   0 grze      (1000) grze      (1000)      232 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/models/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      395 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/models/admin_sidebar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2356 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/models/cms_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6302 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/models/integration_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    19651 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/models/page_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    12522 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/models/snippet_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    18294 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/models/wagtailsettings_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      125 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/search_urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9215 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/settings.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.749374 wagtail-cjkcms-23.4.2/cjkcms/static/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.749374 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.769374 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/bi/
+-rw-r--r--   0 grze      (1000) grze      (1000)    93729 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/bi/bootstrap-icons.css
+-rw-r--r--   0 grze      (1000) grze      (1000)    49971 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/bi/bootstrap-icons.json
+-rw-r--r--   0 grze      (1000) grze      (1000)    55169 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.769374 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/bi/fonts/
+-rw-r--r--   0 grze      (1000) grze      (1000)   164360 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
+-rw-r--r--   0 grze      (1000) grze      (1000)   121340 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.769374 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/css/
+-rw-r--r--   0 grze      (1000) grze      (1000)      846 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/css/cjkcms-admin.css
+-rw-r--r--   0 grze      (1000) grze      (1000)     1039 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/css/cjkcms-editor.css
+-rw-r--r--   0 grze      (1000) grze      (1000)     4375 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/css/cjkcms-front.css
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.749374 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.769374 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/avatars/
+-rw-r--r--   0 grze      (1000) grze      (1000)      535 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/avatars/default.png
+-rw-r--r--   0 grze      (1000) grze      (1000)      384 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/avatars/default.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.769374 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/icons/
+-rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/icons/quote.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.769374 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/logos/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4166 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)     4218 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.769374 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/patterns/
+-rw-r--r--   0 grze      (1000) grze      (1000)    47935 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)    31707 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)    38190 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.779374 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/js/
+-rw-r--r--   0 grze      (1000) grze      (1000)      444 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/js/cjkcms-editor.js
+-rw-r--r--   0 grze      (1000) grze      (1000)     5780 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/js/cjkcms-front.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.779374 wagtail-cjkcms-23.4.2/cjkcms/static/cookieconsent/
+-rw-r--r--   0 grze      (1000) grze      (1000)    18803 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cookieconsent/cookieconsent.css
+-rw-r--r--   0 grze      (1000) grze      (1000)    18743 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/static/cookieconsent/cookieconsent.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.779374 wagtail-cjkcms-23.4.2/cjkcms/templates/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4176 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/404.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     4802 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/500.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.779374 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.779374 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1443 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/accordion_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      974 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/article_block_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1132 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      188 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/base_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2505 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/base_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      740 2023-04-20 08:03:56.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/button_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      746 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      856 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_blurb.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_foot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      730 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_head.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      771 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_head_foot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      990 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_horizontal.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_img.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2618 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_landing1.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2758 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_landing2.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      450 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      276 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2698 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/carousel_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      406 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/column_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/document_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/download_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      103 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/embed_video_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       95 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/external_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      424 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/grid_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/h1_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/h2_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/h3_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      790 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/hero_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/image_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1400 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      627 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/image_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1020 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/modal_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      164 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/page_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      787 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      642 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      956 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      397 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagelist_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      610 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      300 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1065 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagepreview_form.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      244 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pricelist_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      513 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      353 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/quote_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      852 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      998 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      216 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       91 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/rich_text_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1095 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/table_block.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.779374 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/cookieconsent/
+-rw-r--r--   0 grze      (1000) grze      (1000)     3672 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/cookieconsent/languages.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.779374 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/formfields/
+-rw-r--r--   0 grze      (1000) grze      (1000)      267 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/formfields/date.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      416 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/formfields/datetime.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.789374 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/formfields/mailchimp/
+-rw-r--r--   0 grze      (1000) grze      (1000)     9267 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     6469 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      264 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/formfields/time.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.789374 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/
+-rw-r--r--   0 grze      (1000) grze      (1000)      465 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/align-left.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/check-square-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/columns.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      359 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/desktop.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      571 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/font.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      292 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/google.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      813 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      666 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/hashtag.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      840 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/header.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/list-alt.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      459 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/map.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      448 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/newspaper-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      721 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      635 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/recycle.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      174 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/stop.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      505 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/th-large.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      762 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/universal-access.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      548 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/usd.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      225 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/window-maximize.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      199 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/window-minimize.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.789374 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/
+-rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      689 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      579 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/classifier_nav.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/codered_banner.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      268 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/form_honeypot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1061 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/pagination.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.789374 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/stream_forms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      532 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.789374 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2002 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/article_index_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1705 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/article_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1018 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/article_page.search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     7931 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/base.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/form_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      248 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/form_page_landing.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/home_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2610 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      582 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/search_result.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2462 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/stream_form_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      838 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/web_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      623 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/web_page_notitle.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      122 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/robots.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.789374 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/
+-rw-r--r--   0 grze      (1000) grze      (1000)      430 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/footer.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2027 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/frontend_assets.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1196 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      836 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/lang_selector.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2586 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/navbar.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      386 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/navbar_search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/tracking_g3.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      831 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/tracking_g4.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.789374 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/widgets/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1384 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.759374 wagtail-cjkcms-23.4.2/cjkcms/templates/wagtailadmin/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.789374 wagtail-cjkcms-23.4.2/cjkcms/templates/wagtailadmin/block_forms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      754 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      550 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/wagtailadmin/block_forms/struct.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.789374 wagtail-cjkcms-23.4.2/cjkcms/templates/wagtailadmin/shared/
+-rw-r--r--   0 grze      (1000) grze      (1000)      885 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.789374 wagtail-cjkcms-23.4.2/cjkcms/templatetags/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/templatetags/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      327 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/templatetags/auth_extras.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6785 2023-04-20 08:01:03.000000 wagtail-cjkcms-23.4.2/cjkcms/templatetags/cjkcms_tags.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4962 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/templatetags/friendly_loader.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1127 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/templatetags/gravatar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/templatetags/txtutils_tags.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.799374 wagtail-cjkcms-23.4.2/cjkcms/tests/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/tests/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4226 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/tests/test_articlepages.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2629 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/tests/test_gravatar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4639 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/tests/test_search_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2665 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/tests/test_settings.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3511 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/tests/test_templatetags.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2678 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/tests/test_urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1520 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/tests/test_webpage.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      506 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/utils.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4488 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/views.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6211 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/wagtail_hooks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1531 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/cjkcms/widgets.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.799374 wagtail-cjkcms-23.4.2/docs/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.799374 wagtail-cjkcms-23.4.2/docs/how-to/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1481 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/docs/how-to/oembed_finder.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      537 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/docs/index.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     5520 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/docs/installation.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.799374 wagtail-cjkcms-23.4.2/docs/management_commands/
+-rw-r--r--   0 grze      (1000) grze      (1000)      318 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/docs/management_commands/clear-embeds.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      193 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/docs/management_commands/index.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      420 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/docs/management_commands/init-collections.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      936 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/docs/quick-start.md
+-rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/docs/requirements.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)     1220 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/docs/why-another-cms.md
+-rw-r--r--   0 grze      (1000) grze      (1000)       93 2023-04-17 17:52:47.000000 wagtail-cjkcms-23.4.2/pyproject.toml
+-rw-r--r--   0 grze      (1000) grze      (1000)     1541 2023-04-20 08:09:53.799374 wagtail-cjkcms-23.4.2/setup.cfg
+-rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-04-17 17:53:25.000000 wagtail-cjkcms-23.4.2/setup.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-20 08:09:53.799374 wagtail-cjkcms-23.4.2/wagtail_cjkcms.egg-info/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2847 2023-04-20 08:09:53.000000 wagtail-cjkcms-23.4.2/wagtail_cjkcms.egg-info/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)     9351 2023-04-20 08:09:53.000000 wagtail-cjkcms-23.4.2/wagtail_cjkcms.egg-info/SOURCES.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-04-20 08:09:53.000000 wagtail-cjkcms-23.4.2/wagtail_cjkcms.egg-info/dependency_links.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)       51 2023-04-20 08:09:53.000000 wagtail-cjkcms-23.4.2/wagtail_cjkcms.egg-info/entry_points.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)       79 2023-04-20 08:09:53.000000 wagtail-cjkcms-23.4.2/wagtail_cjkcms.egg-info/requires.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-04-20 08:09:53.000000 wagtail-cjkcms-23.4.2/wagtail_cjkcms.egg-info/top_level.txt
```

### Comparing `wagtail-cjkcms-23.4.1/CHANGELOG.md` & `wagtail-cjkcms-23.4.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -163,8 +163,11 @@
 - Fixed problem with migration broken by 23.2.5
 
 # 23.3.1 (2023-03-12)
 - Added "cjkcms start [projectname]" command to create a new project with wagtail-cjkcms installed
 
 # 23.4.1 (2023-04-16)
 - Added new layout setting (bootstrap_icon) + static files to load Bootstrap icons css+woff locally.
-- Modified frontend_assets template to load bootstrap icons if set.
+- Modified frontend_assets template to load bootstrap icons if set.
+
+# 23.4.2 (2023-04-20)
+- Fixed problem of request context missing in can_show_item templatetag by adding try/except block.
```

### Comparing `wagtail-cjkcms-23.4.1/LICENSE` & `wagtail-cjkcms-23.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/PKG-INFO` & `wagtail-cjkcms-23.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-cjkcms
-Version: 23.4.1
+Version: 23.4.2
 Summary: Wagtail Content Management System, installable as a Django app into any Wagtail 4.x site. Based on Codered CRX.
 Home-page: https://github.com/cjkpl/wagtail-cjkcms
 Author: Grzegorz Krol
 Author-email: gk@cjk.pl
 License: BSD-3-Clause  # Example license
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-cjkcms-23.4.1/README.md` & `wagtail-cjkcms-23.4.2/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/api/mailchimp.py` & `wagtail-cjkcms-23.4.2/cjkcms/api/mailchimp.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/bin/cjkcms.py` & `wagtail-cjkcms-23.4.2/cjkcms/bin/cjkcms.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/blocks/__init__.py` & `wagtail-cjkcms-23.4.2/cjkcms/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/blocks/base_blocks.py` & `wagtail-cjkcms-23.4.2/cjkcms/blocks/base_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/blocks/content_blocks.py` & `wagtail-cjkcms-23.4.2/cjkcms/blocks/content_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/blocks/html_blocks.py` & `wagtail-cjkcms-23.4.2/cjkcms/blocks/html_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/blocks/layout_blocks.py` & `wagtail-cjkcms-23.4.2/cjkcms/blocks/layout_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/draftail/draftail_extensions.py` & `wagtail-cjkcms-23.4.2/cjkcms/draftail/draftail_extensions.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/draftail/draftail_icons.py` & `wagtail-cjkcms-23.4.2/cjkcms/draftail/draftail_icons.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/fields.py` & `wagtail-cjkcms-23.4.2/cjkcms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/finders/oembed.py` & `wagtail-cjkcms-23.4.2/cjkcms/finders/oembed.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/image_formats.py` & `wagtail-cjkcms-23.4.2/cjkcms/image_formats.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/management/commands/import-csv.py` & `wagtail-cjkcms-23.4.2/cjkcms/management/commands/import-csv.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/management/commands/init-collections.py` & `wagtail-cjkcms-23.4.2/cjkcms/management/commands/init-collections.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/management/commands/init-navbar.py` & `wagtail-cjkcms-23.4.2/cjkcms/management/commands/init-navbar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/management/commands/init-website.py` & `wagtail-cjkcms-23.4.2/cjkcms/management/commands/init-website.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/migrations/0001_initial.py` & `wagtail-cjkcms-23.4.2/cjkcms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py` & `wagtail-cjkcms-23.4.2/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py` & `wagtail-cjkcms-23.4.2/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py` & `wagtail-cjkcms-23.4.2/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py` & `wagtail-cjkcms-23.4.2/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py` & `wagtail-cjkcms-23.4.2/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py` & `wagtail-cjkcms-23.4.2/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/models/cms_models.py` & `wagtail-cjkcms-23.4.2/cjkcms/models/cms_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/models/integration_models.py` & `wagtail-cjkcms-23.4.2/cjkcms/models/integration_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/models/page_models.py` & `wagtail-cjkcms-23.4.2/cjkcms/models/page_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/models/snippet_models.py` & `wagtail-cjkcms-23.4.2/cjkcms/models/snippet_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/models/wagtailsettings_models.py` & `wagtail-cjkcms-23.4.2/cjkcms/models/wagtailsettings_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/settings.py` & `wagtail-cjkcms-23.4.2/cjkcms/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/bootstrap-icons.css` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/bi/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/bootstrap-icons.json` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/bi/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/bootstrap-icons.scss` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/bi/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/cjkcms-admin.css` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/css/cjkcms-admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/cjkcms-editor.css` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/css/cjkcms-editor.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/cjkcms-front.css` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/css/cjkcms-front.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/avatars/default.png` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/avatars/default.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/icons/quote.svg` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/patterns/pattern1.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/patterns/pattern2.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/images/patterns/pattern3.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/js/cjkcms-front.js` & `wagtail-cjkcms-23.4.2/cjkcms/static/cjkcms/js/cjkcms-front.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cookieconsent/cookieconsent.css` & `wagtail-cjkcms-23.4.2/cjkcms/static/cookieconsent/cookieconsent.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/static/cookieconsent/cookieconsent.js` & `wagtail-cjkcms-23.4.2/cjkcms/static/cookieconsent/cookieconsent.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/404.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/404.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/500.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/500.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/accordion_block.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/accordion_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/article_block_card.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/article_block_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/article_masonry_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/base_link_block.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/base_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/button_block.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/button_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_block.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_blurb.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_blurb.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_foot.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_head.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_head.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_head_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_horizontal.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_horizontal2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_img.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_img.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_landing1.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_landing1.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_landing2.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/card_landing2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/carousel_block.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/carousel_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/download_block.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/download_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/hero_block.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/hero_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/image_gallery_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/image_link_block.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/image_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/modal_block.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/modal_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagepreview_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagepreview_form.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pagepreview_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/table_block.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/blocks/table_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/cookieconsent/languages.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/cookieconsent/languages.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/check-square-o.svg` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/check-square-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/font.svg` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/font.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/hashtag.svg` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/hashtag.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/header.svg` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/header.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/list-alt.svg` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/list-alt.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/puzzle-piece.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/recycle.svg` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/recycle.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/universal-access.svg` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/universal-access.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/usd.svg` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/icons/usd.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/classifier_nav.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/classifier_nav.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/pagination.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/article_index_page.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/article_index_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/article_page.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/article_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/article_page.search.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/article_page.search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/base.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/base.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/form_page.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/form_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/search.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/search_result.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/search_result.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/stream_form_page.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/stream_form_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/web_page.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/web_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/web_page_notitle.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/pages/web_page_notitle.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/frontend_assets.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/frontend_scripts.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/lang_selector.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/lang_selector.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/navbar.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/navbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/snippets/tracking_g4.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/block_forms/struct.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/wagtailadmin/block_forms/struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html` & `wagtail-cjkcms-23.4.2/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templatetags/cjkcms_tags.py` & `wagtail-cjkcms-23.4.2/cjkcms/templatetags/cjkcms_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,14 +184,19 @@
     """
     Menu item visibility conditional on selection in cms_settings.AUTH_VISIBILITY_CHOICES
     """
     if item_visibility == "hidden":
         return False
     if item_visibility == "all":
         return True
+
+    try:
+        context["request"].user.is_authenticated
+    except KeyError:
+        return False
     is_auth = context["request"].user.is_authenticated
     return bool(
         is_auth
         and item_visibility == "auth-only"
         or not is_auth
         and item_visibility == "non-auth-only"
     )
```

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templatetags/friendly_loader.py` & `wagtail-cjkcms-23.4.2/cjkcms/templatetags/friendly_loader.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templatetags/gravatar.py` & `wagtail-cjkcms-23.4.2/cjkcms/templatetags/gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/templatetags/txtutils_tags.py` & `wagtail-cjkcms-23.4.2/cjkcms/templatetags/txtutils_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/tests/test_articlepages.py` & `wagtail-cjkcms-23.4.2/cjkcms/tests/test_articlepages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from wagtail.tests.utils import WagtailPageTests
+from wagtail.test.utils import WagtailPageTests
 from cjkcms.models import (
     CjkcmsArticlePage,
     CjkcmsArticleIndexPage,
 )
-from wagtail.tests.utils.form_data import nested_form_data
+from wagtail.test.utils.form_data import nested_form_data
 
 from wagtail.models import Page
 from cjkcms.models.cms_models import ArticlePage, ArticleIndexPage, WebPage
 
 
 class ArticlePageTests(WagtailPageTests):
     """Tests CjkCms Article Pages"""
```

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/tests/test_gravatar.py` & `wagtail-cjkcms-23.4.2/cjkcms/tests/test_gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/tests/test_search_blocks.py` & `wagtail-cjkcms-23.4.2/cjkcms/tests/test_search_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/tests/test_settings.py` & `wagtail-cjkcms-23.4.2/cjkcms/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/tests/test_templatetags.py` & `wagtail-cjkcms-23.4.2/cjkcms/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/tests/test_urls.py` & `wagtail-cjkcms-23.4.2/cjkcms/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/tests/test_webpage.py` & `wagtail-cjkcms-23.4.2/cjkcms/tests/test_webpage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from wagtail.tests.utils import WagtailPageTests
+from wagtail.test.utils import WagtailPageTests
 from cjkcms.models import CjkcmsWebPage
 from cjkcms.models.cms_models import WebPage
-from wagtail.tests.utils.form_data import nested_form_data
+from wagtail.test.utils.form_data import nested_form_data
 
 from wagtail.models import Page
 
 
 class WebPageTests(WagtailPageTests):
     """Tests CjkCms Web Page"""
```

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/utils.py` & `wagtail-cjkcms-23.4.2/cjkcms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/views.py` & `wagtail-cjkcms-23.4.2/cjkcms/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/wagtail_hooks.py` & `wagtail-cjkcms-23.4.2/cjkcms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/cjkcms/widgets.py` & `wagtail-cjkcms-23.4.2/cjkcms/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/docs/how-to/oembed_finder.md` & `wagtail-cjkcms-23.4.2/docs/how-to/oembed_finder.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/docs/index.md` & `wagtail-cjkcms-23.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/docs/installation.md` & `wagtail-cjkcms-23.4.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/docs/quick-start.md` & `wagtail-cjkcms-23.4.2/docs/quick-start.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/docs/why-another-cms.md` & `wagtail-cjkcms-23.4.2/docs/why-another-cms.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/setup.cfg` & `wagtail-cjkcms-23.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/PKG-INFO` & `wagtail-cjkcms-23.4.2/wagtail_cjkcms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-cjkcms
-Version: 23.4.1
+Version: 23.4.2
 Summary: Wagtail Content Management System, installable as a Django app into any Wagtail 4.x site. Based on Codered CRX.
 Home-page: https://github.com/cjkpl/wagtail-cjkcms
 Author: Grzegorz Krol
 Author-email: gk@cjk.pl
 License: BSD-3-Clause  # Example license
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/SOURCES.txt` & `wagtail-cjkcms-23.4.2/wagtail_cjkcms.egg-info/SOURCES.txt`

 * *Files identical despite different names*


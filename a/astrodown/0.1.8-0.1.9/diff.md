# Comparing `tmp/astrodown-0.1.8.tar.gz` & `tmp/astrodown-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrodown-0.1.8.tar", max compression
+gzip compressed data, was "astrodown-0.1.9.tar", max compression
```

## Comparing `astrodown-0.1.8.tar` & `astrodown-0.1.9.tar`

### file list

```diff
@@ -1,125 +1,122 @@
--rw-r--r--   0        0        0     3635 2023-04-02 22:14:27.636944 astrodown-0.1.8/README.md
--rw-r--r--   0        0        0       22 2023-04-02 23:05:54.321804 astrodown-0.1.8/astrodown/__init__.py
--rw-r--r--   0        0        0       33 2023-04-02 18:22:16.031704 astrodown-0.1.8/astrodown/__main__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:22:11.619683 astrodown-0.1.8/astrodown/cli/__init__.py
--rw-r--r--   0        0        0     2051 2023-03-29 22:39:33.149153 astrodown-0.1.8/astrodown/cli/check.py
--rw-r--r--   0        0        0      477 2023-04-03 04:45:16.857756 astrodown-0.1.8/astrodown/cli/init.py
--rw-r--r--   0        0        0      104 2023-03-30 02:18:20.166909 astrodown-0.1.8/astrodown/cli/install.py
--rw-r--r--   0        0        0     1290 2023-04-02 23:53:10.195419 astrodown-0.1.8/astrodown/cli/new.py
--rw-r--r--   0        0        0     2426 2023-04-03 04:41:48.709070 astrodown-0.1.8/astrodown/cli/utils.py
--rw-r--r--   0        0        0     5844 2023-04-03 04:44:30.861374 astrodown-0.1.8/astrodown/commands.py
--rw-r--r--   0        0        0      174 2023-04-03 04:41:06.971864 astrodown-0.1.8/astrodown/constants.py
--rw-r--r--   0        0        0     1505 2023-02-22 05:56:29.813316 astrodown-0.1.8/astrodown/js.py
--rw-r--r--   0        0        0     3881 2023-04-03 04:34:44.316541 astrodown-0.1.8/astrodown/quarto.py
--rw-r--r--   0        0        0      209 2023-04-02 19:53:50.641885 astrodown-0.1.8/astrodown/templates/__init__.py
--rw-r--r--   0        0        0      153 2023-04-02 20:19:40.339443 astrodown-0.1.8/astrodown/templates/basic/cookiecutter.json
--rw-r--r--   0        0        0       46 2023-04-02 22:07:42.295560 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/.env.example
--rw-r--r--   0        0        0      298 2023-04-02 22:07:42.297528 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/.gitignore
--rw-r--r--   0        0        0      983 2023-04-02 22:07:42.299083 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      128 2023-04-02 22:09:55.945960 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/README.md
--rw-r--r--   0        0        0      145 2023-04-02 22:41:19.119312 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/_astrodown.yml
--rw-r--r--   0        0        0      325 2023-04-02 22:07:42.293511 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/_quarto.yml
--rw-r--r--   0        0        0     1096 2023-04-02 22:08:38.368777 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/analysis/py.qmd
--rw-r--r--   0        0        0      362 2023-04-02 22:07:42.300954 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/astro.config.mjs
--rw-r--r--   0        0        0     4206 2023-04-02 22:07:42.271239 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/data/mtcars.qmd
--rw-r--r--   0        0        0      465 2023-04-02 22:09:15.233528 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/index.qmd
--rw-r--r--   0        0        0     1159 2023-04-03 05:06:02.616456 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/package.json
--rw-r--r--   0        0        0     1266 2023-04-02 22:07:42.278560 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/scripts/algolia.ts
--rw-r--r--   0        0        0     1509 2023-04-03 04:36:50.461374 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/scripts/post-render.py
--rw-r--r--   0        0        0      442 2023-04-02 22:07:42.280857 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/BaseHead.astro
--rw-r--r--   0        0        0     1146 2023-04-02 22:07:42.281155 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/Card.astro
--rw-r--r--   0        0        0      285 2023-04-02 22:07:42.281340 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/Network.astro
--rw-r--r--   0        0        0      226 2023-04-02 22:07:42.281516 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/SiteFooter.astro
--rw-r--r--   0        0        0      855 2023-04-02 22:07:42.281704 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/SiteHeader.astro
--rw-r--r--   0        0        0      497 2023-04-02 22:07:42.281987 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/analysis/Metadata.astro
--rw-r--r--   0        0        0     1016 2023-04-02 22:07:42.282256 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/data/DataPreview.tsx
--rw-r--r--   0        0        0      846 2023-04-02 22:07:42.282584 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Alert.astro
--rw-r--r--   0        0        0      235 2023-04-02 22:07:42.282769 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Badge.astro
--rw-r--r--   0        0        0      316 2023-04-02 22:07:42.282945 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Link.astro
--rw-r--r--   0        0        0     2871 2023-04-02 22:07:42.283269 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Modal.tsx
--rw-r--r--   0        0        0     2396 2023-04-02 22:07:42.283429 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/SlideOver.tsx
--rw-r--r--   0        0        0     1255 2023-04-02 22:07:42.283582 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Table.tsx
--rw-r--r--   0        0        0      295 2023-04-02 22:07:42.283862 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/content/config.ts
--rw-r--r--   0        0        0       85 2023-04-02 22:07:42.284015 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/env.d.ts
--rw-r--r--   0        0        0      138 2023-04-02 22:07:42.284210 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/index.d.ts
--rw-r--r--   0        0        0     2237 2023-04-02 22:07:42.284490 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/Analysis.astro
--rw-r--r--   0        0        0      615 2023-04-02 22:07:42.284667 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/BaseLayout.astro
--rw-r--r--   0        0        0     2165 2023-04-02 22:07:42.284913 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/Data.astro
--rw-r--r--   0        0        0      519 2023-04-02 22:07:42.285087 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/SidebarLayout.astro
--rw-r--r--   0        0        0     2491 2023-04-02 22:07:42.285356 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/lib/graph.ts
--rw-r--r--   0        0        0      286 2023-04-02 22:07:42.285505 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/lib/python.ts
--rw-r--r--   0        0        0      371 2023-04-02 22:07:42.285651 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/lib/utils.ts
--rw-r--r--   0        0        0      536 2023-04-02 22:07:42.286178 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/analysis/[...slug].astro
--rw-r--r--   0        0        0     2409 2023-04-02 22:07:42.286398 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/analysis/index.astro
--rw-r--r--   0        0        0      581 2023-04-02 22:07:42.286748 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/data/[...slug].astro
--rw-r--r--   0        0        0      973 2023-04-02 22:07:42.286926 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/data/index.astro
--rw-r--r--   0        0        0      273 2023-04-02 22:07:42.287219 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/graph/index.astro
--rw-r--r--   0        0        0      921 2023-04-03 04:52:41.525666 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/index.astro
--rw-r--r--   0        0        0     1671 2023-04-02 22:07:42.287893 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/playground/[...slug].astro
--rw-r--r--   0        0        0      639 2023-04-02 22:07:42.288078 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/playground/index.astro
--rw-r--r--   0        0        0     1191 2023-04-02 22:07:42.288242 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/schema.ts
--rw-r--r--   0        0        0      191 2023-04-02 22:07:42.288533 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/styles/global.css
--rw-r--r--   0        0        0      160 2023-04-02 22:07:42.288689 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/types.ts
--rw-r--r--   0        0        0      343 2023-04-02 22:07:42.308689 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/tailwind.config.cjs
--rw-r--r--   0        0        0      550 2023-04-02 22:07:42.310288 astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/tsconfig.json
--rw-r--r--   0        0        0      153 2023-04-02 21:26:12.967477 astrodown-0.1.8/astrodown/templates/full/cookiecutter.json
--rw-r--r--   0        0        0       46 2023-04-02 21:23:55.167407 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/.env.example
--rw-r--r--   0        0        0      298 2023-04-02 21:23:55.166359 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/.gitignore
--rw-r--r--   0        0        0      983 2023-04-02 21:23:38.651325 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      127 2023-04-02 21:40:40.683185 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/README.md
--rw-r--r--   0        0        0      146 2023-04-02 22:37:00.542485 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/_astrodown.yml
--rw-r--r--   0        0        0      325 2023-04-02 21:23:38.648293 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/_quarto.yml
--rw-r--r--   0        0        0      903 2023-04-02 21:44:20.020944 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/marketing.qmd
--rw-r--r--   0        0        0     1096 2023-04-02 21:44:54.322023 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/python/py.qmd
--rw-r--r--   0        0        0      575 2023-04-02 21:23:38.650367 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/r/r.qmd
--rw-r--r--   0        0        0      627 2023-04-02 21:44:10.138895 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/test.qmd
--rw-r--r--   0        0        0      318 2023-04-02 21:23:55.194338 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/apps/my-app/app.py
--rw-r--r--   0        0        0      362 2023-04-02 21:23:55.146070 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/astro.config.mjs
--rw-r--r--   0        0        0      221 2023-04-02 21:23:55.194058 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/data/diamonds/diamond-test.qmd
--rw-r--r--   0        0        0      802 2023-04-02 21:23:55.193577 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/data/iris/index.qmd
--rw-r--r--   0        0        0     4206 2023-04-02 21:23:55.193867 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/data/mtcars.qmd
--rw-r--r--   0        0        0      465 2023-04-02 21:46:23.364794 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/index.qmd
--rw-r--r--   0        0        0     1707 2023-04-02 21:23:55.145769 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/models/svm.joblib
--rw-r--r--   0        0        0     1159 2023-04-03 05:05:49.748144 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/package.json
--rw-r--r--   0        0        0     1266 2023-04-02 21:23:55.167003 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/scripts/algolia.ts
--rw-r--r--   0        0        0     1509 2023-04-03 04:36:38.814565 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/scripts/post-render.py
--rw-r--r--   0        0        0      442 2023-04-02 21:23:55.255427 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/BaseHead.astro
--rw-r--r--   0        0        0     1146 2023-04-02 21:23:55.253764 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/Card.astro
--rw-r--r--   0        0        0      285 2023-04-02 21:23:55.253645 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/Network.astro
--rw-r--r--   0        0        0      226 2023-04-02 21:23:55.254860 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/SiteFooter.astro
--rw-r--r--   0        0        0      855 2023-04-02 21:23:55.255092 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/SiteHeader.astro
--rw-r--r--   0        0        0      497 2023-04-02 21:23:55.253958 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/analysis/Metadata.astro
--rw-r--r--   0        0        0     1016 2023-04-02 21:23:55.255314 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/data/DataPreview.tsx
--rw-r--r--   0        0        0      846 2023-04-02 21:23:55.254311 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Alert.astro
--rw-r--r--   0        0        0      235 2023-04-02 21:23:55.254415 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Badge.astro
--rw-r--r--   0        0        0      316 2023-04-02 21:23:55.254177 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Link.astro
--rw-r--r--   0        0        0     2871 2023-04-02 21:23:55.254755 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Modal.tsx
--rw-r--r--   0        0        0     2396 2023-04-02 21:23:55.254643 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/SlideOver.tsx
--rw-r--r--   0        0        0     1255 2023-04-02 21:23:55.254533 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Table.tsx
--rw-r--r--   0        0        0      295 2023-04-02 21:23:55.252193 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/content/config.ts
--rw-r--r--   0        0        0       85 2023-04-02 21:23:55.250828 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/env.d.ts
--rw-r--r--   0        0        0      138 2023-04-02 21:23:55.256544 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/index.d.ts
--rw-r--r--   0        0        0     2237 2023-04-02 21:23:55.255755 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/Analysis.astro
--rw-r--r--   0        0        0      615 2023-04-02 21:23:55.255864 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/BaseLayout.astro
--rw-r--r--   0        0        0     2165 2023-04-02 21:23:55.255635 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/Data.astro
--rw-r--r--   0        0        0      519 2023-04-02 21:23:55.255974 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/SidebarLayout.astro
--rw-r--r--   0        0        0     2491 2023-04-02 21:23:55.256423 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/lib/graph.ts
--rw-r--r--   0        0        0      286 2023-04-02 21:23:55.256199 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/lib/python.ts
--rw-r--r--   0        0        0      371 2023-04-02 21:23:55.256312 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/lib/utils.ts
--rw-r--r--   0        0        0      536 2023-04-02 21:23:55.257017 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/analysis/[...slug].astro
--rw-r--r--   0        0        0     2409 2023-04-02 21:23:55.256896 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/analysis/index.astro
--rw-r--r--   0        0        0      581 2023-04-02 21:23:55.258202 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/data/[...slug].astro
--rw-r--r--   0        0        0      973 2023-04-02 21:23:55.258090 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/data/index.astro
--rw-r--r--   0        0        0      273 2023-04-02 21:23:55.257685 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/graph/index.astro
--rw-r--r--   0        0        0      921 2023-04-03 04:52:23.708207 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/index.astro
--rw-r--r--   0        0        0     1671 2023-04-02 21:23:55.257350 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/playground/[...slug].astro
--rw-r--r--   0        0        0      639 2023-04-02 21:23:55.257228 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/playground/index.astro
--rw-r--r--   0        0        0     1191 2023-04-02 21:23:55.250651 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/schema.ts
--rw-r--r--   0        0        0      191 2023-04-02 21:23:55.253411 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/styles/global.css
--rw-r--r--   0        0        0      160 2023-04-02 21:23:55.253195 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/types.ts
--rw-r--r--   0        0        0      343 2023-04-02 21:23:55.166134 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/tailwind.config.cjs
--rw-r--r--   0        0        0      550 2023-04-02 21:23:55.167298 astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/tsconfig.json
--rw-r--r--   0        0        0      195 2023-04-02 23:50:48.976744 astrodown-0.1.8/astrodown/utils.py
--rw-r--r--   0        0        0      615 2023-04-03 05:08:08.066431 astrodown-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     8559 2023-04-03 05:08:51.122151 astrodown-0.1.8/setup.py
--rw-r--r--   0        0        0     4246 2023-04-03 05:08:51.122394 astrodown-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3635 2023-04-02 22:14:27.636944 astrodown-0.1.9/README.md
+-rw-r--r--   0        0        0       22 2023-04-04 20:54:44.251974 astrodown-0.1.9/astrodown/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-02 18:22:16.031704 astrodown-0.1.9/astrodown/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:22:11.619683 astrodown-0.1.9/astrodown/cli/__init__.py
+-rw-r--r--   0        0        0     2051 2023-03-29 22:39:33.149153 astrodown-0.1.9/astrodown/cli/check.py
+-rw-r--r--   0        0        0      477 2023-04-03 04:45:16.857756 astrodown-0.1.9/astrodown/cli/init.py
+-rw-r--r--   0        0        0      104 2023-03-30 02:18:20.166909 astrodown-0.1.9/astrodown/cli/install.py
+-rw-r--r--   0        0        0     1290 2023-04-02 23:53:10.195419 astrodown-0.1.9/astrodown/cli/new.py
+-rw-r--r--   0        0        0     2426 2023-04-03 04:41:48.709070 astrodown-0.1.9/astrodown/cli/utils.py
+-rw-r--r--   0        0        0     5844 2023-04-03 04:44:30.861374 astrodown-0.1.9/astrodown/commands.py
+-rw-r--r--   0        0        0      174 2023-04-03 04:41:06.971864 astrodown-0.1.9/astrodown/constants.py
+-rw-r--r--   0        0        0     3881 2023-04-03 04:34:44.316541 astrodown-0.1.9/astrodown/quarto.py
+-rw-r--r--   0        0        0      209 2023-04-02 19:53:50.641885 astrodown-0.1.9/astrodown/templates/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-02 20:19:40.339443 astrodown-0.1.9/astrodown/templates/basic/cookiecutter.json
+-rw-r--r--   0        0        0       46 2023-04-02 22:07:42.295560 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/.env.example
+-rw-r--r--   0        0        0      298 2023-04-02 22:07:42.297528 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/.gitignore
+-rw-r--r--   0        0        0      983 2023-04-02 22:07:42.299083 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      128 2023-04-02 22:09:55.945960 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/README.md
+-rw-r--r--   0        0        0      145 2023-04-02 22:41:19.119312 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/_astrodown.yml
+-rw-r--r--   0        0        0      325 2023-04-02 22:07:42.293511 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/_quarto.yml
+-rw-r--r--   0        0        0     1096 2023-04-02 22:08:38.368777 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/analysis/py.qmd
+-rw-r--r--   0        0        0      362 2023-04-02 22:07:42.300954 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/astro.config.mjs
+-rw-r--r--   0        0        0     4206 2023-04-02 22:07:42.271239 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/data/mtcars.qmd
+-rw-r--r--   0        0        0      465 2023-04-02 22:09:15.233528 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/index.qmd
+-rw-r--r--   0        0        0     1125 2023-04-04 21:02:09.357405 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/package.json
+-rw-r--r--   0        0        0     1266 2023-04-02 22:07:42.278560 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/scripts/algolia.ts
+-rw-r--r--   0        0        0     1509 2023-04-03 04:36:50.461374 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/scripts/post-render.py
+-rw-r--r--   0        0        0      442 2023-04-02 22:07:42.280857 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/BaseHead.astro
+-rw-r--r--   0        0        0     1146 2023-04-02 22:07:42.281155 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/Card.astro
+-rw-r--r--   0        0        0      285 2023-04-02 22:07:42.281340 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/Network.astro
+-rw-r--r--   0        0        0      226 2023-04-02 22:07:42.281516 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/SiteFooter.astro
+-rw-r--r--   0        0        0      855 2023-04-02 22:07:42.281704 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/SiteHeader.astro
+-rw-r--r--   0        0        0      497 2023-04-02 22:07:42.281987 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/analysis/Metadata.astro
+-rw-r--r--   0        0        0     1016 2023-04-02 22:07:42.282256 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/data/DataPreview.tsx
+-rw-r--r--   0        0        0      846 2023-04-02 22:07:42.282584 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Alert.astro
+-rw-r--r--   0        0        0      235 2023-04-02 22:07:42.282769 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Badge.astro
+-rw-r--r--   0        0        0      316 2023-04-02 22:07:42.282945 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Link.astro
+-rw-r--r--   0        0        0     2871 2023-04-02 22:07:42.283269 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Modal.tsx
+-rw-r--r--   0        0        0     2396 2023-04-02 22:07:42.283429 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/SlideOver.tsx
+-rw-r--r--   0        0        0     1255 2023-04-02 22:07:42.283582 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Table.tsx
+-rw-r--r--   0        0        0      295 2023-04-02 22:07:42.283862 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/content/config.ts
+-rw-r--r--   0        0        0       85 2023-04-02 22:07:42.284015 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/env.d.ts
+-rw-r--r--   0        0        0      138 2023-04-02 22:07:42.284210 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/index.d.ts
+-rw-r--r--   0        0        0     2340 2023-04-04 21:01:27.210176 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/Analysis.astro
+-rw-r--r--   0        0        0      615 2023-04-02 22:07:42.284667 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/BaseLayout.astro
+-rw-r--r--   0        0        0     2165 2023-04-02 22:07:42.284913 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/Data.astro
+-rw-r--r--   0        0        0      519 2023-04-02 22:07:42.285087 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/SidebarLayout.astro
+-rw-r--r--   0        0        0     2491 2023-04-02 22:07:42.285356 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/lib/graph.ts
+-rw-r--r--   0        0        0     1055 2023-04-04 21:00:18.252784 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/lib/playground.ts
+-rw-r--r--   0        0        0      286 2023-04-02 22:07:42.285505 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/lib/python.ts
+-rw-r--r--   0        0        0      459 2023-04-04 21:00:34.381074 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/lib/utils.ts
+-rw-r--r--   0        0        0      536 2023-04-02 22:07:42.286178 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/analysis/[...slug].astro
+-rw-r--r--   0        0        0     1553 2023-04-04 21:02:03.479401 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/analysis/index.astro
+-rw-r--r--   0        0        0      581 2023-04-02 22:07:42.286748 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/data/[...slug].astro
+-rw-r--r--   0        0        0      973 2023-04-02 22:07:42.286926 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/data/index.astro
+-rw-r--r--   0        0        0      273 2023-04-02 22:07:42.287219 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/graph/index.astro
+-rw-r--r--   0        0        0      921 2023-04-03 04:52:41.525666 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/index.astro
+-rw-r--r--   0        0        0     1191 2023-04-02 22:07:42.288242 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/schema.ts
+-rw-r--r--   0        0        0      191 2023-04-02 22:07:42.288533 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/styles/global.css
+-rw-r--r--   0        0        0      160 2023-04-02 22:07:42.288689 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/types.ts
+-rw-r--r--   0        0        0      343 2023-04-02 22:07:42.308689 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/tailwind.config.cjs
+-rw-r--r--   0        0        0      550 2023-04-02 22:07:42.310288 astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/tsconfig.json
+-rw-r--r--   0        0        0      153 2023-04-02 21:26:12.967477 astrodown-0.1.9/astrodown/templates/full/cookiecutter.json
+-rw-r--r--   0        0        0       46 2023-04-02 21:23:55.167407 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/.env.example
+-rw-r--r--   0        0        0      298 2023-04-02 21:23:55.166359 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/.gitignore
+-rw-r--r--   0        0        0      983 2023-04-02 21:23:38.651325 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      127 2023-04-02 21:40:40.683185 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/README.md
+-rw-r--r--   0        0        0      146 2023-04-02 22:37:00.542485 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/_astrodown.yml
+-rw-r--r--   0        0        0      325 2023-04-02 21:23:38.648293 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/_quarto.yml
+-rw-r--r--   0        0        0      903 2023-04-02 21:44:20.020944 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/marketing.qmd
+-rw-r--r--   0        0        0     1096 2023-04-02 21:44:54.322023 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/python/py.qmd
+-rw-r--r--   0        0        0      575 2023-04-02 21:23:38.650367 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/r/r.qmd
+-rw-r--r--   0        0        0      627 2023-04-02 21:44:10.138895 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/test.qmd
+-rw-r--r--   0        0        0      318 2023-04-02 21:23:55.194338 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/apps/my-app/app.py
+-rw-r--r--   0        0        0      362 2023-04-02 21:23:55.146070 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/astro.config.mjs
+-rw-r--r--   0        0        0      221 2023-04-02 21:23:55.194058 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/data/diamonds/diamond-test.qmd
+-rw-r--r--   0        0        0      802 2023-04-02 21:23:55.193577 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/data/iris/index.qmd
+-rw-r--r--   0        0        0     4206 2023-04-02 21:23:55.193867 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/data/mtcars.qmd
+-rw-r--r--   0        0        0      465 2023-04-02 21:46:23.364794 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/index.qmd
+-rw-r--r--   0        0        0     1707 2023-04-02 21:23:55.145769 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/models/svm.joblib
+-rw-r--r--   0        0        0     1125 2023-04-04 20:59:40.640992 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/package.json
+-rw-r--r--   0        0        0     1266 2023-04-02 21:23:55.167003 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/scripts/algolia.ts
+-rw-r--r--   0        0        0     1509 2023-04-03 04:36:38.814565 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/scripts/post-render.py
+-rw-r--r--   0        0        0      442 2023-04-02 21:23:55.255427 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/BaseHead.astro
+-rw-r--r--   0        0        0     1146 2023-04-02 21:23:55.253764 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/Card.astro
+-rw-r--r--   0        0        0      285 2023-04-02 21:23:55.253645 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/Network.astro
+-rw-r--r--   0        0        0      226 2023-04-02 21:23:55.254860 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/SiteFooter.astro
+-rw-r--r--   0        0        0      855 2023-04-02 21:23:55.255092 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/SiteHeader.astro
+-rw-r--r--   0        0        0      497 2023-04-02 21:23:55.253958 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/analysis/Metadata.astro
+-rw-r--r--   0        0        0     1016 2023-04-02 21:23:55.255314 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/data/DataPreview.tsx
+-rw-r--r--   0        0        0      846 2023-04-02 21:23:55.254311 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Alert.astro
+-rw-r--r--   0        0        0      235 2023-04-02 21:23:55.254415 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Badge.astro
+-rw-r--r--   0        0        0      316 2023-04-02 21:23:55.254177 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Link.astro
+-rw-r--r--   0        0        0     2871 2023-04-02 21:23:55.254755 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Modal.tsx
+-rw-r--r--   0        0        0     2396 2023-04-02 21:23:55.254643 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/SlideOver.tsx
+-rw-r--r--   0        0        0     1255 2023-04-02 21:23:55.254533 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Table.tsx
+-rw-r--r--   0        0        0      295 2023-04-02 21:23:55.252193 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/content/config.ts
+-rw-r--r--   0        0        0       85 2023-04-02 21:23:55.250828 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/env.d.ts
+-rw-r--r--   0        0        0      138 2023-04-02 21:23:55.256544 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/index.d.ts
+-rw-r--r--   0        0        0     2338 2023-04-04 20:59:05.999390 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/Analysis.astro
+-rw-r--r--   0        0        0      615 2023-04-02 21:23:55.255864 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/BaseLayout.astro
+-rw-r--r--   0        0        0     2165 2023-04-02 21:23:55.255635 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/Data.astro
+-rw-r--r--   0        0        0      519 2023-04-02 21:23:55.255974 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/SidebarLayout.astro
+-rw-r--r--   0        0        0     2491 2023-04-02 21:23:55.256423 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/lib/graph.ts
+-rw-r--r--   0        0        0     1055 2023-04-04 20:56:27.976077 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/lib/playground.ts
+-rw-r--r--   0        0        0      286 2023-04-02 21:23:55.256199 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/lib/python.ts
+-rw-r--r--   0        0        0      458 2023-04-04 20:57:14.324062 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/lib/utils.ts
+-rw-r--r--   0        0        0      536 2023-04-02 21:23:55.257017 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/analysis/[...slug].astro
+-rw-r--r--   0        0        0     1553 2023-04-04 20:58:36.804989 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/analysis/index.astro
+-rw-r--r--   0        0        0      581 2023-04-02 21:23:55.258202 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/data/[...slug].astro
+-rw-r--r--   0        0        0      973 2023-04-02 21:23:55.258090 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/data/index.astro
+-rw-r--r--   0        0        0      273 2023-04-02 21:23:55.257685 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/graph/index.astro
+-rw-r--r--   0        0        0      921 2023-04-03 04:52:23.708207 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/index.astro
+-rw-r--r--   0        0        0     1191 2023-04-02 21:23:55.250651 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/schema.ts
+-rw-r--r--   0        0        0      191 2023-04-02 21:23:55.253411 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/styles/global.css
+-rw-r--r--   0        0        0      160 2023-04-02 21:23:55.253195 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/types.ts
+-rw-r--r--   0        0        0      343 2023-04-02 21:23:55.166134 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/tailwind.config.cjs
+-rw-r--r--   0        0        0      550 2023-04-02 21:23:55.167298 astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/tsconfig.json
+-rw-r--r--   0        0        0      195 2023-04-02 23:50:48.976744 astrodown-0.1.9/astrodown/utils.py
+-rw-r--r--   0        0        0      615 2023-04-04 20:54:41.395345 astrodown-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8326 2023-04-04 21:02:56.870184 astrodown-0.1.9/setup.py
+-rw-r--r--   0        0        0     4246 2023-04-04 21:02:56.870503 astrodown-0.1.9/PKG-INFO
```

### Comparing `astrodown-0.1.8/README.md` & `astrodown-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/cli/check.py` & `astrodown-0.1.9/astrodown/cli/check.py`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/cli/new.py` & `astrodown-0.1.9/astrodown/cli/new.py`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/cli/utils.py` & `astrodown-0.1.9/astrodown/cli/utils.py`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/commands.py` & `astrodown-0.1.9/astrodown/commands.py`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/quarto.py` & `astrodown-0.1.9/astrodown/quarto.py`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/.pre-commit-config.yaml` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/analysis/py.qmd` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/analysis/py.qmd`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/data/mtcars.qmd` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/data/mtcars.qmd`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/package.json` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950980392156863%*

 * *Differences: {"'dependencies'": "{delete: ['@astrodown/mars-react']}"}*

```diff
@@ -1,11 +1,10 @@
 {
     "dependencies": {
         "@astrodown/graph": "^0.0.5",
-        "@astrodown/mars-react": "*",
         "@astrodown/schema": "^0.0.4",
         "@astrojs/react": "^2.0.2",
         "@astrojs/tailwind": "^3.0.1",
         "@codemirror/view": "^6.9.3",
         "@headlessui/react": "^1.7.10",
         "@heroicons/react": "^2.0.14",
         "@nanostores/react": "^0.4.1",
```

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/scripts/algolia.ts` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/scripts/algolia.ts`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/scripts/post-render.py` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/scripts/post-render.py`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/Card.astro` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/Card.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/SiteHeader.astro` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/SiteHeader.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/data/DataPreview.tsx` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/data/DataPreview.tsx`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Alert.astro` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Alert.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Modal.tsx` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Modal.tsx`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/SlideOver.tsx` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/SlideOver.tsx`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Table.tsx` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/components/shared/Table.tsx`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/Analysis.astro` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/Analysis.astro`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 ---
 import type { CollectionEntry } from "astro:content";
 import BaseLayout from "./BaseLayout.astro";
 import SidebarLayout from "./SidebarLayout.astro";
 import Badge from "@components/shared/Badge.astro";
-import { showArray } from "@lib/utils";
+import { objectToBase64j, showArray } from "@lib/utils";
 import Metadata from "@components/analysis/Metadata.astro";
 import type { GraphinData } from "@astrodown/graph";
+import { getCodeFromBody } from "@lib/playground";
 
 export interface Props {
   entry: CollectionEntry<"analysis">;
   graphData?: GraphinData;
 }
 
 const { entry, graphData } = Astro.props;
 
+const code = await getCodeFromBody(entry.body);
+const codeEncoded = objectToBase64(code);
+
 const { Content, headings } = await entry.render();
 const metadataEntries = [
   {
     name: "Author",
     value: showArray(entry.data.author),
   },
   {
@@ -62,21 +66,17 @@
           headings.map((heading) => (
             <li class="text-lg p-2 rounded-lg hover:bg-slate-200 transition duration-200">
               <a href={`#${heading.slug}`}>{heading.text}</a>
             </li>
           ))
         }
       </ul>
-      {
-        entry.data.exports.length > 0 && (
-          <a href={`/playground/${entry.slug}`}>
-            <Badge class="bg-blue-200 text-blue-800">Playground</Badge>
-          </a>
-        )
-      }
+      <a href={`https://tridata.qiushiyan.dev/?code=${codeEncoded}`}>
+        <Badge class="bg-blue-200 text-blue-800">Playground</Badge>
+      </a>
     </div>
     <div slot="main">
       <Content />
     </div>
   </SidebarLayout>
   <!-- <PyscriptPlayground exports={entry.data.exports} client:only="react" /> -->
 </BaseLayout>
```

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/BaseLayout.astro` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/BaseLayout.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/Data.astro` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/Data.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/SidebarLayout.astro` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/layouts/SidebarLayout.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/lib/graph.ts` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/lib/graph.ts`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/analysis/[...slug].astro` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/analysis/[...slug].astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/analysis/index.astro` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/analysis/index.astro`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,46 @@
 ---
 import Badge from "@components/shared/Badge.astro";
 import BaseLayout from "@layouts/BaseLayout.astro";
 import { getCollection } from "astro:content";
 const analysis = await getCollection("analysis");
 analysis.sort((a, b) => {
-    return b.data.date.getDate() - a.data.date.getDate();
+  return b.data.date.getDate() - a.data.date.getDate();
 });
 ---
 
 <BaseLayout>
-    <div class="analysis-list flex flex-col max-w-4xl mx-auto gap-2">
-        {
-            analysis.map((entry) => (
-                <>
-                    <article class="mb-6 transition border-b border-blue-600">
-                        <div class="flex items-center justify-between">
-                            <h3 class="font-serif mb-2 text-xl font-semibold leading-tight sm:text-2xl font-heading">
-                                <a
-                                    href={`/analysis/${entry.slug}`}
-                                    class="hover:text-primary dark:hover:text-blue-700  transition ease-in duration-200"
-                                >
-                                    {entry.data.title}
-                                </a>
-                            </h3>
+  <div class="analysis-list flex flex-col max-w-4xl mx-auto gap-2">
+    {
+      analysis.map((entry) => (
+        <>
+          <article class="mb-6 transition border-b border-blue-600">
+            <div class="flex items-center justify-between">
+              <h3 class="font-serif mb-2 text-xl font-semibold leading-tight sm:text-2xl font-heading">
+                <a
+                  href={`/analysis/${entry.slug}`}
+                  class="hover:text-primary dark:hover:text-blue-700  transition ease-in duration-200"
+                >
+                  {entry.data.title}
+                </a>
+              </h3>
 
-                            <div class="text-sm tracking-tighter">
-                                {entry.data.date.toLocaleDateString()}
-                            </div>
-                        </div>
-                        <p class="text-zinc-800">
-                            {entry.data.description || entry.body.slice(0, 100)}
-                        </p>
-                        <div class="flex items-center justify-between my-2">
-                            <div class="tags">
-                                {entry.data.tags.map((tag) => (
-                                    <Badge class="bg-indigo-100 text-indigo-800">
-                                        {tag}
-                                    </Badge>
-                                ))}
-                            </div>
-
-                            {entry.data.exports.length > 0 && (
-                                <a href={`/playground/${entry.slug}`}>
-                                    <Badge class="bg-blue-200 text-blue-800">
-                                        Playground
-                                    </Badge>
-                                </a>
-                            )}
-                        </div>
-                    </article>
-                </>
-            ))
-        }
-    </div>
+              <div class="text-sm tracking-tighter">
+                {entry.data.date.toLocaleDateString()}
+              </div>
+            </div>
+            <p class="text-zinc-800">
+              {entry.data.description || entry.body.slice(0, 100)}
+            </p>
+            <div class="flex items-center justify-between my-2">
+              <div class="tags">
+                {entry.data.tags.map((tag) => (
+                  <Badge class="bg-indigo-100 text-indigo-800">{tag}</Badge>
+                ))}
+              </div>
+            </div>
+          </article>
+        </>
+      ))
+    }
+  </div>
 </BaseLayout>
```

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/data/[...slug].astro` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/data/[...slug].astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/data/index.astro` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/data/index.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/index.astro` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/pages/index.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/schema.ts` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/src/schema.ts`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/basic/{{ cookiecutter.project_name }}/tsconfig.json` & `astrodown-0.1.9/astrodown/templates/basic/{{ cookiecutter.project_name }}/tsconfig.json`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/.pre-commit-config.yaml` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/marketing.qmd` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/marketing.qmd`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/python/py.qmd` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/python/py.qmd`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/r/r.qmd` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/r/r.qmd`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/test.qmd` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/analysis/test.qmd`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/data/iris/index.qmd` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/data/iris/index.qmd`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/data/mtcars.qmd` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/data/mtcars.qmd`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/models/svm.joblib` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/models/svm.joblib`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/package.json` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950980392156863%*

 * *Differences: {"'dependencies'": "{delete: ['@astrodown/mars-react']}"}*

```diff
@@ -1,11 +1,10 @@
 {
     "dependencies": {
         "@astrodown/graph": "^0.0.5",
-        "@astrodown/mars-react": "*",
         "@astrodown/schema": "^0.0.4",
         "@astrojs/react": "^2.0.2",
         "@astrojs/tailwind": "^3.0.1",
         "@codemirror/view": "^6.9.3",
         "@headlessui/react": "^1.7.10",
         "@heroicons/react": "^2.0.14",
         "@nanostores/react": "^0.4.1",
```

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/scripts/algolia.ts` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/scripts/algolia.ts`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/scripts/post-render.py` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/scripts/post-render.py`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/Card.astro` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/Card.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/SiteHeader.astro` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/SiteHeader.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/data/DataPreview.tsx` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/data/DataPreview.tsx`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Alert.astro` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Alert.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Modal.tsx` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Modal.tsx`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/SlideOver.tsx` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/SlideOver.tsx`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Table.tsx` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/components/shared/Table.tsx`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/Analysis.astro` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/Analysis.astro`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 ---
 import type { CollectionEntry } from "astro:content";
 import BaseLayout from "./BaseLayout.astro";
 import SidebarLayout from "./SidebarLayout.astro";
 import Badge from "@components/shared/Badge.astro";
-import { showArray } from "@lib/utils";
 import Metadata from "@components/analysis/Metadata.astro";
+import { objectToBase64, showArray } from "@lib/utils";
+import { getCodeFromBody } from "@lib/playground";
 import type { GraphinData } from "@astrodown/graph";
 
 export interface Props {
   entry: CollectionEntry<"analysis">;
   graphData?: GraphinData;
 }
 
 const { entry, graphData } = Astro.props;
+const code = await getCodeFromBody(entry.body);
+const codeEncoded = objectToBase64(code);
 
 const { Content, headings } = await entry.render();
 const metadataEntries = [
   {
     name: "Author",
     value: showArray(entry.data.author),
   },
@@ -62,21 +65,17 @@
           headings.map((heading) => (
             <li class="text-lg p-2 rounded-lg hover:bg-slate-200 transition duration-200">
               <a href={`#${heading.slug}`}>{heading.text}</a>
             </li>
           ))
         }
       </ul>
-      {
-        entry.data.exports.length > 0 && (
-          <a href={`/playground/${entry.slug}`}>
-            <Badge class="bg-blue-200 text-blue-800">Playground</Badge>
-          </a>
-        )
-      }
+      <a href={`https://tridata.qiushiyan.dev/?code=${codeEncoded}`}>
+        <Badge class="bg-blue-200 text-blue-800">Playground</Badge>
+      </a>
     </div>
     <div slot="main">
       <Content />
     </div>
   </SidebarLayout>
   <!-- <PyscriptPlayground exports={entry.data.exports} client:only="react" /> -->
 </BaseLayout>
```

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/BaseLayout.astro` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/BaseLayout.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/Data.astro` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/Data.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/SidebarLayout.astro` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/layouts/SidebarLayout.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/lib/graph.ts` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/lib/graph.ts`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/analysis/[...slug].astro` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/analysis/[...slug].astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/analysis/index.astro` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/analysis/index.astro`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,46 @@
 ---
 import Badge from "@components/shared/Badge.astro";
 import BaseLayout from "@layouts/BaseLayout.astro";
 import { getCollection } from "astro:content";
 const analysis = await getCollection("analysis");
 analysis.sort((a, b) => {
-    return b.data.date.getDate() - a.data.date.getDate();
+  return b.data.date.getDate() - a.data.date.getDate();
 });
 ---
 
 <BaseLayout>
-    <div class="analysis-list flex flex-col max-w-4xl mx-auto gap-2">
-        {
-            analysis.map((entry) => (
-                <>
-                    <article class="mb-6 transition border-b border-blue-600">
-                        <div class="flex items-center justify-between">
-                            <h3 class="font-serif mb-2 text-xl font-semibold leading-tight sm:text-2xl font-heading">
-                                <a
-                                    href={`/analysis/${entry.slug}`}
-                                    class="hover:text-primary dark:hover:text-blue-700  transition ease-in duration-200"
-                                >
-                                    {entry.data.title}
-                                </a>
-                            </h3>
+  <div class="analysis-list flex flex-col max-w-4xl mx-auto gap-2">
+    {
+      analysis.map((entry) => (
+        <>
+          <article class="mb-6 transition border-b border-blue-600">
+            <div class="flex items-center justify-between">
+              <h3 class="font-serif mb-2 text-xl font-semibold leading-tight sm:text-2xl font-heading">
+                <a
+                  href={`/analysis/${entry.slug}`}
+                  class="hover:text-primary dark:hover:text-blue-700  transition ease-in duration-200"
+                >
+                  {entry.data.title}
+                </a>
+              </h3>
 
-                            <div class="text-sm tracking-tighter">
-                                {entry.data.date.toLocaleDateString()}
-                            </div>
-                        </div>
-                        <p class="text-zinc-800">
-                            {entry.data.description || entry.body.slice(0, 100)}
-                        </p>
-                        <div class="flex items-center justify-between my-2">
-                            <div class="tags">
-                                {entry.data.tags.map((tag) => (
-                                    <Badge class="bg-indigo-100 text-indigo-800">
-                                        {tag}
-                                    </Badge>
-                                ))}
-                            </div>
-
-                            {entry.data.exports.length > 0 && (
-                                <a href={`/playground/${entry.slug}`}>
-                                    <Badge class="bg-blue-200 text-blue-800">
-                                        Playground
-                                    </Badge>
-                                </a>
-                            )}
-                        </div>
-                    </article>
-                </>
-            ))
-        }
-    </div>
+              <div class="text-sm tracking-tighter">
+                {entry.data.date.toLocaleDateString()}
+              </div>
+            </div>
+            <p class="text-zinc-800">
+              {entry.data.description || entry.body.slice(0, 100)}
+            </p>
+            <div class="flex items-center justify-between my-2">
+              <div class="tags">
+                {entry.data.tags.map((tag) => (
+                  <Badge class="bg-indigo-100 text-indigo-800">{tag}</Badge>
+                ))}
+              </div>
+            </div>
+          </article>
+        </>
+      ))
+    }
+  </div>
 </BaseLayout>
```

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/data/[...slug].astro` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/data/[...slug].astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/data/index.astro` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/data/index.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/index.astro` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/pages/index.astro`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/src/schema.ts` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/src/schema.ts`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/astrodown/templates/full/{{ cookiecutter.project_name }}/tsconfig.json` & `astrodown-0.1.9/astrodown/templates/full/{{ cookiecutter.project_name }}/tsconfig.json`

 * *Files identical despite different names*

### Comparing `astrodown-0.1.8/pyproject.toml` & `astrodown-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "astrodown"
-version = "0.1.8"
+version = "0.1.9"
 description = "A framework for creating shareable data science websites"
 authors = ["Qiushi Yan <qiushi.yann@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyodide-http = "^0.2.0"
```

### Comparing `astrodown-0.1.8/setup.py` & `astrodown-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,14 @@
                          'basic/{{ cookiecutter.project_name }}/src/pages/*',
                          'basic/{{ cookiecutter.project_name '
                          '}}/src/pages/analysis/*',
                          'basic/{{ cookiecutter.project_name '
                          '}}/src/pages/data/*',
                          'basic/{{ cookiecutter.project_name '
                          '}}/src/pages/graph/*',
-                         'basic/{{ cookiecutter.project_name '
-                         '}}/src/pages/playground/*',
                          'basic/{{ cookiecutter.project_name }}/src/styles/*',
                          'full/*',
                          'full/{{ cookiecutter.project_name }}/*',
                          'full/{{ cookiecutter.project_name }}/analysis/*',
                          'full/{{ cookiecutter.project_name '
                          '}}/analysis/python/*',
                          'full/{{ cookiecutter.project_name }}/analysis/r/*',
@@ -62,30 +60,28 @@
                          'full/{{ cookiecutter.project_name }}/src/pages/*',
                          'full/{{ cookiecutter.project_name '
                          '}}/src/pages/analysis/*',
                          'full/{{ cookiecutter.project_name '
                          '}}/src/pages/data/*',
                          'full/{{ cookiecutter.project_name '
                          '}}/src/pages/graph/*',
-                         'full/{{ cookiecutter.project_name '
-                         '}}/src/pages/playground/*',
                          'full/{{ cookiecutter.project_name }}/src/styles/*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'cookiecutter>=2.1.1,<3.0.0',
  'pyodide-http>=0.2.0,<0.3.0',
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['astrodown = astrodown.commands:app']}
 
 setup_kwargs = {
     'name': 'astrodown',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'A framework for creating shareable data science websites',
     'long_description': '# `astrodown`\n\n[bold blue]Astrodown[/bold blue] is a toolkit to build interactive websites for data science projects.\n\nSee a live example at https://astrodown-playground.qiushiyan.dev :sparkles:\n\n**Usage**:\n\n```console\n$ astrodown [OPTIONS] COMMAND [ARGS]...\n```\n\n**Options**:\n\n* `--install-completion`: Install completion for the current shell.\n* `--show-completion`: Show completion for the current shell, to copy it or customize the installation.\n* `--help`: Show this message and exit.\n\n\n    Report [bold red]bugs[/bold red] on [link=https://github.com/astrodown/astrodown-web/]Github[/link]\n    \n\n**Commands**:\n\n* `check`: Check for availabilities of programs...\n* `dev`: [bold blue]Preivew[/bold blue] the website\n* `docs`: [bold blue]Open[/bold blue] documentation...\n* `init`: [bold blue]Create[/bold blue] an astrodown...\n* `install`: [bold blue]Install[/bold blue] JavaScript...\n* `new`: [bold blue]Create[/bold blue] the folder...\n* `render`: [bold blue]Render[/bold blue] all Quarto...\n\n## `astrodown check`\n\nCheck for availabilities of programs required by astrodown\n\n**Usage**:\n\n```console\n$ astrodown check [OPTIONS]\n```\n\n**Options**:\n\n* `--help`: Show this message and exit.\n\n## `astrodown dev`\n\n[bold blue]Preivew[/bold blue] the website\n\n**Usage**:\n\n```console\n$ astrodown dev [OPTIONS]\n```\n\n**Options**:\n\n* `--package-manager [npm|yarn|pnpm]`: package manager to use  [default: PackageManager.npm]\n* `--port INTEGER`: port to run the website  [default: 3000]\n* `--render-quarto / --no-render-quarto`: rerender quarto documents first  [default: no-render-quarto]\n* `--help`: Show this message and exit.\n\n## `astrodown docs`\n\n[bold blue]Open[/bold blue] documentation websites for relevant tools, e.g. Quarto, Python, etc.\n\n**Usage**:\n\n```console\n$ astrodown docs [OPTIONS]\n```\n\n**Options**:\n\n* `--help`: Show this message and exit.\n\n## `astrodown init`\n\n[bold blue]Create[/bold blue] an astrodown project.\n\nMust have Quarto Node.js installed and avaiable in PATH variables, use `astrodown check` for health checks.\n\n**Usage**:\n\n```console\n$ astrodown init [OPTIONS]\n```\n\n**Options**:\n\n* `-p, --path TEXT`: path to create the project, default to the current working directory  [default: /Users/qiushi/workspace/astrodown/astrodown-python]\n* `-n, --name TEXT`: name of the project\n* `-pm, --package-manager [npm|yarn|pnpm]`: package manager to use, default to npm  [default: npm]\n* `-t, --template [basic|full]`: template to use, default to basic  [default: basic]\n* `--help`: Show this message and exit.\n\n## `astrodown install`\n\n[bold blue]Install[/bold blue] JavaScript dependencies.\n\nOnly need to be run once per project.\n\n**Usage**:\n\n```console\n$ astrodown install [OPTIONS]\n```\n\n**Options**:\n\n* `--package-manager [npm|yarn|pnpm]`: package manager to use  [default: PackageManager.npm]\n* `--help`: Show this message and exit.\n\n## `astrodown new`\n\n[bold blue]Create[/bold blue] the folder structure for a new analysis, dataset, model, api, etc.\n\n**Usage**:\n\n```console\n$ astrodown new [OPTIONS] COMPONENT_TYPE:{analysis|dataset|model|shinyapp|api}\n```\n\n**Arguments**:\n\n* `COMPONENT_TYPE:{analysis|dataset|model|shinyapp|api}`: the type of the component to be created  [required]\n\n**Options**:\n\n* `--help`: Show this message and exit.\n\n## `astrodown render`\n\n[bold blue]Render[/bold blue] all Quarto documents.\n\nShould be run every time a Quarto document has changed. Edit _quarto.yml to include/exclude files.\n\n**Usage**:\n\n```console\n$ astrodown render [OPTIONS]\n```\n\n**Options**:\n\n* `--package-manager [npm|yarn|pnpm]`: package manager to use  [default: PackageManager.npm]\n* `--help`: Show this message and exit.\n',
     'author': 'Qiushi Yan',
     'author_email': 'qiushi.yann@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `astrodown-0.1.8/PKG-INFO` & `astrodown-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrodown
-Version: 0.1.8
+Version: 0.1.9
 Summary: A framework for creating shareable data science websites
 Author: Qiushi Yan
 Author-email: qiushi.yann@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```


# Comparing `tmp/freemocap-1.0.6rc0.tar.gz` & `tmp/freemocap-1.0.7rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freemocap-1.0.6rc0.tar", last modified: Tue Mar 28 18:49:07 2023, max compression
+gzip compressed data, was "freemocap-1.0.7rc0.tar", last modified: Thu Apr 20 13:48:12 2023, max compression
```

## Comparing `freemocap-1.0.6rc0.tar` & `freemocap-1.0.7rc0.tar`

### file list

```diff
@@ -1,194 +1,189 @@
--rwxr-xr-x   0        0        0      492 2023-03-28 18:48:59.856993 freemocap-1.0.6rc0/.github/dependabot.yml
--rw-r--r--   0        0        0      423 2023-03-28 18:48:59.856993 freemocap-1.0.6rc0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1083 2023-03-28 18:48:59.856993 freemocap-1.0.6rc0/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rwxr-xr-x   0        0        0     1094 2023-03-28 18:48:59.856993 freemocap-1.0.6rc0/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2215 2023-03-28 18:48:59.856993 freemocap-1.0.6rc0/.gitignore
--rw-r--r--   0        0        0      229 2023-03-28 18:48:59.856993 freemocap-1.0.6rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      418 2023-03-28 18:48:59.856993 freemocap-1.0.6rc0/CITATION.cff
--rw-r--r--   0        0        0      327 2023-03-28 18:48:59.856993 freemocap-1.0.6rc0/CODEOWNERS
--rw-r--r--   0        0        0     3348 2023-03-28 18:48:59.856993 freemocap-1.0.6rc0/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/LICENSE
--rw-r--r--   0        0        0      234 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/MANIFEST.in
--rw-r--r--   0        0        0     4868 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/README.md
--rw-r--r--   0        0        0    44734 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/assets/charuco/charuco_board_image.png
--rw-r--r--   0        0        0   332173 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/assets/charuco/charuco_board_image_highRes.png
--rw-r--r--   0        0        0    26366 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/assets/logo/freemocap-logo-black-border.svg
--rw-r--r--   0        0        0   124841 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png
--rw-r--r--   0        0        0    99678 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/assets/logo/freemocap_skelly_logo.ico
--rwxr-xr-x   0        0        0      607 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/bin/builds/install_packages
--rwxr-xr-x   0        0        0      288 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/bin/installer.sh
--rwxr-xr-x   0        0        0      278 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/bin/linux/build.sh
--rwxr-xr-x   0        0        0      161 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/bin/linux/run_uvicorn_server.sh
--rwxr-xr-x   0        0        0      381 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/bin/linux/run_web_server.sh
--rwxr-xr-x   0        0        0      118 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/bin/linux/shell.sh
--rwxr-xr-x   0        0        0      104 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/bin/linux/test.sh
--rwxr-xr-x   0        0        0       71 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/bin/linux/up.sh
--rw-r--r--   0        0        0      410 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/bin/windows/installChocolatey.cmd
--rw-r--r--   0        0        0      112 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/bin/windows/run_web_server.cmd
--rw-r--r--   0        0        0      331 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/experimental/freemocap-ui/.gitignore
--rw-r--r--   0        0        0     2359 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/experimental/freemocap-ui/README.md
--rw-r--r--   0        0        0      734 2023-03-28 18:48:59.860993 freemocap-1.0.6rc0/experimental/freemocap-ui/config-overrides.js
--rw-r--r--   0        0        0  1263565 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/package-lock.json
--rw-r--r--   0        0        0     2548 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/package.json
--rw-r--r--   0        0        0     3585 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/public/favicon.ico
--rw-r--r--   0        0        0     1963 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/public/index.html
--rw-r--r--   0        0        0     4153 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/public/logo192.png
--rw-r--r--   0        0        0    12066 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/public/logo512.png
--rw-r--r--   0        0        0      492 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/public/manifest.json
--rw-r--r--   0        0        0       67 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/public/robots.txt
--rw-r--r--   0        0        0       33 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/scripts/cert.sh
--rw-r--r--   0        0        0      582 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/App.css
--rw-r--r--   0        0        0      366 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/App.test.tsx
--rw-r--r--   0        0        0      193 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/App.tsx
--rw-r--r--   0        0        0      346 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/app/hooks.ts
--rw-r--r--   0        0        0      445 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/app/store.ts
--rw-r--r--   0        0        0      941 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/components/start-stop-process.tsx
--rw-r--r--   0        0        0      475 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/components/webcam/LivePreview.tsx
--rw-r--r--   0        0        0     1057 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx
--rw-r--r--   0        0        0      104 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/components/webcam/webcam.tsx
--rw-r--r--   0        0        0      610 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx
--rw-r--r--   0        0        0     1291 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/features/counter/Counter.module.css
--rw-r--r--   0        0        0     1758 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/features/counter/Counter.tsx
--rw-r--r--   0        0        0      214 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/features/counter/counterAPI.ts
--rw-r--r--   0        0        0      842 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts
--rw-r--r--   0        0        0     2983 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/features/counter/counterSlice.ts
--rw-r--r--   0        0        0      291 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/hooks/use-device-stream.ts
--rw-r--r--   0        0        0      791 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx
--rw-r--r--   0        0        0      366 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/index.css
--rw-r--r--   0        0        0      623 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/index.tsx
--rw-r--r--   0        0        0      417 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/Copyright.tsx
--rw-r--r--   0        0        0     1625 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/Header.tsx
--rw-r--r--   0        0        0     2353 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/Navigator.tsx
--rw-r--r--   0        0        0     4303 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/Paperbase.tsx
--rw-r--r--   0        0        0      394 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/content/BaseContent.tsx
--rw-r--r--   0        0        0      273 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/content/BasePaper.tsx
--rw-r--r--   0        0        0     1943 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/content/Content.tsx
--rw-r--r--   0        0        0      737 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/routing/router.tsx
--rw-r--r--   0        0        0     1122 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/logo.svg
--rw-r--r--   0        0        0       40 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/react-app-env.d.ts
--rw-r--r--   0        0        0     5290 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/serviceWorker.ts
--rw-r--r--   0        0        0      629 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/services/Capture.tsx
--rw-r--r--   0        0        0      370 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/services/Record.ts
--rw-r--r--   0        0        0      198 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/services/cam.ts
--rw-r--r--   0        0        0      325 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/services/download.ts
--rw-r--r--   0        0        0     1717 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/services/frame-capture.tsx
--rw-r--r--   0        0        0      497 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/services/image_send_worker.ts
--rw-r--r--   0        0        0     2044 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/services/recorder.ts
--rw-r--r--   0        0        0     1560 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/services/supported_recorder.ts
--rw-r--r--   0        0        0      254 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/setupTests.ts
--rw-r--r--   0        0        0     1384 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/Capture.tsx
--rw-r--r--   0        0        0      733 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/Config.tsx
--rw-r--r--   0        0        0     1153 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/SessionWorkflow.tsx
--rw-r--r--   0        0        0      109 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/ShowCameras.tsx
--rw-r--r--   0        0        0      124 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/UserConfig.tsx
--rw-r--r--   0        0        0      965 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx
--rw-r--r--   0        0        0      792 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx
--rw-r--r--   0        0        0     1023 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx
--rw-r--r--   0        0        0     1976 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx
--rw-r--r--   0        0        0      599 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/freemocap-ui/tsconfig.json
--rw-r--r--   0        0        0      789 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/python_scratch/qt_drag_and_drop.py
--rw-r--r--   0        0        0     1609 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/experimental/tool_bar.py
--rw-r--r--   0        0        0     1821 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/__init__.py
--rw-r--r--   0        0        0      888 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/__main__.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/__init__.py
--rw-r--r--   0        0        0     6700 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py
--rw-r--r--   0        0        0    60000 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py
--rw-r--r--   0        0        0     2613 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/__init__.py
--rw-r--r--   0        0        0     1504 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py
--rw-r--r--   0        0        0       36 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/default_charuco_square_size.py
--rw-r--r--   0        0        0     1177 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py
--rw-r--r--   0        0        0     9539 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/detecting_things_in_2d_images/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/__init__.py
--rw-r--r--   0        0        0    14641 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py
--rw-r--r--   0        0        0    24623 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py
--rw-r--r--   0        0        0     1752 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_names_and_connections.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.868993 freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/__init__.py
--rw-r--r--   0        0        0    57980 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/alpha_freemocap_blender_megascript.py
--rw-r--r--   0        0        0     1091 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/cgtinker_blendarmocap_load.py
--rw-r--r--   0        0        0    37868 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/freemocap_blender_megascript_take2.py
--rw-r--r--   0        0        0     5843 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/call_blender_subprocess_methods.py
--rw-r--r--   0        0        0     1876 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/export_to_blender.py
--rw-r--r--   0        0        0     1445 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/core_processes/post_process_skeleton_data/__init__.py
--rw-r--r--   0        0        0     6228 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/core_processes/post_process_skeleton_data/estimate_skeleton_segment_lengths.py
--rw-r--r--   0        0        0    44329 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/core_processes/post_process_skeleton_data/gap_fill_filter_and_origin_align_skeleton_data.py
--rw-r--r--   0        0        0     1389 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/core_processes/process_motion_capture_videos/__init__.py
--rw-r--r--   0        0        0     8240 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/actions_and_menus/__init__.py
--rw-r--r--   0        0        0     3564 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/actions_and_menus/actions.py
--rw-r--r--   0        0        0     2586 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/actions_and_menus/menu_bar.py
--rw-r--r--   0        0        0     1630 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/freemocap_main.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/main_window/__init__.py
--rw-r--r--   0        0        0    23348 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/main_window/freemocap_main_window.py
--rw-r--r--   0        0        0    13143 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/AMOLED.qss
--rw-r--r--   0        0        0     7364 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/ElegantDark.qss
--rw-r--r--   0        0        0     7431 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/FunkyTown.qss
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/__init__.py
--rw-r--r--   0        0        0      360 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/compile_scss_to_css.py
--rw-r--r--   0        0        0     1329 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/css_file_watcher.py
--rw-r--r--   0        0        0     2499 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.css
--rw-r--r--   0        0        0     3273 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.scss
--rw-r--r--   0        0        0     1479 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/scss_file_watcher.py
--rw-r--r--   0        0        0      303 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/set_css_style_sheet.py
--rw-r--r--   0        0        0      136 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/stylesheet-branch-more.png
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/utilities/__init__.py
--rw-r--r--   0        0        0      192 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/utilities/get_qt_app.py
--rw-r--r--   0        0        0      856 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/__init__.py
--rw-r--r--   0        0        0     6852 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/active_recording_widget.py
--rw-r--r--   0        0        0     6590 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/camera_controller_group_box.py
--rw-r--r--   0        0        0     3265 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/central_tab_widget.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/__init__.py
--rw-r--r--   0        0        0    13441 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py
--rw-r--r--   0        0        0     2328 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/__init__.py
--rw-r--r--   0        0        0        2 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_3d_triangulation_parameter_group.py
--rw-r--r--   0        0        0     7510 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py
--rw-r--r--   0        0        0     9808 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py
--rw-r--r--   0        0        0     4435 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/visualization_control_panel.py
--rw-r--r--   0        0        0     2312 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel_dock_widget.py
--rw-r--r--   0        0        0     6631 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/directory_view_widget.py
--rw-r--r--   0        0        0     4110 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/home_widget.py
--rw-r--r--   0        0        0     4736 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/import_videos_window.py
--rw-r--r--   0        0        0     3085 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/jupyter_console_widget.py
--rw-r--r--   0        0        0     2684 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/widgets/log_view_widget.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/workers/__init__.py
--rw-r--r--   0        0        0     2272 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py
--rw-r--r--   0        0        0     1489 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/parameter_info_models/__init__.py
--rw-r--r--   0        0        0     9779 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/parameter_info_models/recording_info_model.py
--rw-r--r--   0        0        0     1308 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/parameter_info_models/recording_processing_parameter_models.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/system/__init__.py
--rw-r--r--   0        0        0     1477 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/system/logging/configure_logging.py
--rw-r--r--   0        0        0     8232 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/system/paths_and_files_names.py
--rw-r--r--   0        0        0      251 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/system/start_file.py
--rw-r--r--   0        0        0        0 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/system/user_data/__init__.py
--rw-r--r--   0        0        0      863 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/system/user_data/pipedream_pings.py
--rw-r--r--   0        0        0     1817 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/tests/test_mediapipe_2d_data_shape.py
--rw-r--r--   0        0        0     2363 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/tests/test_mediapipe_3d_data_shape.py
--rw-r--r--   0        0        0      809 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/tests/test_synchronized_video_frame_counts.py
--rw-r--r--   0        0        0      130 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/tests/test_test.py
--rw-r--r--   0        0        0     1276 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/tests/test_total_body_center_of_mass_data_shape.py
--rw-r--r--   0        0        0      743 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0      645 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/utilities/get_video_paths.py
--rw-r--r--   0        0        0      447 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/utilities/project_3d_data_to_z_plane.py
--rw-r--r--   0        0        0      497 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/utilities/rotate_by_90_degrees_around_x_axis.py
--rw-r--r--   0        0        0      513 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/freemocap/utilities/save_dictionary_to_json.py
--rw-r--r--   0        0        0     5252 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/ipython_jupyter_notebooks/batch_process_session_folders.ipynb
--rw-r--r--   0        0        0    21821 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb
--rw-r--r--   0        0        0    13464 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb
--rw-r--r--   0        0        0     3594 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/pyproject.toml
--rw-r--r--   0        0        0      300 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/requirements.txt
--rw-r--r--   0        0        0       50 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/setup.py
--rw-r--r--   0        0        0     1045 2023-03-28 18:48:59.872993 freemocap-1.0.6rc0/src/gui/main/main.py
--rw-r--r--   0        0        0     7614 1970-01-01 00:00:00.000000 freemocap-1.0.6rc0/PKG-INFO
+-rwxr-xr-x   0        0        0      492 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/.github/dependabot.yml
+-rw-r--r--   0        0        0      423 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1083 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rwxr-xr-x   0        0        0     1094 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2215 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/.gitignore
+-rw-r--r--   0        0        0      229 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      418 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/CITATION.cff
+-rw-r--r--   0        0        0      327 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/CODEOWNERS
+-rw-r--r--   0        0        0     3348 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/LICENSE
+-rw-r--r--   0        0        0      234 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/MANIFEST.in
+-rw-r--r--   0        0        0     4868 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/README.md
+-rw-r--r--   0        0        0    44734 2023-04-20 13:48:04.306031 freemocap-1.0.7rc0/assets/charuco/charuco_board_image.png
+-rw-r--r--   0        0        0   332173 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/assets/charuco/charuco_board_image_highRes.png
+-rw-r--r--   0        0        0    26366 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/assets/logo/freemocap-logo-black-border.svg
+-rw-r--r--   0        0        0   124841 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png
+-rw-r--r--   0        0        0    99678 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/assets/logo/freemocap_skelly_logo.ico
+-rwxr-xr-x   0        0        0      607 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/bin/builds/install_packages
+-rwxr-xr-x   0        0        0      288 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/bin/installer.sh
+-rwxr-xr-x   0        0        0      278 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/bin/linux/build.sh
+-rwxr-xr-x   0        0        0      161 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/bin/linux/run_uvicorn_server.sh
+-rwxr-xr-x   0        0        0      381 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/bin/linux/run_web_server.sh
+-rwxr-xr-x   0        0        0      118 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/bin/linux/shell.sh
+-rwxr-xr-x   0        0        0      104 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/bin/linux/test.sh
+-rwxr-xr-x   0        0        0       71 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/bin/linux/up.sh
+-rw-r--r--   0        0        0      410 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/bin/windows/installChocolatey.cmd
+-rw-r--r--   0        0        0      112 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/bin/windows/run_web_server.cmd
+-rw-r--r--   0        0        0      331 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/experimental/freemocap-ui/.gitignore
+-rw-r--r--   0        0        0     2359 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/experimental/freemocap-ui/README.md
+-rw-r--r--   0        0        0      734 2023-04-20 13:48:04.310031 freemocap-1.0.7rc0/experimental/freemocap-ui/config-overrides.js
+-rw-r--r--   0        0        0  1263565 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/package-lock.json
+-rw-r--r--   0        0        0     2548 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/package.json
+-rw-r--r--   0        0        0     3585 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/public/favicon.ico
+-rw-r--r--   0        0        0     1963 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/public/index.html
+-rw-r--r--   0        0        0     4153 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/public/logo192.png
+-rw-r--r--   0        0        0    12066 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/public/logo512.png
+-rw-r--r--   0        0        0      492 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/public/manifest.json
+-rw-r--r--   0        0        0       67 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/public/robots.txt
+-rw-r--r--   0        0        0       33 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/scripts/cert.sh
+-rw-r--r--   0        0        0      582 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/App.css
+-rw-r--r--   0        0        0      366 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/App.test.tsx
+-rw-r--r--   0        0        0      193 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/App.tsx
+-rw-r--r--   0        0        0      346 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/app/hooks.ts
+-rw-r--r--   0        0        0      445 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/app/store.ts
+-rw-r--r--   0        0        0      941 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/components/start-stop-process.tsx
+-rw-r--r--   0        0        0      475 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/components/webcam/LivePreview.tsx
+-rw-r--r--   0        0        0     1057 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx
+-rw-r--r--   0        0        0      104 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/components/webcam/webcam.tsx
+-rw-r--r--   0        0        0      610 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx
+-rw-r--r--   0        0        0     1291 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/features/counter/Counter.module.css
+-rw-r--r--   0        0        0     1758 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/features/counter/Counter.tsx
+-rw-r--r--   0        0        0      214 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/features/counter/counterAPI.ts
+-rw-r--r--   0        0        0      842 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts
+-rw-r--r--   0        0        0     2983 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/features/counter/counterSlice.ts
+-rw-r--r--   0        0        0      291 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/hooks/use-device-stream.ts
+-rw-r--r--   0        0        0      791 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx
+-rw-r--r--   0        0        0      366 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/index.css
+-rw-r--r--   0        0        0      623 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/index.tsx
+-rw-r--r--   0        0        0      417 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/Copyright.tsx
+-rw-r--r--   0        0        0     1625 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/Header.tsx
+-rw-r--r--   0        0        0     2353 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/Navigator.tsx
+-rw-r--r--   0        0        0     4303 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/Paperbase.tsx
+-rw-r--r--   0        0        0      394 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/content/BaseContent.tsx
+-rw-r--r--   0        0        0      273 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/content/BasePaper.tsx
+-rw-r--r--   0        0        0     1943 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/content/Content.tsx
+-rw-r--r--   0        0        0      737 2023-04-20 13:48:04.318031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/routing/router.tsx
+-rw-r--r--   0        0        0     1122 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/logo.svg
+-rw-r--r--   0        0        0       40 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/react-app-env.d.ts
+-rw-r--r--   0        0        0     5290 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/serviceWorker.ts
+-rw-r--r--   0        0        0      629 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/services/Capture.tsx
+-rw-r--r--   0        0        0      370 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/services/Record.ts
+-rw-r--r--   0        0        0      198 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/services/cam.ts
+-rw-r--r--   0        0        0      325 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/services/download.ts
+-rw-r--r--   0        0        0     1717 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/services/frame-capture.tsx
+-rw-r--r--   0        0        0      497 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/services/image_send_worker.ts
+-rw-r--r--   0        0        0     2044 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/services/recorder.ts
+-rw-r--r--   0        0        0     1560 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/services/supported_recorder.ts
+-rw-r--r--   0        0        0      254 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/setupTests.ts
+-rw-r--r--   0        0        0     1384 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/Capture.tsx
+-rw-r--r--   0        0        0      733 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/Config.tsx
+-rw-r--r--   0        0        0     1153 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/SessionWorkflow.tsx
+-rw-r--r--   0        0        0      109 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/ShowCameras.tsx
+-rw-r--r--   0        0        0      124 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/UserConfig.tsx
+-rw-r--r--   0        0        0      965 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx
+-rw-r--r--   0        0        0      792 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx
+-rw-r--r--   0        0        0     1023 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx
+-rw-r--r--   0        0        0     1976 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx
+-rw-r--r--   0        0        0      599 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/freemocap-ui/tsconfig.json
+-rw-r--r--   0        0        0      789 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/python_scratch/qt_drag_and_drop.py
+-rw-r--r--   0        0        0     1609 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/experimental/tool_bar.py
+-rw-r--r--   0        0        0     1821 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/__init__.py
+-rw-r--r--   0        0        0      888 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/__init__.py
+-rw-r--r--   0        0        0     6700 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py
+-rw-r--r--   0        0        0    60000 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py
+-rw-r--r--   0        0        0     2613 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/__init__.py
+-rw-r--r--   0        0        0     1504 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py
+-rw-r--r--   0        0        0       36 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/default_charuco_square_size.py
+-rw-r--r--   0        0        0     1177 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py
+-rw-r--r--   0        0        0     9539 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/detecting_things_in_2d_images/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/__init__.py
+-rw-r--r--   0        0        0    14641 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py
+-rw-r--r--   0        0        0    24623 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py
+-rw-r--r--   0        0        0     1752 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_names_and_connections.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/__init__.py
+-rw-r--r--   0        0        0    57980 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/alpha_freemocap_blender_megascript.py
+-rw-r--r--   0        0        0     1091 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/cgtinker_blendarmocap_load.py
+-rw-r--r--   0        0        0    37868 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/freemocap_blender_megascript_take2.py
+-rw-r--r--   0        0        0     5843 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/call_blender_subprocess_methods.py
+-rw-r--r--   0        0        0     1876 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/export_to_blender.py
+-rw-r--r--   0        0        0     1445 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/post_process_skeleton_data/__init__.py
+-rw-r--r--   0        0        0     6228 2023-04-20 13:48:04.322031 freemocap-1.0.7rc0/freemocap/core_processes/post_process_skeleton_data/estimate_skeleton_segment_lengths.py
+-rw-r--r--   0        0        0    44609 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/core_processes/post_process_skeleton_data/gap_fill_filter_and_origin_align_skeleton_data.py
+-rw-r--r--   0        0        0     1389 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/core_processes/process_motion_capture_videos/__init__.py
+-rw-r--r--   0        0        0     8240 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/actions_and_menus/__init__.py
+-rw-r--r--   0        0        0     4270 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/actions_and_menus/actions.py
+-rw-r--r--   0        0        0     2379 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/actions_and_menus/menu_bar.py
+-rw-r--r--   0        0        0     1630 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/freemocap_main.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/main_window/__init__.py
+-rw-r--r--   0        0        0    23251 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/main_window/freemocap_main_window.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/style_sheet/__init__.py
+-rw-r--r--   0        0        0      360 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/style_sheet/compile_scss_to_css.py
+-rw-r--r--   0        0        0     1329 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/style_sheet/css_file_watcher.py
+-rw-r--r--   0        0        0     3260 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.scss
+-rw-r--r--   0        0        0     1479 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/style_sheet/scss_file_watcher.py
+-rw-r--r--   0        0        0      303 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/style_sheet/set_css_style_sheet.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/utilities/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/utilities/get_qt_app.py
+-rw-r--r--   0        0        0      856 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/__init__.py
+-rw-r--r--   0        0        0     6852 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/active_recording_widget.py
+-rw-r--r--   0        0        0     6901 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/camera_controller_group_box.py
+-rw-r--r--   0        0        0     3265 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/central_tab_widget.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/__init__.py
+-rw-r--r--   0        0        0    13441 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py
+-rw-r--r--   0        0        0     2328 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/__init__.py
+-rw-r--r--   0        0        0        2 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_3d_triangulation_parameter_group.py
+-rw-r--r--   0        0        0     7510 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py
+-rw-r--r--   0        0        0     9808 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py
+-rw-r--r--   0        0        0     4435 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/visualization_control_panel.py
+-rw-r--r--   0        0        0     2312 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel_dock_widget.py
+-rw-r--r--   0        0        0     6631 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/directory_view_widget.py
+-rw-r--r--   0        0        0     4427 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/home_widget.py
+-rw-r--r--   0        0        0     4736 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/import_videos_window.py
+-rw-r--r--   0        0        0     3085 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/jupyter_console_widget.py
+-rw-r--r--   0        0        0     2684 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/widgets/log_view_widget.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/workers/__init__.py
+-rw-r--r--   0        0        0     2272 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py
+-rw-r--r--   0        0        0     1489 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/parameter_info_models/__init__.py
+-rw-r--r--   0        0        0     9731 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/parameter_info_models/recording_info_model.py
+-rw-r--r--   0        0        0     1308 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/parameter_info_models/recording_processing_parameter_models.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/system/__init__.py
+-rw-r--r--   0        0        0     1477 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/system/logging/configure_logging.py
+-rw-r--r--   0        0        0     8232 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/system/paths_and_files_names.py
+-rw-r--r--   0        0        0      251 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/system/start_file.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/system/user_data/__init__.py
+-rw-r--r--   0        0        0      863 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/system/user_data/pipedream_pings.py
+-rw-r--r--   0        0        0     1817 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/tests/test_mediapipe_2d_data_shape.py
+-rw-r--r--   0        0        0     2363 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/tests/test_mediapipe_3d_data_shape.py
+-rw-r--r--   0        0        0      809 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/tests/test_synchronized_video_frame_counts.py
+-rw-r--r--   0        0        0      130 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/tests/test_test.py
+-rw-r--r--   0        0        0     1276 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/tests/test_total_body_center_of_mass_data_shape.py
+-rw-r--r--   0        0        0      743 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0      645 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/utilities/get_video_paths.py
+-rw-r--r--   0        0        0      447 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/utilities/project_3d_data_to_z_plane.py
+-rw-r--r--   0        0        0      497 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/utilities/rotate_by_90_degrees_around_x_axis.py
+-rw-r--r--   0        0        0      513 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/freemocap/utilities/save_dictionary_to_json.py
+-rw-r--r--   0        0        0     5252 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/ipython_jupyter_notebooks/batch_process_session_folders.ipynb
+-rw-r--r--   0        0        0    21821 2023-04-20 13:48:04.326031 freemocap-1.0.7rc0/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb
+-rw-r--r--   0        0        0    13464 2023-04-20 13:48:04.330031 freemocap-1.0.7rc0/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb
+-rw-r--r--   0        0        0     3594 2023-04-20 13:48:04.330031 freemocap-1.0.7rc0/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-20 13:48:04.330031 freemocap-1.0.7rc0/requirements.txt
+-rw-r--r--   0        0        0       50 2023-04-20 13:48:04.330031 freemocap-1.0.7rc0/setup.py
+-rw-r--r--   0        0        0     1045 2023-04-20 13:48:04.330031 freemocap-1.0.7rc0/src/gui/main/main.py
+-rw-r--r--   0        0        0     7614 1970-01-01 00:00:00.000000 freemocap-1.0.7rc0/PKG-INFO
```

### Comparing `freemocap-1.0.6rc0/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `freemocap-1.0.7rc0/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/.github/workflows/python-testing.yml` & `freemocap-1.0.7rc0/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/.gitignore` & `freemocap-1.0.7rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/CONTRIBUTING.md` & `freemocap-1.0.7rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/LICENSE` & `freemocap-1.0.7rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/README.md` & `freemocap-1.0.7rc0/README.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/assets/charuco/charuco_board_image.png` & `freemocap-1.0.7rc0/assets/charuco/charuco_board_image.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/assets/charuco/charuco_board_image_highRes.png` & `freemocap-1.0.7rc0/assets/charuco/charuco_board_image_highRes.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/assets/logo/freemocap-logo-black-border.svg` & `freemocap-1.0.7rc0/assets/logo/freemocap-logo-black-border.svg`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png` & `freemocap-1.0.7rc0/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/assets/logo/freemocap_skelly_logo.ico` & `freemocap-1.0.7rc0/assets/logo/freemocap_skelly_logo.ico`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/bin/builds/install_packages` & `freemocap-1.0.7rc0/bin/builds/install_packages`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/README.md` & `freemocap-1.0.7rc0/experimental/freemocap-ui/README.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/config-overrides.js` & `freemocap-1.0.7rc0/experimental/freemocap-ui/config-overrides.js`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/package-lock.json` & `freemocap-1.0.7rc0/experimental/freemocap-ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/package.json` & `freemocap-1.0.7rc0/experimental/freemocap-ui/package.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/public/favicon.ico` & `freemocap-1.0.7rc0/experimental/freemocap-ui/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/public/index.html` & `freemocap-1.0.7rc0/experimental/freemocap-ui/public/index.html`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/public/logo192.png` & `freemocap-1.0.7rc0/experimental/freemocap-ui/public/logo192.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/public/logo512.png` & `freemocap-1.0.7rc0/experimental/freemocap-ui/public/logo512.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/App.css` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/App.css`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/components/start-stop-process.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/components/start-stop-process.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/features/counter/Counter.module.css` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/features/counter/Counter.module.css`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/features/counter/Counter.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/features/counter/Counter.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/features/counter/counterSlice.ts` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/features/counter/counterSlice.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/index.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/Header.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/Header.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/Navigator.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/Navigator.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/Paperbase.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/Paperbase.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/content/Content.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/content/Content.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/layout/routing/router.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/layout/routing/router.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/logo.svg` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/logo.svg`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/serviceWorker.ts` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/serviceWorker.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/services/Capture.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/services/Capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/services/frame-capture.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/services/frame-capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/services/recorder.ts` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/services/recorder.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/services/supported_recorder.ts` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/services/supported_recorder.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/Capture.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/Capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/Config.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/Config.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/SessionWorkflow.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/SessionWorkflow.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx` & `freemocap-1.0.7rc0/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/freemocap-ui/tsconfig.json` & `freemocap-1.0.7rc0/experimental/freemocap-ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/python_scratch/qt_drag_and_drop.py` & `freemocap-1.0.7rc0/experimental/python_scratch/qt_drag_and_drop.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/experimental/tool_bar.py` & `freemocap-1.0.7rc0/experimental/tool_bar.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/__init__.py` & `freemocap-1.0.7rc0/freemocap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for freemocap"""
 
 __author__ = """Skelly FreeMoCap"""
 __email__ = "info@freemocap.org"
-__version__ = "v1.0.6-rc"
+__version__ = "v1.0.7-rc"
 __description__ = "A free and open source markerless motion capture system for everyone 💀✨"
 
 __package_name__ = "freemocap"
 __repo_url__ = f"https://github.com/freemocap/{__package_name__}/"
 __repo_issues_url__ = f"{__repo_url__}issues"
 
 import sys
```

### Comparing `freemocap-1.0.6rc0/freemocap/__main__.py` & `freemocap-1.0.7rc0/freemocap/__main__.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py` & `freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py` & `freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py` & `freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py` & `freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py` & `freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py` & `freemocap-1.0.7rc0/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py` & `freemocap-1.0.7rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py` & `freemocap-1.0.7rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_names_and_connections.py` & `freemocap-1.0.7rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_names_and_connections.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/alpha_freemocap_blender_megascript.py` & `freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/alpha_freemocap_blender_megascript.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/cgtinker_blendarmocap_load.py` & `freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/cgtinker_blendarmocap_load.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/freemocap_blender_megascript_take2.py` & `freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/freemocap_blender_megascript_take2.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/call_blender_subprocess_methods.py` & `freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/call_blender_subprocess_methods.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/export_to_blender.py` & `freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/export_to_blender.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py` & `freemocap-1.0.7rc0/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/post_process_skeleton_data/estimate_skeleton_segment_lengths.py` & `freemocap-1.0.7rc0/freemocap/core_processes/post_process_skeleton_data/estimate_skeleton_segment_lengths.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/post_process_skeleton_data/gap_fill_filter_and_origin_align_skeleton_data.py` & `freemocap-1.0.7rc0/freemocap/core_processes/post_process_skeleton_data/gap_fill_filter_and_origin_align_skeleton_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,18 +74,18 @@
         trajectory_frame_xyz = inputData_frame_marker_xyz[:, marker_number, :]
 
         if marker_number < NUMBER_OF_MEDIAPIPE_BODY_MARKERS:
             df = pd.DataFrame(trajectory_frame_xyz).interpolate(method="linear", axis=0)
             df.fillna(method="bfill", axis=0, inplace=True)
             df.fillna(method="ffill", axis=0, inplace=True)
 
-            if np.any(np.isnan(df.to_numpy())):
-                raise ValueError("Nans still present after interpolation")
-            if np.any(np.isinf(df.to_numpy())):
-                raise ValueError("Infs still present after interpolation")
+            # if np.any(np.isnan(df.to_numpy())):
+            #     raise ValueError("Nans still present after interpolation")
+            # if np.any(np.isinf(df.to_numpy())):
+            #     raise ValueError("Infs still present after interpolation")
 
             interpolatedData_frame_marker_xyz[:, marker_number, :] = df.to_numpy()
 
     return interpolatedData_frame_marker_xyz
 
 
 # %%
@@ -95,29 +95,33 @@
     normal_cutoff = cutoff / nyquist_freq
     # Get the filter coefficients
     b, a = signal.butter(order, normal_cutoff, btype="low", analog=False)
     y = signal.filtfilt(b, a, data)
     return y
 
 
-def butterworth_filter_skeleton(skeleton_3d_data, cutoff, sampling_rate, order):
+def butterworth_filter_skeleton(skeleton_frame_marker_xyz, cutoff, sampling_rate, order):
     """Take in a 3d skeleton numpy array and calculate_center_of_mass a low pass butterworth filter on each marker in the data"""
 
-    butterworth_filtered_data = skeleton_3d_data.copy()
+    butterworth_filtered_data = skeleton_frame_marker_xyz.copy()
 
     for marker_number in range(NUMBER_OF_MEDIAPIPE_BODY_MARKERS):
-        for dimension in range(3):
+        trajectory_xyz = skeleton_frame_marker_xyz[:, marker_number, :]
+        if np.any(np.isnan(trajectory_xyz)):
+            logger.warning(f"Trajectory number {marker_number} has nans, skipping butterworth filter")
+            continue
+        for dimension in range(trajectory_xyz.shape[1]):
             butterworth_filtered_data[:, marker_number, dimension] = butterworth_lowpass_zerolag_filter(
-                skeleton_3d_data[:, marker_number, dimension],
+                trajectory_xyz[:,dimension],
                 cutoff,
                 sampling_rate,
                 order,
             )
 
-    assert skeleton_3d_data.shape == butterworth_filtered_data.shape
+    assert skeleton_frame_marker_xyz.shape == butterworth_filtered_data.shape
 
     return butterworth_filtered_data
 
 
 # %%
 def find_velocity_values_within_limit(skeleton_velocity_data, velocity_limit):
     """
```

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py` & `freemocap-1.0.7rc0/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py` & `freemocap-1.0.7rc0/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/actions_and_menus/actions.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/actions_and_menus/actions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-from PyQt6.QtGui import QAction
+from PyQt6.QtGui import QAction, QDesktopServices
+from PyQt6.QtCore import QUrl
 
 
 CREATE_NEW_RECORDING_ACTION_NAME = "New Recording"
 LOAD_MOST_RECENT_RECORDING_ACTION_NAME = "Load Most Recent Recording"
 LOAD_RECORDING_ACTION_NAME = "Load Recording"
 IMPORT_VIDEOS_ACTION_NAME = "Import Videos"
 KILL_THREADS_AND_PROCESSES_ACTION_NAME = "Kill Threads and Processes"
 REBOOT_GUI_ACTION_NAME = "Reboot GUI"
 EXIT_ACTION_NAME = "Exit"
 
+OPEN_DOCS_ACTION_NAME = "Open Documentation"
+FREEMOCAP_FOUNDATION_ACTION_NAME = "Freemocap Foundation"
+
+DONATE_ACTION_NAME = "Donate to Freemocap"
+
 
 class Actions:
     def __init__(self, freemocap_main_window):
         # File
         self.create_new_recording_action = QAction(CREATE_NEW_RECORDING_ACTION_NAME, parent=freemocap_main_window)
         self.create_new_recording_action.setShortcut("Ctrl+N")
         self.create_new_recording_action.triggered.connect(freemocap_main_window.handle_start_new_session_action)
@@ -45,27 +51,31 @@
             freemocap_main_window.kill_running_threads_and_processes
         )
 
         self.exit_action = QAction("E&xit", parent=freemocap_main_window)
         self.exit_action.setShortcut("Ctrl+Q")
         self.exit_action.triggered.connect(freemocap_main_window.close)
 
-        # # Help
-        # open_docs_action = QAction("Open  &Documentation", parent=main_window)
-        # about_us_action = QAction("&About Us", parent=main_window)
-        #
+        # Help
+        self.open_docs_action = QAction(OPEN_DOCS_ACTION_NAME, parent=freemocap_main_window)
+        self.open_docs_action.triggered.connect(lambda: QDesktopServices.openUrl(QUrl("https://freemocap.readthedocs.io/en/latest/")))
+        
+        self.freemocap_foundation_action = QAction(FREEMOCAP_FOUNDATION_ACTION_NAME, parent=freemocap_main_window)
+        self.freemocap_foundation_action.triggered.connect(lambda: QDesktopServices.openUrl(QUrl("https://freemocap.org/about-us.html")))
+
         # # Navigation
         # show_camera_control_panel_action = QAction("&1 - Show Camera Control Panel", parent=main_window)
         # show_camera_control_panel_action.setShortcut("Ctrl+1")
         #
         # show_calibrate_capture_volume_panel_action = QAction(
         #     "&2 - Show Calibrate Capture Volume Panel", parent=main_window
         # )
         # show_calibrate_capture_volume_panel_action.setShortcut("Ctrl+2")
         #
         # show_motion_capture_videos_panel_action = QAction("&3 - Show Motion Capture Videos Panel", parent=main_window)
         # show_motion_capture_videos_panel_action.setShortcut("Ctrl+3")
         #
-        # # Support
-        # donate_action = QAction("&Donate", parent=main_window)
-        # send_usage_statistics_action = QAction("Send &User Statistics", parent=main_window)
-        # user_survey_action = QAction("&User Survey", parent=main_window)
+        # Support
+        self.donate_action = QAction(DONATE_ACTION_NAME, parent=freemocap_main_window)
+        self.donate_action.triggered.connect(lambda: QDesktopServices.openUrl(QUrl("https://freemocap.org/about-us.html#donate")))
+        # self.send_usage_statistics_action = QAction("Send &User Statistics", parent=freemocap_main_window)
+        # self.user_survey_action = QAction("&User Survey", parent=freemocap_main_window)
```

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/actions_and_menus/menu_bar.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/actions_and_menus/menu_bar.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from PyQt6.QtWidgets import QMainWindow, QMenuBar
-
 from freemocap.gui.qt.actions_and_menus.actions import Actions
 
 
 class MenuBar(QMenuBar):
     def __init__(self, actions: Actions, parent: QMainWindow = None):
         super().__init__(parent=parent)
 
@@ -29,32 +28,26 @@
         # navigation_menu = QMenu("Na&vigation", parent=self)
         # self.addMenu(navigation_menu)
         #
         # navigation_menu.addAction(self._show_camera_control_panel_action)
         # navigation_menu.addAction(self._show_calibrate_capture_volume_panel_action)
         # navigation_menu.addAction(self._show_motion_capture_videos_panel_action)
         #
-        # # help menu
-        # help_menu = QMenu("&Help", parent=self)
-        # self.addMenu(help_menu)
-        # help_menu.setEnabled(False)
-        #
-        # help_menu.addAction(self._open_docs_action)
-        # help_menu.addAction(self._about_us_action)
-        #
-        # # support menu
-        # support_menu = QMenu(
-        #     "\U00002665 &Support the FreeMoCap Project", parent=self
-        # )
-        # support_menu.setEnabled(False)
-        # self.addMenu(support_menu)
+        # help menu
+        help_menu = self.addMenu("&Help")
+
+        help_menu.addAction(actions.open_docs_action)
+        help_menu.addAction(actions.freemocap_foundation_action)
         #
-        # support_menu.addAction(self._donate_action)
-        # support_menu.addAction(self._send_usage_statistics_action)
-        # support_menu.addAction(self._user_survey_action)
+        # support menu
+        support_menu = self.addMenu("&Support the Freemocap Project")
+   
+        support_menu.addAction(actions.donate_action)
+        # support_menu.addAction(actions.send_usage_statistics_action)
+        # support_menu.addAction(actions.user_survey_action)
 
 
 if __name__ == "__main__":
     import sys
     from PyQt6.QtWidgets import QApplication, QLabel
 
     app = QApplication(sys.argv)
```

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/freemocap_main.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/freemocap_main.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/main_window/freemocap_main_window.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/main_window/freemocap_main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         self.setWindowTitle("freemocap \U0001F480 \U00002728")
 
         dummy_widget = QWidget()
         self._layout = QHBoxLayout()
         dummy_widget.setLayout(self._layout)
         self.setCentralWidget(dummy_widget)
 
-        self._css_file_watcher = self._set_up_stylesheet()
+        self._scss_file_watcher = self._set_up_stylesheet()
 
         self._freemocap_data_folder_path = freemocap_data_folder_path
         self._pipedream_pings = pipedream_pings
 
         self._kill_thread_event = multiprocessing.Event()
 
         self._active_recording_info_widget = ActiveRecordingInfoWidget(parent=self)
@@ -199,16 +199,15 @@
                 self._controller_group_box.update_recording_name_string()
         except Exception as e:
             logger.exception(e)
 
     def _set_up_stylesheet(self):
         apply_css_style_sheet(self, get_css_stylesheet_path())
         scss_file_watcher = SCSSFileWatcher(path_to_scss_file=get_scss_stylesheet_path(), path_to_css_file=get_css_stylesheet_path(), parent=self)
-        css_file_watcher = CSSFileWatcher(path_to_css_file=get_css_stylesheet_path(), parent=self)
-        return css_file_watcher
+        return scss_file_watcher
 
     def _create_new_synchronized_videos_folder(self) -> str:
         new_recording_folder_path = self._controller_group_box.get_new_recording_path()
         logger.info(f"Creating new recording folder at: {new_recording_folder_path}")
         self._active_recording_info_widget.set_active_recording(recording_folder_path=new_recording_folder_path)
         return self._active_recording_info_widget.active_recording_info.synchronized_videos_folder_path
```

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/css_file_watcher.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/style_sheet/css_file_watcher.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.css` & `freemocap-1.0.7rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.scss`

 * *Files 27% similar despite different names*

```diff
@@ -1,127 +1,168 @@
- /* If you want to update the appearance of the GUI, please make changes to the `qt_stylesheet.scss` file. */
-* {
-  font-family: "Dosis", sans-serif;
-  /*font-size: 12px;*/
-  color: #333333; }
+$dark-charcoal: #333333;
+$skelly-bone-blue: #a4d6d9;
+$cadet-skelly: cadetblue;
+$laser-red: #d95158;
+$disabled-laser-red: #8c5454;
+$freemocap-green: #365d5f;
+$freemocap-dark-green: #254342;
+$button-blue: #29394a;
+$tree-heading-blue: #5793cf;
+$disabled-button-blue: #687e90;
+$tree-primary: #7983b1;
+$tree-secondary: #a3b1ed;
+$plain-white: white;
+$plain-black: black;
 
-QGroupBox {
-  border: 1px solid #254342;
-  border-radius: 4px;
-  margin-top: 10px;
-  font-weight: bold; }
+* {
+    font-family: "Dosis", sans-serif;
+    /*font-size: 12px;*/
+    color: $dark-charcoal;
+}
 
 QGroupBox {
-  background-color: #a4d6d9; }
+    border: 1px solid $freemocap-dark-green;
+    border-radius: 4px;
+    margin-top: 10px;
+    font-weight: bold;
+    background-color: $skelly-bone-blue;
+}
 
 QStatusBar {
-  color: #365d5f; }
+    color: $freemocap-green;
+}
 
 QMainWindow {
-  background-color: #365d5f; }
+    background-color: $freemocap-green;
+}
 
 QTabWidget::pane {
-  border: 1px solid white;
-  top: 1px;
-  background: cadetblue; }
+    border: 1px solid $plain-white;
+    top: 1px;
+    background: $cadet-skelly;
+}
 
 QTabBar::tab {
-  border: 1px solid;
-  padding: 5px;
-  color: #365d5f;
-  border-top-left-radius: 20px;
-  border-top-right-radius: 5px;
-  /*min-width: 200px;*/ }
+    border: 1px solid;
+    padding: 5px;
+    color: $freemocap-green;
+    border-top-left-radius: 20px;
+    border-top-right-radius: 5px;
+    /*min-width: 200px;*/
+}
 
 QTabBar::tab {
-  background: white;
-  border-color: #365d5f;
-  margin-bottom: -5px;
-  font-weight: bolder;
-  font-size: 16px; }
+    background: $plain-white;
+    border-color: $freemocap-green;
+    margin-bottom: -5px;
+    font-weight: bolder;
+    font-size: 16px;
+}
 
 QTabBar::tab:selected {
-  background: #365d5f;
-  color: white;
-  border-color: white; }
+    background: $freemocap-green;
+    color: $plain-white;
+    border-color: $plain-white;
+}
 
 QPushButton {
-  font-weight: bold;
-  border-radius: 4px;
-  border: 2px solid #29394a;
-  background-color: #29394a;
-  color: white; }
+    font-weight: bold;
+    border-radius: 4px;
+    border: 2px solid $button-blue;
+    background-color: $button-blue;
+    color: $plain-white;
+}
 
 QPushButton:disabled {
-  background-color: #7983b1;
-  border: 1px solid #7983b1;
-  color: #a4d6d9; }
+    background-color: $tree-primary;
+    border: 1px solid $tree-primary;
+    color: $skelly-bone-blue;
+}
 
 QPushButton:hover {
-  border: 3px solid white; }
+    border: 3px solid $plain-white;
+}
 
 QPushButton#start_recording_button {
-  font-size: 18px;
-  background-color: #d95158; }
-
+    font-size: 18px;
+    background-color: $laser-red;
+}
 QPushButton#start_recording_button:disabled {
-  background-color: #8c5454; }
+    background-color: $disabled-laser-red;
+}
 
 QPushButton#stop_recording_button {
-  font-size: 18px; }
+    font-size: 18px;
 
+}
 QPushButton#stop_recording_button:enabled {
-  /*font-size: 24px;*/
-  border: 3px solid #d95158; }
+    /*font-size: 24px;*/
+    border: 3px solid $laser-red;
+}
 
 WelcomeScreenButton {
-  border: 2px solid #333333;
-  background-color: #365d5f;
-  color: white;
-  font-size: 24px;
-  border-radius: 20px;
-  padding: 10px; }
-
-WelcomeScreenButton[recommended_next=true] {
-  background-color: #d95158;
-  color: white; }
+    border: 2px solid $dark-charcoal;
+    background-color: $freemocap-green;
+    color: $plain-white;
+    font-size: 24px;
+    border-radius: 20px;
+    padding: 10px;
+}
+
+WelcomeScreenButton[recommended_next = true] {
+    background-color: $laser-red;
+    color: $plain-white;
+}
 
 QLabel {
-  font-size: 14px;
-  color: #333333; }
+    font-size: 14px;
+    color: $dark-charcoal;
+
+    QTreeView & {
+        color: $plain-black;
+  }
+}
 
 QLabel:disabled {
-  color: #a4d6d9; }
+    color: $skelly-bone-blue
+}
 
 QLineEdit {
-  border: 1px solid #29394a;
-  border-radius: 4px;
-  padding: 0 8px;
-  color: #333333; }
-
+    border: 1px solid $button-blue;
+    border-radius: 4px;
+    padding: 0 8px;
+    color: $dark-charcoal;
+    background-color: $plain-white;
+}
 QLineEdit:disabled {
-  color: #333333;
-  background-color: #29394a; }
+    color: $dark-charcoal;
+    background-color: $disabled-button-blue;
+}
 
 QTreeView {
-  background-color: #7983b1;
-  alternate-background-color: #a3b1ed;
-  color: white;
-  font-weight: bold;
-  font-family: "Roboto", sans-serif;
-  font-size: 12px; }
+    background-color: $tree-primary;
+    color: $plain-black;
+    font-weight: bold;
+    font-family: "Roboto", sans-serif;
+    font-size: 12px;
+}
 
 QTreeView::item:has-children {
-  background-color: #29394a;
-  color: white; }
+    background-color: $tree-heading-blue;
+    color: $plain-white;
+}
 
 QTreeView::item:selected,
-QTreeView::item:hover {
-  background-color: white;
-  color: #333333; }
+    QTreeView::item:hover{
+    background-color: $plain-white;
+    color: $dark-charcoal;
+}
 
 LogViewWidget {
-  background-color: #254342;
-  color: white;
-  font-family: "Roboto", sans-serif;
-  font-size: 12px;
-  padding: 8px; }
+    background-color: $freemocap-dark-green;
+    color: $plain-white;
+    font-family: "Roboto", sans-serif;
+    font-size: 12px;
+    padding: 8px;
+}
+
+
```

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/style_sheet/scss_file_watcher.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/style_sheet/scss_file_watcher.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/active_recording_widget.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/active_recording_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/camera_controller_group_box.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/camera_controller_group_box.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         self._layout.addLayout(calibration_recording_option_layout)
 
         self._layout.addLayout(self._create_videos_will_save_to_layout())
 
         self._layout.addWidget(self._skellycam_controller)
 
     def _create_videos_will_save_to_layout(self):
+        vbox = QVBoxLayout()
+
         hbox = QHBoxLayout()
         self._recording_string_tag_line_edit = QLineEdit(parent=self)
         self._recording_string_tag_line_edit.setPlaceholderText("(Optional)")
 
         recording_string_tag_form_layout = QFormLayout(parent=self)
         recording_string_tag_form_layout.addRow("Tag:", self._recording_string_tag_line_edit)
         hbox.addLayout(recording_string_tag_form_layout)
@@ -61,15 +63,21 @@
         hbox.setAlignment(Qt.AlignmentFlag.AlignLeft)
         videos_will_save_to_label = QLabel("Videos will save to folder: ")
         videos_will_save_to_label.setStyleSheet("font-size: 10px;")
         hbox.addWidget(videos_will_save_to_label)
         self._recording_path_label = QLabel(f"{self.get_new_recording_path()}")
         self._recording_path_label.setStyleSheet("font-family: monospace; font-size: 10px;")
         hbox.addWidget(self._recording_path_label)
-        return hbox
+
+        vbox.addLayout(hbox)
+
+        lag_note_label = QLabel("NOTE: If you experience lag in your camera views, decrease the resolution and/or use fewer cameras.\nWe are working on a fix which should be done 'soon' (written: 2023-04-05)")
+        vbox.addWidget(lag_note_label)
+
+        return vbox
 
     def _create_mocap_recording_option_layout(self):
         hbox = QHBoxLayout()
         hbox.setAlignment(Qt.AlignmentFlag.AlignLeft)
 
         self._mocap_videos_radio_button = QRadioButton("Record Motion Capture Videos")
         hbox.addWidget(self._mocap_videos_radio_button)
```

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/central_tab_widget.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/central_tab_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel/visualization_control_panel.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel/visualization_control_panel.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/control_panel_dock_widget.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/control_panel_dock_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/directory_view_widget.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/directory_view_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/home_widget.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/home_widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -65,18 +65,23 @@
 
         self._import_videos_button = WelcomeScreenButton(f"{IMPORT_VIDEOS_ACTION_NAME}")
         self._import_videos_button.clicked.connect(actions.import_videos_action.trigger)
         self._layout.addWidget(self._import_videos_button, alignment=Qt.AlignmentFlag.AlignCenter)
 
         self._layout.addStretch(1)
 
-        send_pings_string = "Send ping to devs to let us know when you make a new session (being able to show that people are using this thing will help us get funding for this project :D )"
+        send_pings_string = "Send anonymous usage information"
         self._send_pings_checkbox = QCheckBox(send_pings_string)
         self._send_pings_checkbox.setChecked(True)
-        self._layout.addWidget(self._send_pings_checkbox)
+        self._layout.addWidget(self._send_pings_checkbox, alignment=Qt.AlignmentFlag.AlignCenter)
+
+        privacy_policy_link_string = '<a href="https://freemocap.readthedocs.io/en/latest/privacy_policy/" style="color: #333333;">Click here to view our privacy policy</a>'
+        self._privacy_policy_link = QLabel(privacy_policy_link_string)
+        self._privacy_policy_link.setOpenExternalLinks(True)
+        self._layout.addWidget(self._privacy_policy_link, alignment=Qt.AlignmentFlag.AlignCenter)
 
         self.style().polish(self)
 
     def _welcome_to_freemocap_title(self):
         # TO DO - this shouldn't be part of the `camera_view_panel` - it should be its own thing that gets swapped out on session start
         logger.info("Creating `welcome to freemocap` layout")
```

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/import_videos_window.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/import_videos_window.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/jupyter_console_widget.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/jupyter_console_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/widgets/log_view_widget.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/widgets/log_view_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py` & `freemocap-1.0.7rc0/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/parameter_info_models/recording_info_model.py` & `freemocap-1.0.7rc0/freemocap/parameter_info_models/recording_info_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,22 +206,24 @@
     def check_blender_file_status(self) -> bool:
         return Path(self.recording_info_model.blender_file_path).is_file()
 
     def check_calibration_toml_status(self) -> bool:
         return Path(self.recording_info_model.calibration_toml_path).is_file()
 
     def get_number_of_mp4s_in_synched_videos_directory(self) -> float:
+
         synchronized_directory_path = Path(self.recording_info_model.synchronized_videos_folder_path)
-        video_count = 0.0
 
+        if not synchronized_directory_path.exists():
+            return 0
+
+        video_count = 0
         for file in synchronized_directory_path.iterdir():
             if file.is_file() and file.suffix.lower() == '.mp4':
                 video_count += 1
-
-        logger.info(f"Number of `.mp4`'s in {self.recording_info_model.synchronized_videos_folder_path}: {video_count}")
         return video_count
 
     def get_number_of_frames_in_videos(self):
         timestamps_directory_path = Path(self.recording_info_model.synchronized_videos_folder_path) / "timestamps"
 
         if timestamps_directory_path.exists() and timestamps_directory_path.is_dir():
             frame_counts = {}
```

### Comparing `freemocap-1.0.6rc0/freemocap/parameter_info_models/recording_processing_parameter_models.py` & `freemocap-1.0.7rc0/freemocap/parameter_info_models/recording_processing_parameter_models.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/system/logging/configure_logging.py` & `freemocap-1.0.7rc0/freemocap/system/logging/configure_logging.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/system/paths_and_files_names.py` & `freemocap-1.0.7rc0/freemocap/system/paths_and_files_names.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/system/user_data/pipedream_pings.py` & `freemocap-1.0.7rc0/freemocap/system/user_data/pipedream_pings.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/tests/test_mediapipe_2d_data_shape.py` & `freemocap-1.0.7rc0/freemocap/tests/test_mediapipe_2d_data_shape.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/tests/test_mediapipe_3d_data_shape.py` & `freemocap-1.0.7rc0/freemocap/tests/test_mediapipe_3d_data_shape.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/tests/test_synchronized_video_frame_counts.py` & `freemocap-1.0.7rc0/freemocap/tests/test_synchronized_video_frame_counts.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/tests/test_total_body_center_of_mass_data_shape.py` & `freemocap-1.0.7rc0/freemocap/tests/test_total_body_center_of_mass_data_shape.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `freemocap-1.0.7rc0/freemocap/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/utilities/get_video_paths.py` & `freemocap-1.0.7rc0/freemocap/utilities/get_video_paths.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/freemocap/utilities/save_dictionary_to_json.py` & `freemocap-1.0.7rc0/freemocap/utilities/save_dictionary_to_json.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/ipython_jupyter_notebooks/batch_process_session_folders.ipynb` & `freemocap-1.0.7rc0/ipython_jupyter_notebooks/batch_process_session_folders.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb` & `freemocap-1.0.7rc0/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb` & `freemocap-1.0.7rc0/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/pyproject.toml` & `freemocap-1.0.7rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     "Blender3d",
     "synchronization",
     "computer vision"
 ]
 
 #dynamic = ["dependencies"]
 dependencies = [
-    "skellycam==2023.2.1076",
+    "skellycam==2023.4.1080",
     "skelly_viewer",
     'mediapipe; platform_system != "Darwin" or platform_machine != "arm64"',
     'mediapipe-silicon; platform_system == "Darwin" and platform_machine == "arm64"',
     "opencv-contrib-python==4.6.0.66",
     "toml",
     "aniposelib",
     "libsass",
@@ -86,15 +86,15 @@
 
 [project.urls]
 Homepage = "https://freemocap.org"
 Documentation = "https://freemocap.readthedocs.io/en/latest/"
 Github = "https://github.com/freemocap/freemocap"
 
 [tool.bumpver]
-current_version = "v1.0.6-rc"
+current_version = "v1.0.7-rc"
 version_pattern = "vMAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `freemocap-1.0.6rc0/src/gui/main/main.py` & `freemocap-1.0.7rc0/src/gui/main/main.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.6rc0/PKG-INFO` & `freemocap-1.0.7rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freemocap
-Version: 1.0.6rc0
+Version: 1.0.7rc0
 Summary: Top-level package for freemocap
 Keywords: camera,stream,video,image,opencv,skelly,freemocap,motion capture,markerless motion capture,mocap,markerless mocap,markerless,kinematic,animation,3d animation,Blender,Blender3d,synchronization,computer vision
 Author: Endurance Idehen, Aaron Cherian, Jonathan Samir Matthis
 Author-email: Skelly FreeMoCap <info@freemocap.org>
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
@@ -30,15 +30,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB)
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Video (UVC)
-Requires-Dist: skellycam==2023.2.1076
+Requires-Dist: skellycam==2023.4.1080
 Requires-Dist: skelly_viewer
 Requires-Dist: mediapipe; platform_system != "Darwin" or platform_machine != "arm64"
 Requires-Dist: mediapipe-silicon; platform_system == "Darwin" and platform_machine == "arm64"
 Requires-Dist: opencv-contrib-python==4.6.0.66
 Requires-Dist: toml
 Requires-Dist: aniposelib
 Requires-Dist: libsass
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: freemocap Version: 1.0.6rc0 Summary: Top-level
+Metadata-Version: 2.1 Name: freemocap Version: 1.0.7rc0 Summary: Top-level
 package for freemocap Keywords:
 camera,stream,video,image,opencv,skelly,freemocap,motion capture,markerless
 motion capture,mocap,markerless mocap,markerless,kinematic,animation,3d
 animation,Blender,Blender3d,synchronization,computer vision Author: Endurance
 Idehen, Aaron Cherian, Jonathan Samir Matthis Author-email: Skelly FreeMoCap
 freemocap.org> Requires-Python: >=3.8, <3.11 Description-Content-Type: text/
 markdown Classifier: Development Status :: 3 - Alpha Classifier: License :: OSI
@@ -20,15 +20,15 @@
 Classifier: Topic :: Multimedia :: Video :: Capture Classifier: Topic ::
 Multimedia :: Video :: Display Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing Classifier:
 Topic :: Scientific/Engineering :: Visualization Classifier: Topic ::
 Scientific/Engineering :: Human Machine Interfaces Classifier: Topic :: System
 :: Hardware Classifier: Topic :: System :: Hardware :: Universal Serial Bus
 (USB) Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) ::
-Video (UVC) Requires-Dist: skellycam==2023.2.1076 Requires-Dist: skelly_viewer
+Video (UVC) Requires-Dist: skellycam==2023.4.1080 Requires-Dist: skelly_viewer
 Requires-Dist: mediapipe; platform_system != "Darwin" or platform_machine !=
 "arm64" Requires-Dist: mediapipe-silicon; platform_system == "Darwin" and
 platform_machine == "arm64" Requires-Dist: opencv-contrib-python==4.6.0.66
 Requires-Dist: toml Requires-Dist: aniposelib Requires-Dist: libsass Requires-
 Dist: black ; extra == "dev" Requires-Dist: bumpver ; extra == "dev" Requires-
 Dist: isort ; extra == "dev" Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev" Requires-Dist: flit ; extra == "dev"
```


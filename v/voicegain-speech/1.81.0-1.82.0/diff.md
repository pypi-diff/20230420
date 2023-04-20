# Comparing `tmp/voicegain-speech-1.81.0.tar.gz` & `tmp/voicegain-speech-1.82.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicegain-speech-1.81.0.tar", last modified: Tue Mar 21 02:37:12 2023, max compression
+gzip compressed data, was "voicegain-speech-1.82.0.tar", last modified: Thu Apr 20 20:01:32 2023, max compression
```

## Comparing `voicegain-speech-1.81.0.tar` & `voicegain-speech-1.82.0.tar`

### file list

```diff
@@ -1,439 +1,439 @@
-drwxr-xr-x   0     1001     1002        0 2023-03-21 02:37:12.804071 voicegain-speech-1.81.0/
--rw-r--r--   0     1001     1002    11357 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/LICENSE
--rw-r--r--   0     1001     1002     2923 2023-03-21 02:37:12.804071 voicegain-speech-1.81.0/PKG-INFO
--rw-r--r--   0     1001     1002     2491 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/README.md
--rw-r--r--   0     1001     1002       79 2023-03-21 02:37:12.804071 voicegain-speech-1.81.0/setup.cfg
--rw-r--r--   0     1001     1002      709 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/setup.py
-drwxr-xr-x   0     1001     1002        0 2023-03-21 02:37:12.744071 voicegain-speech-1.81.0/voicegain_speech/
--rw-r--r--   0     1001     1002    59453 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/__init__.py
-drwxr-xr-x   0     1001     1002        0 2023-03-21 02:37:12.748071 voicegain-speech-1.81.0/voicegain_speech/api/
--rw-r--r--   0     1001     1002      821 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/__init__.py
--rw-r--r--   0     1001     1002    33053 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/aivr_api.py
--rw-r--r--   0     1001     1002    51988 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/aivr_callback_api.py
--rw-r--r--   0     1001     1002    38996 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/asr_callback_api.py
--rw-r--r--   0     1001     1002    34368 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/audiocodes_api.py
--rw-r--r--   0     1001     1002   107298 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/data_api.py
--rw-r--r--   0     1001     1002   143411 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/greg_api.py
--rw-r--r--   0     1001     1002    62985 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/lm_api.py
--rw-r--r--   0     1001     1002    47934 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/recognize_api.py
--rw-r--r--   0     1001     1002   113446 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/sa_api.py
--rw-r--r--   0     1001     1002    36947 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/security_api.py
--rw-r--r--   0     1001     1002    57126 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/training_api.py
--rw-r--r--   0     1001     1002    98391 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/transcribe_api.py
--rw-r--r--   0     1001     1002    55501 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api/websocket_api.py
--rw-r--r--   0     1001     1002    51711 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/api_client.py
--rw-r--r--   0     1001     1002    38172 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/configuration.py
--rw-r--r--   0     1001     1002    30215 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/exceptions.py
-drwxr-xr-x   0     1001     1002        0 2023-03-21 02:37:12.804071 voicegain-speech-1.81.0/voicegain_speech/models/
--rw-r--r--   0     1001     1002    58269 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/__init__.py
--rw-r--r--   0     1001     1002    39904 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/ac_control_messages.py
--rw-r--r--   0     1001     1002    31167 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/ac_end.py
--rw-r--r--   0     1001     1002    31175 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/ac_error.py
--rw-r--r--   0     1001     1002    31293 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/ac_hypothesis.py
--rw-r--r--   0     1001     1002    30022 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/ac_hypothesis_alternatives.py
--rw-r--r--   0     1001     1002    31263 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/ac_recognition.py
--rw-r--r--   0     1001     1002    31426 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/ac_recognition_alternatives.py
--rw-r--r--   0     1001     1002    32300 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/ac_response_messages.py
--rw-r--r--   0     1001     1002    39387 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/ac_start.py
--rw-r--r--   0     1001     1002    31439 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/ac_start_stt_speech_contexts.py
--rw-r--r--   0     1001     1002    30292 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/ac_started.py
--rw-r--r--   0     1001     1002    30361 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/ac_stop.py
--rw-r--r--   0     1001     1002    31039 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/account_and_context_id.py
--rw-r--r--   0     1001     1002    33942 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/advanced_regex.py
--rw-r--r--   0     1001     1002    29969 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aircall.py
--rw-r--r--   0     1001     1002    30009 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aircall_all_of.py
--rw-r--r--   0     1001     1002    35908 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_callback_response.py
--rw-r--r--   0     1001     1002    31324 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_callback_response_final.py
--rw-r--r--   0     1001     1002    29986 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_conference_transfer.py
--rw-r--r--   0     1001     1002    30644 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_disconnect.py
--rw-r--r--   0     1001     1002    33582 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_event.py
--rw-r--r--   0     1001     1002    29387 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_event_type.py
--rw-r--r--   0     1001     1002    32845 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_existing_session.py
--rw-r--r--   0     1001     1002    32457 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_logic.py
--rw-r--r--   0     1001     1002    29250 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_logic_media.py
--rw-r--r--   0     1001     1002    31199 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_logic_transfer.py
--rw-r--r--   0     1001     1002    29336 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_logic_type.py
--rw-r--r--   0     1001     1002    41198 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_new_session.py
--rw-r--r--   0     1001     1002    30741 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_phone_transfer.py
--rw-r--r--   0     1001     1002    33731 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_prompt.py
--rw-r--r--   0     1001     1002    30428 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_prompt_completion.py
--rw-r--r--   0     1001     1002    35144 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_prompt_playing.py
--rw-r--r--   0     1001     1002    29952 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_prompt_properties_audio.py
--rw-r--r--   0     1001     1002    29962 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_prompt_properties_html.py
--rw-r--r--   0     1001     1002    36609 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_question.py
--rw-r--r--   0     1001     1002    29347 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_recognition_result.py
--rw-r--r--   0     1001     1002    35414 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_recording.py
--rw-r--r--   0     1001     1002    41592 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_response_properties_audio.py
--rw-r--r--   0     1001     1002    31539 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_response_properties_html.py
--rw-r--r--   0     1001     1002    34209 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_session_user.py
--rw-r--r--   0     1001     1002    30315 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_session_user_base.py
--rw-r--r--   0     1001     1002    33081 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_session_user_fs.py
--rw-r--r--   0     1001     1002    31781 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivr_transfer.py
--rw-r--r--   0     1001     1002    32109 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/aivrs_question_specifics.py
--rw-r--r--   0     1001     1002    29341 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_processing_event.py
--rw-r--r--   0     1001     1002    29432 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_processing_status.py
--rw-r--r--   0     1001     1002    29352 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_processing_status_additional.py
--rw-r--r--   0     1001     1002    29407 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_processing_status_after_input_started.py
--rw-r--r--   0     1001     1002    29434 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_processing_status_for_callback.py
--rw-r--r--   0     1001     1002    29343 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_recognition_result.py
--rw-r--r--   0     1001     1002    42646 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_common.py
--rw-r--r--   0     1001     1002    56662 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_recognition.py
--rw-r--r--   0     1001     1002    52026 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_recognition_defaults.py
--rw-r--r--   0     1001     1002    43339 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_recognition_grammars_etc.py
--rw-r--r--   0     1001     1002    38095 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_recognition_timeouts.py
--rw-r--r--   0     1001     1002    52114 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription.py
--rw-r--r--   0     1001     1002    59679 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_async.py
--rw-r--r--   0     1001     1002    31362 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_async_all_of.py
--rw-r--r--   0     1001     1002    50133 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_common.py
--rw-r--r--   0     1001     1002    36242 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_common_lm.py
--rw-r--r--   0     1001     1002    34421 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_default_timeouts.py
--rw-r--r--   0     1001     1002    55383 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_defaults.py
--rw-r--r--   0     1001     1002    50764 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_sa.py
--rw-r--r--   0     1001     1002    31548 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_speakers.py
--rw-r--r--   0     1001     1002    32965 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py
--rw-r--r--   0     1001     1002    33897 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_audio_input_source.py
--rw-r--r--   0     1001     1002    29353 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_mode.py
--rw-r--r--   0     1001     1002    29397 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_mode_recognition.py
--rw-r--r--   0     1001     1002    29314 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_mode_speech_analytics.py
--rw-r--r--   0     1001     1002    29360 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_mode_transcription.py
--rw-r--r--   0     1001     1002    31534 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_post_response_base.py
--rw-r--r--   0     1001     1002    30929 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_post_response_base_audio.py
--rw-r--r--   0     1001     1002    32607 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_reco_post_response.py
--rw-r--r--   0     1001     1002    30284 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_reco_post_response_sessions.py
--rw-r--r--   0     1001     1002    30196 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_recognition_callback_response.py
--rw-r--r--   0     1001     1002    31828 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_recognition_request.py
--rw-r--r--   0     1001     1002    31958 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_recognition_response.py
--rw-r--r--   0     1001     1002    34717 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_recognition_result.py
--rw-r--r--   0     1001     1002    29983 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_recognition_result_all_of.py
--rw-r--r--   0     1001     1002    32667 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_result_full.py
--rw-r--r--   0     1001     1002    30556 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_result_full_all_of.py
--rw-r--r--   0     1001     1002    30656 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_result_full_all_of_audio.py
--rw-r--r--   0     1001     1002    30070 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_result_full_all_of_audio_source.py
--rw-r--r--   0     1001     1002    30082 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py
--rw-r--r--   0     1001     1002    42350 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_result_full_all_of_result.py
--rw-r--r--   0     1001     1002    33086 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_result_incremental.py
--rw-r--r--   0     1001     1002    30903 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_result_incremental_detail.py
--rw-r--r--   0     1001     1002    30941 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_result_incremental_detail_control_status.py
--rw-r--r--   0     1001     1002    38829 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_result_incremental_detail_result.py
--rw-r--r--   0     1001     1002    34212 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py
--rw-r--r--   0     1001     1002    33088 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_session_established.py
--rw-r--r--   0     1001     1002    32470 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_session_short_info.py
--rw-r--r--   0     1001     1002    30097 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_session_url.py
--rw-r--r--   0     1001     1002    32665 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_transc_post_response.py
--rw-r--r--   0     1001     1002    30318 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_transc_post_response_sessions.py
--rw-r--r--   0     1001     1002    35163 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_transc_session_established.py
--rw-r--r--   0     1001     1002    30124 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_transcription_callback_response.py
--rw-r--r--   0     1001     1002    31729 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_transcription_request.py
--rw-r--r--   0     1001     1002    31138 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_transcription_response.py
--rw-r--r--   0     1001     1002    31566 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/async_transcription_response_shared.py
--rw-r--r--   0     1001     1002    29317 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_channel.py
--rw-r--r--   0     1001     1002    29295 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_channel_selector.py
--rw-r--r--   0     1001     1002    29388 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_channel_selector_offline_async.py
--rw-r--r--   0     1001     1002    29249 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_channels.py
--rw-r--r--   0     1001     1002    29944 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_for_data_object.py
--rw-r--r--   0     1001     1002    29364 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_format.py
--rw-r--r--   0     1001     1002    33795 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_input_async.py
--rw-r--r--   0     1001     1002    30010 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_input_async_source.py
--rw-r--r--   0     1001     1002    32932 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_input_base.py
--rw-r--r--   0     1001     1002    29119 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_input_data.py
--rw-r--r--   0     1001     1002    31301 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_input_data_all_of.py
--rw-r--r--   0     1001     1002    31201 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_input_data_all_of_source.py
--rw-r--r--   0     1001     1002    34758 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_input_sync.py
--rw-r--r--   0     1001     1002    31017 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_input_sync_source.py
--rw-r--r--   0     1001     1002    33976 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_resource_uri.py
--rw-r--r--   0     1001     1002    29349 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_zone_class.py
--rw-r--r--   0     1001     1002    31260 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/audio_zone_item.py
--rw-r--r--   0     1001     1002    29790 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/basic_success_response.py
--rw-r--r--   0     1001     1002    31292 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/builtin.py
--rw-r--r--   0     1001     1002    31352 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/builtin_all_of.py
--rw-r--r--   0     1001     1002    29631 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/call_attributes.py
--rw-r--r--   0     1001     1002    34746 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/callback_req.py
--rw-r--r--   0     1001     1002    31504 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/callback_req_reco.py
--rw-r--r--   0     1001     1002    29918 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/callback_resp.py
--rw-r--r--   0     1001     1002    33700 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/caption.py
--rw-r--r--   0     1001     1002    30760 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/compliance_settings.py
--rw-r--r--   0     1001     1002    29310 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/config_value_status.py
--rw-r--r--   0     1001     1002    29367 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/content_type.py
--rw-r--r--   0     1001     1002    32827 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/continuous_recognition.py
--rw-r--r--   0     1001     1002    50044 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/core_aivr_session.py
--rw-r--r--   0     1001     1002    39069 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/core_aivr_session_telco_data.py
--rw-r--r--   0     1001     1002    29274 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/creating_entity.py
--rw-r--r--   0     1001     1002    30959 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/criterion_config.py
--rw-r--r--   0     1001     1002    30860 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/criterion_satisfied.py
--rw-r--r--   0     1001     1002    29786 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/data_obj_ref.py
--rw-r--r--   0     1001     1002    44311 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/data_object.py
--rw-r--r--   0     1001     1002    29780 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/data_object_all_of.py
--rw-r--r--   0     1001     1002    38308 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/data_object_base.py
--rw-r--r--   0     1001     1002    34669 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/data_object_ids.py
--rw-r--r--   0     1001     1002    44090 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/data_object_no_sos_ref.py
--rw-r--r--   0     1001     1002    39281 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/data_object_with_audio.py
--rw-r--r--   0     1001     1002    29724 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/debug_info.py
--rw-r--r--   0     1001     1002    30330 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/debug_settings.py
--rw-r--r--   0     1001     1002    32329 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/demo.py
--rw-r--r--   0     1001     1002    32409 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/demo_all_of.py
--rw-r--r--   0     1001     1002    30716 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/diarization_data.py
--rw-r--r--   0     1001     1002    30585 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/diarization_zone.py
--rw-r--r--   0     1001     1002    35781 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/diarization_zone_item.py
--rw-r--r--   0     1001     1002    32447 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/disconnect.py
--rw-r--r--   0     1001     1002    32527 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/disconnect_all_of.py
--rw-r--r--   0     1001     1002    30779 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/error.py
--rw-r--r--   0     1001     1002    30839 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/error_all_of.py
--rw-r--r--   0     1001     1002    30827 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/error_info.py
--rw-r--r--   0     1001     1002    31388 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/estimated_queue_wait.py
--rw-r--r--   0     1001     1002    29329 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/experiment_platform.py
--rw-r--r--   0     1001     1002    31802 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/file_location.py
--rw-r--r--   0     1001     1002    35736 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/formatter.py
--rw-r--r--   0     1001     1002    30704 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/grammar.py
--rw-r--r--   0     1001     1002    30011 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg.py
--rw-r--r--   0     1001     1002    30051 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_all_of.py
--rw-r--r--   0     1001     1002    37162 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio.py
--rw-r--r--   0     1001     1002    31027 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_all_of.py
--rw-r--r--   0     1001     1002    32672 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_base.py
--rw-r--r--   0     1001     1002    33677 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_base_with_audio.py
--rw-r--r--   0     1001     1002    30017 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_id.py
--rw-r--r--   0     1001     1002    30669 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_input.py
--rw-r--r--   0     1001     1002    29999 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_input_audio_hash.py
--rw-r--r--   0     1001     1002    29917 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_input_audio_id.py
--rw-r--r--   0     1001     1002    29944 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_input_data.py
--rw-r--r--   0     1001     1002    34024 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set.py
--rw-r--r--   0     1001     1002    31347 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_base.py
--rw-r--r--   0     1001     1002    31420 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_base_inclusive.py
--rw-r--r--   0     1001     1002    32260 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_core.py
--rw-r--r--   0     1001     1002    30024 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_id.py
--rw-r--r--   0     1001     1002    32289 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_inclusive.py
--rw-r--r--   0     1001     1002    32369 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_inclusive_core.py
--rw-r--r--   0     1001     1002    32280 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_inner.py
--rw-r--r--   0     1001     1002    31118 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_response.py
--rw-r--r--   0     1001     1002    35486 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_thin.py
--rw-r--r--   0     1001     1002    38630 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment.py
--rw-r--r--   0     1001     1002    35987 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_base.py
--rw-r--r--   0     1001     1002    34723 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_base_inclusive.py
--rw-r--r--   0     1001     1002    31678 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_base_platform_data.py
--rw-r--r--   0     1001     1002    30062 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_id.py
--rw-r--r--   0     1001     1002    37490 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_inclusive.py
--rw-r--r--   0     1001     1002    35661 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_modifiable.py
--rw-r--r--   0     1001     1002    35285 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_platform_external_asr.py
--rw-r--r--   0     1001     1002    30328 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_platform_upload.py
--rw-r--r--   0     1001     1002    31040 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_platform_voicegain.py
--rw-r--r--   0     1001     1002    31146 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_response.py
--rw-r--r--   0     1001     1002    29430 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_status.py
--rw-r--r--   0     1001     1002    29359 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_status_modifiable.py
--rw-r--r--   0     1001     1002    34341 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_grammar.py
--rw-r--r--   0     1001     1002    31613 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_grammar_base.py
--rw-r--r--   0     1001     1002    30617 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_grammar_base_light.py
--rw-r--r--   0     1001     1002    30079 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_grammar_id.py
--rw-r--r--   0     1001     1002    31545 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_grammar_inner.py
--rw-r--r--   0     1001     1002    33421 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_grammar_light.py
--rw-r--r--   0     1001     1002    30730 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_interpretation.py
--rw-r--r--   0     1001     1002    34960 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_question.py
--rw-r--r--   0     1001     1002    32213 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_question_base.py
--rw-r--r--   0     1001     1002    30110 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_question_id.py
--rw-r--r--   0     1001     1002    33236 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_question_inner.py
--rw-r--r--   0     1001     1002    30956 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py
--rw-r--r--   0     1001     1002    33432 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py
--rw-r--r--   0     1001     1002    30869 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py
--rw-r--r--   0     1001     1002    30799 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py
--rw-r--r--   0     1001     1002    30073 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_recog_base_with_exp.py
--rw-r--r--   0     1001     1002    36922 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_recognition.py
--rw-r--r--   0     1001     1002    34214 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_recognition_base.py
--rw-r--r--   0     1001     1002    30091 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_recognition_id.py
--rw-r--r--   0     1001     1002    29378 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_review_status.py
--rw-r--r--   0     1001     1002    32341 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_source_of_truth.py
--rw-r--r--   0     1001     1002    33215 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_truth_update.py
--rw-r--r--   0     1001     1002    32975 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/greg_truth_updates.py
--rw-r--r--   0     1001     1002    31960 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/grxml.py
--rw-r--r--   0     1001     1002    32060 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/grxml_all_of.py
--rw-r--r--   0     1001     1002    30469 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/gui_input.py
--rw-r--r--   0     1001     1002    29087 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/hangup.py
--rw-r--r--   0     1001     1002    29759 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/html_checkbox.py
--rw-r--r--   0     1001     1002    31573 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/html_choice_item.py
--rw-r--r--   0     1001     1002    29791 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/html_radio_buttons.py
--rw-r--r--   0     1001     1002    29854 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/html_text_entry.py
--rw-r--r--   0     1001     1002    29247 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/if_exists.py
--rw-r--r--   0     1001     1002    33271 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/incident.py
--rw-r--r--   0     1001     1002    29778 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/inline_data.py
--rw-r--r--   0     1001     1002    30983 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/inline_object.py
--rw-r--r--   0     1001     1002    30995 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/inline_object1.py
--rw-r--r--   0     1001     1002    34398 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/input.py
--rw-r--r--   0     1001     1002    34538 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/input_all_of.py
--rw-r--r--   0     1001     1002    30698 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/integration.py
--rw-r--r--   0     1001     1002    35874 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/jjsgf.py
--rw-r--r--   0     1001     1002    36014 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/jjsgf_all_of.py
--rw-r--r--   0     1001     1002    31165 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/keyword_spot_example.py
--rw-r--r--   0     1001     1002    31150 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/keyword_spot_group.py
--rw-r--r--   0     1001     1002    32893 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/keyword_spot_item.py
--rw-r--r--   0     1001     1002    29371 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/lang_model_status.py
--rw-r--r--   0     1001     1002    30147 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/language.py
--rw-r--r--   0     1001     1002    39474 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/language_model_doc.py
--rw-r--r--   0     1001     1002    37931 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/language_model_doc_modifiable.py
--rw-r--r--   0     1001     1002    32689 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/language_model_src_data.py
--rw-r--r--   0     1001     1002    29248 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/lm_type.py
--rw-r--r--   0     1001     1002    29910 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/min_max_speakers.py
--rw-r--r--   0     1001     1002    32751 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/min_max_speakers_diarization.py
--rw-r--r--   0     1001     1002    29400 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/mood_type.py
--rw-r--r--   0     1001     1002    31243 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/mrc_pv1_asr_settings.py
--rw-r--r--   0     1001     1002    31216 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/mrc_pv2_asr_settings.py
--rw-r--r--   0     1001     1002    29247 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/mrcp_version.py
--rw-r--r--   0     1001     1002    31730 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/name_value_pair.py
--rw-r--r--   0     1001     1002    30742 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/named_entity_concept.py
--rw-r--r--   0     1001     1002    29842 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/named_entity_type.py
--rw-r--r--   0     1001     1002    49627 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/new_speech_analytics_session.py
--rw-r--r--   0     1001     1002    38041 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/new_speech_analytics_session_response.py
--rw-r--r--   0     1001     1002    30074 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/new_speech_analytics_session_response_poll.py
--rw-r--r--   0     1001     1002    29980 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/new_speech_analytics_session_response_websocket.py
--rw-r--r--   0     1001     1002    30628 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/non_session_error_response.py
--rw-r--r--   0     1001     1002    29167 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/non_session_error_response400.py
--rw-r--r--   0     1001     1002    29167 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/non_session_error_response401.py
--rw-r--r--   0     1001     1002    32061 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/output.py
--rw-r--r--   0     1001     1002    32141 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/output_all_of.py
--rw-r--r--   0     1001     1002    34343 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/overtalk.py
--rw-r--r--   0     1001     1002    32535 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/phone_audio_input.py
--rw-r--r--   0     1001     1002    30753 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/phone_audio_input_prompt.py
--rw-r--r--   0     1001     1002    33384 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/phrase_spot_example.py
--rw-r--r--   0     1001     1002    33250 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/phrase_spot_group.py
--rw-r--r--   0     1001     1002    40893 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/phrase_spot_item.py
--rw-r--r--   0     1001     1002    32214 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/phrase_spot_item_location.py
--rw-r--r--   0     1001     1002    31994 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/phrase_spot_item_location_dialogue.py
--rw-r--r--   0     1001     1002    30854 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/phrase_spot_item_slots.py
--rw-r--r--   0     1001     1002    32790 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/pii_redaction_conf.py
--rw-r--r--   0     1001     1002    32799 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/poll_req.py
--rw-r--r--   0     1001     1002    33368 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/poll_resp.py
--rw-r--r--   0     1001     1002    32658 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/portal_output_init.py
--rw-r--r--   0     1001     1002    30127 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/pre_fetch.py
--rw-r--r--   0     1001     1002    40796 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/progress.py
--rw-r--r--   0     1001     1002    31612 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/progress_callback.py
--rw-r--r--   0     1001     1002    29534 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/progress_phase.py
--rw-r--r--   0     1001     1002    32656 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/quartiles_energy.py
--rw-r--r--   0     1001     1002    32632 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/quartiles_pitch.py
--rw-r--r--   0     1001     1002    34441 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/reco_alt.py
--rw-r--r--   0     1001     1002    31642 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/recog_nlsml.py
--rw-r--r--   0     1001     1002    30812 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/recog_nlsml_no_exp.py
--rw-r--r--   0     1001     1002    33906 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/recog_obj.py
--rw-r--r--   0     1001     1002    33144 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/recog_obj_no_exp.py
--rw-r--r--   0     1001     1002    33805 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/recognition_result.py
--rw-r--r--   0     1001     1002    33632 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/requested_content.py
--rw-r--r--   0     1001     1002    32832 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/resource_uri.py
--rw-r--r--   0     1001     1002    34984 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/s3.py
--rw-r--r--   0     1001     1002    35144 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/s3_all_of.py
--rw-r--r--   0     1001     1002    34848 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/s3_audio_input.py
--rw-r--r--   0     1001     1002    31352 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/s3_metadata_mapping.py
--rw-r--r--   0     1001     1002    31130 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/s3_tag_mapping.py
--rw-r--r--   0     1001     1002    29264 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/sa_conf_type.py
--rw-r--r--   0     1001     1002    29383 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/sample_rate.py
--rw-r--r--   0     1001     1002    29960 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/session_content.py
--rw-r--r--   0     1001     1002    31472 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/session_error_response.py
--rw-r--r--   0     1001     1002    37488 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/session_init_recognition.py
--rw-r--r--   0     1001     1002    39730 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/session_init_transcription.py
--rw-r--r--   0     1001     1002    32892 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/session_init_transcription_diarization.py
--rw-r--r--   0     1001     1002    30694 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/session_success_response.py
--rw-r--r--   0     1001     1002    35303 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/settings_async_transcription.py
--rw-r--r--   0     1001     1002    32224 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/settings_recognition.py
--rw-r--r--   0     1001     1002    32197 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/settings_sync_transcription.py
--rw-r--r--   0     1001     1002    34209 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/silence.py
--rw-r--r--   0     1001     1002    30855 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/slot_entity.py
--rw-r--r--   0     1001     1002    30802 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/slot_keyword.py
--rw-r--r--   0     1001     1002    30889 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/sos_ref.py
--rw-r--r--   0     1001     1002    33548 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speaker_result.py
--rw-r--r--   0     1001     1002    44356 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_base_result.py
--rw-r--r--   0     1001     1002    32031 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_channel.py
--rw-r--r--   0     1001     1002    45729 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_channel_result.py
--rw-r--r--   0     1001     1002    34015 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_channel_with_transcribe.py
--rw-r--r--   0     1001     1002    70655 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config.py
--rw-r--r--   0     1001     1002    34473 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config_identifying.py
--rw-r--r--   0     1001     1002    67930 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config_modifiable.py
--rw-r--r--   0     1001     1002    66650 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config_modifiable_base.py
--rw-r--r--   0     1001     1002    31340 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py
--rw-r--r--   0     1001     1002    30883 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config_name_optional.py
--rw-r--r--   0     1001     1002    31037 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config_name_required.py
--rw-r--r--   0     1001     1002    50083 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_core_result.py
--rw-r--r--   0     1001     1002    35010 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_core_result_all_of.py
--rw-r--r--   0     1001     1002    30949 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_criteria_data.py
--rw-r--r--   0     1001     1002    31414 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_emotion.py
--rw-r--r--   0     1001     1002    30617 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_emotion_data.py
--rw-r--r--   0     1001     1002    36738 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_emotion_item.py
--rw-r--r--   0     1001     1002    30663 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_keyword.py
--rw-r--r--   0     1001     1002    30953 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_keyword_data.py
--rw-r--r--   0     1001     1002    35987 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_keyword_item.py
--rw-r--r--   0     1001     1002    36239 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py
--rw-r--r--   0     1001     1002    31633 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_named_entity.py
--rw-r--r--   0     1001     1002    37037 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_named_entity_item.py
--rw-r--r--   0     1001     1002    37325 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py
--rw-r--r--   0     1001     1002    32719 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase.py
--rw-r--r--   0     1001     1002    30936 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_data.py
--rw-r--r--   0     1001     1002    30762 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_group.py
--rw-r--r--   0     1001     1002    31035 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_group_data.py
--rw-r--r--   0     1001     1002    36150 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_group_item.py
--rw-r--r--   0     1001     1002    38059 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_item.py
--rw-r--r--   0     1001     1002    39459 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py
--rw-r--r--   0     1001     1002    30833 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_slots.py
--rw-r--r--   0     1001     1002    61063 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_result.py
--rw-r--r--   0     1001     1002    46390 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_result_detail.py
--rw-r--r--   0     1001     1002    30848 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_session_modifiable.py
--rw-r--r--   0     1001     1002    37783 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_session_poll_response.py
--rw-r--r--   0     1001     1002    31485 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/start_end_time_for_sub_criterion.py
--rw-r--r--   0     1001     1002    30171 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/stomp_ping.py
--rw-r--r--   0     1001     1002    30948 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/stomp_word_correction.py
--rw-r--r--   0     1001     1002    35009 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/stomp_ws_word.py
--rw-r--r--   0     1001     1002    35377 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/stream_resp.py
--rw-r--r--   0     1001     1002    32938 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/stream_setup.py
--rw-r--r--   0     1001     1002    29391 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/streaming_protocol.py
--rw-r--r--   0     1001     1002    38570 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/sub_criterion_config.py
--rw-r--r--   0     1001     1002    40956 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/sub_criterion_satisfied.py
--rw-r--r--   0     1001     1002    31931 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/sync_audio_input_source.py
--rw-r--r--   0     1001     1002    30879 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/sync_recognition_request.py
--rw-r--r--   0     1001     1002    32444 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/sync_recognition_response.py
--rw-r--r--   0     1001     1002    30047 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/sync_session_established.py
--rw-r--r--   0     1001     1002    30763 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/sync_transcription_request.py
--rw-r--r--   0     1001     1002    32502 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/sync_transcription_response.py
--rw-r--r--   0     1001     1002    32941 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/sync_transcription_result.py
--rw-r--r--   0     1001     1002    38657 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/talk_time.py
--rw-r--r--   0     1001     1002    31188 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/topic_score.py
--rw-r--r--   0     1001     1002    29287 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/training_set_bucket_type.py
--rw-r--r--   0     1001     1002    38929 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/training_set_doc.py
--rw-r--r--   0     1001     1002    30847 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/training_set_doc_defaults.py
--rw-r--r--   0     1001     1002    36307 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/training_set_doc_statistics.py
--rw-r--r--   0     1001     1002    34381 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/training_set_key.py
--rw-r--r--   0     1001     1002    33631 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/training_set_modifiable.py
--rw-r--r--   0     1001     1002    29379 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/training_set_status.py
--rw-r--r--   0     1001     1002    29419 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/training_set_status_modifiable.py
--rw-r--r--   0     1001     1002    29307 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/training_set_store_type.py
--rw-r--r--   0     1001     1002    31549 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/transcribe_alt.py
--rw-r--r--   0     1001     1002    30831 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/transcribe_session_id.py
--rw-r--r--   0     1001     1002    33849 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/transcribe_session_modify_request.py
--rw-r--r--   0     1001     1002    31526 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/transcribe_session_modify_request_mute.py
--rw-r--r--   0     1001     1002    30354 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/transcribe_session_modify_request_pause.py
--rw-r--r--   0     1001     1002    34383 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/transcript_position_range.py
--rw-r--r--   0     1001     1002    34563 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/transcript_position_range_for_phrase.py
--rw-r--r--   0     1001     1002    35799 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py
--rw-r--r--   0     1001     1002    36120 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/transfer.py
--rw-r--r--   0     1001     1002    36260 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/transfer_all_of.py
--rw-r--r--   0     1001     1002    29303 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/vad_mode.py
--rw-r--r--   0     1001     1002    32108 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/version.py
--rw-r--r--   0     1001     1002    37760 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/websocket.py
--rw-r--r--   0     1001     1002    38351 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/websocket_init.py
--rw-r--r--   0     1001     1002    30321 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/websocket_init_reco.py
--rw-r--r--   0     1001     1002    35916 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/websocket_modifiable.py
--rw-r--r--   0     1001     1002    32384 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/websocket_msg.py
--rw-r--r--   0     1001     1002    29250 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/websocket_protocol.py
--rw-r--r--   0     1001     1002    30725 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/websocket_resp.py
--rw-r--r--   0     1001     1002    30082 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/word_alternatives.py
--rw-r--r--   0     1001     1002    31262 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/word_cloud_item.py
--rw-r--r--   0     1001     1002    31103 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/word_correction.py
--rw-r--r--   0     1001     1002    36113 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/word_item_timed.py
--rw-r--r--   0     1001     1002    31188 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/word_item_timing.py
--rw-r--r--   0     1001     1002    30443 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/word_tree_ids.py
--rw-r--r--   0     1001     1002    36490 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/word_tree_item.py
--rw-r--r--   0     1001     1002    33045 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/words_item.py
--rw-r--r--   0     1001     1002    36348 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/words_section.py
--rw-r--r--   0     1001     1002    32894 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/words_section_meta.py
--rw-r--r--   0     1001     1002    31896 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/words_section_meta_mc.py
--rw-r--r--   0     1001     1002    33875 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/words_section_single_column.py
--rw-r--r--   0     1001     1002    29956 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/words_section_words.py
--rw-r--r--   0     1001     1002    38086 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/models/words_websocket_item.py
--rw-r--r--   0     1001     1002    38926 2023-03-21 02:37:10.000000 voicegain-speech-1.81.0/voicegain_speech/rest.py
-drwxr-xr-x   0     1001     1002        0 2023-03-21 02:37:12.744071 voicegain-speech-1.81.0/voicegain_speech.egg-info/
--rw-r--r--   0     1001     1002     2923 2023-03-21 02:37:12.000000 voicegain-speech-1.81.0/voicegain_speech.egg-info/PKG-INFO
--rw-r--r--   0     1001     1002    20760 2023-03-21 02:37:12.000000 voicegain-speech-1.81.0/voicegain_speech.egg-info/SOURCES.txt
--rw-r--r--   0     1001     1002        1 2023-03-21 02:37:12.000000 voicegain-speech-1.81.0/voicegain_speech.egg-info/dependency_links.txt
--rw-r--r--   0     1001     1002       48 2023-03-21 02:37:12.000000 voicegain-speech-1.81.0/voicegain_speech.egg-info/requires.txt
--rw-r--r--   0     1001     1002       17 2023-03-21 02:37:12.000000 voicegain-speech-1.81.0/voicegain_speech.egg-info/top_level.txt
+drwxr-xr-x   0     1001     1002        0 2023-04-20 20:01:32.058720 voicegain-speech-1.82.0/
+-rw-r--r--   0     1001     1002    11357 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/LICENSE
+-rw-r--r--   0     1001     1002     2923 2023-04-20 20:01:32.058720 voicegain-speech-1.82.0/PKG-INFO
+-rw-r--r--   0     1001     1002     2491 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/README.md
+-rw-r--r--   0     1001     1002       79 2023-04-20 20:01:32.058720 voicegain-speech-1.82.0/setup.cfg
+-rw-r--r--   0     1001     1002      709 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/setup.py
+drwxr-xr-x   0     1001     1002        0 2023-04-20 20:01:31.986720 voicegain-speech-1.82.0/voicegain_speech/
+-rw-r--r--   0     1001     1002    59453 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/__init__.py
+drwxr-xr-x   0     1001     1002        0 2023-04-20 20:01:31.990720 voicegain-speech-1.82.0/voicegain_speech/api/
+-rw-r--r--   0     1001     1002      821 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/__init__.py
+-rw-r--r--   0     1001     1002    33053 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/aivr_api.py
+-rw-r--r--   0     1001     1002    51988 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/aivr_callback_api.py
+-rw-r--r--   0     1001     1002    38996 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/asr_callback_api.py
+-rw-r--r--   0     1001     1002    34368 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/audiocodes_api.py
+-rw-r--r--   0     1001     1002   107298 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/data_api.py
+-rw-r--r--   0     1001     1002   143411 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/greg_api.py
+-rw-r--r--   0     1001     1002    62985 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/lm_api.py
+-rw-r--r--   0     1001     1002    47934 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/recognize_api.py
+-rw-r--r--   0     1001     1002   113446 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/sa_api.py
+-rw-r--r--   0     1001     1002    36947 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/security_api.py
+-rw-r--r--   0     1001     1002    57126 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/training_api.py
+-rw-r--r--   0     1001     1002    98391 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/transcribe_api.py
+-rw-r--r--   0     1001     1002    55501 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api/websocket_api.py
+-rw-r--r--   0     1001     1002    51711 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/api_client.py
+-rw-r--r--   0     1001     1002    38172 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/configuration.py
+-rw-r--r--   0     1001     1002    30215 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/exceptions.py
+drwxr-xr-x   0     1001     1002        0 2023-04-20 20:01:32.058720 voicegain-speech-1.82.0/voicegain_speech/models/
+-rw-r--r--   0     1001     1002    58269 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/__init__.py
+-rw-r--r--   0     1001     1002    39904 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/ac_control_messages.py
+-rw-r--r--   0     1001     1002    31167 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/ac_end.py
+-rw-r--r--   0     1001     1002    31175 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/ac_error.py
+-rw-r--r--   0     1001     1002    31293 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/ac_hypothesis.py
+-rw-r--r--   0     1001     1002    30022 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/ac_hypothesis_alternatives.py
+-rw-r--r--   0     1001     1002    31263 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/ac_recognition.py
+-rw-r--r--   0     1001     1002    31426 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/ac_recognition_alternatives.py
+-rw-r--r--   0     1001     1002    32300 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/ac_response_messages.py
+-rw-r--r--   0     1001     1002    39387 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/ac_start.py
+-rw-r--r--   0     1001     1002    31439 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/ac_start_stt_speech_contexts.py
+-rw-r--r--   0     1001     1002    30292 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/ac_started.py
+-rw-r--r--   0     1001     1002    30361 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/ac_stop.py
+-rw-r--r--   0     1001     1002    31039 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/account_and_context_id.py
+-rw-r--r--   0     1001     1002    33942 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/advanced_regex.py
+-rw-r--r--   0     1001     1002    29969 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aircall.py
+-rw-r--r--   0     1001     1002    30009 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aircall_all_of.py
+-rw-r--r--   0     1001     1002    35908 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_callback_response.py
+-rw-r--r--   0     1001     1002    31324 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_callback_response_final.py
+-rw-r--r--   0     1001     1002    29986 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_conference_transfer.py
+-rw-r--r--   0     1001     1002    30644 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_disconnect.py
+-rw-r--r--   0     1001     1002    33582 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_event.py
+-rw-r--r--   0     1001     1002    29387 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_event_type.py
+-rw-r--r--   0     1001     1002    32845 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_existing_session.py
+-rw-r--r--   0     1001     1002    32457 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_logic.py
+-rw-r--r--   0     1001     1002    29250 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_logic_media.py
+-rw-r--r--   0     1001     1002    31199 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_logic_transfer.py
+-rw-r--r--   0     1001     1002    29336 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_logic_type.py
+-rw-r--r--   0     1001     1002    41198 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_new_session.py
+-rw-r--r--   0     1001     1002    30741 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_phone_transfer.py
+-rw-r--r--   0     1001     1002    33731 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_prompt.py
+-rw-r--r--   0     1001     1002    30428 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_prompt_completion.py
+-rw-r--r--   0     1001     1002    35144 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_prompt_playing.py
+-rw-r--r--   0     1001     1002    29952 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_prompt_properties_audio.py
+-rw-r--r--   0     1001     1002    29962 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_prompt_properties_html.py
+-rw-r--r--   0     1001     1002    36609 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_question.py
+-rw-r--r--   0     1001     1002    29347 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_recognition_result.py
+-rw-r--r--   0     1001     1002    35414 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_recording.py
+-rw-r--r--   0     1001     1002    41592 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_response_properties_audio.py
+-rw-r--r--   0     1001     1002    31539 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_response_properties_html.py
+-rw-r--r--   0     1001     1002    34209 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_session_user.py
+-rw-r--r--   0     1001     1002    30315 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_session_user_base.py
+-rw-r--r--   0     1001     1002    33081 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_session_user_fs.py
+-rw-r--r--   0     1001     1002    31781 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivr_transfer.py
+-rw-r--r--   0     1001     1002    32109 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/aivrs_question_specifics.py
+-rw-r--r--   0     1001     1002    29341 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_processing_event.py
+-rw-r--r--   0     1001     1002    29432 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_processing_status.py
+-rw-r--r--   0     1001     1002    29352 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_processing_status_additional.py
+-rw-r--r--   0     1001     1002    29407 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_processing_status_after_input_started.py
+-rw-r--r--   0     1001     1002    29434 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_processing_status_for_callback.py
+-rw-r--r--   0     1001     1002    29343 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_recognition_result.py
+-rw-r--r--   0     1001     1002    42646 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_common.py
+-rw-r--r--   0     1001     1002    56662 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_recognition.py
+-rw-r--r--   0     1001     1002    52026 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_recognition_defaults.py
+-rw-r--r--   0     1001     1002    43339 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_recognition_grammars_etc.py
+-rw-r--r--   0     1001     1002    38095 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_recognition_timeouts.py
+-rw-r--r--   0     1001     1002    52114 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription.py
+-rw-r--r--   0     1001     1002    59679 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_async.py
+-rw-r--r--   0     1001     1002    31362 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_async_all_of.py
+-rw-r--r--   0     1001     1002    50133 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_common.py
+-rw-r--r--   0     1001     1002    36242 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_common_lm.py
+-rw-r--r--   0     1001     1002    34421 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_default_timeouts.py
+-rw-r--r--   0     1001     1002    55383 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_defaults.py
+-rw-r--r--   0     1001     1002    50764 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_sa.py
+-rw-r--r--   0     1001     1002    31548 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_speakers.py
+-rw-r--r--   0     1001     1002    32965 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py
+-rw-r--r--   0     1001     1002    33897 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_audio_input_source.py
+-rw-r--r--   0     1001     1002    29353 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_mode.py
+-rw-r--r--   0     1001     1002    29397 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_mode_recognition.py
+-rw-r--r--   0     1001     1002    29314 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_mode_speech_analytics.py
+-rw-r--r--   0     1001     1002    29360 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_mode_transcription.py
+-rw-r--r--   0     1001     1002    31534 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_post_response_base.py
+-rw-r--r--   0     1001     1002    30929 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_post_response_base_audio.py
+-rw-r--r--   0     1001     1002    32607 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_reco_post_response.py
+-rw-r--r--   0     1001     1002    30284 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_reco_post_response_sessions.py
+-rw-r--r--   0     1001     1002    30196 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_recognition_callback_response.py
+-rw-r--r--   0     1001     1002    31828 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_recognition_request.py
+-rw-r--r--   0     1001     1002    31958 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_recognition_response.py
+-rw-r--r--   0     1001     1002    34717 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_recognition_result.py
+-rw-r--r--   0     1001     1002    29983 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_recognition_result_all_of.py
+-rw-r--r--   0     1001     1002    32667 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_result_full.py
+-rw-r--r--   0     1001     1002    30556 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_result_full_all_of.py
+-rw-r--r--   0     1001     1002    30656 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_result_full_all_of_audio.py
+-rw-r--r--   0     1001     1002    30070 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_result_full_all_of_audio_source.py
+-rw-r--r--   0     1001     1002    30082 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py
+-rw-r--r--   0     1001     1002    42350 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_result_full_all_of_result.py
+-rw-r--r--   0     1001     1002    33086 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_result_incremental.py
+-rw-r--r--   0     1001     1002    30903 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_result_incremental_detail.py
+-rw-r--r--   0     1001     1002    30941 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_result_incremental_detail_control_status.py
+-rw-r--r--   0     1001     1002    38829 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_result_incremental_detail_result.py
+-rw-r--r--   0     1001     1002    34212 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py
+-rw-r--r--   0     1001     1002    33088 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_session_established.py
+-rw-r--r--   0     1001     1002    32470 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_session_short_info.py
+-rw-r--r--   0     1001     1002    30097 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_session_url.py
+-rw-r--r--   0     1001     1002    32665 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_transc_post_response.py
+-rw-r--r--   0     1001     1002    30318 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_transc_post_response_sessions.py
+-rw-r--r--   0     1001     1002    35163 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_transc_session_established.py
+-rw-r--r--   0     1001     1002    30124 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_transcription_callback_response.py
+-rw-r--r--   0     1001     1002    31729 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_transcription_request.py
+-rw-r--r--   0     1001     1002    31138 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_transcription_response.py
+-rw-r--r--   0     1001     1002    31566 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/async_transcription_response_shared.py
+-rw-r--r--   0     1001     1002    29317 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_channel.py
+-rw-r--r--   0     1001     1002    29295 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_channel_selector.py
+-rw-r--r--   0     1001     1002    29388 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_channel_selector_offline_async.py
+-rw-r--r--   0     1001     1002    29249 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_channels.py
+-rw-r--r--   0     1001     1002    29944 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_for_data_object.py
+-rw-r--r--   0     1001     1002    29364 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_format.py
+-rw-r--r--   0     1001     1002    33795 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_input_async.py
+-rw-r--r--   0     1001     1002    30010 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_input_async_source.py
+-rw-r--r--   0     1001     1002    32932 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_input_base.py
+-rw-r--r--   0     1001     1002    29119 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_input_data.py
+-rw-r--r--   0     1001     1002    31301 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_input_data_all_of.py
+-rw-r--r--   0     1001     1002    31201 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_input_data_all_of_source.py
+-rw-r--r--   0     1001     1002    34758 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_input_sync.py
+-rw-r--r--   0     1001     1002    31017 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_input_sync_source.py
+-rw-r--r--   0     1001     1002    33976 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_resource_uri.py
+-rw-r--r--   0     1001     1002    29349 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_zone_class.py
+-rw-r--r--   0     1001     1002    31260 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/audio_zone_item.py
+-rw-r--r--   0     1001     1002    29790 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/basic_success_response.py
+-rw-r--r--   0     1001     1002    31292 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/builtin.py
+-rw-r--r--   0     1001     1002    31352 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/builtin_all_of.py
+-rw-r--r--   0     1001     1002    29631 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/call_attributes.py
+-rw-r--r--   0     1001     1002    34746 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/callback_req.py
+-rw-r--r--   0     1001     1002    31504 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/callback_req_reco.py
+-rw-r--r--   0     1001     1002    29918 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/callback_resp.py
+-rw-r--r--   0     1001     1002    33700 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/caption.py
+-rw-r--r--   0     1001     1002    30760 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/compliance_settings.py
+-rw-r--r--   0     1001     1002    29310 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/config_value_status.py
+-rw-r--r--   0     1001     1002    29367 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/content_type.py
+-rw-r--r--   0     1001     1002    32827 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/continuous_recognition.py
+-rw-r--r--   0     1001     1002    50044 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/core_aivr_session.py
+-rw-r--r--   0     1001     1002    39069 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/core_aivr_session_telco_data.py
+-rw-r--r--   0     1001     1002    29274 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/creating_entity.py
+-rw-r--r--   0     1001     1002    30959 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/criterion_config.py
+-rw-r--r--   0     1001     1002    30860 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/criterion_satisfied.py
+-rw-r--r--   0     1001     1002    29786 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/data_obj_ref.py
+-rw-r--r--   0     1001     1002    44311 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/data_object.py
+-rw-r--r--   0     1001     1002    29780 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/data_object_all_of.py
+-rw-r--r--   0     1001     1002    38308 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/data_object_base.py
+-rw-r--r--   0     1001     1002    34669 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/data_object_ids.py
+-rw-r--r--   0     1001     1002    44090 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/data_object_no_sos_ref.py
+-rw-r--r--   0     1001     1002    39281 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/data_object_with_audio.py
+-rw-r--r--   0     1001     1002    29724 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/debug_info.py
+-rw-r--r--   0     1001     1002    30330 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/debug_settings.py
+-rw-r--r--   0     1001     1002    32329 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/demo.py
+-rw-r--r--   0     1001     1002    32409 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/demo_all_of.py
+-rw-r--r--   0     1001     1002    30716 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/diarization_data.py
+-rw-r--r--   0     1001     1002    30585 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/diarization_zone.py
+-rw-r--r--   0     1001     1002    35781 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/diarization_zone_item.py
+-rw-r--r--   0     1001     1002    32447 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/disconnect.py
+-rw-r--r--   0     1001     1002    32527 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/disconnect_all_of.py
+-rw-r--r--   0     1001     1002    30779 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/error.py
+-rw-r--r--   0     1001     1002    30839 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/error_all_of.py
+-rw-r--r--   0     1001     1002    30827 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/error_info.py
+-rw-r--r--   0     1001     1002    31388 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/estimated_queue_wait.py
+-rw-r--r--   0     1001     1002    29329 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/experiment_platform.py
+-rw-r--r--   0     1001     1002    31802 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/file_location.py
+-rw-r--r--   0     1001     1002    35736 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/formatter.py
+-rw-r--r--   0     1001     1002    30704 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/grammar.py
+-rw-r--r--   0     1001     1002    30011 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg.py
+-rw-r--r--   0     1001     1002    30051 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_all_of.py
+-rw-r--r--   0     1001     1002    37162 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio.py
+-rw-r--r--   0     1001     1002    31027 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_all_of.py
+-rw-r--r--   0     1001     1002    32672 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_base.py
+-rw-r--r--   0     1001     1002    33677 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_base_with_audio.py
+-rw-r--r--   0     1001     1002    30017 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_id.py
+-rw-r--r--   0     1001     1002    30669 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_input.py
+-rw-r--r--   0     1001     1002    29999 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_input_audio_hash.py
+-rw-r--r--   0     1001     1002    29917 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_input_audio_id.py
+-rw-r--r--   0     1001     1002    29944 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_input_data.py
+-rw-r--r--   0     1001     1002    34024 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set.py
+-rw-r--r--   0     1001     1002    31347 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_base.py
+-rw-r--r--   0     1001     1002    31420 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_base_inclusive.py
+-rw-r--r--   0     1001     1002    32260 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_core.py
+-rw-r--r--   0     1001     1002    30024 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_id.py
+-rw-r--r--   0     1001     1002    32289 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_inclusive.py
+-rw-r--r--   0     1001     1002    32369 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_inclusive_core.py
+-rw-r--r--   0     1001     1002    32280 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_inner.py
+-rw-r--r--   0     1001     1002    31118 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_response.py
+-rw-r--r--   0     1001     1002    35486 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_thin.py
+-rw-r--r--   0     1001     1002    38630 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment.py
+-rw-r--r--   0     1001     1002    35987 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_base.py
+-rw-r--r--   0     1001     1002    34723 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_base_inclusive.py
+-rw-r--r--   0     1001     1002    31678 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_base_platform_data.py
+-rw-r--r--   0     1001     1002    30062 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_id.py
+-rw-r--r--   0     1001     1002    37490 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_inclusive.py
+-rw-r--r--   0     1001     1002    35661 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_modifiable.py
+-rw-r--r--   0     1001     1002    35285 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_platform_external_asr.py
+-rw-r--r--   0     1001     1002    30328 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_platform_upload.py
+-rw-r--r--   0     1001     1002    31040 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_platform_voicegain.py
+-rw-r--r--   0     1001     1002    31146 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_response.py
+-rw-r--r--   0     1001     1002    29430 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_status.py
+-rw-r--r--   0     1001     1002    29359 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_status_modifiable.py
+-rw-r--r--   0     1001     1002    34341 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_grammar.py
+-rw-r--r--   0     1001     1002    31613 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_grammar_base.py
+-rw-r--r--   0     1001     1002    30617 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_grammar_base_light.py
+-rw-r--r--   0     1001     1002    30079 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_grammar_id.py
+-rw-r--r--   0     1001     1002    31545 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_grammar_inner.py
+-rw-r--r--   0     1001     1002    33421 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_grammar_light.py
+-rw-r--r--   0     1001     1002    30730 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_interpretation.py
+-rw-r--r--   0     1001     1002    34960 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_question.py
+-rw-r--r--   0     1001     1002    32213 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_question_base.py
+-rw-r--r--   0     1001     1002    30110 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_question_id.py
+-rw-r--r--   0     1001     1002    33236 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_question_inner.py
+-rw-r--r--   0     1001     1002    30956 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py
+-rw-r--r--   0     1001     1002    33432 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py
+-rw-r--r--   0     1001     1002    30869 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py
+-rw-r--r--   0     1001     1002    30799 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py
+-rw-r--r--   0     1001     1002    30073 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_recog_base_with_exp.py
+-rw-r--r--   0     1001     1002    36922 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_recognition.py
+-rw-r--r--   0     1001     1002    34214 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_recognition_base.py
+-rw-r--r--   0     1001     1002    30091 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_recognition_id.py
+-rw-r--r--   0     1001     1002    29378 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_review_status.py
+-rw-r--r--   0     1001     1002    32341 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_source_of_truth.py
+-rw-r--r--   0     1001     1002    33215 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_truth_update.py
+-rw-r--r--   0     1001     1002    32975 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/greg_truth_updates.py
+-rw-r--r--   0     1001     1002    31960 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/grxml.py
+-rw-r--r--   0     1001     1002    32060 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/grxml_all_of.py
+-rw-r--r--   0     1001     1002    30469 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/gui_input.py
+-rw-r--r--   0     1001     1002    29087 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/hangup.py
+-rw-r--r--   0     1001     1002    29759 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/html_checkbox.py
+-rw-r--r--   0     1001     1002    31573 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/html_choice_item.py
+-rw-r--r--   0     1001     1002    29791 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/html_radio_buttons.py
+-rw-r--r--   0     1001     1002    29854 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/html_text_entry.py
+-rw-r--r--   0     1001     1002    29247 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/if_exists.py
+-rw-r--r--   0     1001     1002    33271 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/incident.py
+-rw-r--r--   0     1001     1002    29778 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/inline_data.py
+-rw-r--r--   0     1001     1002    30983 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/inline_object.py
+-rw-r--r--   0     1001     1002    30995 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/inline_object1.py
+-rw-r--r--   0     1001     1002    34398 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/input.py
+-rw-r--r--   0     1001     1002    34538 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/input_all_of.py
+-rw-r--r--   0     1001     1002    30698 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/integration.py
+-rw-r--r--   0     1001     1002    35874 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/jjsgf.py
+-rw-r--r--   0     1001     1002    36014 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/jjsgf_all_of.py
+-rw-r--r--   0     1001     1002    31165 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/keyword_spot_example.py
+-rw-r--r--   0     1001     1002    31150 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/keyword_spot_group.py
+-rw-r--r--   0     1001     1002    32893 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/keyword_spot_item.py
+-rw-r--r--   0     1001     1002    29371 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/lang_model_status.py
+-rw-r--r--   0     1001     1002    30147 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/language.py
+-rw-r--r--   0     1001     1002    39474 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/language_model_doc.py
+-rw-r--r--   0     1001     1002    37931 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/language_model_doc_modifiable.py
+-rw-r--r--   0     1001     1002    32689 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/language_model_src_data.py
+-rw-r--r--   0     1001     1002    29248 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/lm_type.py
+-rw-r--r--   0     1001     1002    29910 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/min_max_speakers.py
+-rw-r--r--   0     1001     1002    32751 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/min_max_speakers_diarization.py
+-rw-r--r--   0     1001     1002    29400 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/mood_type.py
+-rw-r--r--   0     1001     1002    31243 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/mrc_pv1_asr_settings.py
+-rw-r--r--   0     1001     1002    31216 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/mrc_pv2_asr_settings.py
+-rw-r--r--   0     1001     1002    29247 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/mrcp_version.py
+-rw-r--r--   0     1001     1002    31730 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/name_value_pair.py
+-rw-r--r--   0     1001     1002    30742 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/named_entity_concept.py
+-rw-r--r--   0     1001     1002    29842 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/named_entity_type.py
+-rw-r--r--   0     1001     1002    49627 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/new_speech_analytics_session.py
+-rw-r--r--   0     1001     1002    38041 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/new_speech_analytics_session_response.py
+-rw-r--r--   0     1001     1002    30074 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/new_speech_analytics_session_response_poll.py
+-rw-r--r--   0     1001     1002    29980 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/new_speech_analytics_session_response_websocket.py
+-rw-r--r--   0     1001     1002    30628 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/non_session_error_response.py
+-rw-r--r--   0     1001     1002    29167 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/non_session_error_response400.py
+-rw-r--r--   0     1001     1002    29167 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/non_session_error_response401.py
+-rw-r--r--   0     1001     1002    32061 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/output.py
+-rw-r--r--   0     1001     1002    32141 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/output_all_of.py
+-rw-r--r--   0     1001     1002    34343 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/overtalk.py
+-rw-r--r--   0     1001     1002    32535 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/phone_audio_input.py
+-rw-r--r--   0     1001     1002    30753 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/phone_audio_input_prompt.py
+-rw-r--r--   0     1001     1002    33384 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/phrase_spot_example.py
+-rw-r--r--   0     1001     1002    33250 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/phrase_spot_group.py
+-rw-r--r--   0     1001     1002    40893 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/phrase_spot_item.py
+-rw-r--r--   0     1001     1002    32214 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/phrase_spot_item_location.py
+-rw-r--r--   0     1001     1002    31994 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/phrase_spot_item_location_dialogue.py
+-rw-r--r--   0     1001     1002    30854 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/phrase_spot_item_slots.py
+-rw-r--r--   0     1001     1002    32790 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/pii_redaction_conf.py
+-rw-r--r--   0     1001     1002    32799 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/poll_req.py
+-rw-r--r--   0     1001     1002    33368 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/poll_resp.py
+-rw-r--r--   0     1001     1002    32658 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/portal_output_init.py
+-rw-r--r--   0     1001     1002    30127 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/pre_fetch.py
+-rw-r--r--   0     1001     1002    40796 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/progress.py
+-rw-r--r--   0     1001     1002    31612 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/progress_callback.py
+-rw-r--r--   0     1001     1002    29534 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/progress_phase.py
+-rw-r--r--   0     1001     1002    32656 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/quartiles_energy.py
+-rw-r--r--   0     1001     1002    32632 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/quartiles_pitch.py
+-rw-r--r--   0     1001     1002    34441 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/reco_alt.py
+-rw-r--r--   0     1001     1002    31642 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/recog_nlsml.py
+-rw-r--r--   0     1001     1002    30812 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/recog_nlsml_no_exp.py
+-rw-r--r--   0     1001     1002    33906 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/recog_obj.py
+-rw-r--r--   0     1001     1002    33144 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/recog_obj_no_exp.py
+-rw-r--r--   0     1001     1002    33805 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/recognition_result.py
+-rw-r--r--   0     1001     1002    33632 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/requested_content.py
+-rw-r--r--   0     1001     1002    32832 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/resource_uri.py
+-rw-r--r--   0     1001     1002    34984 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/s3.py
+-rw-r--r--   0     1001     1002    35144 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/s3_all_of.py
+-rw-r--r--   0     1001     1002    34848 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/s3_audio_input.py
+-rw-r--r--   0     1001     1002    31352 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/s3_metadata_mapping.py
+-rw-r--r--   0     1001     1002    31130 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/s3_tag_mapping.py
+-rw-r--r--   0     1001     1002    29264 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/sa_conf_type.py
+-rw-r--r--   0     1001     1002    29383 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/sample_rate.py
+-rw-r--r--   0     1001     1002    29960 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/session_content.py
+-rw-r--r--   0     1001     1002    31472 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/session_error_response.py
+-rw-r--r--   0     1001     1002    37488 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/session_init_recognition.py
+-rw-r--r--   0     1001     1002    39730 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/session_init_transcription.py
+-rw-r--r--   0     1001     1002    32892 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/session_init_transcription_diarization.py
+-rw-r--r--   0     1001     1002    30694 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/session_success_response.py
+-rw-r--r--   0     1001     1002    35303 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/settings_async_transcription.py
+-rw-r--r--   0     1001     1002    32224 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/settings_recognition.py
+-rw-r--r--   0     1001     1002    32197 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/settings_sync_transcription.py
+-rw-r--r--   0     1001     1002    34209 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/silence.py
+-rw-r--r--   0     1001     1002    30855 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/slot_entity.py
+-rw-r--r--   0     1001     1002    30802 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/slot_keyword.py
+-rw-r--r--   0     1001     1002    30889 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/sos_ref.py
+-rw-r--r--   0     1001     1002    33548 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speaker_result.py
+-rw-r--r--   0     1001     1002    44356 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_base_result.py
+-rw-r--r--   0     1001     1002    32031 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_channel.py
+-rw-r--r--   0     1001     1002    45729 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_channel_result.py
+-rw-r--r--   0     1001     1002    34015 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_channel_with_transcribe.py
+-rw-r--r--   0     1001     1002    70655 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config.py
+-rw-r--r--   0     1001     1002    34473 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config_identifying.py
+-rw-r--r--   0     1001     1002    67930 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config_modifiable.py
+-rw-r--r--   0     1001     1002    66650 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config_modifiable_base.py
+-rw-r--r--   0     1001     1002    31340 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py
+-rw-r--r--   0     1001     1002    30883 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config_name_optional.py
+-rw-r--r--   0     1001     1002    31037 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config_name_required.py
+-rw-r--r--   0     1001     1002    50083 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_core_result.py
+-rw-r--r--   0     1001     1002    35010 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_core_result_all_of.py
+-rw-r--r--   0     1001     1002    30949 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_criteria_data.py
+-rw-r--r--   0     1001     1002    31414 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_emotion.py
+-rw-r--r--   0     1001     1002    30617 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_emotion_data.py
+-rw-r--r--   0     1001     1002    36738 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_emotion_item.py
+-rw-r--r--   0     1001     1002    30663 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_keyword.py
+-rw-r--r--   0     1001     1002    30953 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_keyword_data.py
+-rw-r--r--   0     1001     1002    35987 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_keyword_item.py
+-rw-r--r--   0     1001     1002    36239 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py
+-rw-r--r--   0     1001     1002    31633 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_named_entity.py
+-rw-r--r--   0     1001     1002    37037 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_named_entity_item.py
+-rw-r--r--   0     1001     1002    37325 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py
+-rw-r--r--   0     1001     1002    32719 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase.py
+-rw-r--r--   0     1001     1002    30936 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_data.py
+-rw-r--r--   0     1001     1002    30762 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_group.py
+-rw-r--r--   0     1001     1002    31035 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_group_data.py
+-rw-r--r--   0     1001     1002    36150 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_group_item.py
+-rw-r--r--   0     1001     1002    38059 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_item.py
+-rw-r--r--   0     1001     1002    39459 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py
+-rw-r--r--   0     1001     1002    30833 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_slots.py
+-rw-r--r--   0     1001     1002    61063 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_result.py
+-rw-r--r--   0     1001     1002    46390 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_result_detail.py
+-rw-r--r--   0     1001     1002    30848 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_session_modifiable.py
+-rw-r--r--   0     1001     1002    37783 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_session_poll_response.py
+-rw-r--r--   0     1001     1002    31485 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/start_end_time_for_sub_criterion.py
+-rw-r--r--   0     1001     1002    30171 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/stomp_ping.py
+-rw-r--r--   0     1001     1002    30948 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/stomp_word_correction.py
+-rw-r--r--   0     1001     1002    35009 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/stomp_ws_word.py
+-rw-r--r--   0     1001     1002    35377 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/stream_resp.py
+-rw-r--r--   0     1001     1002    32938 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/stream_setup.py
+-rw-r--r--   0     1001     1002    29391 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/streaming_protocol.py
+-rw-r--r--   0     1001     1002    38570 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/sub_criterion_config.py
+-rw-r--r--   0     1001     1002    40956 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/sub_criterion_satisfied.py
+-rw-r--r--   0     1001     1002    31931 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/sync_audio_input_source.py
+-rw-r--r--   0     1001     1002    30879 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/sync_recognition_request.py
+-rw-r--r--   0     1001     1002    32444 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/sync_recognition_response.py
+-rw-r--r--   0     1001     1002    30047 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/sync_session_established.py
+-rw-r--r--   0     1001     1002    30763 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/sync_transcription_request.py
+-rw-r--r--   0     1001     1002    32502 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/sync_transcription_response.py
+-rw-r--r--   0     1001     1002    32941 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/sync_transcription_result.py
+-rw-r--r--   0     1001     1002    38657 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/talk_time.py
+-rw-r--r--   0     1001     1002    31188 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/topic_score.py
+-rw-r--r--   0     1001     1002    29287 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/training_set_bucket_type.py
+-rw-r--r--   0     1001     1002    38929 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/training_set_doc.py
+-rw-r--r--   0     1001     1002    30847 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/training_set_doc_defaults.py
+-rw-r--r--   0     1001     1002    36307 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/training_set_doc_statistics.py
+-rw-r--r--   0     1001     1002    34381 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/training_set_key.py
+-rw-r--r--   0     1001     1002    33631 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/training_set_modifiable.py
+-rw-r--r--   0     1001     1002    29379 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/training_set_status.py
+-rw-r--r--   0     1001     1002    29419 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/training_set_status_modifiable.py
+-rw-r--r--   0     1001     1002    29307 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/training_set_store_type.py
+-rw-r--r--   0     1001     1002    31549 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/transcribe_alt.py
+-rw-r--r--   0     1001     1002    30831 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/transcribe_session_id.py
+-rw-r--r--   0     1001     1002    33849 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/transcribe_session_modify_request.py
+-rw-r--r--   0     1001     1002    31526 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/transcribe_session_modify_request_mute.py
+-rw-r--r--   0     1001     1002    30354 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/transcribe_session_modify_request_pause.py
+-rw-r--r--   0     1001     1002    34383 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/transcript_position_range.py
+-rw-r--r--   0     1001     1002    34563 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/transcript_position_range_for_phrase.py
+-rw-r--r--   0     1001     1002    35799 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py
+-rw-r--r--   0     1001     1002    36120 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/transfer.py
+-rw-r--r--   0     1001     1002    36260 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/transfer_all_of.py
+-rw-r--r--   0     1001     1002    29303 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/vad_mode.py
+-rw-r--r--   0     1001     1002    32108 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/version.py
+-rw-r--r--   0     1001     1002    37760 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/websocket.py
+-rw-r--r--   0     1001     1002    38351 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/websocket_init.py
+-rw-r--r--   0     1001     1002    30321 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/websocket_init_reco.py
+-rw-r--r--   0     1001     1002    35916 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/websocket_modifiable.py
+-rw-r--r--   0     1001     1002    32384 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/websocket_msg.py
+-rw-r--r--   0     1001     1002    29250 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/websocket_protocol.py
+-rw-r--r--   0     1001     1002    30725 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/websocket_resp.py
+-rw-r--r--   0     1001     1002    30082 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/word_alternatives.py
+-rw-r--r--   0     1001     1002    31262 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/word_cloud_item.py
+-rw-r--r--   0     1001     1002    31103 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/word_correction.py
+-rw-r--r--   0     1001     1002    36113 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/word_item_timed.py
+-rw-r--r--   0     1001     1002    31188 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/word_item_timing.py
+-rw-r--r--   0     1001     1002    30443 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/word_tree_ids.py
+-rw-r--r--   0     1001     1002    36490 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/word_tree_item.py
+-rw-r--r--   0     1001     1002    33045 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/words_item.py
+-rw-r--r--   0     1001     1002    36348 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/words_section.py
+-rw-r--r--   0     1001     1002    32894 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/words_section_meta.py
+-rw-r--r--   0     1001     1002    31896 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/words_section_meta_mc.py
+-rw-r--r--   0     1001     1002    33875 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/words_section_single_column.py
+-rw-r--r--   0     1001     1002    29956 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/words_section_words.py
+-rw-r--r--   0     1001     1002    38086 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/models/words_websocket_item.py
+-rw-r--r--   0     1001     1002    38926 2023-04-20 20:01:29.000000 voicegain-speech-1.82.0/voicegain_speech/rest.py
+drwxr-xr-x   0     1001     1002        0 2023-04-20 20:01:31.986720 voicegain-speech-1.82.0/voicegain_speech.egg-info/
+-rw-r--r--   0     1001     1002     2923 2023-04-20 20:01:31.000000 voicegain-speech-1.82.0/voicegain_speech.egg-info/PKG-INFO
+-rw-r--r--   0     1001     1002    20760 2023-04-20 20:01:31.000000 voicegain-speech-1.82.0/voicegain_speech.egg-info/SOURCES.txt
+-rw-r--r--   0     1001     1002        1 2023-04-20 20:01:31.000000 voicegain-speech-1.82.0/voicegain_speech.egg-info/dependency_links.txt
+-rw-r--r--   0     1001     1002       48 2023-04-20 20:01:31.000000 voicegain-speech-1.82.0/voicegain_speech.egg-info/requires.txt
+-rw-r--r--   0     1001     1002       17 2023-04-20 20:01:31.000000 voicegain-speech-1.82.0/voicegain_speech.egg-info/top_level.txt
```

### Comparing `voicegain-speech-1.81.0/LICENSE` & `voicegain-speech-1.82.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/PKG-INFO` & `voicegain-speech-1.82.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: voicegain-speech
-Version: 1.81.0
+Version: 1.82.0
 Summary: Voicegain Speech-to-Text Python SDK
 Home-page: UNKNOWN
 Author: Huishen Zhan, Kuo Zhang, Jacek Jarmulak
 Author-email: huishen@voicegain.ai, kuo@voicegain.ai, jacek@voicegain.ai
 License: UNKNOWN
-Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.81.0.tar.gz
+Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.82.0.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Voicegain Speech-to-Text Python SDK
 
 Python SDK for the [Voicegain](https://www.voicegain.ai) [Speech-to-Text API](https://portal.voicegain.ai/api/v1/index.html).
```

### Comparing `voicegain-speech-1.81.0/README.md` & `voicegain-speech-1.82.0/README.md`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/setup.py` & `voicegain-speech-1.82.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 REQUIRES = ["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil"]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="voicegain-speech",
-    version="1.81.0",
+    version="1.82.0",
     author="Huishen Zhan, Kuo Zhang, Jacek Jarmulak",
     author_email="huishen@voicegain.ai, kuo@voicegain.ai, jacek@voicegain.ai",
     description="Voicegain Speech-to-Text Python SDK",
-    download_url='https://github.com/voicegain/python-sdk/archive/refs/tags/1.81.0.tar.gz',
+    download_url='https://github.com/voicegain/python-sdk/archive/refs/tags/1.82.0.tar.gz',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=REQUIRES,
     packages=setuptools.find_packages(),
     include_package_data=True,
 )
```

### Comparing `voicegain-speech-1.81.0/voicegain_speech/__init__.py` & `voicegain-speech-1.82.0/voicegain_speech/__init__.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/__init__.py` & `voicegain-speech-1.82.0/voicegain_speech/api/__init__.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/aivr_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/aivr_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/aivr_callback_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/aivr_callback_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/asr_callback_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/asr_callback_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/audiocodes_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/audiocodes_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/data_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/data_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/greg_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/greg_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/lm_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/lm_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/recognize_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/recognize_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/sa_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/sa_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/security_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/security_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/training_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/training_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/transcribe_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/transcribe_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api/websocket_api.py` & `voicegain-speech-1.82.0/voicegain_speech/api/websocket_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/api_client.py` & `voicegain-speech-1.82.0/voicegain_speech/api_client.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/configuration.py` & `voicegain-speech-1.82.0/voicegain_speech/configuration.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/exceptions.py` & `voicegain-speech-1.82.0/voicegain_speech/exceptions.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/__init__.py` & `voicegain-speech-1.82.0/voicegain_speech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/ac_control_messages.py` & `voicegain-speech-1.82.0/voicegain_speech/models/ac_control_messages.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/ac_end.py` & `voicegain-speech-1.82.0/voicegain_speech/models/ac_end.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/ac_error.py` & `voicegain-speech-1.82.0/voicegain_speech/models/ac_error.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/ac_hypothesis.py` & `voicegain-speech-1.82.0/voicegain_speech/models/ac_hypothesis.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/ac_hypothesis_alternatives.py` & `voicegain-speech-1.82.0/voicegain_speech/models/ac_hypothesis_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/ac_recognition.py` & `voicegain-speech-1.82.0/voicegain_speech/models/ac_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/ac_recognition_alternatives.py` & `voicegain-speech-1.82.0/voicegain_speech/models/ac_recognition_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/ac_response_messages.py` & `voicegain-speech-1.82.0/voicegain_speech/models/ac_response_messages.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/ac_start.py` & `voicegain-speech-1.82.0/voicegain_speech/models/ac_start.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/ac_start_stt_speech_contexts.py` & `voicegain-speech-1.82.0/voicegain_speech/models/ac_start_stt_speech_contexts.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/ac_started.py` & `voicegain-speech-1.82.0/voicegain_speech/models/ac_started.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/ac_stop.py` & `voicegain-speech-1.82.0/voicegain_speech/models/ac_stop.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/account_and_context_id.py` & `voicegain-speech-1.82.0/voicegain_speech/models/account_and_context_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/advanced_regex.py` & `voicegain-speech-1.82.0/voicegain_speech/models/advanced_regex.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aircall.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aircall.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aircall_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aircall_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_callback_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_callback_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_callback_response_final.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_callback_response_final.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_conference_transfer.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_conference_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_disconnect.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_disconnect.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_event.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_event.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_event_type.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_event_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_existing_session.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_existing_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_logic.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_logic.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_logic_media.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_logic_media.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_logic_transfer.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_logic_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_logic_type.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_logic_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_new_session.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_new_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_phone_transfer.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_phone_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_prompt.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_prompt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_prompt_completion.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_prompt_completion.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_prompt_playing.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_prompt_playing.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_prompt_properties_audio.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_prompt_properties_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_prompt_properties_html.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_prompt_properties_html.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_question.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_question.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_recognition_result.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_recording.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_recording.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_response_properties_audio.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_response_properties_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_response_properties_html.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_response_properties_html.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_session_user.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_session_user.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_session_user_base.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_session_user_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_session_user_fs.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_session_user_fs.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivr_transfer.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivr_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/aivrs_question_specifics.py` & `voicegain-speech-1.82.0/voicegain_speech/models/aivrs_question_specifics.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_processing_event.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_processing_event.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_processing_status.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_processing_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_processing_status_additional.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_processing_status_additional.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_processing_status_after_input_started.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_processing_status_after_input_started.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_processing_status_for_callback.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_processing_status_for_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_recognition_result.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_common.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_common.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_recognition.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_recognition_defaults.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_recognition_defaults.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_recognition_grammars_etc.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_recognition_grammars_etc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_recognition_timeouts.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_recognition_timeouts.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_async.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_async.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_async_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_async_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_common.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_common.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_common_lm.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_common_lm.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_default_timeouts.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_default_timeouts.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_defaults.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_defaults.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_sa.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_sa.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_speakers.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_speakers.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py` & `voicegain-speech-1.82.0/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_audio_input_source.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_audio_input_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_mode.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_mode.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_mode_recognition.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_mode_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_mode_speech_analytics.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_mode_speech_analytics.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_mode_transcription.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_mode_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_post_response_base.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_post_response_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_post_response_base_audio.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_post_response_base_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_reco_post_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_reco_post_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_reco_post_response_sessions.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_reco_post_response_sessions.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_recognition_callback_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_recognition_callback_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_recognition_request.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_recognition_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_recognition_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_recognition_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_recognition_result.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_recognition_result_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_recognition_result_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_result_full.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_result_full.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_result_full_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_result_full_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_result_full_all_of_audio.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_result_full_all_of_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_result_full_all_of_audio_source.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_result_full_all_of_audio_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_result_full_all_of_result.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_result_full_all_of_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_result_incremental.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_result_incremental.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_result_incremental_detail.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_result_incremental_detail.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_result_incremental_detail_control_status.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_result_incremental_detail_control_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_result_incremental_detail_result.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_result_incremental_detail_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_session_established.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_session_established.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_session_short_info.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_session_short_info.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_session_url.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_session_url.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_transc_post_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_transc_post_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_transc_post_response_sessions.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_transc_post_response_sessions.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_transc_session_established.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_transc_session_established.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_transcription_callback_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_transcription_callback_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_transcription_request.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_transcription_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_transcription_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_transcription_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/async_transcription_response_shared.py` & `voicegain-speech-1.82.0/voicegain_speech/models/async_transcription_response_shared.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_channel.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_channel.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_channel_selector.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_channel_selector.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_channel_selector_offline_async.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_channel_selector_offline_async.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_channels.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_channels.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_for_data_object.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_for_data_object.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_format.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_format.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_input_async.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_input_async.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_input_async_source.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_input_async_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_input_base.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_input_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_input_data.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_input_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_input_data_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_input_data_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_input_data_all_of_source.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_input_data_all_of_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_input_sync.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_input_sync.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_input_sync_source.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_input_sync_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_resource_uri.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_resource_uri.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_zone_class.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_zone_class.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/audio_zone_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/audio_zone_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/basic_success_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/basic_success_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/builtin.py` & `voicegain-speech-1.82.0/voicegain_speech/models/builtin.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/builtin_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/builtin_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/call_attributes.py` & `voicegain-speech-1.82.0/voicegain_speech/models/call_attributes.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/callback_req.py` & `voicegain-speech-1.82.0/voicegain_speech/models/callback_req.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/callback_req_reco.py` & `voicegain-speech-1.82.0/voicegain_speech/models/callback_req_reco.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/callback_resp.py` & `voicegain-speech-1.82.0/voicegain_speech/models/callback_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/caption.py` & `voicegain-speech-1.82.0/voicegain_speech/models/caption.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/compliance_settings.py` & `voicegain-speech-1.82.0/voicegain_speech/models/compliance_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/config_value_status.py` & `voicegain-speech-1.82.0/voicegain_speech/models/config_value_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/content_type.py` & `voicegain-speech-1.82.0/voicegain_speech/models/content_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/continuous_recognition.py` & `voicegain-speech-1.82.0/voicegain_speech/models/continuous_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/core_aivr_session.py` & `voicegain-speech-1.82.0/voicegain_speech/models/core_aivr_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/core_aivr_session_telco_data.py` & `voicegain-speech-1.82.0/voicegain_speech/models/core_aivr_session_telco_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/creating_entity.py` & `voicegain-speech-1.82.0/voicegain_speech/models/creating_entity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/criterion_config.py` & `voicegain-speech-1.82.0/voicegain_speech/models/criterion_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/criterion_satisfied.py` & `voicegain-speech-1.82.0/voicegain_speech/models/criterion_satisfied.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/data_obj_ref.py` & `voicegain-speech-1.82.0/voicegain_speech/models/data_obj_ref.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/data_object.py` & `voicegain-speech-1.82.0/voicegain_speech/models/data_object.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/data_object_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/data_object_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/data_object_base.py` & `voicegain-speech-1.82.0/voicegain_speech/models/data_object_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/data_object_ids.py` & `voicegain-speech-1.82.0/voicegain_speech/models/data_object_ids.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/data_object_no_sos_ref.py` & `voicegain-speech-1.82.0/voicegain_speech/models/data_object_no_sos_ref.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/data_object_with_audio.py` & `voicegain-speech-1.82.0/voicegain_speech/models/data_object_with_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/debug_info.py` & `voicegain-speech-1.82.0/voicegain_speech/models/debug_info.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/debug_settings.py` & `voicegain-speech-1.82.0/voicegain_speech/models/debug_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/demo.py` & `voicegain-speech-1.82.0/voicegain_speech/models/demo.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/demo_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/demo_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/diarization_data.py` & `voicegain-speech-1.82.0/voicegain_speech/models/diarization_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/diarization_zone.py` & `voicegain-speech-1.82.0/voicegain_speech/models/diarization_zone.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/diarization_zone_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/diarization_zone_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/disconnect.py` & `voicegain-speech-1.82.0/voicegain_speech/models/disconnect.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/disconnect_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/disconnect_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/error.py` & `voicegain-speech-1.82.0/voicegain_speech/models/error.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/error_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/error_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/error_info.py` & `voicegain-speech-1.82.0/voicegain_speech/models/error_info.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/estimated_queue_wait.py` & `voicegain-speech-1.82.0/voicegain_speech/models/estimated_queue_wait.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/experiment_platform.py` & `voicegain-speech-1.82.0/voicegain_speech/models/experiment_platform.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/file_location.py` & `voicegain-speech-1.82.0/voicegain_speech/models/file_location.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/formatter.py` & `voicegain-speech-1.82.0/voicegain_speech/models/formatter.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/grammar.py` & `voicegain-speech-1.82.0/voicegain_speech/models/grammar.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_base.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_base_with_audio.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_base_with_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_id.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_input.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_input_audio_hash.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_input_audio_hash.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_input_audio_id.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_input_audio_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_input_data.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_input_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_base.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_base_inclusive.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_base_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_core.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_id.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_inclusive.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_inclusive_core.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_inclusive_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_inner.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_inner.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_set_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_set_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_audio_thin.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_audio_thin.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_base.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_base_inclusive.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_base_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_base_platform_data.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_base_platform_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_id.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_inclusive.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_modifiable.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_platform_external_asr.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_platform_external_asr.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_platform_upload.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_platform_upload.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_platform_voicegain.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_platform_voicegain.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_status.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_experiment_status_modifiable.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_experiment_status_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_grammar.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_grammar.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_grammar_base.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_grammar_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_grammar_base_light.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_grammar_base_light.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_grammar_id.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_grammar_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_grammar_inner.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_grammar_inner.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_grammar_light.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_grammar_light.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_interpretation.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_interpretation.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_question.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_question.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_question_base.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_question_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_question_id.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_question_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_question_inner.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_question_inner.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_recog_base_with_exp.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_recog_base_with_exp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_recognition.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_recognition_base.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_recognition_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_recognition_id.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_recognition_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_review_status.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_review_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_source_of_truth.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_source_of_truth.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_truth_update.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_truth_update.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/greg_truth_updates.py` & `voicegain-speech-1.82.0/voicegain_speech/models/greg_truth_updates.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/grxml.py` & `voicegain-speech-1.82.0/voicegain_speech/models/grxml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/grxml_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/grxml_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/gui_input.py` & `voicegain-speech-1.82.0/voicegain_speech/models/gui_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/hangup.py` & `voicegain-speech-1.82.0/voicegain_speech/models/hangup.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/html_checkbox.py` & `voicegain-speech-1.82.0/voicegain_speech/models/html_checkbox.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/html_choice_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/html_choice_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/html_radio_buttons.py` & `voicegain-speech-1.82.0/voicegain_speech/models/html_radio_buttons.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/html_text_entry.py` & `voicegain-speech-1.82.0/voicegain_speech/models/html_text_entry.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/if_exists.py` & `voicegain-speech-1.82.0/voicegain_speech/models/if_exists.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/incident.py` & `voicegain-speech-1.82.0/voicegain_speech/models/incident.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/inline_data.py` & `voicegain-speech-1.82.0/voicegain_speech/models/inline_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/inline_object.py` & `voicegain-speech-1.82.0/voicegain_speech/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/inline_object1.py` & `voicegain-speech-1.82.0/voicegain_speech/models/inline_object1.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/input.py` & `voicegain-speech-1.82.0/voicegain_speech/models/input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/input_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/input_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/integration.py` & `voicegain-speech-1.82.0/voicegain_speech/models/integration.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/jjsgf.py` & `voicegain-speech-1.82.0/voicegain_speech/models/jjsgf.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/jjsgf_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/jjsgf_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/keyword_spot_example.py` & `voicegain-speech-1.82.0/voicegain_speech/models/keyword_spot_example.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/keyword_spot_group.py` & `voicegain-speech-1.82.0/voicegain_speech/models/keyword_spot_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/keyword_spot_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/keyword_spot_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/lang_model_status.py` & `voicegain-speech-1.82.0/voicegain_speech/models/lang_model_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/language.py` & `voicegain-speech-1.82.0/voicegain_speech/models/language.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/language_model_doc.py` & `voicegain-speech-1.82.0/voicegain_speech/models/language_model_doc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/language_model_doc_modifiable.py` & `voicegain-speech-1.82.0/voicegain_speech/models/language_model_doc_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/language_model_src_data.py` & `voicegain-speech-1.82.0/voicegain_speech/models/language_model_src_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/lm_type.py` & `voicegain-speech-1.82.0/voicegain_speech/models/lm_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/min_max_speakers.py` & `voicegain-speech-1.82.0/voicegain_speech/models/min_max_speakers.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/min_max_speakers_diarization.py` & `voicegain-speech-1.82.0/voicegain_speech/models/min_max_speakers_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/mood_type.py` & `voicegain-speech-1.82.0/voicegain_speech/models/mood_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/mrc_pv1_asr_settings.py` & `voicegain-speech-1.82.0/voicegain_speech/models/mrc_pv1_asr_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/mrc_pv2_asr_settings.py` & `voicegain-speech-1.82.0/voicegain_speech/models/mrc_pv2_asr_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/mrcp_version.py` & `voicegain-speech-1.82.0/voicegain_speech/models/mrcp_version.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/name_value_pair.py` & `voicegain-speech-1.82.0/voicegain_speech/models/name_value_pair.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/named_entity_concept.py` & `voicegain-speech-1.82.0/voicegain_speech/models/named_entity_concept.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/named_entity_type.py` & `voicegain-speech-1.82.0/voicegain_speech/models/named_entity_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/new_speech_analytics_session.py` & `voicegain-speech-1.82.0/voicegain_speech/models/new_speech_analytics_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/new_speech_analytics_session_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/new_speech_analytics_session_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/new_speech_analytics_session_response_poll.py` & `voicegain-speech-1.82.0/voicegain_speech/models/new_speech_analytics_session_response_poll.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/new_speech_analytics_session_response_websocket.py` & `voicegain-speech-1.82.0/voicegain_speech/models/new_speech_analytics_session_response_websocket.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/non_session_error_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/non_session_error_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/non_session_error_response400.py` & `voicegain-speech-1.82.0/voicegain_speech/models/non_session_error_response400.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/non_session_error_response401.py` & `voicegain-speech-1.82.0/voicegain_speech/models/non_session_error_response401.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/output.py` & `voicegain-speech-1.82.0/voicegain_speech/models/output.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/output_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/output_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/overtalk.py` & `voicegain-speech-1.82.0/voicegain_speech/models/overtalk.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/phone_audio_input.py` & `voicegain-speech-1.82.0/voicegain_speech/models/phone_audio_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/phone_audio_input_prompt.py` & `voicegain-speech-1.82.0/voicegain_speech/models/phone_audio_input_prompt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/phrase_spot_example.py` & `voicegain-speech-1.82.0/voicegain_speech/models/phrase_spot_example.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/phrase_spot_group.py` & `voicegain-speech-1.82.0/voicegain_speech/models/phrase_spot_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/phrase_spot_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/phrase_spot_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/phrase_spot_item_location.py` & `voicegain-speech-1.82.0/voicegain_speech/models/phrase_spot_item_location.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/phrase_spot_item_location_dialogue.py` & `voicegain-speech-1.82.0/voicegain_speech/models/phrase_spot_item_location_dialogue.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/phrase_spot_item_slots.py` & `voicegain-speech-1.82.0/voicegain_speech/models/phrase_spot_item_slots.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/pii_redaction_conf.py` & `voicegain-speech-1.82.0/voicegain_speech/models/pii_redaction_conf.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/poll_req.py` & `voicegain-speech-1.82.0/voicegain_speech/models/poll_req.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/poll_resp.py` & `voicegain-speech-1.82.0/voicegain_speech/models/poll_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/portal_output_init.py` & `voicegain-speech-1.82.0/voicegain_speech/models/portal_output_init.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/pre_fetch.py` & `voicegain-speech-1.82.0/voicegain_speech/models/pre_fetch.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/progress.py` & `voicegain-speech-1.82.0/voicegain_speech/models/progress.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/progress_callback.py` & `voicegain-speech-1.82.0/voicegain_speech/models/progress_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/progress_phase.py` & `voicegain-speech-1.82.0/voicegain_speech/models/progress_phase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/quartiles_energy.py` & `voicegain-speech-1.82.0/voicegain_speech/models/quartiles_energy.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/quartiles_pitch.py` & `voicegain-speech-1.82.0/voicegain_speech/models/quartiles_pitch.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/reco_alt.py` & `voicegain-speech-1.82.0/voicegain_speech/models/reco_alt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/recog_nlsml.py` & `voicegain-speech-1.82.0/voicegain_speech/models/recog_nlsml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/recog_nlsml_no_exp.py` & `voicegain-speech-1.82.0/voicegain_speech/models/recog_nlsml_no_exp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/recog_obj.py` & `voicegain-speech-1.82.0/voicegain_speech/models/recog_obj.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/recog_obj_no_exp.py` & `voicegain-speech-1.82.0/voicegain_speech/models/recog_obj_no_exp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/recognition_result.py` & `voicegain-speech-1.82.0/voicegain_speech/models/recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/requested_content.py` & `voicegain-speech-1.82.0/voicegain_speech/models/requested_content.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/resource_uri.py` & `voicegain-speech-1.82.0/voicegain_speech/models/resource_uri.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/s3.py` & `voicegain-speech-1.82.0/voicegain_speech/models/s3.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/s3_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/s3_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/s3_audio_input.py` & `voicegain-speech-1.82.0/voicegain_speech/models/s3_audio_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/s3_metadata_mapping.py` & `voicegain-speech-1.82.0/voicegain_speech/models/s3_metadata_mapping.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/s3_tag_mapping.py` & `voicegain-speech-1.82.0/voicegain_speech/models/s3_tag_mapping.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/sa_conf_type.py` & `voicegain-speech-1.82.0/voicegain_speech/models/sa_conf_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/sample_rate.py` & `voicegain-speech-1.82.0/voicegain_speech/models/sample_rate.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/session_content.py` & `voicegain-speech-1.82.0/voicegain_speech/models/session_content.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/session_error_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/session_error_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/session_init_recognition.py` & `voicegain-speech-1.82.0/voicegain_speech/models/session_init_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/session_init_transcription.py` & `voicegain-speech-1.82.0/voicegain_speech/models/session_init_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/session_init_transcription_diarization.py` & `voicegain-speech-1.82.0/voicegain_speech/models/session_init_transcription_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/session_success_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/session_success_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/settings_async_transcription.py` & `voicegain-speech-1.82.0/voicegain_speech/models/settings_async_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/settings_recognition.py` & `voicegain-speech-1.82.0/voicegain_speech/models/settings_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/settings_sync_transcription.py` & `voicegain-speech-1.82.0/voicegain_speech/models/settings_sync_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/silence.py` & `voicegain-speech-1.82.0/voicegain_speech/models/silence.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/slot_entity.py` & `voicegain-speech-1.82.0/voicegain_speech/models/slot_entity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/slot_keyword.py` & `voicegain-speech-1.82.0/voicegain_speech/models/slot_keyword.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/sos_ref.py` & `voicegain-speech-1.82.0/voicegain_speech/models/sos_ref.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speaker_result.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speaker_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_base_result.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_base_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_channel.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_channel.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_channel_result.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_channel_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_channel_with_transcribe.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_channel_with_transcribe.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config_identifying.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config_identifying.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config_modifiable.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config_modifiable_base.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config_modifiable_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config_name_optional.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config_name_optional.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_config_name_required.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_config_name_required.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_core_result.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_core_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_core_result_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_core_result_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_criteria_data.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_criteria_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_emotion.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_emotion.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_emotion_data.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_emotion_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_emotion_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_emotion_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_keyword.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_keyword.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_keyword_data.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_keyword_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_keyword_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_keyword_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_named_entity.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_named_entity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_named_entity_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_named_entity_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_data.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_group.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_group_data.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_group_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_group_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_group_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_phrase_slots.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_phrase_slots.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_result.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_result_detail.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_result_detail.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_session_modifiable.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_session_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/speech_analytics_session_poll_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/speech_analytics_session_poll_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/start_end_time_for_sub_criterion.py` & `voicegain-speech-1.82.0/voicegain_speech/models/start_end_time_for_sub_criterion.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/stomp_ping.py` & `voicegain-speech-1.82.0/voicegain_speech/models/stomp_ping.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/stomp_word_correction.py` & `voicegain-speech-1.82.0/voicegain_speech/models/stomp_word_correction.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/stomp_ws_word.py` & `voicegain-speech-1.82.0/voicegain_speech/models/stomp_ws_word.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/stream_resp.py` & `voicegain-speech-1.82.0/voicegain_speech/models/stream_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/stream_setup.py` & `voicegain-speech-1.82.0/voicegain_speech/models/stream_setup.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/streaming_protocol.py` & `voicegain-speech-1.82.0/voicegain_speech/models/streaming_protocol.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/sub_criterion_config.py` & `voicegain-speech-1.82.0/voicegain_speech/models/sub_criterion_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/sub_criterion_satisfied.py` & `voicegain-speech-1.82.0/voicegain_speech/models/sub_criterion_satisfied.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/sync_audio_input_source.py` & `voicegain-speech-1.82.0/voicegain_speech/models/sync_audio_input_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/sync_recognition_request.py` & `voicegain-speech-1.82.0/voicegain_speech/models/sync_recognition_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/sync_recognition_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/sync_recognition_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/sync_session_established.py` & `voicegain-speech-1.82.0/voicegain_speech/models/sync_session_established.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/sync_transcription_request.py` & `voicegain-speech-1.82.0/voicegain_speech/models/sync_transcription_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/sync_transcription_response.py` & `voicegain-speech-1.82.0/voicegain_speech/models/sync_transcription_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/sync_transcription_result.py` & `voicegain-speech-1.82.0/voicegain_speech/models/sync_transcription_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/talk_time.py` & `voicegain-speech-1.82.0/voicegain_speech/models/talk_time.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/topic_score.py` & `voicegain-speech-1.82.0/voicegain_speech/models/topic_score.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/training_set_bucket_type.py` & `voicegain-speech-1.82.0/voicegain_speech/models/training_set_bucket_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/training_set_doc.py` & `voicegain-speech-1.82.0/voicegain_speech/models/training_set_doc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/training_set_doc_defaults.py` & `voicegain-speech-1.82.0/voicegain_speech/models/training_set_doc_defaults.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/training_set_doc_statistics.py` & `voicegain-speech-1.82.0/voicegain_speech/models/training_set_doc_statistics.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/training_set_key.py` & `voicegain-speech-1.82.0/voicegain_speech/models/training_set_key.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/training_set_modifiable.py` & `voicegain-speech-1.82.0/voicegain_speech/models/training_set_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/training_set_status.py` & `voicegain-speech-1.82.0/voicegain_speech/models/training_set_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/training_set_status_modifiable.py` & `voicegain-speech-1.82.0/voicegain_speech/models/training_set_status_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/training_set_store_type.py` & `voicegain-speech-1.82.0/voicegain_speech/models/training_set_store_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/transcribe_alt.py` & `voicegain-speech-1.82.0/voicegain_speech/models/transcribe_alt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/transcribe_session_id.py` & `voicegain-speech-1.82.0/voicegain_speech/models/transcribe_session_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/transcribe_session_modify_request.py` & `voicegain-speech-1.82.0/voicegain_speech/models/transcribe_session_modify_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/transcribe_session_modify_request_mute.py` & `voicegain-speech-1.82.0/voicegain_speech/models/transcribe_session_modify_request_mute.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/transcribe_session_modify_request_pause.py` & `voicegain-speech-1.82.0/voicegain_speech/models/transcribe_session_modify_request_pause.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/transcript_position_range.py` & `voicegain-speech-1.82.0/voicegain_speech/models/transcript_position_range.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/transcript_position_range_for_phrase.py` & `voicegain-speech-1.82.0/voicegain_speech/models/transcript_position_range_for_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py` & `voicegain-speech-1.82.0/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/transfer.py` & `voicegain-speech-1.82.0/voicegain_speech/models/transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/transfer_all_of.py` & `voicegain-speech-1.82.0/voicegain_speech/models/transfer_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/vad_mode.py` & `voicegain-speech-1.82.0/voicegain_speech/models/vad_mode.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/version.py` & `voicegain-speech-1.82.0/voicegain_speech/models/version.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/websocket.py` & `voicegain-speech-1.82.0/voicegain_speech/models/websocket.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/websocket_init.py` & `voicegain-speech-1.82.0/voicegain_speech/models/websocket_init.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/websocket_init_reco.py` & `voicegain-speech-1.82.0/voicegain_speech/models/websocket_init_reco.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/websocket_modifiable.py` & `voicegain-speech-1.82.0/voicegain_speech/models/websocket_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/websocket_msg.py` & `voicegain-speech-1.82.0/voicegain_speech/models/websocket_msg.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/websocket_protocol.py` & `voicegain-speech-1.82.0/voicegain_speech/models/websocket_protocol.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/websocket_resp.py` & `voicegain-speech-1.82.0/voicegain_speech/models/websocket_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/word_alternatives.py` & `voicegain-speech-1.82.0/voicegain_speech/models/word_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/word_cloud_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/word_cloud_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/word_correction.py` & `voicegain-speech-1.82.0/voicegain_speech/models/word_correction.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/word_item_timed.py` & `voicegain-speech-1.82.0/voicegain_speech/models/word_item_timed.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/word_item_timing.py` & `voicegain-speech-1.82.0/voicegain_speech/models/word_item_timing.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/word_tree_ids.py` & `voicegain-speech-1.82.0/voicegain_speech/models/word_tree_ids.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/word_tree_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/word_tree_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/words_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/words_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/words_section.py` & `voicegain-speech-1.82.0/voicegain_speech/models/words_section.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/words_section_meta.py` & `voicegain-speech-1.82.0/voicegain_speech/models/words_section_meta.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/words_section_meta_mc.py` & `voicegain-speech-1.82.0/voicegain_speech/models/words_section_meta_mc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/words_section_single_column.py` & `voicegain-speech-1.82.0/voicegain_speech/models/words_section_single_column.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/words_section_words.py` & `voicegain-speech-1.82.0/voicegain_speech/models/words_section_words.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/models/words_websocket_item.py` & `voicegain-speech-1.82.0/voicegain_speech/models/words_websocket_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech/rest.py` & `voicegain-speech-1.82.0/voicegain_speech/rest.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.81.0/voicegain_speech.egg-info/PKG-INFO` & `voicegain-speech-1.82.0/voicegain_speech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: voicegain-speech
-Version: 1.81.0
+Version: 1.82.0
 Summary: Voicegain Speech-to-Text Python SDK
 Home-page: UNKNOWN
 Author: Huishen Zhan, Kuo Zhang, Jacek Jarmulak
 Author-email: huishen@voicegain.ai, kuo@voicegain.ai, jacek@voicegain.ai
 License: UNKNOWN
-Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.81.0.tar.gz
+Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.82.0.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Voicegain Speech-to-Text Python SDK
 
 Python SDK for the [Voicegain](https://www.voicegain.ai) [Speech-to-Text API](https://portal.voicegain.ai/api/v1/index.html).
```

### Comparing `voicegain-speech-1.81.0/voicegain_speech.egg-info/SOURCES.txt` & `voicegain-speech-1.82.0/voicegain_speech.egg-info/SOURCES.txt`

 * *Files identical despite different names*


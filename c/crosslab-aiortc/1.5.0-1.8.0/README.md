# Comparing `tmp/crosslab-aiortc-1.5.0.tar.gz` & `tmp/crosslab_aiortc-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab-aiortc-1.5.0.tar", last modified: Mon Apr  3 18:48:34 2023, max compression
+gzip compressed data, was "crosslab_aiortc-1.8.0.tar", last modified: Wed Apr 17 10:34:41 2024, max compression
```

## Comparing `crosslab-aiortc-1.5.0.tar` & `crosslab_aiortc-1.8.0.tar`

### file list

```diff
@@ -1,154 +1,156 @@
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.720249 crosslab-aiortc-1.5.0/
--rw-r--r--   0 vscode    (1000) vscode     (984)     1512 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/LICENSE
--rw-r--r--   0 vscode    (1000) vscode     (984)      182 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode     (984)     5439 2023-04-03 18:48:34.720249 crosslab-aiortc-1.5.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode     (984)     4380 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/README.rst
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.703582 crosslab-aiortc-1.5.0/docs/
--rw-r--r--   0 vscode    (1000) vscode     (984)      604 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode     (984)     2310 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/docs/api.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)    17292 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/docs/changelog.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)     5741 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     1414 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)      207 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/docs/examples.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)      545 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/docs/helpers.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)     2418 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)       48 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/docs/license.rst
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.700248 crosslab-aiortc-1.5.0/examples/
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.703582 crosslab-aiortc-1.5.0/examples/datachannel-cli/
--rw-r--r--   0 vscode    (1000) vscode     (984)      703 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/examples/datachannel-cli/README.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)     3356 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/examples/datachannel-cli/cli.py
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.703582 crosslab-aiortc-1.5.0/examples/datachannel-filexfer/
--rw-r--r--   0 vscode    (1000) vscode     (984)      889 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/examples/datachannel-filexfer/README.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)     3348 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/examples/datachannel-filexfer/filexfer.py
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.703582 crosslab-aiortc-1.5.0/examples/datachannel-vpn/
--rw-r--r--   0 vscode    (1000) vscode     (984)     1361 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/examples/datachannel-vpn/README.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)     2504 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/examples/datachannel-vpn/tuntap.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     2879 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/examples/datachannel-vpn/vpn.py
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.703582 crosslab-aiortc-1.5.0/examples/janus/
--rw-r--r--   0 vscode    (1000) vscode     (984)     1353 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/examples/janus/README.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)     8015 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/examples/janus/janus.py
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.706915 crosslab-aiortc-1.5.0/examples/server/
--rw-r--r--   0 vscode    (1000) vscode     (984)     1334 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/examples/server/README.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)  1173624 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/examples/server/demo-instruct.wav
--rw-r--r--   0 vscode    (1000) vscode     (984)     3115 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/examples/server/index.html
--rw-r--r--   0 vscode    (1000) vscode     (984)     6764 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/examples/server/server.py
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.706915 crosslab-aiortc-1.5.0/examples/videostream-cli/
--rw-r--r--   0 vscode    (1000) vscode     (984)     1420 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/examples/videostream-cli/README.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)     5028 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/examples/videostream-cli/cli.py
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.706915 crosslab-aiortc-1.5.0/examples/webcam/
--rw-r--r--   0 vscode    (1000) vscode     (984)     2522 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/examples/webcam/README.rst
--rw-r--r--   0 vscode    (1000) vscode     (984)      828 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/examples/webcam/index.html
--rw-r--r--   0 vscode    (1000) vscode     (984)     5126 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/examples/webcam/webcam.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     2025 2023-04-03 18:42:49.000000 crosslab-aiortc-1.5.0/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode     (984)       38 2023-04-03 18:48:34.720249 crosslab-aiortc-1.5.0/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode     (984)      335 2023-04-03 18:38:23.000000 crosslab-aiortc-1.5.0/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.700248 crosslab-aiortc-1.5.0/src/
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.706915 crosslab-aiortc-1.5.0/src/_cffi_src/
--rw-r--r--   0 vscode    (1000) vscode     (984)     1036 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/_cffi_src/build_opus.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     6783 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/_cffi_src/build_vpx.py
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.710249 crosslab-aiortc-1.5.0/src/aiortc/
--rw-r--r--   0 vscode    (1000) vscode     (984)     1619 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/__init__.py
--rw-r--r--   0 vscode    (1000) vscode     (984)      824 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/clock.py
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.710249 crosslab-aiortc-1.5.0/src/aiortc/codecs/
--rw-r--r--   0 vscode    (1000) vscode     (984)     5366 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/codecs/__init__.py
--rw-r--r--   0 vscode    (1000) vscode     (984)      635 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/codecs/base.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     2936 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/codecs/g711.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    11625 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/codecs/h264.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     3226 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/codecs/opus.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    13416 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/codecs/vpx.py
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.710249 crosslab-aiortc-1.5.0/src/aiortc/contrib/
--rw-r--r--   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/contrib/__init__.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    19345 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/contrib/media.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     6411 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/contrib/signaling.py
--rw-r--r--   0 vscode    (1000) vscode     (984)      626 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/events.py
--rw-r--r--   0 vscode    (1000) vscode     (984)      180 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/exceptions.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     4092 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/jitterbuffer.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     4069 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/mediastreams.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    20679 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/rate.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     1040 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/rtcconfiguration.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     6531 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/rtcdatachannel.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    20837 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/rtcdtlstransport.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    11423 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/rtcicetransport.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    48100 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/rtcpeerconnection.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     4612 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/rtcrtpparameters.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    20729 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/rtcrtpreceiver.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    17053 2023-04-03 18:34:18.000000 crosslab-aiortc-1.5.0/src/aiortc/rtcrtpsender.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     4198 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/rtcrtptransceiver.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    60760 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/rtcsctptransport.py
--rw-r--r--   0 vscode    (1000) vscode     (984)      500 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/rtcsessiondescription.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    24732 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/src/aiortc/rtp.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    20957 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/sdp.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     2879 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/stats.py
--rw-r--r--   0 vscode    (1000) vscode     (984)      978 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/src/aiortc/utils.py
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.710249 crosslab-aiortc-1.5.0/src/crosslab_aiortc.egg-info/
--rw-r--r--   0 vscode    (1000) vscode     (984)     5439 2023-04-03 18:48:34.000000 crosslab-aiortc-1.5.0/src/crosslab_aiortc.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode     (984)     3481 2023-04-03 18:48:34.000000 crosslab-aiortc-1.5.0/src/crosslab_aiortc.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode     (984)        1 2023-04-03 18:48:34.000000 crosslab-aiortc-1.5.0/src/crosslab_aiortc.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode     (984)      236 2023-04-03 18:48:34.000000 crosslab-aiortc-1.5.0/src/crosslab_aiortc.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode     (984)        7 2023-04-03 18:48:34.000000 crosslab-aiortc-1.5.0/src/crosslab_aiortc.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:48:34.720249 crosslab-aiortc-1.5.0/tests/
--rw-r--r--   0 vscode    (1000) vscode     (984)        0 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/__init__.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     4816 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/codecs.py
--rw-r--r--   0 vscode    (1000) vscode     (984)       23 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/h264_0000.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)      913 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/h264_0001.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)      914 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/h264_0002.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)      560 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/h264_0003.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)        8 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_bye.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)        8 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_bye_invalid.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)        4 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_bye_no_sources.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)        8 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_bye_padding.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)        8 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_psfb_invalid.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       12 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_psfb_pli.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       32 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_rr.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)        8 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_rr_invalid.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       52 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_rtpfb.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)        8 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_rtpfb_invalid.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       52 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_sdes.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       32 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_sdes_item_truncated.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       14 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_sdes_source_truncated.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       52 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_sr.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)        8 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtcp_sr_invalid.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)      172 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtp.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       16 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtp_dtmf.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)      236 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtp_only_padding.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)      244 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtp_only_padding_with_header_extensions.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)      180 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtp_with_csrc.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       74 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/rtp_with_sdes_mid.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       72 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_abort.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       24 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_cookie_echo.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       32 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_data.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       32 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_data_padding.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       24 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_error.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       24 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_forward_tsn.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       56 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_heartbeat.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)      100 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_init.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)      100 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_init_bad_verification.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       28 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_reconfig_add_out.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       36 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_reconfig_reset_out.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       28 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_reconfig_response.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       40 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_sack.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)       20 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/sctp_shutdown.bin
--rw-r--r--   0 vscode    (1000) vscode     (984)     1030 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/test_clock.py
--rw-r--r--   0 vscode    (1000) vscode     (984)      507 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/test_codecs.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    25185 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_contrib_media.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     6533 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_contrib_signaling.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     5146 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/test_g711.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    11456 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_h264.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    11810 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/test_jitterbuffer.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     1866 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_mediastreams.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     3223 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/test_opus.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     2101 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/test_ortc.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    31734 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_rate.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    18554 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_rtcdtlstransport.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    12620 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_rtcicetransport.py
--rw-r--r--   0 vscode    (1000) vscode     (984)   183370 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_rtcpeerconnection.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    18849 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/test_rtcrtpreceiver.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    14692 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_rtcrtpsender.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     1756 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/test_rtcrtptransceiver.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    92649 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_rtcsctptransport.py
--rw-r--r--   0 vscode    (1000) vscode     (984)      622 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_rtcsessiondescription.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    26490 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_rtp.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    76647 2023-04-03 18:35:20.000000 crosslab-aiortc-1.5.0/tests/test_sdp.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     2064 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/test_utils.py
--rw-r--r--   0 vscode    (1000) vscode     (984)    10351 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/test_vpx.py
--rw-r--r--   0 vscode    (1000) vscode     (984)     2846 2023-04-03 18:19:42.000000 crosslab-aiortc-1.5.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.988031 crosslab_aiortc-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-17 10:34:41.988031 crosslab_aiortc-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.960031 crosslab_aiortc-1.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/docs/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.956031 crosslab_aiortc-1.8.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.960031 crosslab_aiortc-1.8.0/examples/datachannel-cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/datachannel-cli/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/datachannel-cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.960031 crosslab_aiortc-1.8.0/examples/datachannel-filexfer/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/datachannel-filexfer/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/datachannel-filexfer/filexfer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.960031 crosslab_aiortc-1.8.0/examples/datachannel-vpn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/datachannel-vpn/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/datachannel-vpn/tuntap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/datachannel-vpn/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.960031 crosslab_aiortc-1.8.0/examples/janus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/janus/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/janus/janus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.964031 crosslab_aiortc-1.8.0/examples/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/server/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)  1173624 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/server/demo-instruct.wav
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/server/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.964031 crosslab_aiortc-1.8.0/examples/videostream-cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/videostream-cli/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/videostream-cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.964031 crosslab_aiortc-1.8.0/examples/webcam/
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/webcam/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/webcam/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/examples/webcam/webcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:34:41.988031 crosslab_aiortc-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.956031 crosslab_aiortc-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.964031 crosslab_aiortc-1.8.0/src/_cffi_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/_cffi_src/build_opus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/_cffi_src/build_vpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.972031 crosslab_aiortc-1.8.0/src/aiortc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/clock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.972031 crosslab_aiortc-1.8.0/src/aiortc/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/codecs/_opus.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/codecs/_vpx.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/codecs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/codecs/g711.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/codecs/h264.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/codecs/opus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13416 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/codecs/vpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.972031 crosslab_aiortc-1.8.0/src/aiortc/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19358 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/contrib/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/contrib/signaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/jitterbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/mediastreams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20679 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rtcconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rtcdatachannel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23153 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rtcdtlstransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rtcicetransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48556 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rtcpeerconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rtcrtpparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20867 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rtcrtpreceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rtcrtpsender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rtcrtptransceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60760 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rtcsctptransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rtcsessiondescription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24732 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/rtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20957 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/sdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/src/aiortc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.984031 crosslab_aiortc-1.8.0/src/crosslab_aiortc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-17 10:34:41.000000 crosslab_aiortc-1.8.0/src/crosslab_aiortc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-17 10:34:41.000000 crosslab_aiortc-1.8.0/src/crosslab_aiortc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:34:41.000000 crosslab_aiortc-1.8.0/src/crosslab_aiortc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-17 10:34:41.000000 crosslab_aiortc-1.8.0/src/crosslab_aiortc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 10:34:41.000000 crosslab_aiortc-1.8.0/src/crosslab_aiortc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:41.984031 crosslab_aiortc-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/h264_0000.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/h264_0001.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/h264_0002.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/h264_0003.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_bye.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_bye_invalid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_bye_no_sources.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_bye_padding.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_psfb_invalid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_psfb_pli.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_rr.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_rr_invalid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_rtpfb.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_rtpfb_invalid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_sdes.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_sdes_item_truncated.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_sdes_source_truncated.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_sr.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtcp_sr_invalid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtp.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtp_dtmf.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtp_only_padding.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtp_only_padding_with_header_extensions.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtp_with_csrc.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/rtp_with_sdes_mid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_abort.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_cookie_echo.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_data.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_data_padding.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_error.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_forward_tsn.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_heartbeat.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_init.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_init_bad_verification.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_reconfig_add_out.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_reconfig_reset_out.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_reconfig_response.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_sack.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/sctp_shutdown.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25185 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_contrib_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_contrib_signaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_g711.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_h264.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_jitterbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_mediastreams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_opus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_ortc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31734 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19439 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_rtcdtlstransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_rtcicetransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)   181301 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_rtcpeerconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_rtcrtpreceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_rtcrtpsender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_rtcrtptransceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92649 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_rtcsctptransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_rtcsessiondescription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26490 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_rtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76647 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_sdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/test_vpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-17 10:34:37.000000 crosslab_aiortc-1.8.0/tests/utils.py
```

### Comparing `crosslab-aiortc-1.5.0/LICENSE` & `crosslab_aiortc-1.8.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018-2023 Jeremy Lainé.
+Copyright (c) Jeremy Lainé.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
     * Redistributions of source code must retain the above copyright notice,
       this list of conditions and the following disclaimer.
```

### Comparing `crosslab-aiortc-1.5.0/PKG-INFO` & `crosslab_aiortc-1.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,73 @@
 Metadata-Version: 2.1
 Name: crosslab-aiortc
-Version: 1.5.0
+Version: 1.8.0
 Summary: An implementation of WebRTC and ORTC
-Author-email: Jeremy Lainé <jeremy.laine@m4x.org>
 License: BSD-3-Clause
-Project-URL: homepage, https://github.com/aiortc/aiortc
+Project-URL: homepage, https://github.com/GOLDi2/aiortc
 Project-URL: changelog, https://aiortc.readthedocs.io/en/stable/changelog.html
 Project-URL: documentation, https://aiortc.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: aioice<1.0.0,>=0.9.0
+Requires-Dist: av<12.0.0,>=9.0.0
+Requires-Dist: cffi>=1.0.0
+Requires-Dist: cryptography>=42.0.0
+Requires-Dist: dataclasses; python_version < "3.7"
+Requires-Dist: google-crc32c>=1.1
+Requires-Dist: pyee>=9.0.0
+Requires-Dist: pylibsrtp>=0.10.0
+Requires-Dist: pyopenssl>=24.0.0
+Provides-Extra: dev
+Requires-Dist: aiohttp>=3.7.0; extra == "dev"
+Requires-Dist: coverage[toml]>=7.2.2; extra == "dev"
+Requires-Dist: numpy>=1.19.0; extra == "dev"
+
+.. image:: docs/_static/aiortc.svg
+   :width: 120px
+   :alt: aiortc
+
+.. image:: https://img.shields.io/pypi/l/aiortc.svg
+   :target: https://pypi.python.org/pypi/aiortc
+   :alt: License
+
+.. image:: https://img.shields.io/pypi/v/aiortc.svg
+   :target: https://pypi.python.org/pypi/aiortc
+   :alt: Version
+
+.. image:: https://img.shields.io/pypi/pyversions/aiortc.svg
+   :target: https://pypi.python.org/pypi/aiortc
+   :alt: Python versions
+
+.. image:: https://github.com/aiortc/aiortc/workflows/tests/badge.svg
+   :target: https://github.com/aiortc/aiortc/actions
+   :alt: Tests
+
+.. image:: https://img.shields.io/codecov/c/github/aiortc/aiortc.svg
+   :target: https://codecov.io/gh/aiortc/aiortc
+   :alt: Coverage
 
-aiortc
-======
-
-|rtd| |pypi-v| |pypi-pyversions| |pypi-l| |tests| |codecov| |gitter|
-
-.. |rtd| image:: https://readthedocs.org/projects/aiortc/badge/?version=latest
+.. image:: https://readthedocs.org/projects/aiortc/badge/?version=latest
    :target: https://aiortc.readthedocs.io/
+   :alt: Documentation
 
-.. |pypi-v| image:: https://img.shields.io/pypi/v/aiortc.svg
-    :target: https://pypi.python.org/pypi/aiortc
-
-.. |pypi-pyversions| image:: https://img.shields.io/pypi/pyversions/aiortc.svg
-    :target: https://pypi.python.org/pypi/aiortc
-
-.. |pypi-l| image:: https://img.shields.io/pypi/l/aiortc.svg
-    :target: https://pypi.python.org/pypi/aiortc
-
-.. |tests| image:: https://github.com/aiortc/aiortc/workflows/tests/badge.svg
-    :target: https://github.com/aiortc/aiortc/actions
-
-.. |codecov| image:: https://img.shields.io/codecov/c/github/aiortc/aiortc.svg
-    :target: https://codecov.io/gh/aiortc/aiortc
-
-.. |gitter| image:: https://img.shields.io/gitter/room/aiortc/Lobby.svg
-    :target: https://gitter.im/aiortc/Lobby
+This is a fork of the aiortc project with slight modification neeeded in the crosslab project
 
 What is ``aiortc``?
 -------------------
 
 ``aiortc`` is a library for `Web Real-Time Communication (WebRTC)`_ and
 `Object Real-Time Communication (ORTC)`_ in Python. It is built on top of
 ``asyncio``, Python's standard asynchronous I/O framework.
@@ -106,56 +121,46 @@
 - Sending and receiving video (VP8 / H.264)
 - Bundling audio / video / data channels
 - RTCP reports, including NACK / PLI to recover from packet loss
 
 Installing
 ----------
 
-Since release 0.9.28 binary wheels are available on PyPI for Linux, Mac and
-Windows. The easiest way to install ``aiortc`` is to run:
+The easiest way to install ``aiortc`` is to run:
 
 .. code:: bash
 
     pip install aiortc
 
 Building from source
 --------------------
 
 If there are no wheels for your system or if you wish to build aiortc from
 source you will need a couple of libraries installed on your system:
 
-- OpenSSL 1.0.2 or greater
-- FFmpeg 4.0 or greater
-- LibVPX for video encoding / decoding
 - Opus for audio encoding / decoding
+- LibVPX for video encoding / decoding
 
 Linux
 .....
 
 On Debian/Ubuntu run:
 
 .. code:: bash
 
-    apt install libavdevice-dev libavfilter-dev libopus-dev libvpx-dev pkg-config
-
-`pylibsrtp` comes with binary wheels for most platforms, but if it needs to be
-built from you will also need to run:
-
-.. code:: bash
-
-    apt install libsrtp2-dev
+    apt install libopus-dev libvpx-dev
 
 OS X
 ....
 
 On OS X run:
 
 .. code:: bash
 
-    brew install ffmpeg opus libvpx pkg-config
+    brew install opus libvpx
 
 License
 -------
 
 ``aiortc`` is released under the `BSD license`_.
 
 .. _BSD license: https://aiortc.readthedocs.io/en/latest/license.html
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `crosslab-aiortc-1.5.0/README.rst` & `crosslab_aiortc-1.8.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-aiortc
-======
+.. image:: docs/_static/aiortc.svg
+   :width: 120px
+   :alt: aiortc
+
+.. image:: https://img.shields.io/pypi/l/aiortc.svg
+   :target: https://pypi.python.org/pypi/aiortc
+   :alt: License
+
+.. image:: https://img.shields.io/pypi/v/aiortc.svg
+   :target: https://pypi.python.org/pypi/aiortc
+   :alt: Version
+
+.. image:: https://img.shields.io/pypi/pyversions/aiortc.svg
+   :target: https://pypi.python.org/pypi/aiortc
+   :alt: Python versions
+
+.. image:: https://github.com/aiortc/aiortc/workflows/tests/badge.svg
+   :target: https://github.com/aiortc/aiortc/actions
+   :alt: Tests
+
+.. image:: https://img.shields.io/codecov/c/github/aiortc/aiortc.svg
+   :target: https://codecov.io/gh/aiortc/aiortc
+   :alt: Coverage
 
-|rtd| |pypi-v| |pypi-pyversions| |pypi-l| |tests| |codecov| |gitter|
-
-.. |rtd| image:: https://readthedocs.org/projects/aiortc/badge/?version=latest
+.. image:: https://readthedocs.org/projects/aiortc/badge/?version=latest
    :target: https://aiortc.readthedocs.io/
+   :alt: Documentation
 
-.. |pypi-v| image:: https://img.shields.io/pypi/v/aiortc.svg
-    :target: https://pypi.python.org/pypi/aiortc
-
-.. |pypi-pyversions| image:: https://img.shields.io/pypi/pyversions/aiortc.svg
-    :target: https://pypi.python.org/pypi/aiortc
-
-.. |pypi-l| image:: https://img.shields.io/pypi/l/aiortc.svg
-    :target: https://pypi.python.org/pypi/aiortc
-
-.. |tests| image:: https://github.com/aiortc/aiortc/workflows/tests/badge.svg
-    :target: https://github.com/aiortc/aiortc/actions
-
-.. |codecov| image:: https://img.shields.io/codecov/c/github/aiortc/aiortc.svg
-    :target: https://codecov.io/gh/aiortc/aiortc
-
-.. |gitter| image:: https://img.shields.io/gitter/room/aiortc/Lobby.svg
-    :target: https://gitter.im/aiortc/Lobby
+This is a fork of the aiortc project with slight modification neeeded in the crosslab project
 
 What is ``aiortc``?
 -------------------
 
 ``aiortc`` is a library for `Web Real-Time Communication (WebRTC)`_ and
 `Object Real-Time Communication (ORTC)`_ in Python. It is built on top of
 ``asyncio``, Python's standard asynchronous I/O framework.
@@ -80,56 +84,46 @@
 - Sending and receiving video (VP8 / H.264)
 - Bundling audio / video / data channels
 - RTCP reports, including NACK / PLI to recover from packet loss
 
 Installing
 ----------
 
-Since release 0.9.28 binary wheels are available on PyPI for Linux, Mac and
-Windows. The easiest way to install ``aiortc`` is to run:
+The easiest way to install ``aiortc`` is to run:
 
 .. code:: bash
 
     pip install aiortc
 
 Building from source
 --------------------
 
 If there are no wheels for your system or if you wish to build aiortc from
 source you will need a couple of libraries installed on your system:
 
-- OpenSSL 1.0.2 or greater
-- FFmpeg 4.0 or greater
-- LibVPX for video encoding / decoding
 - Opus for audio encoding / decoding
+- LibVPX for video encoding / decoding
 
 Linux
 .....
 
 On Debian/Ubuntu run:
 
 .. code:: bash
 
-    apt install libavdevice-dev libavfilter-dev libopus-dev libvpx-dev pkg-config
-
-`pylibsrtp` comes with binary wheels for most platforms, but if it needs to be
-built from you will also need to run:
-
-.. code:: bash
-
-    apt install libsrtp2-dev
+    apt install libopus-dev libvpx-dev
 
 OS X
 ....
 
 On OS X run:
 
 .. code:: bash
 
-    brew install ffmpeg opus libvpx pkg-config
+    brew install opus libvpx
 
 License
 -------
 
 ``aiortc`` is released under the `BSD license`_.
 
 .. _BSD license: https://aiortc.readthedocs.io/en/latest/license.html
```

### Comparing `crosslab-aiortc-1.5.0/docs/Makefile` & `crosslab_aiortc-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/docs/api.rst` & `crosslab_aiortc-1.8.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/docs/changelog.rst` & `crosslab_aiortc-1.8.0/docs/changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,75 @@
 Changelog
 =========
 
 .. currentmodule:: aiortc
 
+1.8.0
+-----
+
+* Only send / receive RTP according to :attr:`RTCRtpTransceiver.currentDirection`.
+* Close the :class:`RTCPeerConnection` if all DTLS transports are closed.
+* Free the encoder as soon as the :class:`RTCRtpSender` stops to save memory.
+* Modernise JavaScript in `server` and `webcam` examples.
+
+1.7.0
+-----
+
+ * Add support for GCM based SRTP protection profiles.
+ * Reduce supported DTLS cipher list to avoid Client Hello fragmentation.
+ * Fix `utcnow()` deprecation warning on Python 3.12.
+
+1.6.0
+-----
+
+ * Build wheels using `Py_LIMITED_ABI` to make them compatible with future Python versions.
+ * Build wheels using opus 1.4 and vpx 1.13.1.
+ * Use unique IDs for audio and video header extensions.
+ * Allow :class:`~aiortc.contrib.media.MediaRecorder` to record audio from pulse.
+
 1.5.0
 -----
 
  * Make H.264 send a full picture when picture loss occurs.
  * Fix TURN over TCP by updating `aioice` to 0.9.0.
  * Make use of the `ifaddr` package instead of the unmaintained `netifaces` package.
 
 1.4.0
 -----
 
  * Build wheels for Python 3.11.
- * Allow :class:`aiortc.contrib.media.MediaPlayer` to send media without transcoding.
- * Allow :class:`aiortc.contrib.media.MediaPlayer` to specify a timeout when opening media.
- * Make :class:`aiortc.RTCSctpTransport` transmit packets sooner to reduce datachannel latency.
- * Refactor :class:`aiortc.RTCDtlsTransport` to use PyOpenSSL.
- * Make :class:`aiortc.RTCPeerConnection` log sent and received SDP when using verbose logging.
+ * Allow :class:`~aiortc.contrib.media.MediaPlayer` to send media without transcoding.
+ * Allow :class:`~aiortc.contrib.media.MediaPlayer` to specify a timeout when opening media.
+ * Make :class:`RTCSctpTransport` transmit packets sooner to reduce datachannel latency.
+ * Refactor :class:`RTCDtlsTransport` to use PyOpenSSL.
+ * Make :class:`RTCPeerConnection` log sent and received SDP when using verbose logging.
 
 1.3.2
 -----
 
  * Limit size of NACK reports to avoid excessive packet size.
  * Improve H.264 codec matching.
- * Determine video size from first frame received by :class:`aiortc.contrib.media.MediaRecorder`.
+ * Determine video size from first frame received by :class:`~aiortc.contrib.media.MediaRecorder`.
  * Fix a deprecation warning when using `av` >= 9.1.0.
  * Tolerate STUN URLs containing a `protocol` querystring argument.
 
 1.3.1
 -----
 
  * Build wheels for aarch64 on Linux.
- * Adapt :class:`aiortc.contrib.media.MediaPlayer` for PyAV 9.x.
+ * Adapt :class:`~aiortc.contrib.media.MediaPlayer` for PyAV 9.x.
  * Ensure H.264 produces B-frames by resetting picture type.
 
 1.3.0
 -----
 
  * Build wheels for Python 3.10 and for arm64 on Mac.
  * Build wheels against `libvpx` 1.10.
- * Add support for looping in :class:`aiortc.contrib.media.MediaPlayer`.
- * Add unbuffered option to :class:`aiortc.contrib.media.MediaRelay`.
+ * Add support for looping in :class:`~aiortc.contrib.media.MediaPlayer`.
+ * Add unbuffered option to :class:`~aiortc.contrib.media.MediaRelay`.
  * Calculate audio energy and send in RTP header extension.
  * Fix a race condition in RTP sender/receiver shutdown.
  * Improve performance of H.264 bitstream splitting code.
  * Update imports for `pyee` version 9.x.
  * Fully switch to `google-crc32c` instead of `crc32`.
  * Drop support for Python 3.6.
  * Remove `apprtc` code as the service is no longer publicly hosted.
@@ -62,15 +85,15 @@
 -----
 
  * Fix jitter buffer to avoid severe picture corruption under packet loss and
    send Picture Loss Indication (PLI) when needed.
  * Make H.264 encoder honour the bitrate from the bandwidth estimator.
  * Add support for hardware-accelerated H.264 encoding on Raspberry Pi 4 using
    the `h264_omx` codec.
- * Add :class:`aiortc.contrib.media.MediaRelay` class to allow sending media
+ * Add :class:`~aiortc.contrib.media.MediaRelay` class to allow sending media
    tracks to multiple consumers.
 
 1.1.2
 -----
 
  * Add :attr:`RTCPeerConnection.connectionState` property.
  * Correctly detect RTCIceTransport `"failed"` state.
@@ -230,21 +253,21 @@
 ....
 
   * Call SSL_CTX_set_ecdh_auto for OpenSSL 1.0.2.
 
 Media
 .....
 
-  * Correctly route REMB packets to the :class:`aiortc.RTCRtpSender`.
+  * Correctly route REMB packets to the :class:`RTCRtpSender`.
 
 Examples
 ........
 
-  * :class:`aiortc.contrib.media.MediaPlayer` : release resources (e.g. webcam) when the player stops.
-  * :class:`aiortc.contrib.signaling.ApprtcSignaling` : make AppRTC signaling available for more examples.
+  * :class:`~aiortc.contrib.media.MediaPlayer` : release resources (e.g. webcam) when the player stops.
+  * :class:`~aiortc.contrib.signaling.ApprtcSignaling` : make AppRTC signaling available for more examples.
   * `datachannel-cli` : make uvloop optional.
   * `videostream-cli` : animate the flag with a wave effect.
   * `webcam` : explicitly set frame rate to 30 fps for webcams.
 
 0.9.20
 ------
 
@@ -257,15 +280,15 @@
 .............
 
   * Fix documentation build by installing `crc32c` instead of `crcmod`.
 
 Examples
 ........
 
-  * :class:`aiortc.contrib.media.MediaPlayer` : skip frames with no presentation timestamp (pts).
+  * :class:`~aiortc.contrib.media.MediaPlayer` : skip frames with no presentation timestamp (pts).
 
 0.9.19
 ------
 
 Data channels
 .............
 
@@ -435,15 +458,15 @@
     reduces the response time.
   * Adjust package requirements to accept PyAV < 7.0.0.
 
 Examples
 ........
 
   * `webcam` : force Chrome to use "unified-plan" semantics to enabled `addTransceiver`.
-  * :class:`aiortc.contrib.media.MediaPlayer` : don't sleep at all when playing from webcam.
+  * :class:`~aiortc.contrib.media.MediaPlayer` : don't sleep at all when playing from webcam.
     This eliminates the constant one-second lag in the `webcam` demo.
 
 0.9.9
 -----
 
 .. warning::
 
@@ -456,21 +479,21 @@
   * Use a jitter buffer for incoming audio.
   * Add :meth:`RTCPeerConnection.addTransceiver` method.
   * Add :attr:`RTCRtpTransceiver.direction` to manage transceiver direction.
 
 Examples
 ........
 
-  * `apprtc` : demonstrate the use of :class:`aiortc.contrib.media.MediaPlayer`
-    and :class:`aiortc.contrib.media.MediaRecorder`.
+  * `apprtc` : demonstrate the use of :class:`~aiortc.contrib.media.MediaPlayer`
+    and :class:`~aiortc.contrib.media.MediaRecorder`.
   * `webcam` : new examples illustrating sending video from a webcam to a browser.
-  * :class:`aiortc.contrib.media.MediaPlayer` : don't sleep if a frame lacks timing information.
-  * :class:`aiortc.contrib.media.MediaPlayer` : remove `start()` and `stop()` methods.
-  * :class:`aiortc.contrib.media.MediaRecorder` : use `libx264` for encoding.
-  * :class:`aiortc.contrib.media.MediaRecorder` : make `start()` and `stop()` coroutines.
+  * :class:`~aiortc.contrib.media.MediaPlayer` : don't sleep if a frame lacks timing information.
+  * :class:`~aiortc.contrib.media.MediaPlayer` : remove `start()` and `stop()` methods.
+  * :class:`~aiortc.contrib.media.MediaRecorder` : use `libx264` for encoding.
+  * :class:`~aiortc.contrib.media.MediaRecorder` : make `start()` and `stop()` coroutines.
 
 0.9.8
 -----
 
 Media
 .....
 
@@ -485,17 +508,17 @@
 
   * Add the :meth:`RTCPeerConnection.getStats()` coroutine to retrieve statistics.
   * Add initial :class:`RTCTransportStats` to report transport statistics.
 
 Examples
 ........
 
-  * Add new :class:`aiortc.contrib.media.MediaPlayer` class to read audio / video from a file.
-  * Add new :class:`aiortc.contrib.media.MediaRecorder` class to write audio / video to a file.
-  * Add new :class:`aiortc.contrib.media.MediaBlackhole` class to discard audio / video.
+  * Add new :class:`~aiortc.contrib.media.MediaPlayer` class to read audio / video from a file.
+  * Add new :class:`~aiortc.contrib.media.MediaRecorder` class to write audio / video to a file.
+  * Add new :class:`~aiortc.contrib.media.MediaBlackhole` class to discard audio / video.
 
 0.9.7
 -----
 
 Media
 .....
 
@@ -671,21 +694,21 @@
 ...............
 
   * Add :meth:`RTCPeerConnection.addIceCandidate()` method to handle trickled ICE candidates.
 
 Media
 .....
 
-  * Make stop() methods of :class:`aiortc.RTCRtpReceiver`, :class:`aiortc.RTCRtpSender`
+  * Make stop() methods of :class:`RTCRtpReceiver`, :class:`RTCRtpSender`
     and :class:`RTCRtpTransceiver` coroutines to enable clean shutdown.
 
 Data channels
 .............
 
-  * Clean up :class:`aiortc.RTCDataChannel` shutdown sequence.
+  * Clean up :class:`RTCDataChannel` shutdown sequence.
 
   * Support receiving an SCTP `RE-CONFIG` to raise number of inbound streams.
 
 Examples
 ........
 
   * `server`:
@@ -713,19 +736,19 @@
   * Add `BUNDLE` support to use a single ICE/DTLS transport for multiple media.
 
   * Move media encoding / decoding off the main thread.
 
 Data channels
 .............
 
-  * Use SCTP `ABORT` instead of `SHUTDOWN` when stopping :class:`aiortc.RTCSctpTransport`.
+  * Use SCTP `ABORT` instead of `SHUTDOWN` when stopping :class:`RTCSctpTransport`.
 
   * Advertise support for SCTP `RE-CONFIG` extension.
 
-  * Make :class:`aiortc.RTCDataChannel` emit `open` and `close` events.
+  * Make :class:`RTCDataChannel` emit `open` and `close` events.
 
 Examples
 ........
 
   * Add an example of how to connect to appr.tc.
 
   * Capture audio frames to a WAV file in server example.
```

### Comparing `crosslab-aiortc-1.5.0/docs/contributing.rst` & `crosslab_aiortc-1.8.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/docs/helpers.rst` & `crosslab_aiortc-1.8.0/docs/helpers.rst`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/docs/index.rst` & `crosslab_aiortc-1.8.0/docs/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 aiortc
 =========
 
-|pypi-v| |pypi-pyversions| |pypi-l| |tests| |codecov| |gitter|
-
-.. |pypi-v| image:: https://img.shields.io/pypi/v/aiortc.svg
-    :target: https://pypi.python.org/pypi/aiortc
-
-.. |pypi-pyversions| image:: https://img.shields.io/pypi/pyversions/aiortc.svg
-    :target: https://pypi.python.org/pypi/aiortc
-
-.. |pypi-l| image:: https://img.shields.io/pypi/l/aiortc.svg
-    :target: https://pypi.python.org/pypi/aiortc
-
-.. |tests| image:: https://github.com/aiortc/aiortc/workflows/tests/badge.svg
-    :target: https://github.com/aiortc/aiortc/actions
-
-.. |codecov| image:: https://img.shields.io/codecov/c/github/aiortc/aiortc.svg
-    :target: https://codecov.io/gh/aiortc/aiortc
-
-.. |gitter| image:: https://img.shields.io/gitter/room/aiortc/Lobby.svg
-    :target: https://gitter.im/aiortc/Lobby
+.. image:: https://img.shields.io/pypi/l/aiortc.svg
+   :target: https://pypi.python.org/pypi/aiortc
+   :alt: License
+
+.. image:: https://img.shields.io/pypi/v/aiortc.svg
+   :target: https://pypi.python.org/pypi/aiortc
+   :alt: Version
+
+.. image:: https://img.shields.io/pypi/pyversions/aiortc.svg
+   :target: https://pypi.python.org/pypi/aiortc
+   :alt: Python versions
+
+.. image:: https://github.com/aiortc/aiortc/workflows/tests/badge.svg
+   :target: https://github.com/aiortc/aiortc/actions
+   :alt: Tests
+
+.. image:: https://img.shields.io/codecov/c/github/aiortc/aiortc.svg
+   :target: https://codecov.io/gh/aiortc/aiortc
+   :alt: Coverage
 
 ``aiortc`` is a library for `Web Real-Time Communication (WebRTC)`_ and
 `Object Real-Time Communication (ORTC)`_ in Python. It is built on top of
 ``asyncio``, Python's standard asynchronous I/O framework.
 
 The API closely follows its Javascript counterpart while using pythonic
 constructs:
```

### Comparing `crosslab-aiortc-1.5.0/examples/datachannel-cli/README.rst` & `crosslab_aiortc-1.8.0/examples/datachannel-cli/README.rst`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/examples/datachannel-cli/cli.py` & `crosslab_aiortc-1.8.0/examples/datachannel-cli/cli.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/examples/datachannel-filexfer/README.rst` & `crosslab_aiortc-1.8.0/examples/datachannel-filexfer/README.rst`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/examples/datachannel-filexfer/filexfer.py` & `crosslab_aiortc-1.8.0/examples/datachannel-filexfer/filexfer.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/examples/datachannel-vpn/README.rst` & `crosslab_aiortc-1.8.0/examples/datachannel-vpn/README.rst`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/examples/datachannel-vpn/tuntap.py` & `crosslab_aiortc-1.8.0/examples/datachannel-vpn/tuntap.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/examples/datachannel-vpn/vpn.py` & `crosslab_aiortc-1.8.0/examples/datachannel-vpn/vpn.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/examples/janus/README.rst` & `crosslab_aiortc-1.8.0/examples/janus/README.rst`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/examples/janus/janus.py` & `crosslab_aiortc-1.8.0/examples/janus/janus.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,17 +214,17 @@
     parser = argparse.ArgumentParser(description="Janus")
     parser.add_argument("url", help="Janus root URL, e.g. http://localhost:8088/janus")
     parser.add_argument(
         "--room",
         type=int,
         default=1234,
         help="The video room ID to join (default: 1234).",
-    ),
-    parser.add_argument("--play-from", help="Read the media from a file and sent it."),
-    parser.add_argument("--record-to", help="Write received media to a file."),
+    )
+    parser.add_argument("--play-from", help="Read the media from a file and sent it.")
+    parser.add_argument("--record-to", help="Write received media to a file.")
     parser.add_argument(
         "--play-without-decoding",
         help=(
             "Read the media without decoding it (experimental). "
             "For now it only works with an MPEGTS container with only H.264 video."
         ),
         action="store_true",
```

### Comparing `crosslab-aiortc-1.5.0/examples/server/README.rst` & `crosslab_aiortc-1.8.0/examples/server/README.rst`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/examples/server/demo-instruct.wav` & `crosslab_aiortc-1.8.0/examples/server/demo-instruct.wav`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/examples/server/index.html` & `crosslab_aiortc-1.8.0/examples/server/index.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+<!DOCTYPE html>
 <html>
 <head>
     <meta charset="UTF-8"/>
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>WebRTC demo</title>
     <style>
     button {
@@ -37,24 +38,30 @@
         <option value='{"ordered": false, "maxRetransmits": 0}'>Unordered, no retransmissions</option>
         <option value='{"ordered": false, "maxPacketLifetime": 500}'>Unordered, 500ms lifetime</option>
     </select>
 </div>
 <div class="option">
     <input id="use-audio" checked="checked" type="checkbox"/>
     <label for="use-audio">Use audio</label>
+    <select id="audio-input">
+        <option value="" selected>Default device</option>
+    </select>
     <select id="audio-codec">
         <option value="default" selected>Default codecs</option>
         <option value="opus/48000/2">Opus</option>
         <option value="PCMU/8000">PCMU</option>
         <option value="PCMA/8000">PCMA</option>
     </select>
 </div>
 <div class="option">
     <input id="use-video" type="checkbox"/>
     <label for="use-video">Use video</label>
+    <select id="video-input">
+        <option value="" selected>Default device</option>
+    </select>
     <select id="video-resolution">
         <option value="" selected>Default resolution</option>
         <option value="320x240">320x240</option>
         <option value="640x480">640x480</option>
         <option value="960x540">960x540</option>
         <option value="1280x720">1280x720</option>
     </select>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 ********** OOppttiioonnss **********
 Use datachannel[One of: Ordered, reliable/Unordered, no retransmissions/
 Unordered, 500ms lifetime]
-Use audio[One of: Default codecs/Opus/PCMU/PCMA]
-??Use video[One of: Default resolution/320x240/640x480/960x540/1280x720][One of:
-No transform/Edge detection/Cartoon effect/Rotate][One of: Default codecs/VP8/
-H264]
+Use audio[One of: Default device][One of: Default codecs/Opus/PCMU/PCMA]
+??Use video[One of: Default device][One of: Default resolution/320x240/640x480/
+960x540/1280x720][One of: No transform/Edge detection/Cartoon effect/Rotate]
+[One of: Default codecs/VP8/H264]
 ??Use STUN server
 Start Stop
 ********** SSttaattee **********
 ICE gathering state:
 ICE connection state:
 Signaling state:
 ********** MMeeddiiaa **********
```

### Comparing `crosslab-aiortc-1.5.0/examples/server/server.py` & `crosslab_aiortc-1.8.0/examples/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     parser.add_argument("--key-file", help="SSL key file (for HTTPS)")
     parser.add_argument(
         "--host", default="0.0.0.0", help="Host for HTTP server (default: 0.0.0.0)"
     )
     parser.add_argument(
         "--port", type=int, default=8080, help="Port for HTTP server (default: 8080)"
     )
-    parser.add_argument("--record-to", help="Write received media to a file."),
+    parser.add_argument("--record-to", help="Write received media to a file.")
     parser.add_argument("--verbose", "-v", action="count")
     args = parser.parse_args()
 
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
     else:
         logging.basicConfig(level=logging.INFO)
```

### Comparing `crosslab-aiortc-1.5.0/examples/videostream-cli/README.rst` & `crosslab_aiortc-1.8.0/examples/videostream-cli/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 Additional options
 ------------------
 
 If you want to play a media file instead of sending the example image, run:
 
 .. code-block:: console
 
-   $ python cli.py --play-from video.mp4
+   $ python cli.py offer --play-from video.mp4
 
 If you want to recording the received video you can run one of the following:
 
 .. code-block:: console
 
    $ python cli.py answer --record-to video.mp4
    $ python cli.py answer --record-to video-%3d.png
```

### Comparing `crosslab-aiortc-1.5.0/examples/videostream-cli/cli.py` & `crosslab_aiortc-1.8.0/examples/videostream-cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,16 +119,16 @@
             print("Exiting")
             break
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Video stream from the command line")
     parser.add_argument("role", choices=["offer", "answer"])
-    parser.add_argument("--play-from", help="Read the media from a file and sent it."),
-    parser.add_argument("--record-to", help="Write received media to a file."),
+    parser.add_argument("--play-from", help="Read the media from a file and sent it.")
+    parser.add_argument("--record-to", help="Write received media to a file.")
     parser.add_argument("--verbose", "-v", action="count")
     add_signaling_arguments(parser)
     args = parser.parse_args()
 
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
```

### Comparing `crosslab-aiortc-1.5.0/examples/webcam/README.rst` & `crosslab_aiortc-1.8.0/examples/webcam/README.rst`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/examples/webcam/index.html` & `crosslab_aiortc-1.8.0/examples/webcam/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+<!DOCTYPE html>
 <html>
 <head>
     <meta charset="UTF-8"/>
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>WebRTC webcam</title>
     <style>
     button {
```

### Comparing `crosslab-aiortc-1.5.0/examples/webcam/webcam.py` & `crosslab_aiortc-1.8.0/examples/webcam/webcam.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     pcs.clear()
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="WebRTC webcam demo")
     parser.add_argument("--cert-file", help="SSL certificate file (for HTTPS)")
     parser.add_argument("--key-file", help="SSL key file (for HTTPS)")
-    parser.add_argument("--play-from", help="Read the media from a file and sent it."),
+    parser.add_argument("--play-from", help="Read the media from a file and sent it.")
     parser.add_argument(
         "--play-without-decoding",
         help=(
             "Read the media without decoding it (experimental). "
             "For now it only works with an MPEGTS container with only H.264 video."
         ),
         action="store_true",
```

### Comparing `crosslab-aiortc-1.5.0/pyproject.toml` & `crosslab_aiortc-1.8.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 [build-system]
-requires = ["cffi>=1.0.0", "setuptools"]
+requires = ["cffi>=1.0.0", "setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crosslab-aiortc"
 description = "An implementation of WebRTC and ORTC"
 readme = "README.rst"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = { text = "BSD-3-Clause" }
-authors = [
-    { name = "Jeremy Lainé", email = "jeremy.laine@m4x.org" },
-]
+
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "aioice>=0.9.0,<1.0.0",
-    "av>=9.0.0,<11.0.0",
+    "av>=9.0.0,<12.0.0",
     "cffi>=1.0.0",
-    "cryptography>=2.2,<39",
+    "cryptography>=42.0.0",
     'dataclasses; python_version < "3.7"',
     "google-crc32c>=1.1",
     "pyee>=9.0.0",
-    "pylibsrtp>=0.5.6",
-    "pyopenssl>=23.1.0",
+    "pylibsrtp>=0.10.0",
+    "pyopenssl>=24.0.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "aiohttp>=3.7.0",
     "coverage[toml]>=7.2.2",
     "numpy>=1.19.0",
 ]
 
 [project.urls]
-homepage = "https://github.com/aiortc/aiortc"
+homepage = "https://github.com/GOLDi2/aiortc"
 changelog = "https://aiortc.readthedocs.io/en/stable/changelog.html"
 documentation = "https://aiortc.readthedocs.io/"
 
 [tool.coverage.report]
 exclude_lines = ["pragma: no cover"]
 
 [tool.coverage.run]
@@ -61,15 +59,15 @@
 disallow_untyped_decorators = true
 ignore_missing_imports = true
 mypy_path = "stubs"
 strict_optional = false
 warn_redundant_casts = true
 warn_unused_ignores = true
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
     "E",  # pycodestyle
     "F",  # Pyflakes
     "W",  # pycodestyle
     "I",  # isort
 ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `crosslab-aiortc-1.5.0/src/_cffi_src/build_opus.py` & `crosslab_aiortc-1.8.0/src/_cffi_src/build_opus.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/_cffi_src/build_vpx.py` & `crosslab_aiortc-1.8.0/src/_cffi_src/build_vpx.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/__init__.py` & `crosslab_aiortc-1.8.0/src/aiortc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ruff: noqa: F401
 import logging
 
 import av.logging
 
 from .exceptions import InvalidAccessError, InvalidStateError
-from .mediastreams import MediaStreamTrack, VideoStreamTrack
+from .mediastreams import AudioStreamTrack, MediaStreamTrack, VideoStreamTrack
 from .rtcconfiguration import RTCConfiguration, RTCIceServer
 from .rtcdatachannel import RTCDataChannel, RTCDataChannelParameters
 from .rtcdtlstransport import (
     RTCCertificate,
     RTCDtlsFingerprint,
     RTCDtlsParameters,
     RTCDtlsTransport,
@@ -43,14 +43,14 @@
     RTCOutboundRtpStreamStats,
     RTCRemoteInboundRtpStreamStats,
     RTCRemoteOutboundRtpStreamStats,
     RTCStatsReport,
     RTCTransportStats,
 )
 
-__version__ = "1.5.0"
+__version__ = "1.8.0"
 
 # Disable PyAV's logging framework as it can lead to thread deadlocks.
 av.logging.restore_default_callback()
 
 # Set default logging handler to avoid "No handler found" warnings.
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/clock.py` & `crosslab_aiortc-1.8.0/src/aiortc/clock.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/codecs/__init__.py` & `crosslab_aiortc-1.8.0/src/aiortc/codecs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,29 +28,32 @@
             mimeType="audio/opus", clockRate=48000, channels=2, payloadType=96
         ),
         PCMU_CODEC,
         PCMA_CODEC,
     ],
     "video": [],
 }
+# Note, the id space for these extensions is shared across media types when BUNDLE
+# is negotiated. If you add a audio- or video-specific extension, make sure it has
+# a unique id.
 HEADER_EXTENSIONS: Dict[str, List[RTCRtpHeaderExtensionParameters]] = {
     "audio": [
         RTCRtpHeaderExtensionParameters(
             id=1, uri="urn:ietf:params:rtp-hdrext:sdes:mid"
         ),
         RTCRtpHeaderExtensionParameters(
             id=2, uri="urn:ietf:params:rtp-hdrext:ssrc-audio-level"
         ),
     ],
     "video": [
         RTCRtpHeaderExtensionParameters(
             id=1, uri="urn:ietf:params:rtp-hdrext:sdes:mid"
         ),
         RTCRtpHeaderExtensionParameters(
-            id=2, uri="http://www.webrtc.org/experiments/rtp-hdrext/abs-send-time"
+            id=3, uri="http://www.webrtc.org/experiments/rtp-hdrext/abs-send-time"
         ),
     ],
 }
 
 
 def init_codecs() -> None:
     dynamic_pt = 97
```

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/codecs/base.py` & `crosslab_aiortc-1.8.0/src/aiortc/codecs/base.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/codecs/g711.py` & `crosslab_aiortc-1.8.0/src/aiortc/codecs/g711.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/codecs/h264.py` & `crosslab_aiortc-1.8.0/src/aiortc/codecs/h264.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/codecs/opus.py` & `crosslab_aiortc-1.8.0/src/aiortc/codecs/opus.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/codecs/vpx.py` & `crosslab_aiortc-1.8.0/src/aiortc/codecs/vpx.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/contrib/media.py` & `crosslab_aiortc-1.8.0/src/aiortc/contrib/media.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,15 @@
     :param format: The format to use, defaults to autodect.
     :param options: Additional options to pass to FFmpeg.
     :param timeout: Open/read timeout to pass to FFmpeg.
     :param loop: Whether to repeat playback indefinitely (requires a seekable file).
     """
 
     def __init__(
-        self, file, format=None, options={}, timeout=None, loop=False, decode=True
+        self, file, format=None, options=None, timeout=None, loop=False, decode=True
     ):
         self.__container = av.open(
             file=file, format=format, mode="r", options=options, timeout=timeout
         )
         self.__thread: Optional[threading.Thread] = None
         self.__thread_quit: Optional[threading.Event] = None
 
@@ -414,26 +414,26 @@
         player = MediaRecorder('/path/to/file-%3d.png')
 
     :param file: The path to a file, or a file-like object.
     :param format: The format to use, defaults to autodect.
     :param options: Additional options to pass to FFmpeg.
     """
 
-    def __init__(self, file, format=None, options={}):
+    def __init__(self, file, format=None, options=None):
         self.__container = av.open(file=file, format=format, mode="w", options=options)
         self.__tracks = {}
 
     def addTrack(self, track):
         """
         Add a track to be recorded.
 
         :param track: A :class:`aiortc.MediaStreamTrack`.
         """
         if track.kind == "audio":
-            if self.__container.format.name in ("wav", "alsa"):
+            if self.__container.format.name in ("wav", "alsa", "pulse"):
                 codec_name = "pcm_s16le"
             elif self.__container.format.name == "mp3":
                 codec_name = "mp3"
             else:
                 codec_name = "aac"
             stream = self.__container.add_stream(codec_name)
         else:
```

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/contrib/signaling.py` & `crosslab_aiortc-1.8.0/src/aiortc/contrib/signaling.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/events.py` & `crosslab_aiortc-1.8.0/src/aiortc/events.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/jitterbuffer.py` & `crosslab_aiortc-1.8.0/src/aiortc/jitterbuffer.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/mediastreams.py` & `crosslab_aiortc-1.8.0/src/aiortc/mediastreams.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/rate.py` & `crosslab_aiortc-1.8.0/src/aiortc/rate.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/rtcconfiguration.py` & `crosslab_aiortc-1.8.0/src/aiortc/rtcconfiguration.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/rtcdatachannel.py` & `crosslab_aiortc-1.8.0/src/aiortc/rtcdatachannel.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/rtcdtlstransport.py` & `crosslab_aiortc-1.8.0/src/aiortc/rtcdtlstransport.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,56 +29,95 @@
     RtcpRtpfbPacket,
     RtcpSrPacket,
     RtpPacket,
     is_rtcp,
 )
 from .stats import RTCStatsReport, RTCTransportStats
 
-SRTP_KEY_LEN = 16
-SRTP_SALT_LEN = 14
-
 CERTIFICATE_T = TypeVar("CERTIFICATE_T", bound="RTCCertificate")
 
 logger = logging.getLogger(__name__)
 
 
+@dataclass(frozen=True)
+class SRTPProtectionProfile:
+    libsrtp_profile: int
+    openssl_profile: bytes
+    key_length: int
+    salt_length: int
+
+    def get_key_and_salt(self, src, idx: int) -> bytes:
+        key_start = idx * self.key_length
+        salt_start = 2 * self.key_length + idx * self.salt_length
+        return (
+            src[key_start : key_start + self.key_length]
+            + src[salt_start : salt_start + self.salt_length]
+        )
+
+
+SRTP_AEAD_AES_256_GCM = SRTPProtectionProfile(
+    libsrtp_profile=Policy.SRTP_PROFILE_AEAD_AES_256_GCM,
+    openssl_profile=b"SRTP_AEAD_AES_256_GCM",
+    key_length=32,
+    salt_length=12,
+)
+SRTP_AEAD_AES_128_GCM = SRTPProtectionProfile(
+    libsrtp_profile=Policy.SRTP_PROFILE_AEAD_AES_128_GCM,
+    openssl_profile=b"SRTP_AEAD_AES_128_GCM",
+    key_length=16,
+    salt_length=12,
+)
+SRTP_AES128_CM_SHA1_80 = SRTPProtectionProfile(
+    libsrtp_profile=Policy.SRTP_PROFILE_AES128_CM_SHA1_80,
+    openssl_profile=b"SRTP_AES128_CM_SHA1_80",
+    key_length=16,
+    salt_length=14,
+)
+
+# AES-GCM may not be available depending on how libsrtp2 was built.
+SRTP_PROFILES: List[SRTPProtectionProfile] = []
+for srtp_profile in [
+    SRTP_AEAD_AES_256_GCM,
+    SRTP_AEAD_AES_128_GCM,
+    SRTP_AES128_CM_SHA1_80,
+]:
+    try:
+        Policy(srtp_profile=srtp_profile.libsrtp_profile)
+    except pylibsrtp.Error:  # pragma: no cover
+        pass
+    else:
+        SRTP_PROFILES.append(srtp_profile)
+
+
 def certificate_digest(x509: crypto.X509) -> str:
     return x509.digest("SHA256").decode("ascii")
 
 
 def generate_certificate(key: ec.EllipticCurvePrivateKey) -> x509.Certificate:
     name = x509.Name(
         [
             x509.NameAttribute(
                 x509.NameOID.COMMON_NAME,
                 binascii.hexlify(os.urandom(16)).decode("ascii"),
             )
         ]
     )
+    now = datetime.datetime.now(tz=datetime.timezone.utc)
     builder = (
         x509.CertificateBuilder()
         .subject_name(name)
         .issuer_name(name)
         .public_key(key.public_key())
         .serial_number(x509.random_serial_number())
-        .not_valid_before(datetime.datetime.utcnow() - datetime.timedelta(days=1))
-        .not_valid_after(datetime.datetime.utcnow() + datetime.timedelta(days=30))
+        .not_valid_before(now - datetime.timedelta(days=1))
+        .not_valid_after(now + datetime.timedelta(days=30))
     )
     return builder.sign(key, hashes.SHA256(), default_backend())
 
 
-def get_srtp_key_salt(src, idx: int) -> bytes:
-    key_start = idx * SRTP_KEY_LEN
-    salt_start = 2 * SRTP_KEY_LEN + idx * SRTP_SALT_LEN
-    return (
-        src[key_start : key_start + SRTP_KEY_LEN]
-        + src[salt_start : salt_start + SRTP_SALT_LEN]
-    )
-
-
 class State(enum.Enum):
     NEW = 0
     CONNECTING = 1
     CONNECTED = 2
     CLOSED = 3
     FAILED = 4
 
@@ -111,17 +150,15 @@
         self._cert = cert
 
     @property
     def expires(self) -> datetime.datetime:
         """
         The date and time after which the certificate will be considered invalid.
         """
-        return self._cert.to_cryptography().not_valid_after.replace(
-            tzinfo=datetime.timezone.utc
-        )
+        return self._cert.to_cryptography().not_valid_after_utc
 
     def getFingerprints(self) -> List[RTCDtlsFingerprint]:
         """
         Returns the list of certificate fingerprints, one of which is computed
         with the digest algorithm used in the certificate signature.
         """
         return [
@@ -141,23 +178,27 @@
         key = ec.generate_private_key(ec.SECP256R1(), default_backend())
         cert = generate_certificate(key)
         return cls(
             key=crypto.PKey.from_cryptography_key(key),
             cert=crypto.X509.from_cryptography(cert),
         )
 
-    def _create_ssl_context(self) -> SSL.Context:
+    def _create_ssl_context(
+        self, srtp_profiles: List[SRTPProtectionProfile]
+    ) -> SSL.Context:
         ctx = SSL.Context(SSL.DTLS_METHOD)
         ctx.set_verify(
             SSL.VERIFY_PEER | SSL.VERIFY_FAIL_IF_NO_PEER_CERT, lambda *args: 1
         )
         ctx.use_certificate(self._cert)
         ctx.use_privatekey(self._key)
-        ctx.set_cipher_list(b"HIGH:!CAMELLIA:!aNULL")
-        ctx.set_tlsext_use_srtp(b"SRTP_AES128_CM_SHA1_80")
+        ctx.set_cipher_list(
+            b"ECDHE-ECDSA-AES128-GCM-SHA256:ECDHE-ECDSA-CHACHA20-POLY1305:ECDHE-ECDSA-AES128-SHA:ECDHE-ECDSA-AES256-SHA"
+        )
+        ctx.set_tlsext_use_srtp(b":".join(x.openssl_profile for x in srtp_profiles))
 
         return ctx
 
 
 @dataclass
 class RTCDtlsParameters:
     """
@@ -303,17 +344,17 @@
         self.__tx_bytes = 0
         self.__tx_packets = 0
 
         # SRTP
         self._rx_srtp: Session = None
         self._tx_srtp: Session = None
 
-        # SSL init
-        self.ssl = SSL.Connection(certificate._create_ssl_context())
-
+        # SSL
+        self._srtp_profiles = SRTP_PROFILES
+        self._ssl: Optional[SSL.Connection] = None
         self.__local_certificate = certificate
 
     @property
     def state(self) -> str:
         """
         The current state of the DTLS transport.
 
@@ -354,24 +395,30 @@
         # For ORTC however, we determine the DTLS role based on the ICE role.
         if self._role == "auto":
             if self.transport.role == "controlling":
                 self._set_role("server")
             else:
                 self._set_role("client")
 
+        # Initialise SSL.
+        self._ssl = SSL.Connection(
+            self.__local_certificate._create_ssl_context(
+                srtp_profiles=self._srtp_profiles
+            )
+        )
         if self._role == "server":
-            self.ssl.set_accept_state()
+            self._ssl.set_accept_state()
         else:
-            self.ssl.set_connect_state()
+            self._ssl.set_connect_state()
 
         self._set_state(State.CONNECTING)
         try:
             while not self.encrypted:
                 try:
-                    self.ssl.do_handshake()
+                    self._ssl.do_handshake()
                 except SSL.WantReadError:
                     await self._write_ssl()
                     await self._recv_next()
                 except SSL.Error as exc:
                     self.__log_debug("x DTLS handshake failed (error %s)", exc)
                     self._set_state(State.FAILED)
                     return
@@ -379,15 +426,15 @@
                     self.encrypted = True
         except ConnectionError:
             self.__log_debug("x DTLS handshake failed (connection error)")
             self._set_state(State.FAILED)
             return
 
         # check remote fingerprint
-        x509 = self.ssl.get_peer_certificate()
+        x509 = self._ssl.get_peer_certificate()
         remote_fingerprint = certificate_digest(x509)
         fingerprint_is_valid = False
         for f in remoteParameters.fingerprints:
             if (
                 f.algorithm.lower() == "sha-256"
                 and f.value.lower() == remote_fingerprint.lower()
             ):
@@ -395,30 +442,51 @@
                 break
         if not fingerprint_is_valid:
             self.__log_debug("x DTLS handshake failed (fingerprint mismatch)")
             self._set_state(State.FAILED)
             return
 
         # generate keying material
-        view = self.ssl.export_keying_material(
-            b"EXTRACTOR-dtls_srtp", 2 * (SRTP_KEY_LEN + SRTP_SALT_LEN)
+        openssl_profile = self._ssl.get_selected_srtp_profile()
+        for srtp_profile in self._srtp_profiles:
+            if srtp_profile.openssl_profile == openssl_profile:
+                self.__log_debug(
+                    "x DTLS handshake negotiated %s",
+                    srtp_profile.openssl_profile.decode(),
+                )
+                break
+        else:
+            self.__log_debug("x DTLS handshake failed (no SRTP profile negotiated)")
+            self._set_state(State.FAILED)
+            return
+        view = self._ssl.export_keying_material(
+            b"EXTRACTOR-dtls_srtp",
+            2 * (srtp_profile.key_length + srtp_profile.salt_length),
         )
         if self._role == "server":
-            srtp_tx_key = get_srtp_key_salt(view, 1)
-            srtp_rx_key = get_srtp_key_salt(view, 0)
+            srtp_tx_key = srtp_profile.get_key_and_salt(view, 1)
+            srtp_rx_key = srtp_profile.get_key_and_salt(view, 0)
         else:
-            srtp_tx_key = get_srtp_key_salt(view, 0)
-            srtp_rx_key = get_srtp_key_salt(view, 1)
+            srtp_tx_key = srtp_profile.get_key_and_salt(view, 0)
+            srtp_rx_key = srtp_profile.get_key_and_salt(view, 1)
 
-        rx_policy = Policy(key=srtp_rx_key, ssrc_type=Policy.SSRC_ANY_INBOUND)
+        rx_policy = Policy(
+            key=srtp_rx_key,
+            ssrc_type=Policy.SSRC_ANY_INBOUND,
+            srtp_profile=srtp_profile.libsrtp_profile,
+        )
         rx_policy.allow_repeat_tx = True
         rx_policy.window_size = 1024
         self._rx_srtp = Session(rx_policy)
 
-        tx_policy = Policy(key=srtp_tx_key, ssrc_type=Policy.SSRC_ANY_OUTBOUND)
+        tx_policy = Policy(
+            key=srtp_tx_key,
+            ssrc_type=Policy.SSRC_ANY_OUTBOUND,
+            srtp_profile=srtp_profile.libsrtp_profile,
+        )
         tx_policy.allow_repeat_tx = True
         tx_policy.window_size = 1024
         self._tx_srtp = Session(tx_policy)
 
         # start data pump
         self.__log_debug("- DTLS handshake complete")
         self._set_state(State.CONNECTED)
@@ -428,17 +496,17 @@
         """
         Stop and close the DTLS transport.
         """
         if self._task is not None:
             self._task.cancel()
             self._task = None
 
-        if self._state in [State.CONNECTING, State.CONNECTED]:
+        if self._ssl and self._state in [State.CONNECTING, State.CONNECTED]:
             try:
-                self.ssl.shutdown()
+                self._ssl.shutdown()
             except SSL.Error:
                 pass
             try:
                 await self._write_ssl()
             except ConnectionError:
                 pass
             self.__log_debug("- DTLS shutdown complete")
@@ -500,37 +568,37 @@
         if receiver is not None:
             await receiver._handle_rtp_packet(packet, arrival_time_ms=arrival_time_ms)
 
     async def _recv_next(self) -> None:
         # get timeout
         timeout = None
         if not self.encrypted:
-            timeout = self.ssl.DTLSv1_get_timeout()
+            timeout = self._ssl.DTLSv1_get_timeout()
 
         # receive next datagram
         if timeout is not None:
             try:
                 data = await asyncio.wait_for(self.transport._recv(), timeout=timeout)
             except asyncio.TimeoutError:
                 self.__log_debug("x DTLS handling timeout")
-                self.ssl.DTLSv1_handle_timeout()
+                self._ssl.DTLSv1_handle_timeout()
                 await self._write_ssl()
                 return
         else:
             data = await self.transport._recv()
 
         self.__rx_bytes += len(data)
         self.__rx_packets += 1
 
         first_byte = data[0]
         if first_byte > 19 and first_byte < 64:
             # DTLS
-            self.ssl.bio_write(data)
+            self._ssl.bio_write(data)
             try:
-                data = self.ssl.recv(1500)
+                data = self._ssl.recv(1500)
             except SSL.ZeroReturnError:
                 data = None
             except SSL.Error:
                 data = b""
             await self._write_ssl()
             if data is None:
                 self.__log_debug("- DTLS shutdown by remote party")
@@ -573,15 +641,15 @@
         self._rtp_header_extensions_map.configure(parameters)
         self._rtp_router.register_sender(sender, ssrc=sender._ssrc)
 
     async def _send_data(self, data: bytes) -> None:
         if self._state != State.CONNECTED:
             raise ConnectionError("Cannot send encrypted data, not connected")
 
-        self.ssl.send(data)
+        self._ssl.send(data)
         await self._write_ssl()
 
     async def _send_rtp(self, data: bytes) -> None:
         if self._state != State.CONNECTED:
             raise ConnectionError("Cannot send encrypted RTP, not connected")
 
         if is_rtcp(data):
@@ -612,15 +680,15 @@
         self._rtp_router.unregister_sender(sender)
 
     async def _write_ssl(self) -> None:
         """
         Flush outgoing data which OpenSSL put in our BIO to the transport.
         """
         try:
-            data = self.ssl.bio_read(1500)
+            data = self._ssl.bio_read(1500)
         except SSL.Error:
             data = b""
         if data:
             await self.transport._send(data)
             self.__tx_bytes += len(data)
             self.__tx_packets += 1
```

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/rtcicetransport.py` & `crosslab_aiortc-1.8.0/src/aiortc/rtcicetransport.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/rtcpeerconnection.py` & `crosslab_aiortc-1.8.0/src/aiortc/rtcpeerconnection.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,18 +307,19 @@
         self.__sctp_mline_index: Optional[int] = None
         self._sctpLegacySdp = True
         self.__sctpRemotePort: Optional[int] = None
         self.__sctpRemoteCaps = None
         self.__stream_id = str(uuid.uuid4())
         self.__transceivers: List[RTCRtpTransceiver] = []
 
+        self.__closeTask: Optional[asyncio.Task] = None
         self.__connectionState = "new"
         self.__iceConnectionState = "new"
         self.__iceGatheringState = "new"
-        self.__isClosed = False
+        self.__isClosed: Optional[asyncio.Future[bool]] = None
         self.__signalingState = "stable"
 
         self.__currentLocalDescription: Optional[sdp.SessionDescription] = None
         self.__currentRemoteDescription: Optional[sdp.SessionDescription] = None
         self.__pendingLocalDescription: Optional[sdp.SessionDescription] = None
         self.__pendingRemoteDescription: Optional[sdp.SessionDescription] = None
 
@@ -475,16 +476,17 @@
         )
 
     async def close(self):
         """
         Terminate the ICE agent, ending ICE processing and streams.
         """
         if self.__isClosed:
+            await self.__isClosed
             return
-        self.__isClosed = True
+        self.__isClosed = asyncio.Future()
         self.__setSignalingState("closed")
 
         # stop senders / receivers
         for transceiver in self.__transceivers:
             await transceiver.stop()
         if self.__sctp:
             await self.__sctp.stop()
@@ -502,14 +504,16 @@
         self.__updateIceConnectionState()
         self.__updateConnectionState()
 
         # no more events will be emitted, so remove all event listeners
         # to facilitate garbage collection.
         self.remove_all_listeners()
 
+        self.__isClosed.set_result(True)
+
     async def createAnswer(self):
         """
         Create an SDP answer to an offer received from a remote peer during
         the offer/answer negotiation of a WebRTC connection.
 
         :rtype: :class:`RTCSessionDescription`
         """
@@ -781,15 +785,15 @@
                     transceiver._transport._set_role(media.dtls.role)
                 elif media.kind == "application":
                     self.__sctp.transport._set_role(media.dtls.role)
 
         # configure direction
         for t in self.__transceivers:
             if description.type in ["answer", "pranswer"]:
-                t._currentDirection = and_direction(t.direction, t._offerDirection)
+                t._setCurrentDirection(and_direction(t.direction, t._offerDirection))
 
         # gather candidates
         await self.__gather()
         for i, media in enumerate(description.media):
             if media.kind in ["audio", "video"]:
                 transceiver = self.__getTransceiverByMLineIndex(i)
                 add_transport_description(media, transceiver._transport)
@@ -863,15 +867,15 @@
                 transceiver._headerExtensions = find_common_header_extensions(
                     HEADER_EXTENSIONS[media.kind], media.rtp.headerExtensions
                 )
 
                 # configure direction
                 direction = reverse_direction(media.direction)
                 if description.type in ["answer", "pranswer"]:
-                    transceiver._currentDirection = direction
+                    transceiver._setCurrentDirection(direction)
                 else:
                     transceiver._offerDirection = direction
 
                 # create remote stream track
                 if (
                     direction in ["recvonly", "sendrecv"]
                     and not transceiver.receiver.track
@@ -1173,14 +1177,22 @@
 
         # update state
         if state != self.__connectionState:
             self.__log_debug("connectionState %s -> %s", self.__connectionState, state)
             self.__connectionState = state
             self.emit("connectionstatechange")
 
+        # if all DTLS connections are closed, initiate a shutdown
+        if (
+            not self.__isClosed
+            and self.__closeTask is None
+            and dtlsStates == set(["closed"])
+        ):
+            self.__closeTask = asyncio.ensure_future(self.close())
+
     def __updateIceConnectionState(self) -> None:
         # compute new state
         # NOTE: we do not have "connected" or "disconnected" states
         states = set(map(lambda x: x.state, self.__iceTransports))
         if self.__isClosed:
             state = "closed"
         elif "failed" in states:
```

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/rtcrtpparameters.py` & `crosslab_aiortc-1.8.0/src/aiortc/rtcrtpparameters.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/rtcrtpreceiver.py` & `crosslab_aiortc-1.8.0/src/aiortc/rtcrtpreceiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,14 +259,15 @@
     :param transport: An :class:`RTCDtlsTransport`.
     """
 
     def __init__(self, kind: str, transport: RTCDtlsTransport) -> None:
         if transport.state == "closed":
             raise InvalidStateError
 
+        self._enabled = True
         self.__active_ssrc: Dict[int, datetime.datetime] = {}
         self.__codecs: Dict[int, RTCRtpCodecParameters] = {}
         self.__decoder_queue: queue.Queue = queue.Queue()
         self.__decoder_thread: Optional[threading.Thread] = None
         self.__kind = kind
         if kind == "audio":
             self.__jitter_buffer = JitterBuffer(capacity=16, prefetch=4)
@@ -446,14 +447,18 @@
 
     async def _handle_rtp_packet(self, packet: RtpPacket, arrival_time_ms: int) -> None:
         """
         Handle an incoming RTP packet.
         """
         self.__log_debug("< %s", packet)
 
+        # If the receiver is disabled, discard the packet.
+        if not self._enabled:
+            return
+
         # feed bitrate estimator
         if self.__remote_bitrate_estimator is not None:
             if packet.extensions.abs_send_time is not None:
                 remb = self.__remote_bitrate_estimator.add(
                     abs_send_time=packet.extensions.abs_send_time,
                     arrival_time_ms=arrival_time_ms,
                     payload_size=len(packet.payload) + packet.padding_size,
```

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/rtcrtpsender.py` & `crosslab_aiortc-1.8.0/src/aiortc/rtcrtpsender.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             self.__kind = trackOrKind
             self.replaceTrack(None)
         self.__cname: Optional[str] = None
         self._ssrc = random32()
         self._rtx_ssrc = random32()
         # FIXME: how should this be initialised?
         self._stream_id = str(uuid.uuid4())
+        self._enabled = True
         self.__encoder: Optional[Encoder] = None
         self.__force_keyframe = False
         self.__loop = asyncio.get_event_loop()
         self.__mid: Optional[str] = None
         self.__rtp_exited = asyncio.Event()
         self.__rtp_header_extensions_map = rtp.HeaderExtensionsMap()
         self.__rtp_started = asyncio.Event()
@@ -264,14 +265,21 @@
                         self.__encoder.target_bitrate = bitrate
             except ValueError:
                 pass
 
     async def _next_encoded_frame(self, codec: RTCRtpCodecParameters):
         # get [Frame|Packet]
         data = await self.__track.recv()
+
+        # If the sender is disabled, drop the frame instead of encoding it.
+        # We still want to read from the track in order to avoid frames
+        # accumulating in memory.
+        if not self._enabled:
+            return None
+
         audio_level = None
 
         if self.__encoder is None:
             self.__encoder = get_encoder(codec)
 
         if isinstance(data, Frame):
             # encode frame
@@ -321,36 +329,42 @@
         timestamp_origin = random32()
         try:
             while True:
                 if not self.__track:
                     await asyncio.sleep(0.02)
                     continue
 
-                if hasattr(self.__track, 'raw_recv'):
-                    packet_bytes=await self.__track.raw_recv()
-                    packet=RtpPacket.parse(packet_bytes)
-                    packet.payload_type=codec.payloadType
+                if hasattr(self.__track, "raw_recv"):
+                    packet_bytes = await self.__track.raw_recv()
+                    packet = RtpPacket.parse(packet_bytes)
+                    packet.payload_type = codec.payloadType
                     packet.ssrc = self._ssrc
 
                     # set header extensions
                     packet.extensions.mid = self.__mid
 
                     # send packet
                     self.__log_debug("> %s", packet)
-                    self.__rtp_history[
-                        packet.sequence_number % RTP_HISTORY_SIZE
-                    ] = packet
+                    self.__rtp_history[packet.sequence_number % RTP_HISTORY_SIZE] = (
+                        packet
+                    )
                     packet_bytes = packet.serialize(self.__rtp_header_extensions_map)
                     await self.transport._send_rtp(packet_bytes)
 
+                    self.__ntp_timestamp = clock.current_ntp_time()
                     self.__rtp_timestamp = packet.timestamp
                     self.__octet_count += len(packet.payload)
                     self.__packet_count += 1
                 else:
+                    # Fetch the next encoded frame. This can be `None` if the sender
+                    # is disabled, in which case we just continue the loop.
                     enc_frame = await self._next_encoded_frame(codec)
+                    if enc_frame is None:
+                        continue
+
                     timestamp = uint32_add(timestamp_origin, enc_frame.timestamp)
 
                     for i, payload in enumerate(enc_frame.payloads):
                         packet = RtpPacket(
                             payload_type=codec.payloadType,
                             sequence_number=sequence_number,
                             timestamp=timestamp,
@@ -361,22 +375,27 @@
 
                         # set header extensions
                         packet.extensions.abs_send_time = (
                             clock.current_ntp_time() >> 14
                         ) & 0x00FFFFFF
                         packet.extensions.mid = self.__mid
                         if enc_frame.audio_level is not None:
-                            packet.extensions.audio_level = (False, -enc_frame.audio_level)
+                            packet.extensions.audio_level = (
+                                False,
+                                -enc_frame.audio_level,
+                            )
 
                         # send packet
                         self.__log_debug("> %s", packet)
                         self.__rtp_history[
                             packet.sequence_number % RTP_HISTORY_SIZE
                         ] = packet
-                        packet_bytes = packet.serialize(self.__rtp_header_extensions_map)
+                        packet_bytes = packet.serialize(
+                            self.__rtp_header_extensions_map
+                        )
                         await self.transport._send_rtp(packet_bytes)
 
                         self.__ntp_timestamp = clock.current_ntp_time()
                         self.__rtp_timestamp = packet.timestamp
                         self.__octet_count += len(payload)
                         self.__packet_count += 1
                         sequence_number = uint16_add(sequence_number, 1)
@@ -388,14 +407,18 @@
             self.__log_warning(traceback.format_exc())
 
         # stop track
         if self.__track:
             self.__track.stop()
             self.__track = None
 
+        # release encoder
+        if self.__encoder:
+            del self.__encoder
+
         self.__log_debug("- RTP finished")
         self.__rtp_exited.set()
 
     async def _run_rtcp(self) -> None:
         self.__log_debug("- RTCP started")
         self.__rtcp_started.set()
```

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/rtcrtptransceiver.py` & `crosslab_aiortc-1.8.0/src/aiortc/rtcrtptransceiver.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     def __init__(
         self,
         kind: str,
         receiver: RTCRtpReceiver,
         sender: RTCRtpSender,
         direction: str = "sendrecv",
     ):
+        self.__currentDirection: Optional[str] = None
         self.__direction = direction
         self.__kind = kind
         self.__mid: Optional[str] = None
         self.__mline_index: Optional[int] = None
         self.__receiver = receiver
         self.__sender = sender
         self.__stopped = False
 
-        self._currentDirection: Optional[str] = None
         self._offerDirection: Optional[str] = None
         self._preferred_codecs: List[RTCRtpCodecCapability] = []
         self._transport: RTCDtlsTransport = None
 
         # FIXME: this is only used by RTCPeerConnection
         self._bundled = False
         self._codecs: List[RTCRtpCodecParameters] = []
@@ -50,15 +50,15 @@
     @property
     def currentDirection(self) -> Optional[str]:
         """
         The currently negotiated direction of the transceiver.
 
         One of `'sendrecv'`, `'sendonly'`, `'recvonly'`, `'inactive'` or `None`.
         """
-        return self._currentDirection
+        return self.__currentDirection
 
     @property
     def direction(self) -> str:
         """
         The preferred direction of the transceiver, which will be used in
         :meth:`RTCPeerConnection.createOffer` and
         :meth:`RTCPeerConnection.createAnswer`.
@@ -126,14 +126,30 @@
         """
         Permanently stops the :class:`RTCRtpTransceiver`.
         """
         await self.__receiver.stop()
         await self.__sender.stop()
         self.__stopped = True
 
+    def _setCurrentDirection(self, direction: str) -> None:
+        self.__currentDirection = direction
+
+        if direction == "sendrecv":
+            self.__sender._enabled = True
+            self.__receiver._enabled = True
+        elif direction == "sendonly":
+            self.__sender._enabled = True
+            self.__receiver._enabled = False
+        elif direction == "recvonly":
+            self.__sender._enabled = False
+            self.__receiver._enabled = True
+        elif direction == "inactive":
+            self.__sender._enabled = False
+            self.__receiver._enabled = False
+
     def _set_mid(self, mid: str) -> None:
         self.__mid = mid
 
     def _get_mline_index(self) -> Optional[int]:
         return self.__mline_index
 
     def _set_mline_index(self, idx: int) -> None:
```

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/rtcsctptransport.py` & `crosslab_aiortc-1.8.0/src/aiortc/rtcsctptransport.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/rtp.py` & `crosslab_aiortc-1.8.0/src/aiortc/rtp.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/sdp.py` & `crosslab_aiortc-1.8.0/src/aiortc/sdp.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/stats.py` & `crosslab_aiortc-1.8.0/src/aiortc/stats.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/aiortc/utils.py` & `crosslab_aiortc-1.8.0/src/aiortc/utils.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/src/crosslab_aiortc.egg-info/PKG-INFO` & `crosslab_aiortc-1.8.0/src/crosslab_aiortc.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,73 @@
 Metadata-Version: 2.1
 Name: crosslab-aiortc
-Version: 1.5.0
+Version: 1.8.0
 Summary: An implementation of WebRTC and ORTC
-Author-email: Jeremy Lainé <jeremy.laine@m4x.org>
 License: BSD-3-Clause
-Project-URL: homepage, https://github.com/aiortc/aiortc
+Project-URL: homepage, https://github.com/GOLDi2/aiortc
 Project-URL: changelog, https://aiortc.readthedocs.io/en/stable/changelog.html
 Project-URL: documentation, https://aiortc.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: aioice<1.0.0,>=0.9.0
+Requires-Dist: av<12.0.0,>=9.0.0
+Requires-Dist: cffi>=1.0.0
+Requires-Dist: cryptography>=42.0.0
+Requires-Dist: dataclasses; python_version < "3.7"
+Requires-Dist: google-crc32c>=1.1
+Requires-Dist: pyee>=9.0.0
+Requires-Dist: pylibsrtp>=0.10.0
+Requires-Dist: pyopenssl>=24.0.0
+Provides-Extra: dev
+Requires-Dist: aiohttp>=3.7.0; extra == "dev"
+Requires-Dist: coverage[toml]>=7.2.2; extra == "dev"
+Requires-Dist: numpy>=1.19.0; extra == "dev"
+
+.. image:: docs/_static/aiortc.svg
+   :width: 120px
+   :alt: aiortc
+
+.. image:: https://img.shields.io/pypi/l/aiortc.svg
+   :target: https://pypi.python.org/pypi/aiortc
+   :alt: License
+
+.. image:: https://img.shields.io/pypi/v/aiortc.svg
+   :target: https://pypi.python.org/pypi/aiortc
+   :alt: Version
+
+.. image:: https://img.shields.io/pypi/pyversions/aiortc.svg
+   :target: https://pypi.python.org/pypi/aiortc
+   :alt: Python versions
+
+.. image:: https://github.com/aiortc/aiortc/workflows/tests/badge.svg
+   :target: https://github.com/aiortc/aiortc/actions
+   :alt: Tests
+
+.. image:: https://img.shields.io/codecov/c/github/aiortc/aiortc.svg
+   :target: https://codecov.io/gh/aiortc/aiortc
+   :alt: Coverage
 
-aiortc
-======
-
-|rtd| |pypi-v| |pypi-pyversions| |pypi-l| |tests| |codecov| |gitter|
-
-.. |rtd| image:: https://readthedocs.org/projects/aiortc/badge/?version=latest
+.. image:: https://readthedocs.org/projects/aiortc/badge/?version=latest
    :target: https://aiortc.readthedocs.io/
+   :alt: Documentation
 
-.. |pypi-v| image:: https://img.shields.io/pypi/v/aiortc.svg
-    :target: https://pypi.python.org/pypi/aiortc
-
-.. |pypi-pyversions| image:: https://img.shields.io/pypi/pyversions/aiortc.svg
-    :target: https://pypi.python.org/pypi/aiortc
-
-.. |pypi-l| image:: https://img.shields.io/pypi/l/aiortc.svg
-    :target: https://pypi.python.org/pypi/aiortc
-
-.. |tests| image:: https://github.com/aiortc/aiortc/workflows/tests/badge.svg
-    :target: https://github.com/aiortc/aiortc/actions
-
-.. |codecov| image:: https://img.shields.io/codecov/c/github/aiortc/aiortc.svg
-    :target: https://codecov.io/gh/aiortc/aiortc
-
-.. |gitter| image:: https://img.shields.io/gitter/room/aiortc/Lobby.svg
-    :target: https://gitter.im/aiortc/Lobby
+This is a fork of the aiortc project with slight modification neeeded in the crosslab project
 
 What is ``aiortc``?
 -------------------
 
 ``aiortc`` is a library for `Web Real-Time Communication (WebRTC)`_ and
 `Object Real-Time Communication (ORTC)`_ in Python. It is built on top of
 ``asyncio``, Python's standard asynchronous I/O framework.
@@ -106,56 +121,46 @@
 - Sending and receiving video (VP8 / H.264)
 - Bundling audio / video / data channels
 - RTCP reports, including NACK / PLI to recover from packet loss
 
 Installing
 ----------
 
-Since release 0.9.28 binary wheels are available on PyPI for Linux, Mac and
-Windows. The easiest way to install ``aiortc`` is to run:
+The easiest way to install ``aiortc`` is to run:
 
 .. code:: bash
 
     pip install aiortc
 
 Building from source
 --------------------
 
 If there are no wheels for your system or if you wish to build aiortc from
 source you will need a couple of libraries installed on your system:
 
-- OpenSSL 1.0.2 or greater
-- FFmpeg 4.0 or greater
-- LibVPX for video encoding / decoding
 - Opus for audio encoding / decoding
+- LibVPX for video encoding / decoding
 
 Linux
 .....
 
 On Debian/Ubuntu run:
 
 .. code:: bash
 
-    apt install libavdevice-dev libavfilter-dev libopus-dev libvpx-dev pkg-config
-
-`pylibsrtp` comes with binary wheels for most platforms, but if it needs to be
-built from you will also need to run:
-
-.. code:: bash
-
-    apt install libsrtp2-dev
+    apt install libopus-dev libvpx-dev
 
 OS X
 ....
 
 On OS X run:
 
 .. code:: bash
 
-    brew install ffmpeg opus libvpx pkg-config
+    brew install opus libvpx
 
 License
 -------
 
 ``aiortc`` is released under the `BSD license`_.
 
 .. _BSD license: https://aiortc.readthedocs.io/en/latest/license.html
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `crosslab-aiortc-1.5.0/src/crosslab_aiortc.egg-info/SOURCES.txt` & `crosslab_aiortc-1.8.0/src/crosslab_aiortc.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 src/aiortc/rtcsctptransport.py
 src/aiortc/rtcsessiondescription.py
 src/aiortc/rtp.py
 src/aiortc/sdp.py
 src/aiortc/stats.py
 src/aiortc/utils.py
 src/aiortc/codecs/__init__.py
+src/aiortc/codecs/_opus.pyi
+src/aiortc/codecs/_vpx.pyi
 src/aiortc/codecs/base.py
 src/aiortc/codecs/g711.py
 src/aiortc/codecs/h264.py
 src/aiortc/codecs/opus.py
 src/aiortc/codecs/vpx.py
 src/aiortc/contrib/__init__.py
 src/aiortc/contrib/media.py
```

### Comparing `crosslab-aiortc-1.5.0/tests/codecs.py` & `crosslab_aiortc-1.8.0/tests/codecs.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/h264_0001.bin` & `crosslab_aiortc-1.8.0/tests/h264_0001.bin`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/h264_0002.bin` & `crosslab_aiortc-1.8.0/tests/h264_0002.bin`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/h264_0003.bin` & `crosslab_aiortc-1.8.0/tests/h264_0003.bin`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_clock.py` & `crosslab_aiortc-1.8.0/tests/test_clock.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_contrib_media.py` & `crosslab_aiortc-1.8.0/tests/test_contrib_media.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_contrib_signaling.py` & `crosslab_aiortc-1.8.0/tests/test_contrib_signaling.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_g711.py` & `crosslab_aiortc-1.8.0/tests/test_g711.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_h264.py` & `crosslab_aiortc-1.8.0/tests/test_h264.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,43 +209,43 @@
     def test_split_bitstream(self):
         # No start code
         packages = list(H264Encoder._split_bitstream(b"\x00\x00\x00\x00"))
         self.assertEqual(packages, [])
 
         # 3-byte start code
         packages = list(
-            H264Encoder._split_bitstream(b"\x00\x00\x01\xFF\x00\x00\x01\xFB")
+            H264Encoder._split_bitstream(b"\x00\x00\x01\xff\x00\x00\x01\xfb")
         )
-        self.assertEqual(packages, [b"\xFF", b"\xFB"])
+        self.assertEqual(packages, [b"\xff", b"\xfb"])
 
         # 4-byte start code
         packages = list(
-            H264Encoder._split_bitstream(b"\x00\x00\x00\x01\xFF\x00\x00\x00\x01\xFB")
+            H264Encoder._split_bitstream(b"\x00\x00\x00\x01\xff\x00\x00\x00\x01\xfb")
         )
-        self.assertEqual(packages, [b"\xFF", b"\xFB"])
+        self.assertEqual(packages, [b"\xff", b"\xfb"])
 
         # Multiple bytes in a packet
         packages = list(
             H264Encoder._split_bitstream(
-                b"\x00\x00\x00\x01\xFF\xAB\xCD\x00\x00\x00\x01\xFB"
+                b"\x00\x00\x00\x01\xff\xab\xcd\x00\x00\x00\x01\xfb"
             )
         )
-        self.assertEqual(packages, [b"\xFF\xAB\xCD", b"\xFB"])
+        self.assertEqual(packages, [b"\xff\xab\xcd", b"\xfb"])
 
         # Skip leading 0s
-        packages = list(H264Encoder._split_bitstream(b"\x00\x00\x00\x01\xFF"))
-        self.assertEqual(packages, [b"\xFF"])
+        packages = list(H264Encoder._split_bitstream(b"\x00\x00\x00\x01\xff"))
+        self.assertEqual(packages, [b"\xff"])
 
         # Both leading and trailing 0s
         packages = list(
             H264Encoder._split_bitstream(
-                b"\x00\x00\x00\x00\x00\x00\x01\xFF\x00\x00\x00\x00\x00"
+                b"\x00\x00\x00\x00\x00\x00\x01\xff\x00\x00\x00\x00\x00"
             )
         )
-        self.assertEqual(packages, [b"\xFF\x00\x00\x00\x00\x00"])
+        self.assertEqual(packages, [b"\xff\x00\x00\x00\x00\x00"])
 
     def test_packetize_one_small(self):
         packages = [bytes([0xFF, 0xFF])]
         packetize_packages = H264Encoder._packetize(packages)
         self.assertListEqual(packages, packetize_packages)
 
         packages = [bytes([0xFF]) * 1300]
```

### Comparing `crosslab-aiortc-1.5.0/tests/test_jitterbuffer.py` & `crosslab_aiortc-1.8.0/tests/test_jitterbuffer.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_mediastreams.py` & `crosslab_aiortc-1.8.0/tests/test_mediastreams.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_opus.py` & `crosslab_aiortc-1.8.0/tests/test_opus.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_ortc.py` & `crosslab_aiortc-1.8.0/tests/test_ortc.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_rate.py` & `crosslab_aiortc-1.8.0/tests/test_rate.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_rtcdtlstransport.py` & `crosslab_aiortc-1.8.0/tests/test_rtcdtlstransport.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import asyncio
 import datetime
 from unittest import TestCase
 from unittest.mock import patch
 
 from aiortc.rtcdtlstransport import (
+    SRTP_AEAD_AES_256_GCM,
+    SRTP_AES128_CM_SHA1_80,
     RTCCertificate,
     RTCDtlsFingerprint,
     RTCDtlsParameters,
     RTCDtlsTransport,
     RtpRouter,
 )
 from aiortc.rtcrtpparameters import (
@@ -401,14 +403,36 @@
 
         await asyncio.gather(
             session1.start(session2.getLocalParameters()),
             session2.start(session1.getLocalParameters()),
         )
         self.assertEqual(session1.state, "failed")
         self.assertEqual(session2.state, "failed")
+
+        await session1.stop()
+        await session2.stop()
+
+    @asynctest
+    async def test_handshake_error_no_common_srtp_profile(self):
+        transport1, transport2 = dummy_ice_transport_pair()
+
+        certificate1 = RTCCertificate.generateCertificate()
+        session1 = RTCDtlsTransport(transport1, [certificate1])
+        session1._srtp_profiles = [SRTP_AEAD_AES_256_GCM]
+
+        certificate2 = RTCCertificate.generateCertificate()
+        session2 = RTCDtlsTransport(transport2, [certificate2])
+        session2._srtp_profiles = [SRTP_AES128_CM_SHA1_80]
+
+        await asyncio.gather(
+            session1.start(session2.getLocalParameters()),
+            session2.start(session1.getLocalParameters()),
+        )
+        self.assertEqual(session1.state, "failed")
+        self.assertEqual(session2.state, "failed")
 
         await session1.stop()
         await session2.stop()
 
     @asynctest
     async def test_lossy_channel(self):
         """
```

### Comparing `crosslab-aiortc-1.5.0/tests/test_rtcicetransport.py` & `crosslab_aiortc-1.8.0/tests/test_rtcicetransport.py`

 * *Files 7% similar despite different names*

```diff
@@ -258,23 +258,29 @@
             [RTCIceServer(urls="stun:stun.l.google.com:19302")],
         )
 
 
 class RTCIceTransportTest(TestCase):
     def setUp(self):
         # save timers
+        self.consent_failures = aioice.ice.CONSENT_FAILURES
+        self.consent_interval = aioice.ice.CONSENT_INTERVAL
         self.retry_max = aioice.stun.RETRY_MAX
         self.retry_rto = aioice.stun.RETRY_RTO
 
         # shorten timers to run tests faster
+        aioice.ice.CONSENT_FAILURES = 1
+        aioice.ice.CONSENT_INTERVAL = 1
         aioice.stun.RETRY_MAX = 1
         aioice.stun.RETRY_RTO = 0.1
 
     def tearDown(self):
         # restore timers
+        aioice.ice.CONSENT_FAILURES = self.consent_failures
+        aioice.ice.CONSENT_INTERVAL = self.consent_interval
         aioice.stun.RETRY_MAX = self.retry_max
         aioice.stun.RETRY_RTO = self.retry_rto
 
     @asynctest
     async def test_construct(self):
         gatherer = RTCIceGatherer()
         connection = RTCIceTransport(gatherer)
@@ -354,14 +360,50 @@
 
         # cleanup
         await asyncio.gather(transport_1.stop(), transport_2.stop())
         self.assertEqual(transport_1.state, "closed")
         self.assertEqual(transport_2.state, "closed")
 
     @asynctest
+    async def test_connect_then_consent_expires(self):
+        gatherer_1 = RTCIceGatherer()
+        transport_1 = RTCIceTransport(gatherer_1)
+
+        gatherer_2 = RTCIceGatherer()
+        transport_2 = RTCIceTransport(gatherer_2)
+
+        # gather candidates
+        await asyncio.gather(gatherer_1.gather(), gatherer_2.gather())
+        for candidate in gatherer_2.getLocalCandidates():
+            await transport_1.addRemoteCandidate(candidate)
+        for candidate in gatherer_1.getLocalCandidates():
+            await transport_2.addRemoteCandidate(candidate)
+        self.assertEqual(transport_1.state, "new")
+        self.assertEqual(transport_2.state, "new")
+
+        # connect
+        await asyncio.gather(
+            transport_1.start(gatherer_2.getLocalParameters()),
+            transport_2.start(gatherer_1.getLocalParameters()),
+        )
+        self.assertEqual(transport_1.state, "completed")
+        self.assertEqual(transport_2.state, "completed")
+
+        # close one side
+        await transport_1.stop()
+        self.assertEqual(transport_1.state, "closed")
+
+        # wait for consent to expire
+        await asyncio.sleep(2)
+
+        # close other side
+        await transport_2.stop()
+        self.assertEqual(transport_2.state, "closed")
+
+    @asynctest
     async def test_connect_when_closed(self):
         gatherer = RTCIceGatherer()
         transport = RTCIceTransport(gatherer)
 
         # stop transport
         await transport.stop()
         self.assertEqual(transport.state, "closed")
```

### Comparing `crosslab-aiortc-1.5.0/tests/test_rtcpeerconnection.py` & `crosslab_aiortc-1.8.0/tests/test_rtcpeerconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -508,14 +508,19 @@
         transport = transceivers[0].receiver.transport
         for i in range(1, len(transceivers)):
             self.assertEqual(transceivers[i].receiver.transport, transport)
             self.assertEqual(transceivers[i].sender.transport, transport)
         if pc.sctp:
             self.assertEqual(pc.sctp.transport, transport)
 
+    def assertClosed(self, pc):
+        self.assertEqual(pc.connectionState, "closed")
+        self.assertEqual(pc.iceConnectionState, "closed")
+        self.assertEqual(pc.signalingState, "closed")
+
     async def assertDataChannelOpen(self, dc):
         await self.sleepWhile(lambda: dc.readyState == "connecting")
         self.assertEqual(dc.readyState, "open")
 
     async def assertIceChecking(self, pc):
         await self.sleepWhile(lambda: pc.iceConnectionState == "new")
         self.assertEqual(pc.iceConnectionState, "checking")
@@ -549,29 +554,23 @@
         total = 0.0
         while f() and total < max_sleep:
             await asyncio.sleep(sleep)
             total += sleep
 
     def setUp(self):
         # save timers
-        self.consent_failures = aioice.ice.CONSENT_FAILURES
-        self.consent_interval = aioice.ice.CONSENT_INTERVAL
         self.retry_max = aioice.stun.RETRY_MAX
         self.retry_rto = aioice.stun.RETRY_RTO
 
         # shorten timers to run tests faster
-        aioice.ice.CONSENT_FAILURES = 1
-        aioice.ice.CONSENT_INTERVAL = 1
         aioice.stun.RETRY_MAX = 1
         aioice.stun.RETRY_RTO = 0.1
 
     def tearDown(self):
         # restore timers
-        aioice.ice.CONSENT_FAILURES = self.consent_failures
-        aioice.ice.CONSENT_INTERVAL = self.consent_interval
         aioice.stun.RETRY_MAX = self.retry_max
         aioice.stun.RETRY_RTO = self.retry_rto
 
     @asynctest
     async def test_addIceCandidate_no_sdpMid_or_sdpMLineIndex(self):
         pc = RTCPeerConnection()
         with self.assertRaises(ValueError) as cm:
@@ -898,16 +897,16 @@
                 "transport",
             ],
         )
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1029,16 +1028,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1090,24 +1089,20 @@
 
         # handle answer
         await pc1.setRemoteDescription(pc2.localDescription)
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
-        # close one side
+        # close one side, which causes the other to shutdown
         await pc1.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-
-        # wait for consent to expire
-        await asyncio.sleep(2)
+        await asyncio.sleep(1)
 
-        # close other side
-        await pc2.close()
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1117,20 +1112,18 @@
         )
         self.assertEqual(
             pc1_states["signalingState"],
             ["stable", "have-local-offer", "stable", "closed"],
         )
 
         self.assertEqual(
-            pc2_states["connectionState"],
-            ["new", "connecting", "connected", "failed", "closed"],
+            pc2_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
-            pc2_states["iceConnectionState"],
-            ["new", "checking", "completed", "failed", "closed"],
+            pc2_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
         )
         self.assertEqual(
             pc2_states["iceGatheringState"], ["new", "gathering", "complete"]
         )
         self.assertEqual(
             pc2_states["signalingState"],
             ["stable", "have-remote-offer", "stable", "closed"],
@@ -1245,16 +1238,16 @@
                 "transport",
             ],
         )
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1352,16 +1345,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1456,16 +1449,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1561,16 +1554,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1665,16 +1658,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1767,16 +1760,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1870,16 +1863,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1972,16 +1965,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -2072,16 +2065,16 @@
         # check a single transport is used
         self.assertBundled(pc1)
         self.assertBundled(pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -2187,16 +2180,16 @@
         if stop_tracks:
             player.audio.stop()
             player.video.stop()
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -2298,16 +2291,16 @@
         # check a single transport is used
         self.assertBundled(pc1)
         self.assertBundled(pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -2404,16 +2397,16 @@
         await done.wait()
         self.assertEqual(pc1.iceConnectionState, "closed")
         self.assertEqual(pc2.iceConnectionState, "failed")
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(pc1_states["connectionState"], ["new", "closed"])
         self.assertEqual(pc1_states["iceConnectionState"], ["new", "closed"])
         self.assertEqual(
             pc1_states["iceGatheringState"], ["new", "gathering", "complete"]
         )
@@ -2544,16 +2537,16 @@
         # check a single transport is used
         self.assertBundled(pc1)
         self.assertBundled(pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"],
             ["new", "connecting", "connected", "connecting", "connected", "closed"],
         )
         self.assertEqual(
@@ -2685,16 +2678,16 @@
                 "transport",
             ],
         )
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -2793,16 +2786,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -2899,16 +2892,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -3011,16 +3004,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -3120,16 +3113,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -3182,16 +3175,16 @@
         await self.assertIceCompleted(pc1, pc2)
         self.assertEqual(dc1.readyState, "closed")
         await self.assertDataChannelOpen(dc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
     @asynctest
     async def test_connect_datachannel_negotiated_and_close_immediately(self):
         pc1 = RTCPeerConnection()
         pc2 = RTCPeerConnection()
 
         # create two negotiated data channels
@@ -3215,16 +3208,16 @@
         await self.assertIceCompleted(pc1, pc2)
         self.assertEqual(dc1.readyState, "closed")
         await self.assertDataChannelOpen(dc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
     @asynctest
     async def test_connect_datachannel_legacy_sdp(self):
         pc1 = RTCPeerConnection()
         pc1._sctpLegacySdp = True
         pc1_data_messages = []
         pc1_states = track_states(pc1)
@@ -3354,16 +3347,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -3516,16 +3509,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -3673,16 +3666,16 @@
 
         # close data channels
         await self.closeDataChannel(dc1)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -3744,16 +3737,16 @@
         dc4 = pc1.createDataChannel("chat4")
         await self.assertDataChannelOpen(dc4)
         self.assertEqual(dc4.id, 3)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
     def test_create_datachannel_with_maxpacketlifetime_and_maxretransmits(self):
         pc = RTCPeerConnection()
         with self.assertRaises(ValueError) as cm:
             pc.createDataChannel("chat", maxPacketLifeTime=500, maxRetransmits=0)
         self.assertEqual(
             str(cm.exception),
@@ -3964,16 +3957,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"],
             ["new", "connecting", "connected", "connecting", "connected", "closed"],
         )
         self.assertEqual(
@@ -4157,16 +4150,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -4263,16 +4256,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -4369,16 +4362,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -4505,16 +4498,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -4934,16 +4927,16 @@
 
         # allow media to flow long enough to collect stats
         await asyncio.sleep(2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
```

### Comparing `crosslab-aiortc-1.5.0/tests/test_rtcrtpreceiver.py` & `crosslab_aiortc-1.8.0/tests/test_rtcrtpreceiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,14 +446,36 @@
             await receiver.receive(RTCRtpReceiveParameters(codecs=[VP8_CODEC]))
 
             # receive RTP with unknown payload type
             packet = RtpPacket(payload_type=123)
             await receiver._handle_rtp_packet(packet, arrival_time_ms=0)
 
     @asynctest
+    async def test_rtp_disabled(self):
+        async with create_receiver("audio") as receiver:
+            self.assertEqual(receiver._enabled, True)
+            receiver._track = RemoteStreamTrack(kind="audio")
+
+            await receiver.receive(RTCRtpReceiveParameters(codecs=[PCMU_CODEC]))
+            receiver._enabled = False
+            self.assertEqual(receiver._enabled, False)
+
+            # receive RTP while disabled.
+            packet = RtpPacket(payload_type=0)
+            await receiver._handle_rtp_packet(packet, arrival_time_ms=0)
+
+            # check stats
+            report = await receiver.getStats()
+            self.assertIsInstance(report, RTCStatsReport)
+            self.assertEqual(
+                sorted([s.type for s in report.values()]),
+                ["transport"],
+            )
+
+    @asynctest
     async def test_rtp_rtx(self):
         async with create_receiver("video") as receiver:
             receiver._track = RemoteStreamTrack(kind="video")
 
             await receiver.receive(
                 RTCRtpReceiveParameters(
                     codecs=[
```

### Comparing `crosslab-aiortc-1.5.0/tests/test_rtcrtpsender.py` & `crosslab_aiortc-1.8.0/tests/test_rtcrtpsender.py`

 * *Files 5% similar despite different names*

```diff
@@ -386,14 +386,39 @@
                     break
             self.assertIsNotNone(found_rtx)
             self.assertEqual(found_rtx.payload_type, 101)
             self.assertEqual(found_rtx.ssrc, 2345)
             self.assertEqual(found_rtx.payload[0:2], pack("!H", packet.sequence_number))
 
     @asynctest
+    async def test_disabled(self):
+        async with dummy_dtls_transport_pair() as (local_transport, _):
+            sender = RTCRtpSender(AudioStreamTrack(), local_transport)
+            self.assertEqual(sender.kind, "audio")
+            self.assertEqual(sender._enabled, True)
+
+            await sender.send(RTCRtpParameters(codecs=[PCMU_CODEC]))
+            sender._enabled = False
+            self.assertEqual(sender._enabled, False)
+
+            # check stats
+            report = await sender.getStats()
+            self.assertIsInstance(report, RTCStatsReport)
+            self.assertEqual(
+                sorted([s.type for s in report.values()]),
+                ["outbound-rtp", "transport"],
+            )
+
+            outbound_rtp = report["outbound-rtp_" + str(id(sender))]
+            self.assertEqual(outbound_rtp.packetsSent, 0)
+
+            # clean shutdown
+            await sender.stop()
+
+    @asynctest
     async def test_stop(self):
         async with dummy_dtls_transport_pair() as (local_transport, _):
             sender = RTCRtpSender(AudioStreamTrack(), local_transport)
             self.assertEqual(sender.kind, "audio")
 
             await sender.send(RTCRtpParameters(codecs=[PCMU_CODEC]))
```

### Comparing `crosslab-aiortc-1.5.0/tests/test_rtcrtptransceiver.py` & `crosslab_aiortc-1.8.0/tests/test_rtcrtptransceiver.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_rtcsctptransport.py` & `crosslab_aiortc-1.8.0/tests/test_rtcsctptransport.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_rtcsessiondescription.py` & `crosslab_aiortc-1.8.0/tests/test_rtcsessiondescription.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_rtp.py` & `crosslab_aiortc-1.8.0/tests/test_rtp.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_sdp.py` & `crosslab_aiortc-1.8.0/tests/test_sdp.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_utils.py` & `crosslab_aiortc-1.8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/test_vpx.py` & `crosslab_aiortc-1.8.0/tests/test_vpx.py`

 * *Files identical despite different names*

### Comparing `crosslab-aiortc-1.5.0/tests/utils.py` & `crosslab_aiortc-1.8.0/tests/utils.py`

 * *Files identical despite different names*


#
# Copyright (c) 2018 Nordic Semiconductor
#
# SPDX-License-Identifier: LicenseRef-BSD-5-Clause-Nordic
#

set(NRFXLIB_DIR ${CMAKE_CURRENT_LIST_DIR})
add_subdirectory_ifdef(CONFIG_NRFXLIB_NFC    nfc)
add_subdirectory_ifdef(CONFIG_BT_LL_NRFXLIB  ble_controller)
add_subdirectory_ifdef(CONFIG_BSD_LIBRARY    bsdlib)
add_subdirectory_ifdef(CONFIG_NRFXLIB_CRYPTO crypto)

#
# Copyright (C) 2020-2022 HandsomeMod Project
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=qcom-firmware
PKG_VERSION:=r1034.2.1
PKG_RELEASE:=2

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/humuu135/handsomemod-qcom-firmware
PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.xz
PKG_SOURCE_VERSION:=e26b4ea4792928fe15477db1a32aecf869a9a361
PKG_MIRROR_HASH:=9793b00f252e5ffe24c30bde330dea6e2d9f1a7fcd1f0c1528d11fefcb5d6df6

PKG_MAINTAINER:=Handsomeyingyan <handsomeyingyan@gmail.com>
STRIP:=:

include $(INCLUDE_DIR)/package.mk

define Package/qcom-firmware-default
  SECTION:=firmware
  CATEGORY:=Firmware
endef

define Build/Compile
	mkdir $(PKG_BUILD_DIR)/dragonboard
	mcopy -i $(PKG_BUILD_DIR)/dragonboard-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/dragonboard
	mkdir $(PKG_BUILD_DIR)/openstick-ufi001b
	mcopy -i $(PKG_BUILD_DIR)/openstick-ufi001b-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-ufi001b
	mkdir $(PKG_BUILD_DIR)/openstick-ufi001c
	mcopy -i $(PKG_BUILD_DIR)/openstick-ufi001c-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-ufi001c
	mkdir $(PKG_BUILD_DIR)/openstick-ufi003
	mcopy -i $(PKG_BUILD_DIR)/openstick-ufi003-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-ufi003
	mkdir $(PKG_BUILD_DIR)/openstick-sp970
	mcopy -i $(PKG_BUILD_DIR)/openstick-sp970-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-sp970
	mkdir $(PKG_BUILD_DIR)/openstick-uz801
	mcopy -i $(PKG_BUILD_DIR)/openstick-uz801-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-uz801
	mkdir $(PKG_BUILD_DIR)/openstick-hmuf02
	mcopy -i $(PKG_BUILD_DIR)/openstick-hmuf02-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-hmuf02
	mkdir $(PKG_BUILD_DIR)/openstick-jz01
	mcopy -i $(PKG_BUILD_DIR)/openstick-jz01-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-jz01
	mkdir $(PKG_BUILD_DIR)/wt88047
	mcopy -i $(PKG_BUILD_DIR)/wt88047-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/wt88047
	mkdir $(PKG_BUILD_DIR)/wt86047
	mcopy -i $(PKG_BUILD_DIR)/wt86047-modem.bin -p -m -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/wt86047	
endef

define Package/qcom-apq8016-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm apq8016 WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-ufi001b-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick UFI001B WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-ufi001c-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick UFI001C WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-ufi003-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick UFI003 WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-sp970-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick SP970 WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-uz801-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick UZ801 WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-hmuf02-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick HMUF02 WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-jz01-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Openstick JZ01 WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-wt8x047-wcnss-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Redmi 2 WIFI & Bluetooth firmware
endef

define Package/qcom-apq8016-wcnss-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm apq8016 WIFI nv data
endef

define Package/qcom-msm8916-wcnss-wt88047-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Wingtech Wt88047
endef

define Package/qcom-msm8916-wcnss-openstick-ufi001b-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick UFI001B
endef

define Package/qcom-msm8916-wcnss-openstick-ufi001c-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick UFI001C
endef

define Package/qcom-msm8916-wcnss-openstick-ufi003-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick UFI003
endef

define Package/qcom-msm8916-wcnss-openstick-sp970-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick SP970
endef

define Package/qcom-msm8916-wcnss-openstick-uz801-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick UZ801
endef

define Package/qcom-msm8916-wcnss-openstick-hmuf02-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick HMUF02
endef

define Package/qcom-msm8916-wcnss-openstick-jz01-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Handsome Openstick JZ01
endef

define Package/qcom-apq8016-modem-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm apq8016 modem firmware
endef

define Package/qcom-msm8916-modem-wt88047-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for wingtech wt88047
endef

define Package/qcom-msm8916-modem-wt86047-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for wingtech wt86047
endef

define Package/qcom-msm8916-modem-openstick-ufi001b-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick UFI001B
endef

define Package/qcom-msm8916-modem-openstick-ufi001c-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick UFI001C
endef

define Package/qcom-msm8916-modem-openstick-ufi003-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick UFI003
endef

define Package/qcom-msm8916-modem-openstick-sp970-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick SP970
endef

define Package/qcom-msm8916-modem-openstick-uz801-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick UZ801
endef

define Package/qcom-msm8916-modem-openstick-hmuf02-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick HMUF02
endef

define Package/qcom-msm8916-modem-openstick-jz01-firmware
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Handsome Openstick JZ01
endef

define Package/qcom-apq8016-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/dragonboard/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-ufi001b-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-ufi001c-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001c/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-ufi003-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-sp970-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-uz801-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-hmuf02-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-hmuf02/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-jz01-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-jz01/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-wt8x047-wcnss-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-apq8016-wcnss-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/dragonboard-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-wcnss-wt88047-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt8x047-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-wcnss-openstick-ufi001b-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-wcnss-openstick-ufi001c-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001c-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-wcnss-openstick-ufi003-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-wcnss-openstick-sp970-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-wcnss-openstick-uz801-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-wcnss-openstick-hmuf02-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-hmuf02-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-wcnss-openstick-jz01-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-jz01-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-apq8016-modem-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/dragonboard/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/dragonboard/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-wt88047-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-wt86047-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt86047/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt86047/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-openstick-ufi001b-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-openstick-ufi001c-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001c/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001c/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-openstick-ufi003-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-openstick-sp970-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-openstick-uz801-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-openstick-hmuf02-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-hmuf02/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-hmuf02/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-modem-openstick-jz01-firmware/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-jz01/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-jz01/modem.* \
		$(1)/lib/firmware
endef

$(eval $(call BuildPackage,qcom-apq8016-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi001b-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi001c-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi003-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-sp970-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-uz801-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-hmuf02-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-openstick-jz01-wcnss-firmware))
$(eval $(call BuildPackage,qcom-msm8916-wt8x047-wcnss-firmware))
$(eval $(call BuildPackage,qcom-apq8016-wcnss-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-wt88047-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-ufi001b-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-ufi001c-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-ufi003-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-sp970-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-uz801-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-hmuf02-nv))
$(eval $(call BuildPackage,qcom-msm8916-wcnss-openstick-jz01-nv))
$(eval $(call BuildPackage,qcom-apq8016-modem-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-wt88047-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-wt86047-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-ufi001b-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-ufi001c-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-ufi003-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-sp970-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-uz801-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-hmuf02-firmware))
$(eval $(call BuildPackage,qcom-msm8916-modem-openstick-jz01-firmware))

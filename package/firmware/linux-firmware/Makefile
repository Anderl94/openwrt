#
# Copyright (C) 2014 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=linux-firmware
PKG_VERSION:=20240510
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/pesa1234/linux-firmware-next
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2024-05-10
PKG_SOURCE_VERSION:=0df1489f7aa846eb297ddd1df4545693bd6a3520
PKG_MIRROR_HASH:=10ed061a7bcef5647b6deeedfbfd39722fea5327ca9d909dff0e900ddc7a90ce

PKG_MAINTAINER:=Felix Fietkau <nbd@nbd.name>

SCAN_DEPS = *.mk

include $(INCLUDE_DIR)/package.mk

RSTRIP:=:
STRIP:=:

define Package/firmware-default
  SECTION:=firmware
  CATEGORY:=Firmware
  URL:=https://github.com/pesa1234/linux-firmware-next.git
  TITLE:=$(1)
  DEPENDS:=$(2)
  LICENSE_FILES:=$(3)
  LICENSE:=$(4)
endef

define Build/Compile

endef

include $(wildcard ./*.mk)
#$(eval $(call BuildPackage,linux-firmware))

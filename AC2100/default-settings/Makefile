#
# Copyright (C) 2016-2023 GitHub 
#
# This is free software, licensed under the GNU General Public License v3.
# See /LICENSE for more information.


include $(TOPDIR)/rules.mk

PKG_NAME:=default-settings              #定义包名
PKG_VERSION:=2
PKG_RELEASE:=37
PKG_LICENSE:=GPLv3
PKG_LICENSE_FILES:=LICENSE

include $(INCLUDE_DIR)/package.mk

define Package/default-settings         #设置包信息和依赖
  SECTION:=luci
  CATEGORY:=LuCI
  TITLE:=LuCI support for Default Settings
  PKGARCH:=all
  DEPENDS:=+luci-base +luci 
endef

define Package/default-settings/description
        Language Support Packages.
endef

define Build/Compile
endef

define Package/default-settings/install     #把文件 99-default-settings 写入 /etc/uci-defaults/ 目录下，如果是其他文件的话也可以用这种方法把特定文件写入固件中，比如证书
        $(INSTALL_DIR) $(1)/etc/uci-defaults
        $(INSTALL_BIN) ./files/zzz-default-settings $(1)/etc/uci-defaults/99-default-settings
endef

$(eval $(call BuildPackage,default-settings))

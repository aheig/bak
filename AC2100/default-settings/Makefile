include $(TOPDIR)/rules.mk

PKG_NAME:=default-settings              #定义包名
PKG_VERSION:=1
PKG_RELEASE:=1
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
        LuCI support for Default Settings.
endef

define Build/Compile
endef

define Package/default-settings/install     #把文件 99-default-settings 写入 /etc/uci-defaults/ 目录下，如果是其他文件的话也可以用这种方法把特定文件写入固件中，比如证书
        $(INSTALL_DIR) $(1)/etc/uci-defaults
        $(INSTALL_BIN) ./files/99-default-settings $(1)/etc/uci-defaults/99-default-settings
endef

$(eval $(call BuildPackage,default-settings))

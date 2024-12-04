include $(ROOTDIR)/rules.mk

PKG_NAME:=ss-tunnel-xor
PKG_SOURCE_DATE:=2024-12-03

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/lixingcong/ss-tunnel-xor
PKG_SOURCE_VERSION:=610e340559e302c930a192d821c1ba1107a79795

include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/cmake.mk

$(eval $(call BuildPackage,ss-tunnel-xor))

romfs:
	$(INSTALL_DIR) $(ROMFSDIR)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/ss-tunnel-xor $(ROMFSDIR)/usr/bin/ss-tunnel-xor

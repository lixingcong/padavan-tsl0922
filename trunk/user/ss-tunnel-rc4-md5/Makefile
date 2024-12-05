include $(ROOTDIR)/rules.mk

PKG_NAME:=ss-tunnel-rc4-md5
PKG_SOURCE_DATE:=2024-12-05

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/lixingcong/ss-tunnel-rc4-md5
PKG_SOURCE_VERSION:=c9d2570bff3560e950bfb69e7600ccc64c4c53d6

include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/cmake.mk

$(eval $(call BuildPackage,ss-tunnel-rc4-md5))

romfs:
	$(INSTALL_DIR) $(ROMFSDIR)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/ss-tunnel-rc4-md5 $(ROMFSDIR)/usr/bin/ss-tunnel-rc4-md5

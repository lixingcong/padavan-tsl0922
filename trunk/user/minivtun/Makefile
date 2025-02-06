include $(ROOTDIR)/rules.mk

PKG_NAME:=minivtun
PKG_SOURCE_DATE:=2024-01-03

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/rssnsj/minivtun
PKG_SOURCE_VERSION:=d7007bd8a79eadcd38d8e652dffaca93c2580cd2

include $(INCLUDE_DIR)/package.mk

MAKE_PATH:=src

$(eval $(call BuildPackage,minivtun))

romfs:
	$(INSTALL_DIR) $(ROMFSDIR)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/src/minivtun $(ROMFSDIR)/usr/bin/minivtun

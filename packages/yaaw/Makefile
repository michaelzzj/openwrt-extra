#
# Copyright (C) 2014 nanpuyue <nanpuyue@gmail.com>
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=yaaw
<<<<<<< HEAD
PKG_VERSION:=20160417
=======
PKG_VERSION:=2014-07-12
>>>>>>> refs/remotes/nanpuyue/master
PKG_RELEASE:=1
PKG_MAINTAINER:=nanpuyue <nanpuyue@gmail.com>

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=git://github.com/binux/yaaw.git
PKG_SOURCE_SUBDIR:=$(PKG_NAME)-$(PKG_VERSION)
<<<<<<< HEAD
PKG_SOURCE_VERSION:=84a0fb8f13a067bd32bb17936f0a74742ffcc224
=======
PKG_SOURCE_VERSION:=c23ae2456ec95778651411e5b148b836307f6d8d
>>>>>>> refs/remotes/nanpuyue/master
PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION)-$(PKG_SOURCE_VERSION).tar.gz

include $(INCLUDE_DIR)/package.mk

define Package/yaaw
  SECTION:=net
  CATEGORY:=Network
  SUBMENU:=Download Manager
  DEPENDS:=+aria2
  TITLE:=Yet another aria2 web frontend
  URL:=https://github.com/binux/yaaw
  PKGARCH:=all
endef

define Package/yaaw/description
	Yet Another Aria2 Web Frontend in pure HTML/CSS/Javascirpt.
endef

define Build/Compile
endef

define Package/yaaw/install
	$(INSTALL_DIR) $(1)/www/yaaw
	$(CP) $(PKG_BUILD_DIR)/js $(1)/www/yaaw
	$(CP) $(PKG_BUILD_DIR)/img $(1)/www/yaaw
	$(CP) $(PKG_BUILD_DIR)/css $(1)/www/yaaw
	$(CP) $(PKG_BUILD_DIR)/index.html $(1)/www/yaaw
	$(CP) $(PKG_BUILD_DIR)/offline.appcache $(1)/www/yaaw
endef

$(eval $(call BuildPackage,yaaw))

#
# Makefile
#
# $Id: //poco/1.7/OSP/samples/WebSession/Makefile#2 $
#
# Makefile for WebSession sample
#

BUNDLE_TOOL = $(POCO_BASE)/OSP/BundleCreator/$(POCO_HOST_BINDIR)/bundle

include $(POCO_BASE)/build/rules/global

objects = WebSession

target         = com.appinf.osp.samples.websession
target_version = 1
target_libs    = PocoOSPWeb PocoOSP PocoNet PocoUtil PocoXML PocoFoundation

postbuild      = $(SET_LD_LIBRARY_PATH) $(BUNDLE_TOOL) -n$(OSNAME) -a$(OSARCH) -o../bundles WebSession.bndlspec

include $(POCO_BASE)/build/rules/dylib

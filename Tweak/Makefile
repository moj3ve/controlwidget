export ARCHS = arm64 armv7 arm64e

include $(THEOS)/makefiles/common.mk

BUNDLE_NAME = ControlWidgetCCBundle

$(BUNDLE_NAME)_BUNDLE_EXTENSION = bundle
$(BUNDLE_NAME)_CFLAGS = -fobjc-arc -Iheaders
$(BUNDLE_NAME)_FILES = $(wildcard *.m) $(wildcard *.xm)
$(BUNDLE_NAME)_LDFLAGS = Frameworks/ControlCenterUIKit.tbd
$(BUNDLE_NAME)_INSTALL_PATH = /Library/ControlCenter/Bundles/
$(BUNDLE_NAME)_EXTRA_FRAMEWORKS = Cephei

include $(THEOS_MAKE_PATH)/bundle.mk
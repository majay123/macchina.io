#
# Makefile
#
# Makefile for macchina.io HelloSensor sample #1
#

include $(POCO_BASE)/build/rules/global
include $(POCO_BASE)/OSP/BundleCreator/BundleCreator.make

objects = BundleActivator

target          = io.macchina.samples.sensor1
target_includes = $(PROJECT_BASE)/devices/Devices/include
target_libs     = IoTDevices PocoOSP PocoUtil PocoJSON PocoXML PocoFoundation

postbuild = $(SET_LD_LIBRARY_PATH) $(BUNDLE_TOOL) -n$(OSNAME) -a$(OSARCH) -o../bundles HelloSensor1.bndlspec

include $(POCO_BASE)/build/rules/dylib

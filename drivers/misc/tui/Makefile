#
# Makefile for the stui Module
#

obj-$(CONFIG_SAMSUNG_TUI)	+= main.o
obj-$(CONFIG_SAMSUNG_TUI)	+= stui_core.o
obj-$(CONFIG_SAMSUNG_TUI)	+= stui_inf.o

ccflags-$(CONFIG_SAMSUNG_TUI)	+= -DUSE_TEE_CLIENT_API
ccflags-$(CONFIG_SAMSUNG_TUI)	+= -Idrivers/misc/tzdev/include/tzdev
ccflags-$(CONFIG_SAMSUNG_TUI)	+= -Idrivers/video/fbdev/exynos/dpu30
obj-$(CONFIG_SAMSUNG_TUI)	+= platforms/exynos980/


# SPDX-License-Identifier: GPL-2.0
#
# Samsung Clock specific Makefile
#

obj-$(CONFIG_SOC_EXYNOS3250)	+= clk-exynos3250.o
obj-$(CONFIG_ARCH_EXYNOS4)	+= clk-exynos4.o
obj-$(CONFIG_ARCH_EXYNOS4)	+= clk-exynos4412-isp.o
obj-$(CONFIG_SOC_EXYNOS5250)	+= clk-exynos5250.o
obj-$(CONFIG_SOC_EXYNOS5250)	+= clk-exynos5-subcmu.o
obj-$(CONFIG_SOC_EXYNOS5260)	+= clk-exynos5260.o
obj-$(CONFIG_SOC_EXYNOS5410)	+= clk-exynos5410.o
obj-$(CONFIG_SOC_EXYNOS5420)	+= clk-exynos5420.o
obj-$(CONFIG_SOC_EXYNOS5420)	+= clk-exynos5-subcmu.o
obj-$(CONFIG_EXYNOS_AUDSS_CLK_CON) += clk-exynos-audss.o
ifeq ($(CONFIG_COMPOSITE_CLK_SAMSUNG), y)
	obj-y				+= composite.o
	obj-$(CONFIG_SOC_EXYNOS9610)	+= clk-exynos9610.o
	obj-$(CONFIG_SOC_EXYNOS9630)	+= clk-exynos9630.o
	obj-$(CONFIG_SOC_EXYNOS9820)	+= clk-exynos9820.o
ifeq ($(CONFIG_SOC_EXYNOS9830_EVT0), y)
	obj-$(CONFIG_SOC_EXYNOS9830_EVT0)	+= clk-exynos9830_evt0.o
else
	obj-$(CONFIG_SOC_EXYNOS9830)	+= clk-exynos9830.o
endif
else
	obj-$(CONFIG_COMMON_CLK)	+= clk.o clk-pll.o clk-cpu.o
	obj-$(CONFIG_EXYNOS_ARM64_COMMON_CLK)	+= clk-exynos5433.o
	obj-$(CONFIG_EXYNOS_ARM64_COMMON_CLK)	+= clk-exynos7.o
endif
obj-$(CONFIG_ARCH_EXYNOS)	+= clk-exynos-clkout.o
obj-$(CONFIG_S3C2410_COMMON_CLK)+= clk-s3c2410.o
obj-$(CONFIG_S3C2410_COMMON_DCLK)+= clk-s3c2410-dclk.o
obj-$(CONFIG_S3C2412_COMMON_CLK)+= clk-s3c2412.o
obj-$(CONFIG_S3C2443_COMMON_CLK)+= clk-s3c2443.o
obj-$(CONFIG_ARCH_S3C64XX)	+= clk-s3c64xx.o
obj-$(CONFIG_ARCH_S5PV210)	+= clk-s5pv210.o clk-s5pv210-audss.o

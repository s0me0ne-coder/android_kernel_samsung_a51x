obj-y		                        += npu-util-autosleepthr.o
obj-y					+= npu-util-liststatemgr.o
obj-y					+= npu-util-msgidgen.o
obj-y					+= npu-util-regs.o
obj-y					+= npu-util-llq.o
obj-y					+= npu-util-common.o
obj-y					+= npu-log.o
obj-y					+= npu-ver.o
obj-y					+= npu-debug.o
obj-y					+= npu-device.o
obj-y					+= npu-core.o
obj-y					+= npu-clock.o
obj-y					+= npu-vertex.o
obj-y					+= npu-binary.o
obj-y					+= npu-queue.o
obj-y					+= npu-qos.o
obj-y					+= npu-system.o
obj-y					+= npu-memory.o
obj-y					+= npu-protodrv.o
obj-y					+= npu-session.o
obj-y					+= npu-fw-test-handler.o
obj-y					+= npu-queue.o
obj-y					+= npu-if-session-protodrv.o
obj-y					+= npu-if-protodrv-mbox2.o
obj-y					+= npu-sessionmgr.o
obj-$(CONFIG_NPU_INTERFACE)	+= interface/
obj-$(CONFIG_NPU_GOLDEN_MATCH)	        += npu-golden.o
obj-$(CONFIG_NPU_GOLDEN_MATCH)	        += npu-util-statekeeper.o
obj-$(CONFIG_NPU_GOLDEN_MATCH)	        += npu-util-comparator.o
obj-$(CONFIG_FIRMWARE_SRAM_DUMP_DEBUGFS)	        += npu-util-memdump.o
obj-$(CONFIG_NPU_SCHEDULER_GOVERNOR)	+= npu-scheduler.o npu-scheduler-governor.o
obj-$(CONFIG_NPU_GOVERNOR_SIMPLE_EXYNOS)	+= npu-scheduler-governor-simple-exynos.o
obj-$(CONFIG_NPU_GOVERNOR_EXYNOS_INTERACTIVE)	+= npu-scheduler-governor-exynos-interactive.o
obj-$(CONFIG_NPU_GOVERNOR_USERSPACE)	+= npu-scheduler-governor-userspace.o
obj-$(CONFIG_NPU_USE_SPROFILER)		+= npu-profile.o
obj-$(CONFIG_NPU_LLC_ENABLE)		+= npu-llc.o
obj-y					+= generated/

ccflags-y += -Idrivers/vision/vision-core/include -Idrivers/vision/npu/core/include -Idrivers/vision/npu/core
ifdef CONFIG_NPU_LOOPBACK
ccflags-y += -Idrivers/vision/npu/core/interface/loopback
else
ccflags-y += -Idrivers/vision/npu/core/interface/hardware
endif

# SoC specific inclusion
ccflags-y += -Idrivers/vision/npu/soc/$(CONFIG_EXYNOS_SOC_NAME)/include

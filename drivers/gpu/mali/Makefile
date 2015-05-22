# Configuration for A10
CONFIG:=ca8-virtex820-m400-1
USING_MMU:=1
USING_UMP:=1
USING_PMM:=1
BUILD:=release
TARGET_PLATFORM:=mali400-pmu
export CONFIG USING_MMU USING_UMP USING_PMM BUILD TARGET_PLATFORM

ccflags-y := -Iinclude/gpu/drm -Idrivers/gpu/mali -O3 -ffast-math -fgcse-lm -fgcse-sm -fsched-spec-load 
	   -fforce-addr -fsingle-precision-constant -mtune=cortex-a8
	   -marm -mfpu=neon -mcpu=cortex-a8

obj-$(CONFIG_MALI) += ump/ mali/

#
# (C) Copyright 2010,2011 Nvidia Corporation.
#
# SPDX-License-Identifier:	GPL-2.0+
#

obj-$(CONFIG_SPL_BUILD) += cpu.o

# The AVP is ARMv4T architecture so we must use special compiler
# flags for any startup files it might use.
CFLAGS_warmboot_avp.o += -march=armv4t

obj-y	+= clock.o funcmux.o pinmux.o
obj-$(CONFIG_TEGRA_LP0) += warmboot.o crypto.o warmboot_avp.o
obj-$(CONFIG_TEGRA_CLOCK_SCALING) += emc.o
obj-$(CONFIG_TEGRA_PMU) += pmu.o

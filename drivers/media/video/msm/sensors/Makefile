GCC_VERSION      := $(shell $(CONFIG_SHELL) $(PWD)/scripts/gcc-version.sh $(CROSS_COMPILE)gcc)
EXTRA_CFLAGS += -Idrivers/media/video/msm
EXTRA_CFLAGS += -Idrivers/media/video/msm/io
ifeq ($(CONFIG_MSM_CAMERA_V4L2),y)
EXTRA_CFLAGS += -Idrivers/media/video/msm/csi
endif
obj-$(CONFIG_MSM_CAMERA_SENSOR) += msm_sensor.o
obj-$(CONFIG_S5K3H1GX) += s5k3h1gx.o
ifeq ($(CONFIG_MSM_CAMERA_V4L2),y)
obj-$(CONFIG_S5K3H2YX) += s5k3h2yx_v4l2.o
obj-$(CONFIG_S5K4E5YX) += s5k4e5yx_v4l2.o
else
obj-$(CONFIG_S5K3H2YX) += s5k3h2yx.o
endif
obj-$(CONFIG_S5K6A1GX) += s5k6a1gx_v4l2.o
obj-$(CONFIG_S5K6AAFX) += s5k6aafx.o
obj-$(CONFIG_OV8830) += ov8830.o
obj-$(CONFIG_MT9D015) += mt9d015.o
obj-$(CONFIG_MT9V113) += mt9v113.o
obj-$(CONFIG_OV2720) += ov2720.o
obj-$(CONFIG_SP3D) += sp3d.o
obj-$(CONFIG_QS_S5K4E1) += qs_s5k4e1.o
obj-$(CONFIG_IMX105) += imx105.o imx105_reg.o

obj-$(CONFIG_MACH_VILLEC2) += mt9v113_ville_reg_lens_9251.o
obj-$(CONFIG_MACH_PYRAMID) += s5k3h1gx_reg_pyd.o mt9v113_reg_pyd.o
obj-$(CONFIG_MACH_MECHA) += s5k6aafx_reg_mecha.o s5k3h1gx_mecha.o s5k3h1gx_reg_mecha.o#HTC_CAM chuck
obj-$(CONFIG_MACH_VIVO) += s5k6aafx_reg_vivo.o
obj-$(CONFIG_MACH_VIVOW) += s5k6aafx_reg_vivo.o
obj-$(CONFIG_MACH_VIVOW_CT) += s5k6aafx_reg_vivo.o
obj-$(CONFIG_MACH_HOLIDAY) += s5k3h2yx_reg_holiday.o s5k6aafx_reg_holiday.o s5k6aafx_reg_holiday_cob.o
obj-$(CONFIG_MACH_VIGOR) += s5k3h2yx_reg_vigor.o ov8830_reg_vigor.o mt9d015_reg_vigor.o
obj-$(CONFIG_MACH_RUBY) += s5k3h2yx_reg_holiday.o mt9d015_reg_vigor.o
obj-$(CONFIG_MACH_DOUBLESHOT) += s5k3h2yx_reg_dot.o mt9v113_reg_dot.o
ifneq ($(CONFIG_MSM_CAMERA_V4L2),y)
obj-$(CONFIG_MACH_RIDER) += s5k3h2yx_reg_holiday.o s5k6aafx_reg_rider.o s5k6aafx_reg_rider_cob.o ov8830_reg_vigor.o
endif
obj-$(CONFIG_MACH_VILLEC2) += s5k3h2yx_reg_holiday.o s5k6aafx_reg_villec2.o s5k6aafx_reg_villec2_cob.o ov8830_reg_vigor.o
obj-$(CONFIG_MACH_RUNNYMEDE) += s5k3h2yx_reg_runnymede.o ov8830_reg_runnymede.o s5k6aafx_reg_runnymede_cob.o
obj-$(CONFIG_MACH_KINGDOM) += s5k6aafx_reg_kingdom_cob.o s5k6aafx_reg_kingdom.o
obj-$(CONFIG_MACH_SHOOTER) += sp3d_reg_3d.o sp3d_reg_2d.o sp3d_reg_com.o sp3d_reg_cal.o s5k6aafx_reg_shooter.o qs_s5k4e1_reg.o s5k6aafx_reg_shooter_cob.o
obj-$(CONFIG_MACH_SHOOTER_K) += sp3d_reg_3d.o sp3d_reg_2d.o sp3d_reg_com.o sp3d_reg_cal.o s5k6aafx_reg_shooter.o qs_s5k4e1_reg.o s5k6aafx_reg_shooter_cob.o
obj-$(CONFIG_MACH_SHOOTER_U) += sp3d_reg_3d.o sp3d_reg_2d.o sp3d_reg_com.o sp3d_reg_cal.o s5k6aafx_reg_shooter.o qs_s5k4e1_reg.o s5k6aafx_reg_shooter_cob.o
obj-$(CONFIG_MACH_SHOOTER_CT) += sp3d_reg_3d.o sp3d_reg_2d.o sp3d_reg_com.o sp3d_reg_cal.o s5k6aafx_reg_shooter.o qs_s5k4e1_reg.o s5k6aafx_reg_shooter_cob.o

ifeq ($(CONFIG_S5K4E1GX),y)
obj-$(CONFIG_MACH_SAGA) += s5k4e1gx.o s5k4e1gx_reg.o
endif

ifeq ($(CONFIG_OV8810),y)
obj-$(CONFIG_MACH_SPADE) += ov8810.o
endif

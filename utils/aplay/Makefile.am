# BlueALSA - Makefile.am
# Copyright (c) 2016-2020 Arkadiusz Bokowy

if ENABLE_APLAY

bin_PROGRAMS = bluealsa-aplay

bluealsa_aplay_SOURCES = \
	../../src/shared/dbus-client.c \
	../../src/shared/ffb.c \
	../../src/shared/log.c \
	alsa-pcm.c \
	dbus.c \
	aplay.c

bluealsa_aplay_CFLAGS = \
	-I$(top_srcdir)/src \
	@ALSA_CFLAGS@ \
	@BLUEZ_CFLAGS@ \
	@DBUS1_CFLAGS@

bluealsa_aplay_LDADD = \
	@ALSA_LIBS@ \
	@BLUEZ_LIBS@ \
	@DBUS1_LIBS@

endif

# SPDX-License-Identifier: GPL-2.0
lib-y		:= clear_user.o delay.o copy_from_user.o		\
		   copy_to_user.o copy_in_user.o copy_page.o		\
		   clear_page.o memchr.o memcpy.o memmove.o memset.o	\
		   memcmp.o strcmp.o strncmp.o strlen.o strnlen.o	\
		   strchr.o strrchr.o csum.o tishift.o

CFLAGS_REMOVE_atomic_ll_sc.o := -pg
GCOV_PROFILE_atomic_ll_sc.o	:= n
KASAN_SANITIZE_atomic_ll_sc.o	:= n
KCOV_INSTRUMENT_atomic_ll_sc.o	:= n
UBSAN_SANITIZE_atomic_ll_sc.o	:= n

lib-$(CONFIG_ARCH_HAS_UACCESS_FLUSHCACHE) += uaccess_flushcache.o

obj-$(CONFIG_CRC32) += crc32.o

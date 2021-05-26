SUBDIRS = a b
ALL_SUBDIRS = $(addprefix ALL, $(SUBDIRS))
CLEAN_SUBDIRS = $(addprefix CLEAN, $(SUBDIRS))

PHONY := $(SUBDIRS)


all: $(ALL_SUBDIRS)

ALL%: %
	$(MAKE) -C $<

PHONY += clean

clean: $(CLEAN_SUBDIRS)

CLEAN%: %
	$(MAKE) -C $< -f Makefile clean


.PHONY: $(PHONY)

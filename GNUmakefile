TOP	= ../..
include $(TOP)/mk/common.make

MODULE	= MDA
MODDIR	= $(datadir)/$(MODULE)
SRCS	= ChimeraExtension.py __init__.py MDA.py
OBJS	= $(SRCS:.py=.pyc)
CLEAN	= $(OBJS)

all: $(OBJS)

install: all
	-mkdir -p $(MODDIR)
	$(RSYNC) $(SRCS) $(OBJS) $(DATA) $(MODDIR)

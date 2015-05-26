# Note: plugindir is set in configure

##############################################################################
# TODO: change libgstplugin.la to something else, e.g. libmysomething.la     #
##############################################################################
plugin_LTLIBRARIES = libgstavb.la

LDFLAGS = -lpci -lrt -lpthread -lm -lgstapp-1.0

##############################################################################
# TODO: for the next set of variables, name the prefix if you named the .la, #
#  e.g. libmysomething.la => libmysomething_la_SOURCES                       #
#                            libmysomething_la_CFLAGS                        #
#                            libmysomething_la_LIBADD                        #
#                            libmysomething_la_LDFLAGS                       #
##############################################################################

# sources used to compile this plug-in

#For Talker uncomment the below:

libgstavb_la_SOURCES = gstavb.c ../../../common/avb.c ../../../common/avb.h ../../../../lib/igb/igb.h gst_avb_playbin.c gst_avb_playbin.h gst_app_src.c gstavbsink.c gstavbsink.h

# compiler and linker flags used to compile this plugin, set in configure.ac
libgstavb_la_CFLAGS = $(GST_CFLAGS) 
libgstavb_la_LIBADD = $(GST_LIBS)  
libgstavb_la_LDFLAGS = $(GST_PLUGIN_LDFLAGS) $(LDFLAGS)
libgstavb_la_LIBTOOLFLAGS = --tag=disable-static
libgstavb_la_EXTRA_CFLAGS=$(EXTRA_CFLAGS)

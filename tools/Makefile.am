INCLUDES = -g -I$(top_srcdir) -I$(top_srcdir)/gitg -I$(top_srcdir)/libgitg $(GITG_DEBUG_FLAGS) $(GITG_CFLAGS)

noinst_PROGRAMS = $(TOOLS_PROGS)
tools_ldadd     = $(top_builddir)/libgitg/libgitg-1.0.la $(PACKAGE_LIBS) $(GITG_LIBS)

TOOLS_PROGS			= gitg-shell gitg-config

gitg_shell_SOURCES		= gitg-shell.c
gitg_shell_LDADD		= $(tools_ldadd)

gitg_config_SOURCES		= gitg-config.c
gitg_config_LDADD		= $(tools_ldadd)

-include $(top_srcdir)/git.mk

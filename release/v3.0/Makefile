
DISTRIB_ROOT := root
DISTRIB_FILES := $(patsubst $(DISTRIB_ROOT)/%,%,$(wildcard $(DISTRIB_ROOT)/*))

.PHONY: .phony
$(MAKECMDGOALS): .phony
	tar --group=None --owner=None --no-acls --no-xattrs --xz -cf cygcheck-dep-$@.tar.xz --recursion -C $(DISTRIB_ROOT)  $(DISTRIB_FILES)

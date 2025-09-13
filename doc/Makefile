# Central Makefile for SDK documentation
SPHINXBUILD   = sphinx-build
BUILDDIR      = _build

.PHONY: html clean

html:
	@echo "Building User Guide..."
	$(SPHINXBUILD) -b html user_guide/source    $(BUILDDIR)/user_guide
	@echo "Building App Notes..."
	$(SPHINXBUILD) -b html appnotes/source      $(BUILDDIR)/appnotes
	@echo "Building SDK Docs..."
	$(SPHINXBUILD) -b html sdk                  $(BUILDDIR)/sdk
	@echo "Building Release Notes..."
	$(SPHINXBUILD) -b html release_notes/source $(BUILDDIR)/release_notes
	@echo "✅ All docs built successfully!"

clean:
	rm -rf $(BUILDDIR)


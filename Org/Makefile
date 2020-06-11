boot:
	$(EDITOR) -u --eval '\
		(with-current-buffer \
			(find-file-noselect "$(SYNC_ORG_TEMPLATE)") \
                        (goto-char (point-min)) \
			(re-search-forward "^#[+]name:preprocess.el$$") \
			(org-babel-tangle (quote (4))) \
			(kill-buffer))'
	./tools/preprocess.el

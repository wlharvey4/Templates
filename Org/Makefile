boot:
	$(EDITOR) --eval "\
		(progn \
			(set-buffer (find-file-noselect \"$(SYNC_ORG_TEMPLATE)\")) \
                        (goto-char (point-min)) \
			(re-search-forward \"^#[+]name:preprocess.el$$\") \
			(org-babel-tangle (quote (4))))"
	$(EMACS) -Q --batch -l tools/preprocess.el

boot:
	$(EDITOR) -u --eval \
		"(with-current-buffer (car (find-file-noselect \"./*.org\" nil nil t)) \
                        (save-excursion \
			(goto-char (point-min)) \
			(re-search-forward \"^#[+]name:preprocess.el$$\") \
			(org-babel-tangle (quote (4))) \
                        (save-buffer)))"
	./tools/preprocess.el

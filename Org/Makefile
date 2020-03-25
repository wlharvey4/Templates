boot:
	emacs -Q $${SYNC_ORG_TEMPLATE} --batch --eval '\
	(progn \
		(re-search-forward "^\\#\\+name:preprocess.el$$") \
		(org-babel-tangle (quote (4))))'
	emacs -Q --batch -l tools/preprocess.el

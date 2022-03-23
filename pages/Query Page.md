query-table:: false
#+BEGIN_QUERY
{:title "Find tag: AWS"
:query [:find (pull ?b [*])
:where
[?b :block/ref-pages ?p]
[?p :block/name "AWS"]
]
}
#+END_QUERY

	-
-
-
-
-
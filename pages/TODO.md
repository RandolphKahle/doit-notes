- #+BEGIN_QUERY
  {:title "🎥 TODOs"
  :query [:find (pull ?b [*])
  :where
  [?b :block/marker ?marker][(contains? #{"TODO" "LATER"} ?marker)]
  ]
  }
  #+END_QUERY
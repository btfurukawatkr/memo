## add .gitkeep to empty folder
`find . -type d -empty -not -path './.git*' -exec touch {}\/.gitkeep \;`

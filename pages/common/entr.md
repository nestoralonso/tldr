# entr

> Run arbitrary commands when files change

- Rebuild project and run tests if the build was successful

`ag -l | entr -s 'make && make test'`

- Reload browser when html files change (requires reload-browser script)

`ls *.css *.html | entr reload-browser Firefox`

- Immediately start the server, block until any of the listed files change, terminate the background process, and finally wait for the server to exit before restarting
`ls *.rb | entr -r ruby main.rb`

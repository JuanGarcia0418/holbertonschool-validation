build:
	hugo -s . -d dist/

post:
	rm -rf content/posts/$(POST_NAME).md
	hugo new posts/$(POST_NAME).md
	sed -i 's/title:*/title: "$(POST_TITLE)"/g' content/posts/$(POST_NAME).md 

clean:
	rm -rf dist/
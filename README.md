#### Startup Institute Berlin

# Web Design Track

### by [nando rossi](http://nan.do)

## Intro

Course material for my 2015 front-end development 101 classes. This page can also be accessed at [http://nandorocker.github.com/siber-webdesign-2015](http://nandorocker.github.com/siber-webdesign-2015).

## Instructions

This repo is made for use with [Jekyll](http://jekyllrb.com). Content is either in HTML or [Markdown](http://daringfireball.net/projects/markdown/syntax). If you have no idea what those things are, here's how to view the content:

### Viewing pages

- Install [Jekyll](http://jekyllrb.com) as described on their site.
- Clone the repo to your computer:

`$ git clone https://github.com/nandorocker/siber-webdesign-2015.git`

- On the repo's directory, run Jekyll:

`$ jekyll serve`

You should now be able to see the pages by pointing your browser to `localhost:4000`.
When you're done, press `control + c` on the terminal and it will stop.

You could also simply run: `$ jekyll build` and open the files at the _site 


### Editing the content

Jekyll's folder system is a bit weird, here's what you need to know about my specific setup:

	-root
	  |_______	Kickoff
	  |			    |______  _posts	  
	  |	  |_______	Module01	  |_______	Module02	  |_______	Module03	  |_______	Module04	  |_______	Module05	  |_______	Module06

Inside the directories listed here, you'll find a folder `_posts` and within that folder, `.md` files. Those files can be edited and if you're running `jekyll serve`, automatically updated (reload your browser).

You can also do a `jekyll build` and it will simply push the files to the `_site` folder, which are plain, readable HTML.
	  

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
# wraith-bradysmeats

Visual regression testing for the [Brady's Meat & Deli](http://bradysmeats.com/) site with [Wraith](http://bbc-news.github.io/wraith/).

# Set up

If you've never used Wraith before, you need to run the following steps to prepare your computer to run it.

1. Run `type rbenv`. If you get a message saying that rbenv was not found, then you'll need to install rbenv. On Mac OS/X, you can do this with:

		brew update
		brew install rbenv
		rbenv init
		# Follow any instructions to update your shell's configuration file.
		# Restart your Terminal window.
		rbenv install 1.9.3-p551
		gem install bundler

2. [Follow the instructions for setting up Wraith's dependencies](http://bbc-news.github.io/wraith/os-install.html).

Now you need to set up this project:

1. Clone this repository.
2. In a terminal, `cd` into the cloned repository.
3. Run `bundle install`

# Use

1. In a terminal, `cd` into the cloned repository.
2. Run `bundle exec wraith capture configs/config.yaml`.

	This will create a `shots/` folder inside the repository. This will contain a bunch of images, along with a `gallery.html` file which you can open in a browser to see the visual regressions.

# Configuration

Make configuration changes in `configs/config.yaml`.

# See also

* [The Wraith project documentation](http://bbc-news.github.io/wraith/)
* [Visually Test Your Website with Wraith](https://pantheon.io/blog/test-website-wraith) (blog by Kate Kligman)
* [Using Wraith for Visual Regression Testing](https://pantheon.io/docs/guides/visual-diff-with-wraith/) (Pantheon documentation)

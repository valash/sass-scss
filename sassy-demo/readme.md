**Hello**

SASS: syntactically awesome stylesheets
its an extension of CSS.
SCSS: Sassy Css

**Why did you choose this subject?**

Intrigued by SASS's claim that it made styling easier, faster, all while being more intuitive are the reasons I choose to learn SASS/SCSS.

**How were you first made aware of it?**

When I was working on a project - whenever I searched something that was related to the styling of the project SASS/SCSS kept popping up in the searches and I decided that I wanted to see what it was all the fuss was about.

**What problem does it solve?**

Sass/SCSS solves the problem of common repetition and maintenance challenges that are present in traditional CSS.

**How does it solve the problem (conceptually)?**
Instead of having code that looks like

```
main section#card ul li {
margin-bottom: 10px;
}

main section#card ul li span {
  position: absolute;
  width: 30px;
  height: 30px;
  background-color: white;
  border-radius: 50%;
  margin-right: 10px;
}

main section#card ul li strong {
  display: inline-block;
  margin-left: 40px;
  margin-top: 10px;
}
```

you can just type this in your main.scss file- which as you can see is a lot faster and clearer than the previous example

```
main {

	section#card {
		background: white;
		color: $fontColo;
		padding: 20px;
		margin: 1em auto;
		border-radius: $borders;
		box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
		width: 80%;
		margin: auto;
		height: 30%;
		background-color: color, primary;

		ul {
			list-style-type: none;
			margin: 0;
			padding: 0;

			li {
				margin-bottom: 10px;

				span {
					position: absolute;
					width: 30px;
					height: 30px;
					background-color: color(primary-light);
					border-radius: 50%;
					margin-right: 10px;
				}
				strong {
					display: inline-block;
					margin-left: max(40px);
					margin-top: 10px;
				}
			}
		}
    }
```

**Why does one use it?**

SASS/SCSS is a favorite among developers for the simple reason that you can use things like variables, mixins, and functions to make styling much easier.

**What are the alternatives?**

Plain CSS

**What is it similar to, if anything?**

Extremely similar to CSS

**What is the history of this technology?+ Who built it and why?**

Hampton Caitlin and Natalie Weizenbaum were the creators of Sass. They built the preprocessor scripting language to be an extension of CSS to "make CSS fun again."

**Who is maintaining it?**
Natalie Weizenbaum is now the primary developer and architect of Sass. Hampton Caitlin no longer works with Sass. Natalie is currently leading a team that keeps Sass updated and current.

**What is your opinion on the technology after having built something with it?**

My opinion of Sass is that it is a great tool. It makes the process of having repeatedly used fonts, colors, sizes, shadows easy as you can just set anything you'd like to a variable, and those variables can be easily changed by just updated the value. Making changing your mind on say a color theme no longer a tedious task.

**What are the biggest conceptual hurdles (if any) you encountered when researching this?**

I personally did not have any.

**What resources do you recommend for interested students?**

YouTube videos and the Sass Documentation are the easiest to follow when initially starting to learn the concepts. Another way of seeing how SCSS compares to CSS is by looking at an already created repo and comparing the main.css file to the SCSS file to see how the two are similar and different.

**Instructions**

The most straightforward installation instructions I found was instead of installing SCSS/Sass on the command line or one's desktop- I installed the VSC extension called "Live Sass Compiler."

When you install the extension "Watch My Sass" will appear in the activity bar of VSC. Click this, and it will compile your SASS/SCSS files to your CSS files with a live browser reload happening at the same time, making styling more straightforward and faster than plain CSS.

Make sure you create a CSS folder in your project and create a folder called _CSS_ and within that folder create a file named _main.scss_ While the extension is running the live server, it will also generate a main.css and main.css.map file and add it to your CSS folder. The main.css file will automatically be linked to your main.scss and will continuously be compiling (translating) the data into plain CSS.

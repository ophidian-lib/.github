## Ophidian = Component Framework + Build System for Obsidian Plugins

Some [Obsidian](https://obsidian.md) plugins are too big to just slap everything in one class.  But as you break things into smaller parts, you end up doing a lot of hard-to-change and fragile `this.that.theOther.thing`, that also makes the parts less reusable.

In addition, if you develop lots of plugins, you'll find yourself duplicating a bunch of build management and release publishing tools and configuration.

So, the Ophidian project exists to solve these problems, via a [component framework](https://github/obsidian-lib/core) and [build/publish system](https://github/ophidian-lib/build).  The core framework includes a variety of useful services that can be used in almost any plugin, and over time, the Ophidian project as a whole will have additional non-core frameworks, when such additional libraries require packages other than those required by the core.

Ophidian libraries (other than the build system) are distributed in TypeScript format, so if you're not using esbuild (as Ophidian's builder does), you'll need to configure your builder to allow compiling Typescript from within your `node_modules`.)

### About the Name

The word "ophidian" roughly means "like a snake", and Ophidian certainly coils around [my Obsidian plugin projects](https://github.com/pjeby?tab=repositories&q=obsidian&type=source&language=&sort=) like a snake, building and publishing them while also devouring their tastiest, most reusable bits to make them part of itself.  (Also, you can think of the "ph" in Ophidian as standing for "plugin help" that replaces all the repetitive "bs" in Obsidian plugin development.)  Last, but far from least, the name was available on npm and my other ideas weren't!


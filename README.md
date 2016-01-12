# wpgdotnetui

[![Join the chat at https://gitter.im/mikesigs/wpgdotnetui](https://badges.gitter.im/mikesigs/wpgdotnetui.svg)](https://gitter.im/mikesigs/wpgdotnetui?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

This is my submission for the new Winnipeg .NET User Group site.

It is using 
- Angular 1.4.2
- TypeScript 1.6
- Restangular
- UI-Router
- Bootstrap 3
- jQuery 2
- node-sass
- Gulp
- and [bootstrap-material-design](http://fezvrasta.github.io/bootstrap-material-design) (a sweet Material Design theme for Bootstrap)

It was generated with the help of [Yeoman](http://yeoman.io/), using the [generator-gulp-angular](https://github.com/Swiip/generator-gulp-angular) uh... generator.

To get up and running you'll need to install Node. I'm running v4.2.4. 
Then do a global install of the following node packages: Yeoman, gulp, bower, and tsd:

`npm install -g yo gulp bower tsd`

You should also consider installing a kick-ass editor. I recommend either [Brackets](http://brackets.io/) or [Visual Studio Code](https://code.visualstudio.com/). You can certainly do your editting in a full blown Visual Studio IDE, but I find that the TypeScript compilation interferes with what you already get out of the amazing gulpfile provided by the Yeoman generator. It's possible, but you have to manually disable TypeScript compilation in the csproj. Fee free to do this and send a PR.

After you have everything setup you'll need to use gulp to build, test, and serve the app. Consequently, the commands to do those things are:

`gulp build` (this is the default task, so you can just run `gulp` instead)

`gulp test`

`gulp serve`

One hella-cool feature of this solution is it uses [Browsersync](https://www.browsersync.io/) combined with [WebPack](https://webpack.github.io/). So after you run `gulp serve`, it continuously monitors your files for changes. When a change occurs it automatically recompiles your code/styles/etc then syncs and reloads your browser(s), all of them. You can have multiple browsers running simultaneously on the same page and they're all synced. Try it. It's awesome for x-browser testing. This also goes for running tests. To add to the 3 commands above, you can also run `gulp test:auto` and it will watch for code changes and re-run your tests after a successful compilation. This makes it super easy to iterate, writing code and running tests on every save.

One last thing. If you're gonna be coding on this in Windows, you'll want something better than the standard command prompt. I highly recommend checking out [cmder](http://cmder.net/). It's just a wrapper around ConEmu but adds a nice theme to it, [clink](https://mridgers.github.io/clink/), and some other great stuff too.

Have fun!

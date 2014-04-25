# Install development dependencies with bundler:
This requires ruby on your system. `$` means run this command in the shell (terminal -> bash/zsh on mac os x)

    # do this once on your system on the terminal (admin permissions (sudo) might be needed)
    $ (sudo) gem install bundler

    # then install the dependencies
    $ cd ./your-js/project/path
    $ bundle

# When developing:
Run `guard` when developing (https://github.com/guard/guard). It watches for changes in your js files and recreates the concatenated `application.js` file. Hit 'enter' in the running guard shell to recreate all compiled files. There are also other rules defined inside the `Guardfile` (copying of files onto the dev server when changed etc.).

    $ cd ./your-js/project/path
    $ guard

The files which are concatenated into `application.js` are defined in the `assets.yml` file. This is a `jammit` configuration file (http://documentcloud.github.io/jammit/)

# SuperCollider 3.7.0 OSX Standalone

Modified from the 3.6.6 version:
https://github.com/dathinaios/sc_osx_standalone/

[SuperCollider ] (http://supercollider.sourceforge.net/) version `3.7.0`

## Usage

0. Navigate to the downloaded folder from the terminal with `cd location_path_of_sc-osx-standalone-master`.
0. Run the standalone with `sh run.sh` script. You should hear some white noise. This is the default sound as defined in `init.scd`.
0. To modify `init.scd` replace the code inside the curly brackets after `doWhenBooted` with your own code:

          s.boot;
          s.doWhenBooted{
            // your own code here
          };

0. Include your extensions in the `SCClassLibrary` folder.
0. [Platypus ](http://sveinbjorn.org/platypus) can be used to convert the script based structure into a native OSX application.
  - Open Platypus
  - Fill in the App name
  - Click the `Select Script` button and choose the `run.sh` file.
  - Drag all the files from the `sc_osx_standalone-master` to the `Bundled Files` field.
  - Optional: to hide the post window change the interface option from `Text Window` to `None`.
  - Click `Create` and choose the location for your app. 

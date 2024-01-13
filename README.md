#  Audio Processing course - Digital Audio Effects

This course explores the development of digital audio fx with the help of [JUCE](https://juce.com/) framework. This C++ framework helps you buils audio applications and plugins for various targets and platforms

Throught several subprojects we'll developped audio plugins.

Several books have been used to make up this course especially [2], [3] and [6]. 

## Use of this repository

The different projects tougth during this course are present in the exercises folder. They consist of submodules and are therefore themselves repositories.
You can clone this repository and the accompanying exercices by launching this command : 

```
git clone --recurse-submodules 
```

Global references on Audio Processing can be found in [audio_processing_ref.md](audio_processing_ref.md) at the root of this repo. This ressources is on an-going work, so feel free to contribute.

## JUCE

JUCE is a C++ framework whose aim is to facilitate audio plugins and applications development for different OSes and/or different plugin format.

When downloaded and extracted, JUCE comes with the Projucer application. This application will generate the relevant project structure depending on your IDE and the type of project you want to build. To know all about the Projucer, you can look at the very first JUCE tutorial : [Getting started with the Projucer](https://docs.juce.com/master/tutorial_new_projucer_project.html)

JUCE also comes with useful Demos and extra applications.


## Test the plugins

Plugins can be tested in two ways : 

- The first one consists of a Pure Data patch
- The second one is to use the AudioPluginHost present in the JUCE folder you've downloaded.

### test_vst.pd

You can download Pure Data [here](https://puredata.info/downloads/pure-data). 

In order for this patch to work the first thing to do when open the software is to install `vstplugin~` externals : go to `Help > Find externals` and look for `vstplugin~`. Choose the first element in the list and click `install`. 

A specific version of Pure Data is available to Mac users to prevent noises while moving VSTs parameters. This version (Pd-0.51.1-eventloop-macOS) can be found [here] (https://github.com/Spacechild1/pure-data/releases/download/v0.51.1-eventloop/Pd-0.51.1-eventloop-macOS.zip).
To prevent the noises, when the program has been launched, go to `Preferences > Startup > Enable event loop`.

From there, you can watch [this video](https://youtu.be/Cs0NPime0kU) to learn more about dealing with VSTs in Pd.

### AudioPluginHost

Taking the advice mentionned in [6], you can use the AudioPluginHost application present in the `JUCE/extra` folder to directly run your plugin in your selected IDE. You'll have to compile it and link it to the specific target of your dafx plugin project. This application offers vst loading as well as routing possibilities.

Another good practice taken from [6] is to add an oscilloscope as well as a spectrum analyzer. As this advice was given by the author having a synthesizer in mind, it can be somewhat relevant for some dafx.

More on how to set your IDE to use AudioPluginHost in the first exercise.

## References

[1] Boulanger, R. and Lazzarini, V. (2010). The Audio Programming Book. The MIT Press.

[2] Zolder, U. (2011). DAFX : Digital Audio Effects. Wiley Publishing. 2nd edition.

[3] Reiss, J. D. and McPherson A. (2015). Audio Effects Theory, Implementation and Application. CRC Press. [Can be download here.](https://github.com/inteljack/EL6183-Digital-Signal-Processing-Lab-2015-Fall/blob/master/mit9m.Audio.Effects.Theory.Implementation.and.Application.pdf)

[4] Pirkle, W. C. (2019). Designing Audio Effects Plugins in C++. Routeledge.

[5] Pirkle, W. C. (2021). Designing Software Synthesizer Plugin in C++. Routeledge. 2nd edition.[Can be download here.](https://bytes.usc.edu/cs455saty/m23_WhyCode/extras/docs/DesigningDAWPluginsWithCPlusPlus.pdf)

[6] Hollemans, M. 2023. Creating Synthsizer Plug-Ins with C++ and JUCE. The Audio Programmer.

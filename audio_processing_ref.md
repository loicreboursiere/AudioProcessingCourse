# References for Audio Processing


## Books
[1] Boulanger, R. and Lazzarini, V. (2010). The Audio Programming Book. The MIT Press.

[2] Zolder, U. (2011). DAFX : Digital Audio Effects. Wiley Publishing. 2nd edition.

[3] Reiss, J. D. and McPherson A. (2015). Audio Effects Theory, Implementation and Application. CRC Press. [Can be download here.](https://github.com/inteljack/EL6183-Digital-Signal-Processing-Lab-2015-Fall/blob/master/mit9m.Audio.Effects.Theory.Implementation.and.Application.pdf)

[4] Pirkle, W. C. (2019). Designing Audio Effects Plugins in C++. Routeledge.

[5] Pirkle, W. C. (2021). Designing Software Synthesizer Plugin in C++. Routeledge. 2nd edition.[Can be download here.](https://bytes.usc.edu/cs455saty/m23_WhyCode/extras/docs/DesigningDAWPluginsWithCPlusPlus.pdf)

[6] 




## Websites, githubs, etc:

- [https://github.com/inteljack/EL6183-Digital-Signal-Processing-Lab-2015-Fall/tree/master](https://github.com/inteljack/EL6183-Digital-Signal-Processing-Lab-2015-Fall/tree/master) : Audio processing course in Python from EL6183-DSP Lab of NYU by professor Ivan Selesnick.

- [https://www.willpirkle.com/fx-book/project-gallery/](https://www.willpirkle.com/fx-book/project-gallery/) : Code coming along with [4].

- [https://github.com/getdunne/audio-effects](https://github.com/getdunne/audio-effects) : Code coming alongside [3].

## Useful Audio Plugins

- [s(M)exoscope](http://armandomontanez.com/smexoscope/)

- [Voxengo SPAN](https://www.voxengo.com/product/span/)

## Useful tricks

### MacOS 
- If an audio won't lauch because the developper can't be verified and you don't manage to launch it by selecting "Open anyway...' in the security options of Mac OS, then you can use this line in a terminal :
```
sudo xattr -d com.apple.quarantine path/to/your/plugin
```


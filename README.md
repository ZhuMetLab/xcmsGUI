# Introduction

For users' convenience, we developed an all-in-one GUI tool, namely, `xcmsGUI-Zhulab`, to integrate data conversion (using `MSConvert` in `ProteoWizard`) and data pre-processing (using `XCMS`) in one analysis. Users only need input raw MS data files (`.d`, `.raw`, or `.wiff`) from vendor instruments to `xcmsGUI`. Then, `xcmsGUI` enables to perform data conversion and peak detection altogether in one step. Finally, a peak table and MS/MS spectra files (`MGF` format) are generated as the input files for [`MetDNA`](http://metdna.zhulab.cn). Sample information file is generated automatically for [`MetDNA`](http://metdna.zhulab.cn).

![Main window](figs/main.png)
# Download

- [All in one](https://github.com/ZhuMetLab/xcmsGUI/releases/download/v1.0.0/xcmsGUI-standalone.zip) contains
	- `xcmsGUI-Zhulab`
	- `R-portable`
	- `PreteoWizard`
- [Stand-alone](https://github.com/ZhuMetLab/xcmsGUI/releases/download/v1.0.0/xcmsGUI-standalone.zip) contains
	- `xcmsGUI-Zhulab` only 

If one have already installed R with xcms and PreteoWizard, [stand-alone](https://github.com/ZhuMetLab/xcmsGUI/releases/download/v1.0.0/xcmsGUI-standalone.zip) version is recommanded.

# Config

- To use [All in one](https://github.com/ZhuMetLab/xcmsGUI/releases/download/v1.0.0/xcmsGUI-standalone.zip) software, one can just run the xcmsGUI.exe after unzip `xcmsGUI-Zhulab-all.zip`
- To use [Stand-alone](https://github.com/ZhuMetLab/xcmsGUI/releases/download/v1.0.0/xcmsGUI-standalone.zip) software, one should have
	- [`R`](https://cran.r-project.org/) and [`ProeoWizard`](https://proteowizard.sourceforge.io/) installed on Windows OS
	- [`xcms`](https://bioconductor.org/packages/release/bioc/html/xcms.html) package installed in R
	- [`xcmsTools`](packages/xcmsTools_1.0.0.tar.gz) package installed in R
	-  config their own R/MSConvert envirenment with 'Options' -> 'Config' in xcmsGUI
![Env config](figs/config.png)

# Peak detection

![Data processing](figs/process.png)

***Note***
1. We support polarity switch mode of ThermoFisher Obitrap instruments (e.g., Exploris 480). Users should just check `Ploarity swith (For Obitrap)` ![Ploarity swith](figs/switch.png) and set data format to `.raw`![raw format](figs/foramt_raw.png)
2. For MS1 only data, users should uncheck `Export MSMS in MGF Format`![Export MSMS](figs/export_check.png)
3. If only MSMS spectra needed, users should just select `-` in `Analysis` and `Run` the program.
![MGF only](figs/mgfonly.png)

# Export MSMS spectra to MGF

![Export MSMS](figs/export.png)

# Saving peak detection parameters for next time

![Save param](figs/saveparam.png)

# Load previous saved parameters

![Load param](figs/loadparam.png)

# License
<a rel="license" href="https://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a>

This work is licensed under the Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)
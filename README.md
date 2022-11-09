# Introduction

`xcmsGUI-Zhulab` is a GUI tool to detect MS peaks with `xcms` `R` package. It can detect MS peaks with XCMS using mzXML data and export MSMS spectra to `MGF` format. Users can also use vender data generated by MS instrument directly. `xcmsGUI-Zhulab` will detect MS peaks after converting the data to `mzXML` files with `MSConvert` in `ProteoWizard` and export MSMS spectra to MGF format.

![Main window](figs/main.png)
# Download

- [All in one](./xcmsGUI.zip) contains
	- `xcmsGUI-Zhulab`
	- `R-portable`
	- `PreteoWizard`
- [Stand-alone](./xcmsGUI-standalone.zip) contains
	- `xcmsGUI-Zhulab` only 

If one have already installed R with xcms and PreteoWizard, [stand-alone](./xcmsGUI-standalone.zip) version is recommanded.

# Config

- To use [All in one](./xcmsGUI.zip) software, one can just run the xcmsGUI.exe after unzip `xcmsGUI-Zhulab-all.zip`
- To use [Stand-alone](./xcmsGUI-standalone.zip) software, one should have
	- R and ProeoWizard installed on Windows OS
	- `xcms` package installed in R
	- [`xcmsTools`](./xcmsTools_0.1.0.tar.gz) package installed in R
	-  config their own R/MSConvert envirenment with 'Options' -> 'Config' in xcmsGUI
![Env config](figs/config.png)

# Peak detection

![Data processing](figs/process.png)

***Note***
1. We support polarity switch mode of ThermoFisher Obitrap instruments (e.g., Exploris 480). Users should just check `Ploarity swith (For Obitrap)` ![Ploarity swith](figs/switch.png)
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
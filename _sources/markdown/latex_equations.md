# LaTeX equations

 In the notebooks we use Markdown to write text, but equations are rendered using LaTeX syntax. LaTeX is a typesetting that allows technical writers and scientists to focus on the content without worrying abouT the format. LaTeX is free under the terms of the LaTeX Project Public License (LPPL).

!>A nice feature of LaTeX is that there is a specific syntax for equations. For instance, you can define inline equations so that this: `$y=mx+b$`, get's converted into this: $y=mx+b$

It is also possible to write equations in separate lines using `$$y = e^{-x}$$`:

$$y = e^{-x}$$


## Examples

Below is a set of equations obtained from the [FAO 56 manual](http://www.fao.org/docrep/X0490E/X0490E00.htm) to calculate reference evapotranspiration. Use this equations as templates to learn how to implement your own equations.


### Reference Evapotranspiration Equation

`$$ETo = \frac{0.408\Delta(Rn-G)+\gamma\frac{900}{T+273}u2(es-ea)}{\Delta+\gamma(1+0.34u2)}$$`

$$ETo = \frac{0.408\Delta(Rn-G)+\gamma\frac{900}{T+273}u2(es-ea)}{\Delta+\gamma(1+0.34u2)}$$

$ETo$ = reference evapotranspiration (mm/day)

$Rn$ = net radiation at the crop surface (MJ/m2/day)

$G$  = soil heat flux density (MJ/m2/day)

$T$ = mean daily air temperature at 2 m height

$u2$ = wind speed at 2 m height (m/s)

$es$ = saturation vapor pressure (kPa)

$ea$ = actual vapor pressure (kPa)

$es-ea$ = saturation vapor pressure deficit (kPa)

$\Delta$ = slope vapor pressure curve (kPa/°C)

$\gamma$ = psychrometric constant (kPa/°C)


### Psychrometric constant
`$$\gamma = \frac{Cp P}{\epsilon \lambda}$$`

$$\gamma = \frac{Cp \ P}{\epsilon \lambda}$$

$\gamma$ = psychrometric constant (kPa/°C)

$\lambda$ = latent heat of vaporization, 2.45 (MJ/kg)

Cp = specific heat at constant pressure (MJ/kg/°C)

$\epsilon$ = ratio of molecular weight of water vapour/dry air = 0.622

$P$ = atmospheric pressure (kPa)

<br/>

### Wind speed at 2 meters above the soil surface

`$$u2 = uz\frac{4.87}{\ln(67.8z-5.42)}$$`

$$u2 = uz\frac{4.87}{\ln(67.8z-5.42)}$$

$u2$ = wind speed at 2 m above ground surface (m/s)

$uz$ = measured wind speed at z m above ground surface (m/s)

$zm$ = height of measurement above ground surface (m)



### Mean saturation vapor pressure

`$$es = \frac{eTmax+eTmin}{2}$$`

$$es = \frac{eTmax+eTmin}{2}$$

$es$ = mean saturation vapor pressure (kPa)

$eTmax$ = saturation vapor pressure at temp Tmax (kPa)

$eTmin$ = saturation vapor pressure at temp Tmin (kPa)

### Slope of vapor pressure

`$$\Delta = \frac{4098\bigg[0.6108\exp\bigg(\frac{17.27 Tmean}{Tmean+237.3}\bigg)\bigg]}{(Tmean+237.3)^2}$$`

$$\Delta = \frac{4098\bigg[0.6108\exp\bigg(\frac{17.27 Tmean}{Tmean+237.3}\bigg)\bigg]}{(Tmean+237.3)^2}$$   

$\Delta$ = slope of saturation vapor pressure curve at air temp T (kPa/°C)

$Tmean$ = average daily air temperture

### Actual vapor pressure

`$$ea = \frac{eTmin\frac{RHmax}{100}+eTmax\frac{RHmin}{100}}{2}$$`

$$ea = \frac{eTmin\frac{RHmax}{100}+eTmax\frac{RHmin}{100}}{2}$$ 

$ea$ = actual vapor pressure (kPa)

$eTmax$ = saturation vapor pressure at temp Tmax (kPa)

$eTmin$ = saturation vapor pressure at temp Tmin (kPa)

$RHmax$ = maximum relative humidity (%)

$RHmin$ = minimum relative humidity (%)

### Extraterrestrial solar radiation

`$$Ra=\frac{24(60)}{\pi}\hspace{2mm}G\hspace{2mm}dr[\omega\sin(\phi)\sin(\delta)+\cos(\phi)\cos(\delta)\sin(\omega)]$$`

$$Ra = \frac{24(60)}{\pi} \hspace{2mm}G \hspace{2mm} dr[\omega\sin(\phi)\sin(\delta)+\cos(\phi)\cos(\delta)\sin(\omega)]$$

$Ra$ = extraterrestrial radiation (MJ/m2/day)

$G$ = solar constant (MJ/m2/min)

$dr$ = $1 + 0.033 \cos(2\pi J/365)$

$J$ = number of the day of the year

$\phi$ = $\pi/180$ decimal degrees  (latitude in radians)

$\delta = 0.409\sin((2\pi J/365)-1.39)\hspace{5mm}$ Solar decimation (rad)

$\omega = \pi/2-(\arccos(-\tan(\phi)\tan(\delta)) \hspace{5mm}$ sunset hour angle (radians)
# 2019-06-26-hayden-rectangle

## What is this?

An exploration of St. Louis Metropolitan Police Department crime reports data to analyze crimes reported inside and outside of the "Hayden Rectangle" between 2017 and 2019.

### Installation

I recommend using a virtual environment.

Use your package manager of choice to install `requirements.txt`. E.g. using `pip`:

```bash
pip install -r requirements.txt
```

### Usage

Inside the project folder, start the jupyter notebook server:

```bash
jupyter notebook
```

`import.ipynb` walks through importing the data from the files in `originals`. `analysis.ipynb` walks through the analysis of the data.

*NOTE: Running the `import` notebook will delete and recreate the `temp` folder.*

## Tell me more

In 2018, the St. Louis Metropolitan Police Department focused on reducing violent crime in a 7+ sq. mi. area of north St. Louis. This came to be known as the "Hayden Rectangle" as the project was announced by Chief John Hayden Jr. ([see previous coverage](https://news.stlpublicradio.org/post/crime-declines-st-louis-police-chief-credits-targeting-specific-neighborhoods#stream/0))

We used [crime reports published by the SLMPD](https://www.slmpd.org/Crimereports.shtml) to look at how crime has changed year-over-year in 2017 (before the increase in policing the area), 2018 (when the program started) and 2019 (as it's ongoing).

## Findings

There's more detail [in the analysis notebook](analysis.ipynb).

All crimes decreased year over year between 2017–18, and continued to decrease between 2018-19, though at a slower rate. This happened both inside and outside the rectangle.

Violent crimes (defined as homicide, robbery, and aggravated assaults with a firearm) throughout the city also decreased between 2017–18 and had a much smaller decrease between 2018–19. Between 2017–18 the decrease was largest outside the rectangle. But between 2018–19, the rectangle saw a decrease while outside the rectangle increased slightly.

## Caveats

We looked at crimes occurring between January-May only, in order to do year-over-year comparisons. We looked at crimes with provided coordinates only, to facilitate an in-rectangle/out-of-rectangle comparison.
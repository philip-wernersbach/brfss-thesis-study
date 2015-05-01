# brfss-thesis-study
The program that crunches Behavioral Risk Factor Surveillance System data for my
Economics thesis on unemployment related lifestyle choices.

##About
I wrote this program in order to facilitate crunching the data for the Center for
Disease Control and Prevention's 2013 Behavioral Risk Factor Surveillance System
survey for my undergraduate Economics thesis at the Northern Kentucky University.
It crunches the BRFSS data and runs several regressions in order to attempt to
determine if certain lifestyle choices are effected by employment status.

I am releasing this program as Free and Open Source Software, as I personally feel
that knowledge should be free, and this is my way of chipping away at the
restrictive paywalls that academia puts knowledge behind, which is a modern day
form of rent-seeking.

##Usage
1. Download the [2013 BRFSS Data in ASCII format](http://www.cdc.gov/brfss/annual_data/annual_2013.html).
2. Extract the `LLCP2013ASC.ZIP` file. A file named `LLCP2013.ASC` will be created.
3. Move the `LLCP2013.ASC` file to the `input` folder in this folder.
4. Download the [Julia language runtime](http://julialang.org/downloads/) and
install it.
5. Open up a terminal in this directory.
6. Run `julia BRFSSThesisStudy.jl`. The code will output regression information
to the terminal, and it will also output several files to the `output` directory.

##Technical Stuff
This program is written in the [Julia language](http://julialang.org),
and it uses the [`GLM.jl`](https://github.com/JuliaStats/GLM.jl), [`Gadfly.jl`](http://gadflyjl.org),
[`DataFrames.jl`](https://github.com/JuliaStats/DataFrames.jl), and [`Match.jl`](https://github.com/kmsquire/Match.jl)
libraries.

##License
This code is licensed under the GNU Affero General Public License version 3. See
the [`LICENSE`](LICENSE) file for the full license text.

# FLOSSY

(Fit Linear periOd-Spacing patternS interactivelY)

## Physical context

Period-spacing patterns are an asteroseismic tool that probes the near-core regions of a star. Tassoul 1980 predicts the period of gravity modes to be equidistant (i.e.  constant $dP$) for a spherical chemically-homogeneous non-rotating star. Keppler and TESS observation have revelead a variety of non constant dP patterns whose features have been associated to the physic inside the star. For instance, Miglio lnked dips in the patterns to gradients in the chemical composition, Timothy 2015 established the relation between the pattern's slope and the interior rotation. The community is currently searching to formalize the physics on it (Eg. Cunha 2019, Townsend 2003) and at the same time applying forward modelling to find constraints in the stellar interior based on observations (May, nature).


The asymptotic analysis of the pulsation equations predicts regularly-spaced periods for gravity
modes. These periods get deflected when a sharp variation in the buoyancy frequency, associated with
strong chemical gradients, is present. These features are known as glitches and their study is one of
the few methods allowing us to probe the physical conditions in a localized region inside a star.
Theoretical works (e.g., Cunha et al. 2015, 2019) provide the analytical bases to interpret the
signatures of glitches of arbitrary amplitude in seismic observables. However, testing the analytical
predictions is not straightforward, because finding a model with a glitch with specific properties (e.g.,
position, amplitude, and width) implies, in the best-case scenario, to explore the space of stellar
parameters until the desired glitch is attained. This approach has clear disadvantages like (1) no warranty to generate the pursued glitch, (2) time consuming, and (3) preclusion of a direct comparison of the effect of different glitches on the seismic data.

This is a Python program that allows to artificially add/remove a Gaussian-like
glitch into/from the buoyancy profile of an already existing stellar model, that way solving points (1-
3). Comparison between the sharpness of the glitch with respect to the local wavelength of gravity
modes is also provided as well as the possibility to remesh the model to allow for a very narrow glitch.
The modification to the buoyancy frequency is done in a consistent way by a correspondent sole
modification of the first adiabatic exponent as described in Ball et al. 2018, section 2.3. The program
counts with an interactive GUI as well as a command line mode.

## Remove a glitch from a stellar model:

The current version can operate only with stellar models stored as unformatted AMDL
files, which is the format that the Aarhus adiabatic pulsation code (ADIPLS, Chistensen-
Dalsgaard 2008) uses.

# GPMDB_GPlates_version
Here is the GPML file for the latest Global Paleomagnetism Data Base (GPMDB)
4.6b. It can be opened using GPlates. **Please note that here the points
visulized are paleopoles**.

Use

```shell
tar xvfz gpmdb46b_gpml.tar.gz
```

to decompress the *.tar.gz file. You may need to install tar first. For example, if
you are using ubuntu Linux, use

```shell
apt-get install tar
```

. For other Linux distros, the command should be similar.

The original file is in Microsoft Access *.MDB format (See its source [here][1]).

This version includes published data up to Dec 2004, all Australian
published data up to Jan 2011, and some additional data published
in 2005-2016. The total number of included paleomagnetic poles is 9514.

GPMDB was originally created by [Michael McElhinny and Jo Lock
(1996)][2], and recently maintained by [Sergei Pisarevsky][3].

[1]: https://confluence.csiro.au/display/cmfr/Palaeomagnetism+and+Rock+Magnetism
[2]: https://link.springer.com/article/10.1007%2FBF01888979
[3]: http://onlinelibrary.wiley.com/doi/10.1029/2003EO200007/full

## How to Use

1. After decompressing the *.tar.gz file, we should have three new files in the
directory: (1) gpmdb46b.gpml, paleomagnetic data; (2) gmap2015_rotation.rot,
Plate kinematics model; (3) gmap2015_plateid.txt, Plate IDs for the kinematics
model.

2. Import gpmdb46b.gpml and gmap2015_rotation.rot into GPlates.

3. In the "Layers" dialogue, under the layer for gpmdb46b.gpml, go to
"Reconstruction options" and click its "Set VGP visibility..." to set "Show VGPs
at times within 0.00 My of VGP's age" (please note that this age is actually the
average age of the High Magnetic Age and the Low Magnetic Age for each
paleopole/VGP; here the High and Low Magnetic Ages are shown as Valid time in
GPlates, i.e. from "High Age" to "Low Age").

## Further Thinking

Paleomagnetic poles should remain their appearances during the time span from
their High Magnetic Ages to their Low Magnetic Ages, not just at one timestamp
(e.g. the mean age used commonly). So the right visulization should be to set
"Show all VGPs at times between Distant Past (check) and Distant Future (check)
in the dialogue of "Set VGP Visibility" in the above Step 3.

Here is an example of paleomagnetic pole visualization in such way (Click on the
image below to view the video):
[![Consistency of paleomagnetic north poles from the North American Craton since 330 Ma](https://img.youtube.com/vi/OjngaZt8o5g/0.jpg)](https://www.youtube.com/watch?v=OjngaZt8o5g "Consistency of paleomagnetic north poles from the North American Craton since 330 Ma")

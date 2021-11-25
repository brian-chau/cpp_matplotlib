# MatPlotLib

To set this up for a Debian based distro:

1. Install `matplotlib`.

> pip3 install matplotlib

2. Find out the actual path to `numpy`:

> cd /

> find . -type d -name "numpy" -print

3. Create a symbolic link to `numpy` using the path you found in step (2).

> sudo ln -s <actual/dir/path/to/numpy> /usr/include/numpy

4. Add `/usr/include/python3.8` into your "include directories" list in your Makefile (adjust based on your actual version of Python)

5. Add `-lpython3.8` into your "library" list in your Makefile

6. Build, and tada!



powerscenarios
=====================

Renewable energy scenarios for stochastic grid operation problems

## How to install

Create a conda environment and install pywtk, powerscenarios

```bash
git clone https://github.com/NREL/pywtk.git
git clone git@github.nrel.gov:isatkaus/powerscenarios.git
cd powerscenarios
conda env update -n powerscenarios
source activate powerscenarios
cp patches/fill_tz.py ../pywtk/pywtk/  # needed patch for pywtk if using py3, or change print statements manually
cd ../pywtk/
python setup.py install
cd ../powerscenarios/
pip install -e .
```

## optional packages
```bash
conda install -c conda-forge gmaps # for visualization of grids (buses, wind sites, power lines, etc)
pip install cufflinks # for quick scenario plotting 
```

## notebooks/ contains examples to get started



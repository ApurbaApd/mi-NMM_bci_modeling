## Abstract
Brain-Computer Interface (BCI) is a system that translates neural activity into commands, allowing
direct communication between the brain and external devices. Despite its clinical application, BCI
systems are unable to robustly capture subjects’ intent due to a limited understanding of the neural
mechanisms underlying BCI control. To address this issue, we introduce a biophysical linear neural
mass model to investigate the associated neural mechanisms of motor imagery-based BCI experiments by
modulating the scale-free spectral characteristics of afferent inputs. We tailor this motor imagery neural
mass model (mi-NMM) to simulate both motor imagery task and resting state, and apply this approach to
a cohort of 19 healthy subjects trained over four sessions where magnetoencephalography (MEG) and
electroencephalography (EEG) signals were simultaneously recorded. Task-dependent modulation of
scale-free cortical dynamics reveals training-induced excitatory–inhibitory reconfiguration in BCI training.
The intra-regional neural connectivity strengths and time scales of the modeled excitatory and inhibitory
neural mass populations capture changes in neural activity across conditions and sessions. Those changes
appear in important areas of the sensorimotor cortex, relevant for motor imagery tasks. We observed these
effects in both EEG and MEG modalities. These findings provide insights into the underlying neural
mechanisms in a motor imagery task in BCI, paving the way to tailored BCI training protocols.



## Set up
First clone the environment to your computer, either download this repo as a `.zip` file or `git clone https://github.com/ApurbaApd/mi-NMM_bci_modeling.git`.

Set up a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html) if you do not have all the packages/compatible versions. The list of dependencies is listed in `environment.yml`.

Set-up environment using conda, detailed instructions can be found [here](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html). Or after cloning this repository, go to the repo by typing `cd spectrome` and then typing:
`conda env create -f environment.yml`

If conda complains about not finding packages/libraries, make sure `conda-forge` is in the list of channels being searched by `conda`.
You may add `conda-forge` to your list of channels with the command: `conda config --add channels conda-forge`.

The default name of the environment is `spectrome`, activate the environment with `source activate spectrome`, and deactivate with `source deactivate` or `conda deactivate`.

If you want to be able to run `spectrome` from anywhere, just add it's path to your PYTHONPATH. For instance, if you downloaded `spectrome` to `~/Documents/spectrome` do `export PYTHONPATH=$PYTHONPATH:~/Documents/spectrome`. You may have to restart your terminal to make sure this change takes effect.

After completing the set-up for conda environment and `spectrome` path, you may go to the `spectrome` folder and type `jupyter notebook` or `jupyter lab` in your terminal to run the Jupyter notebooks.

## Files:
 - `../spectrome/notebooks`: contains the jupyter notebooks, with all the analysis done on the data.
 - `../spectrome/scripts`: It contains the `run_local_model_mi_apd.py`, `run_local_model_mi_apd.py` are the simulation of frequency spectrums with various values of the parameters in different bounds for the HCP template connectome in the case of MI and Rest, respectively. 

 - `../spectrome/data_brain_plotting`: contains jupyter notebooks for brain plots.



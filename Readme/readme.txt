TractoFlow pipeline

Start time: 2023-01-26T14:37:27.304266-05:00

[Command-line]
nextflow run scilus/tractoflow -r 2.4.1 --bids sourcedata/cneuromod.anat.raw/ --fs sourcedata/cneuromod.anat.freesurfer/ --max_dti_shell_value 1550 -profile use_cuda,ABS,cbrain --run_gibbs_correction True -with-singularity 'docker://scilus/scilus:1.4.2' --bidsignore bidsignore --singularity.pullTimeout 60 -w /scratch/bore/work/ --eddy_cmd eddy_cuda9.1 --output_dir . -with-report report_tractoflow.html

[Git Info]

https://github.com/scilus/tractoflow - 2.4.1 [72a8896aa566535bc4c1b6134cdd8022a4ed915f]

[Options]

clean_bids=false
b0_thr_extract_b0=10
dwi_shell_tolerance=20
sh_fitting=false
sh_fitting_order=6
sh_fitting_basis=descoteaux07
dilate_b0_mask_prelim_brain_extraction=5
bet_prelim_f=0.16
run_dwi_denoising=true
extent=7
run_gibbs_correction=true
run_topup=true
config_topup=b02b0.cnf
encoding_direction=y
readout=0.062
prefix_topup=topup_results
run_eddy=true
eddy_cmd=eddy_cuda9.1
bet_topup_before_eddy_f=0.16
use_slice_drop_correction=true
bet_dwi_final_f=0.16
run_t1_denoising=false
run_resample_t1=true
t1_resolution=1
t1_interpolation=lin
fa_mask_threshold=0.4
run_resample_dwi=true
dwi_resolution=1
dwi_interpolation=lin
max_dti_shell_value=1550
min_fodf_shell_value=700
number_of_tissues=3
fa=0.7
min_fa=0.5
min_nvox=300
roi_radius=20
set_frf=true
manual_frf=15,4,4
mean_frf=false
sh_order=8
basis=descoteaux07
fodf_metrics_a_factor=2.0
relative_threshold=0.1
max_fa_in_ventricle=0.1
min_md_in_ventricle=0.003
pft_seeding_mask_type=wm
pft_fa_seeding_mask_threshold=0.1
run_pft_tracking=false
pft_compress_streamlines=true
pft_algo=prob
pft_seeding=npv
pft_nbr_seeds=10
pft_step=0.5
pft_theta=20
pft_sfthres=0.1
pft_sfthres_init=0.5
pft_min_len=20
pft_max_len=200
pft_particles=15
pft_back=2
pft_front=1
pft_compress_value=0.2
pft_random_seed=0
local_seeding_mask_type=wm
local_fa_seeding_mask_threshold=0.1
local_tracking_mask_type=wm
local_fa_tracking_mask_threshold=0.1
run_local_tracking=true
local_compress_streamlines=true
local_algo=prob
local_seeding=npv
local_nbr_seeds=10
local_step=0.5
local_theta=20
local_sfthres=0.1
local_sfthres_init=0.5
local_min_len=20
local_max_len=200
local_compress_value=0.2
local_random_seed=0
processes_brain_extraction_t1=4
processes_denoise_dwi=4
processes_denoise_t1=4
processes_eddy=1
processes_fodf=4
processes_registration=4
run_tractoflow_abs=true
template_t1=/human-data/mni_152_sym_09c/t1
output_dir=.
processes=false
Mean_FRF_Publish_Dir=./Mean_FRF
Readme_Publish_Dir=./Readme
Read_BIDS_Publish_Dir=./Read_BIDS
bids=sourcedata/cneuromod.anat.raw/
fs=sourcedata/cneuromod.anat.freesurfer/
bidsignore=bidsignore
singularity={pullTimeout=60}
input=false
bids_config=false
help=false
dti_shells=false
fodf_shells=false


**Problem 1**

To run the pretrained gaussians, run `python render.py --gaussians_per_splat=4096`. To train the gaussians, run `python train.py --gaussians_per_splat=4096`.

**Problem 2**

Run the bash files `runq21.sh` and `runq22.sh` to run the code for Problem 2.1 and Problem 2.2, respectively. The images generated will be in the `output/` folder.

Use the following command to generate the prompts for 2100 iterations for "a standing corgi dog", and 4100 iterations for everything else. Use `--view_dep_text=1` for view dependency.

`python Q23_nerf_optimization.py --prompt="{prompt}" --iters={iters} --lambda_entropy=0.0005 --lambda_orient=0.01 --latent_iter_ratio=0.2`
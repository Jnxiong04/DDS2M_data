# Dataset explanation
All datasets are in the same format as gum_demo_data.pickle, with the tuple (x_test, y_test, observed_mask, missing_mask, ground_truth)
x_test has been updated to the result of some method of denoising through DDS2M.

demo_recon_degrade.pickle currently has the best alignment error after being put through the GumNet.

Explainations for each pickle file:
1. demo_recon_rand.pickle contains the results of denoising a randomly generated noise tensor
2. demo_recon_orig.pickle contains the results of denoising the original subtomograms in x_test
3. demo_recon_degrade.pickle contains the results of denoising a degraded subtomogram
4. demo_recon_degrade_quad.pickle contains the results of denoising  a degraded subtomogram with a quad noise schedule
5. demo_recon_degrade_qf.pickle contains the results of denoising a degraded subtomogram, with the DDS2M model using Kowshik's finetuned parameters and a quad noise schedule 

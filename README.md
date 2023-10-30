# Depth Map Evaluation

During my internship as part of AI team in [FootFallcam](https://www.footfallcam.com/en/), my first mini-project is to make a scoring model for depth map evaluation.  


# Background
A depth map is a crucial aspect for the company as depth map conditions will greatly affect the result of human tracking. As a result, I was asked to create a scoring model
to help the company filter out some of the "issue" devices.

# My approach
1. Extract live view images, depth maps, and tracking zone coordinates from the company system with C++ programming language
2. Manually annotate the height object in live view with Label studio
3. Take the mask as the ground truth 
4. Compare ground truth with real depth map (try different evaluation metrics)
5. Finalise to use Structural Similarity Index(SSIM)
   - The real depth map has a gradient while the generated ground truth has only black and white
   - SSIM is proven to have a lesser emphasis on color brightness while taking into consideration of luminance, contrast, and structure



# Disclaimer
No dataset will be uploaded in this repo, it has only the baseline of the program



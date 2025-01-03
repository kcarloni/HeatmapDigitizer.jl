# HeatmapDigitizer.jl
digitize a heatmap you found on the internet


preliminary steps: 

- (1) count the number of bins in each dimension `(nx, ny)`
- (2) estimate the number of pixels per bin, and multiply to get the total number of pixels along each axis. crop the image exactly
- (3) record the extrema of the colorbar values `(vmin, vmax)`
- (4) crop the heatmap to remove the black boundary


then call `M = digitize_map( cropped_image_path, cropped_cbar_path, (nx, ny), (vmin, vmax) )`

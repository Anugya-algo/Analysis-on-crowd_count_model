# Analysis-on-crowd_count_model
 1. Crowd Size Classification
Purpose: Categorize image as having a Small, Medium, or Large crowd.
Method: Sum of all density values compared against thresholds.
![Alt Text](images/my_image.png)
 3. Stampede Zone Detection
Purpose: Identify zones with high density and abrupt movement (gradient).
Method: Use of gradient magnitude + density threshold to generate a stampede risk mask.
4. Gradient Field (Flow) Visualization
Purpose: Visualize potential crowd flow or movement direction.
Method: np.gradient() used with plt.quiver() to show vector field on density map.
 5. Population Concentration Index (PCI) Heatmap
Purpose: Identify and quantify density concentration across different regions of the image.
Method: Divide image into a 4x4 grid and calculate total density per patch.
 6. Adaptive Risk Zone Detection
Purpose: Dynamically identify high-risk zones without fixed thresholds.
Method: Calculate risk as density > mean + 1.5 * std. Overlay mask in red.
<p align="center">
  <img src="https://github.com/Anugya-algo/Analysis-on-crowd_count_model/blob/main/Adaptive%20risk%20zone.png" width="400"/>
</p>
![Alt Text]()
 8. DBSCAN-Based Hotspot Clustering
Purpose: Automatically discover density hotspots using unsupervised learning.
Method: DBSCAN clusters points where density exceeds a set threshold.
 9. Crowd Fingerprint Profiles
Purpose: Understand spatial distribution patterns of the crowd.
Method: Sum densities along:
Vertical axis → Vertical Profile  ; Horizontal axis → Horizontal Profile


Title: Object Tracking with Centroid-Based Approach

Description:

This Python code implements object tracking using a centroid-based approach. Object tracking is a critical component in computer vision and artificial intelligence applications, enabling the monitoring and analysis of objects' movement in video sequences.

**Features:**

1. **Centroid-Based Tracking:**
   - The core of this tracking method revolves around calculating the centroids of objects in consecutive frames.
   - Centroids are computed by determining the midpoints of bounding box rectangles around objects.
   - The code efficiently registers, updates, and deregisters objects based on their centroid positions.

2. **Distance Computation:**
   - Utilizes the SciPy library to calculate the Euclidean distance between existing object centroids and centroids of potential matches in the current frame.
   - Determines the nearest centroids using distance metrics, facilitating effective object matching.

3. **Consecutive Frame Handling:**
   - Implements a mechanism to handle consecutive frames where objects are marked as "disappeared."
   - Objects are deregistered if they exceed a specified threshold of consecutive frames without detection.

4. **Dynamic Object Registration:**
   - Dynamically registers new objects for tracking if the system is not currently tracking any objects.
   - New object centroids are added to the tracking list for subsequent frames.

**Usage:**
- This code is versatile and can be integrated into various computer vision applications such as surveillance systems, object recognition, and human tracking.

**Types of Tracking:**
- The implemented centroid-based tracking is particularly effective for scenarios where objects exhibit distinct centroids, making it suitable for tracking various entities like people, vehicles, or other identifiable objects.

**How to Use:**
1. Clone or download the repository.
2. Integrate the `CentroidTracker` class into your Python project.
3. Provide bounding box coordinates (rectangles) for each object in consecutive frames.
4. Utilize the `update` method to track and update object centroids.

Enhance your computer vision projects with this efficient and adaptable centroid-based object tracking code available on GitHub. Start tracking objects seamlessly and gain insights into their movement patterns!

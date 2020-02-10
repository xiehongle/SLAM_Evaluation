# evaluate_ate_scale
Script to compute the Absolute Trajectory RMSE error for the TUM RGB-D dataset, that automatically aligns the scale of the estimated trajectory with ground-truth. It is useful to evaluate trajectories generated by SLAM or VO algorithms.
See the original tool and how to use it here: http://vision.in.tum.de/data/datasets/rgbd-dataset/tools#evaluation

Trajectory and ground-truth are aligned computing a Similarity Transformation (Rotation, Translation and Scale) with the method of Horn:    B. K. P. Horn, “Closed-form solution of absolute orientation using unit quaternions,” Journal of the Optical Society of America A , vol. 4, no. 4, pp. 629–642, 1987. [pdf](http://people.csail.mit.edu/bkph/papers/Absolute_Orientation.pdf)
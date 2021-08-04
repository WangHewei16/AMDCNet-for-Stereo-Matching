# Stereo Matching Based on Convolution Aggregation Network and Visual Sensitivity

### Code
* `./model/`: This folder contains Census model code.
* `./model add smoothing filtering/`: This folder contains the model code which add a soothing filter based on the Cencus model.

98% codes are written in C++, 2% codes are written in C. Codes are written in Visual Studio 2013. The environment of OpenCV is 2.4.9. 

### Data
* `./Part 1-4 test data set and disparity map/`: This folder contains test data and disparity map which are standard images from Middlebury official test datasets.

### Figure
* `Figure1.png`: This figure shows the comparison of different test results. The first column is the perspective image in the original image of the experimental data set, the second column is the ideal parallax image for reference, the third and fourth columns are the result images obtained by the classical algorithm census, and the fifth and sixth columns are stereo matching algorithms based on visual sensitive information. Among them, the red marks in the fourth and sixth columns indicate the mismatching areas of the marks when comparing the two result maps with the ideal disparity map. Through the display of subjective images, we can clearly see that the proposed algorithm can effectively calculate and generate the disparity of the original image, and the matching effect is better than that of the classical algorithm. 

<div align=center><img src="https://github.com/WangHewei16/Stereo-Matching-Algorithm/blob/main/Figure1.png?raw=true"/></div>


* `Figure2.png`: This figure shows the visual sensitive area retention. It shows that this algorithm has been improved and preserved in many visual sensitive areas, such as 'peak', 'lamp' and 'table'.
* `Figure3.png`: This figure shows the disparity image before and after optimization. It shows the results of further comparing the error matching rate of the optimized disparity map.
* `Figure4.png`: This figure shows the other processed images of propose algorithm. It shows the results that experimented with other images in the data set. From this figure, we can find that the algorithm proposed in this paper has good processing effect for most binocular vision images.
* `Figure5.png`: This figure shows a comparison of the other three images processed by the algorithm in this paper and Pyramid Stereo Matching Network, Richer Convolutional Features Network. The first column is the original left view image, which are art, baby and Book respectively, the second example is the real parallax image, the third column is the algorithm image in this paper, the fourth column is the result diagram of Pyramid Stereo Matching Network, and the fifth column is the result generated by the algorithm in literature of Richer Convolutional Features Network.

<div align=center><img src="https://github.com/WangHewei16/Stereo-Matching-Algorithm/blob/main/Figure5.png?raw=true"/></div>


### Table
* `Table1.png`: This table shows the error matching rate obtained by various algorithms. It shows that error matching rate of the proposed algorithm is lower than that of the same kind of algorithm, and the overall matching effect is better.
* `Table2.png`: This table shows the mismatch rate under different Gaussian noise concentrations. It shows that show that when the noise concentration increases, the change degree of the error matching rate of this algorithm is lower, and the sensitivity to noise is lower.
* `Table3.png`: This table shows the comparison results of different algorithms. From this table, we can see the difference between NOCC and all. NOCC is the non occluded area mentioned above, and all is the matching of all areas of the image, including the blind area of parallax. The data of mismatch rate in the table objectively proves the effectiveness of this algorithm, which has more advantages than the same kind of classical algorithms.
* `Table4.png`: This table shows the comparison with different algorithms before and after optimization in non occluded area. The algoirthm in literature [24] is Multi-task Attention Stereo Network (MASNet), the algoirthm in literature [25] is Pyramid Stereo Matching Network, the algoirthm in literature [26] is Richer Convolutional Features Network.

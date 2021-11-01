# Pixelwise Dynamic Convolution Neural Network for LiDAR Depth Data Interpolation

Official code and data of the paper 'Pixelwise Dynamic Convolution Neural Network for LiDAR Depth Data Interpolation,' IEEE Sensors (2021) ([paper](https://ieeexplore.ieee.org/document/9594810))

---
# How to use
### Dependencies
* Pytorch > 1.3

### Run DownloadAndUnzip.sh
In your own directory, please run the following command in terminal.
<br>
> bash ./DownloadAndUnzip.sh 

You can also get the data by the following url.
https://drive.google.com/file/d/1VxAsOcZEwXpjhxe8uJhYqxoZQvTtPWp-/view?usp=sharing

### Quick start
Run the following code.
<br>
> python test.py  --gpu 0 --test ./test_data/minivan --weight InterpolationNetwork.pth --ndir mn

---
### Specification

* test_data
	* minivan : *test data of minivan*
	* minivan_mask : *intended defect data of minivan*
	* miraikan : *test data of miraikan*
	* miraikan_mask : *intended defect data of miraikan*
	* whill : *test data of whill*
	* whill_mask : *intended defect data of whill*

	* test_waymo_list.txt : *list of waymo data for test* (Please download Waymo dataset via official website)
	* waymo_mask : *intended defect data of waymo*

* test_data
	* train_whole : *train data*
	* train_whole_mask : *intended defect data of train data*
	* train_waymo_list.txt :  *list of waymo data for train* (Please download Waymo dataset via official website)


* dynamic_layer.py : *implementation of the pixelwise dynamic convolution layer* 
* network.py : *network architecture definition*
* test.py : *evaluation code*
* utils.py : *code for loading data*

---
# License
The code and data are allowed only for noncommercial usage. Please cite our paper if our data were used in your work.
You can see specific terms of use in the LICENSE.md.

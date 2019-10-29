text-KVQA dataset contains 257,380 images and associated question-answer pairs.
The images of this dataset consists of images from following modalities:
a) Scene Images
b) Movie Posters
c) Book Covers 

We provide questions inquiring about the meta information present in these
images. For example, in scene images we provide KB and QA pairs related to a
brand or a movie or a book.


Getting started
---------------------------------------------------------------
Download instructions:
---------------------
Download all the images, corresponding KBs and QA Pairs from the link mentioned from the project page.

Getting info about dataset:
---------------------------
The KBs and QA pairs are provided in the form of json file.

The KB json file is arranged in following way:

{ 'id': {

	'relation-1' : 'entity-1',
	'relation-2' : 'entity-2',
	.
	.
	.
	'relation-n' : 'entity-n',
	}

}

The QA Pairs json file is arranged in following way:
{
	<image_id>:{
	questions : ['Q1', 'Q2', ... 'QN'],
	answers	: ['A1', 'A2', ... 'AN'],
	"image_file" or "image_url": "<url> or <filename>"
	}
}

<image_id> is of the format <id>_<image_num>, where
<id> is entities' unique id, and
<image_num> is the sequence of images for particular entity (<id>).

If you use this dataset, please cite our ICCV 2019 paper.

@InProceedings{mishraICDAR19,
  author    = "Ajeet Kumar Singh and Anand Mishra and Shashank Shekhar and Anirban Chakraborty",
  title     = "From Strings to Things: A Knowledge-enabled VQA Model that can Read and Reason",
  booktitle = "ICCV",
  year      = "2019",
}
-----------------------------------------------------------------

For any queries about the dataset contact: ajeetk.singh1@tcs.com.

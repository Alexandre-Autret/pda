Welcome to the repository for my Python for Data Analysis project.

The code and report are contained within the "code_markdown.ipynb" jupyter notebook (also available as an HTML file), the dataset is made up of 6 HDF5 .mat files, the PDF contains a short presentation of this project.

Here are the required external libraries:
 - h5py
 - numpy
 - pandas
 - matplotlib
 - seaborn
 - sklearn

The dataset can be found here:
http://mason.gmu.edu/~lzhao9/materials/data/UAV/ (the UCI repo given originally doesn't have it on the page)

Conclusions:
The real challenge with this dataset was to set the exploration phase up, since I'd never worked with HDF5 files, the official documentation was a bit confusing, and I had to do some research on what the various features meant, since they contained technical data.
Once the exploration and cleaning phases were done though, I noticed that the dataset was very easy to work with: as the pairplots show in the report, it was really easy to build an extremely accurate model:
not only were the models working well with the testing set for the same drone used for the training set (Bebop Parrot), they also fit the DBPower UDI and DJI Spark drone data seamlessly.
While some features didn't seem particularly significant, I ultimately decided to keep them since it would've been really difficult to notice any difference in accuracy had I removed them.

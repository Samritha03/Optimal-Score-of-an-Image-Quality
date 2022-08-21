## Blind/Referenceless Image Spatial Quality Evaluator (BRISQUE) Algorithm


### Algorithm

 Step 1- Extract Natural Scene Statistics (NSS)
    
 Step 1.1- Mean Substracted Contrast Normalization (MSCN) 
    
 Step 1.2- Pairwise products for neighbourhood relationships
  
 Step 2- Calculate Feature Vectors
  
 Step 3- Prediction of Image Quality Score
 

### Packages


#### Installation

LibSVM is required. On ubuntu or other Debian-based system, you can install libsvm-dev package from apt as follows:
		
    apt-get install libsvm-dev

The package is in PyPl so you can install it simply by this command:
		
    pip install—process-dependency-links pybrisque


#### Usage

Initialise once:
		
    brisq = BRISQUE( )

and get the BRISQUE feature or score many times:
		
    brisq.get_feature(‘/path’)
	brisq.get_score(‘/image_path’)


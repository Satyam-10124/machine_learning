Types of learning

Supervised learning - labeled data
Unsupervised learning - unlabeled data
SemiSupervised learning - label and unlabeled data
Reinforcement learning - function is optimized by the reward [ajent] 

Split data
 - Test Set
 - Training Set
 - Validation Set
 
 
 mean is always favor to max value [extreme value]
 this can be verified by
 standard deviation - for extreme values standard deviation is high [square of variance cause this high deviation] 
 it is an average dispersion from the average
 
 
Do we need to remove outliers [based on the dataset]
	if your dataset is small you have an outliers.. if we gradually increase the dataset size.. this outliers might be an actual wanted data
	- we can verify with original population and come to a conclution if it is an actual outliers
	- inclue outliers
	- exclude outliers

Data preperation is more important than Model training

Transformation
anomaly

Data:
    - Discriptive statistics
        - mean
        - median
        - min 
        - max
        - variance
        - standard deviation
    leads to sample space understanding
    corelation 

in stock market prediciton.. 

negative correlation if you have 2 stocks and these two are negatively correlated [ if one goes profit and other goes loos since they are negatively correlated ]


Feature selection

noramal distribution 
    has only two variables 
    easy to manuplace
    easy to understand
    have strong mathematical prof

Average tells truth.. 

n = sample size
N = population size

u = population mean
    for sample data set we use n-1 [unbiased estimator]
    biased and unbiased
    to increase value we use n-1

Types of mean
    - Arithmetic mean
    - Geometric mean [ continueous ] 
    - hormonic mean

Median - it needs to be ordered, we will get centered value
        - not influated by outliers and scewness

mode - most occured
range - max-min
    
Reference = https://url-shortener-muruga.vercel.app/l6oa5ia
    
scaling - making the values range [ -1 , 1 ] , mean = 0 , standard deviation = 1
	  when your sample exibits properties of normal distribution then we can go with standard scaler [ bell shaped curve in line polot ]
	
	
	standard scaling = for each feature divide by its mean and subract by its standard diviation
			   Standardize features by removing the mean and scaling to unit variance. The standard score of a sample x is calculated as: z = (x - u) / s.
			   
			   from sklearn.preprocessing import StandardScaler
			   scaler = StandardScaler() 
         		   data_scaled = scaler.fit_transform(data)
         		   
         MinMax scaling = the data should not have outliers
         		  In this approach, the data is scaled to a fixed range — usually 0 to 1.
         		  In contrast to standardization, the cost of having this bounded range is that we will end up with smaller standard deviations, which can
         		  suppress the effect of outliers. Thus MinMax Scalar is sensitive to outliers.
         		   
         		   from sklearn.preprocessing import MinMaxScaler
         		   scaler = MinMaxScaler() 
         		   data_scaled = scaler.fit_transform(data)
         		   
         Robust Scalar (Scaling to median and quantiles) = 
			  Scaling using median and quantiles consists of subtracting the median to all the observations and then dividing by the interquartile difference.
			  It Scales features using statistics that are robust to outliers.
			  
			  X_scaled = (X — X.median) / IQR
			  
			  from sklearn.preprocessing import RobustScaler
			  scaler = RobustScaler() 
			  data_scaled = scaler.fit_transform(data)
			
			  

normalization


maxium abalute scalar
power tranformaton

feature encoding
target encoding
onehot encoding

dot product - projection of one vector over another vector

standard normal distribution

scewness = 1,2,3,4,5,6,7,8,9,10 the mean will be favour to the higher value
anomoly
box-plot
sns
combinations 4C2
diff btw eda cda


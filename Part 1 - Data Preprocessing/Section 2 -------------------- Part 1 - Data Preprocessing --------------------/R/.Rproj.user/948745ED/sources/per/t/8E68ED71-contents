# Data Preprocessing

# Importing the dataset
dataset = read.csv('Data.csv')

# Taking care of missing data
dataset$Age = ifelse(is.na(dataset$Age), # if the value is missing...(True for missings)...
                     ave(dataset$Age, FUN = function(x) mean(x, na.rm = TRUE)), # Fill with mean of values
                     dataset$Age) # what to fill in if it's not missing? Just the value

dataset$Salary = ifelse(is.na(dataset$Salary),
                        ave(dataset$Salary, FUN = function(x) mean(x, na.rm = TRUE)),
                        dataset$Salary)

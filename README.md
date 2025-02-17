# Assignment: Descriptive Statistics for Iris Dataset

# Load the iris dataset (it's built into R)
data(iris)

# 1. Calculate the mean of sepal length
mean_sepal_length <- mean(iris$Sepal.Length)
print(paste("Mean Sepal Length:", mean_sepal_length))

# 2. Calculate the median of sepal width
median_sepal_width <- median(iris$Sepal.Width)
print(paste("Median Sepal Width:", median_sepal_width))

# 3. Calculate the standard deviation of petal length
sd_petal_length <- sd(iris$Petal.Length)
print(paste("Standard Deviation Petal Length:", sd_petal_length))

# 4. Calculate the range of petal width
range_petal_width <- range(iris$Petal.Width)
print(paste("Range Petal Width:", range_petal_width[1], "to", range_petal_width[2]))

# 5. Summarize the entire dataset
summary(iris)

# 6. (Optional) Create a histogram of sepal length
hist(iris$Sepal.Length, 
     main = "Histogram of Sepal Length",
     xlab = "Sepal Length (cm)",
     col = "lightblue",
     border = "black")


#--- Explanation and Justification (Important for your submission) ---

# This script calculates descriptive statistics for the Iris dataset.
# The 'data(iris)' command loads the built-in dataset.

# 1. The mean sepal length is calculated using the 'mean()' function.
# 2. The median sepal width is calculated using the 'median()' function.
# 3. The standard deviation of petal length is calculated using the 'sd()' function.
# 4. The range of petal width is found using the 'range()' function, which returns
#    both the minimum and maximum values.  We then print them separately.
# 5. The 'summary()' function provides a comprehensive overview of the dataset,
#    including min, max, quartiles, mean, and median for each variable.
# 6. (Optional) A histogram visually represents the distribution of sepal lengths.

# These statistics provide insights into the central tendency and spread of
# the different measurements in the Iris dataset.  For example, the mean
# gives us the average value, while the standard deviation tells us how much
# the data points typically deviate from the mean.  The range shows the total
# spread of values.  The summary function provides an efficient way to see
# all of these at once.  The histogram helps visualize the distribution.

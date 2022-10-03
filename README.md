# K-NearestNeighborsClassifier
Problem statement: Build a k nearest neighbor classifier in Python to classify the MNIST digit data. This
is a multi-class classification problem with labels from 0 to 9.

# Conditions:

  1. The value of k: Different groups may have different values of k. The k value for a group is the
maximum of the last two digits of USNs (University Seat Number) of students in the group. For example, if a group has students
with USNs: ENGXXAM0099 and ENGXXAM0084, then the k value for the group is max{99, 84} = 99.
The k value used here is 44.

  2. Number of data points: The MNIST database has 60,000 data points but we will not be using the whole data.
Different groups may have different number of data points to work with: add the last two digits of USNs
of students in the group and multiply it by hundred and add 1000. That will be the size of your data.
For example, if a group has students with USNs: ENGXXAM0099 and ENGXXAM0084, then the n
value for the group is (84+99)×100+1000 = 19300. Use the first n points in the dataset as data.
The n value used here is 7100.

  3. Testing process (cross-validation): Randomly pick 20% of the data for testing. Do the testing k many
times (each time picking the 20% test data randomly) where k is determined as above. Report the
average of scores: a confusion matrix with averaged entries.

  4. Implementation: Write the code for a custom kNN algorithm, and generate an averaged confusion matrix.

# Anomalies
1. Sometimes in the Custom classifier, due to losses in the decimal places, when calculating the total number of elements in the final confusion matrix, the answer may not always be the exact number of testing datapoints used, rather it could be extremely close to the answer.

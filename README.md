# LogicNet
LogicNet: PROBABILISTIC CONTINUOUS LOGICS IN RECONSTRUCTING GENE REGULATORY NETWORKS
#####################################################################################
LogicNet in R:
After installing the LogicNet package in R, run the following commands to predict the Gene Regulatory Network (GRN) and logic functions among regulatory genes:

library(LogicNet)

data <- read.csv("Y3.csv") #  give the path to Y3.csv file

result=LogicNet(data)

result$PREDICTED_EDGES

result$PREDICTED_LOGIC


result$PREDICTED_EDGES shows the predicted directed edges and result$PREDICTED_LOGIC shows the predicted logic functions. For more information please see LogicNet help, using the following command:

help(package="LogicNet")



#####################################################################################
LogicNet in MATLAB:

To have the predicted edges and logic functions, load data and run matlab function LogicNet(data), in which data is the gene expression matrix.

load('Y3')

[PREDICTED_LOGIC,PREDICTED_EDGES]=LogicNet(data);

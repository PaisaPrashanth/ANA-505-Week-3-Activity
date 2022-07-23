# ANA-505-Week-3-Activity
R Studio ANA 505 Week 3 Activity



getwd()
setwd()

women

df_women<-data.frame(women)
df_women

head(df_women,2)

nrow(df_women)
ncol(df_women)
colnames(df_women)
lapply(df_women,class)


summary(df_women)

mean(df_women$height)

df_women[,1]
df_women[,2]


women_df <- data.frame(df_women)


df_women_indx <- women_df[(df_women$height>65),]
df_women_indx


nrow(df_women_indx)


ncol(df_women_indx)


ncol(df_women_indx) 
nrow(df_women_indx)

  
install.packages("ggplot2")
  

library(ggplot2)


ggplot(df_women, aes(x=height, y=weight)) + 
  geom_point()

ggplot(df_women, aes(x=height, y=weight)) + 
  geom_point(shape = 21, colour = "black", fill = "white", size = 5, stroke = 5)

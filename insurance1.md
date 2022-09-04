# rrepro
This is a line from R Studio
Adding more

head(df)
num_cols <- unlist (lapply(df, is.numeric))
num_cols
plot(df[, num_cols])
round(cor(df[, num_cols]),2)
smoker = as.factor(df$smoker)
sex = as.factor(df$sex)
region = as.factor(df$region)
boxplot(df$charges ~ smoker, main = 'smoker')
boxplot(df$charges ~ sex, main = 'sex')
boxplot(df$charges ~ region, main = 'region')
model = lm(charges ~., data =df)
summary(model1)
# MATH 1360 Lab 4
# Sheikh Billah (Alif)

library(mosaic)  

m <- 1:50
win_table <- 0*m

for (j in m){
  n <- 1:1000
  
  winning_door <- sample(c(1,2,3,4,5), length(n), replace=TRUE)
  first_pick <- sample(c(1,2,3,4,5), length(n), replace=TRUE)
  
  wins <-  0
  losses <- 0
  
  for (i in n){
    if (winning_door[i] == first_pick[i]){
      losses <- losses + 1
    }
    else{
      wins <- wins + 1
    }}
  win_table[j] <- wins
}

histogram(
          ~win_table,
          main = "Monty Hall Frequency of Wins",
          xlab = "Wins out of 1000",
          ylab = "Frequency",
          type = "c",
          breaks = seq(620,720,10)
)

mean(win_table)

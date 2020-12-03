# 2ndtest
#ggplot(data.frame(x=c(0:10)), aes(x)) + 
#geom_point(aes(y=dbinom(x, size = 10, prob = 0.5)),
#colour="#0065BD") + 
#theme_light() + 
#geom_vline(xintercept = 5, colour = "gold") +
#labs(x = "k", y = expression(rho["10,0.5"](k)),
#title = "Zähldichte der Binomial(10,0.5)-Verteilung")

ggplot(data.frame(x=1:100), aes(x)) + 
geom_smooth(aes(y=dgeom(x-1, prob = 0.05)),
colour="#0065BD") + 
theme_light() + 
labs(x = "k", y = expression(rho["0.05"](k)),
title = "Zähldichte der Geometrisch(0.05)-Verteilung")


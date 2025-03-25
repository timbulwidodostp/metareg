# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Meta-regression Use metareg (meta) With (In) R Software
install.packages("meta")
library("meta")
metareg = read.csv("https://raw.githubusercontent.com/timbulwidodostp/metareg/main/metareg/metareg.csv",sep = ";")
# Estimation Meta-regression Use metareg (meta) With (In) R Software
metareg$age <- c(55, 65, 55, 65, 55)
metareg$region <- c("Europe", "Europe", "Asia", "Asia", "Europe")
metacont <- metacont(n.e, mean.e, sd.e, n.c, mean.c, sd.c, data = metareg, sm = "MD")
update <- update(metacont, byvar = region)
metareg <- metareg(update, region + age)
summary(metareg)
# Meta-regression Use metareg (meta) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Brant test by Brant (1990) for ordinal logit models to test the parallel regression assumption Use brant With (In) R Software
install.packages("brant")
install.packages("MASS")
library("MASS")
library("brant")
# Estimate Brant test by Brant (1990) for ordinal logit models to test the parallel regression assumption Use brant With (In) R Software
brant = read.csv("https://raw.githubusercontent.com/timbulwidodostp/brant_r/main/brant_r/brant.csv", sep = ";")
brant$Smoke = ordered(brant$Smoke,levels=c("Never","Occas","Regul","Heavy"))
polr <- polr(Smoke ~ Sex + Height, data = brant, Hess = TRUE)
brant(polr)
# Brant test by Brant (1990) for ordinal logit models to test the parallel regression assumption Use brant With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished
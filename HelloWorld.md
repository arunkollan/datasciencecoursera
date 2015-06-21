## This is a markdown file
colname <- toupper(colname)
colname <- gsub("\\." , " " , toupper(colname))
grep(pattern = "HEART ATTACK", x = gsub("\\." , " " , toupper(colname)), value = TRUE)


colele <- function (nele , noutcome)
{
  print(c("ele", nele))
  print(c("noutcome", noutcome))
  tempcol <- gsub("\\." , " " , toupper(nele))
  print(c("tempcol", tempcol))
  ret <- grep(pattern = toupper(noutcome), tempcol, value = TRUE)
  print(c("return value " , ret))
  ret
}

gsub("\\." , " " , toupper(colnames[,1]))


> y <- lapply (x, function(x) str_length(x[1] >0) )
> bad <- is.na(y)
> good <- y[!bad]
> good

colnames <- colnames(x)
    colnumber<- c(1:length(colnames))
    colmatrix <- matrix(nrow = length(colnames), ncol=2)
    colmatrix <- cbind(colnumber, gsub("\\." , " " , toupper(colnames)))
    
cand_colnames <- lapply(colmatrix , function(colmatrix) 
                                                colmatrix[,2] == grep(pattern = "HEART ATTACK",
                                                gsub("\\." , " " , toupper(colnames)), 
                                                value = TRUE) 
                                    )

subset (colmatrix , colmatrix[, 2]  %in% cand_colmatrix, drop = TRUE)
                                    
cand_colnames <- lapply(colmatrix , function(colmatrix) 
                                              grep(pattern = toupper("heart attack") ,
                                              gsub("\\." , " " , toupper(colmatrix[,2 drop = FALSE])), 
                                              value = TRUE) 
                                        )
colnames <- colnames(x)
    colnumber<- c(1:length(colnames))
    colmatrix <- matrix(nrow = length(colnames), ncol=2)
    colmatrix <- cbind(colnumber, toupper(colnames))


clean_ds <- complete.cases(y)
clean_subset <- y[clean_ds, ][,1:2 ]
### Shell lesson
Use the following command to split the gapminder data set into one file per country and year
`while IFS=$'\t' read country year pop continent lifeExp gdp; do echo -e "$country\t$year\t$pop\t$continent\t$lifeExp\t$gdp" > "$country-$year"; done < gapminderDataFiveYear.txt`


For the lesson, ultimately, the students will reassemble all of the files back into one file. 
Over the course of the lesson, these disparate files will be used to teach different tasks and for challenges.
I'm on the fence, but I'm thinking of using awk to print data.

FIXME I will turn this into a WELL DOCUMENTED script later. - Stroot
The intent is to give it to the students *after the bootcamp* so they can practice with the same files.
I realize there is a little magic in that command, but I hope to give enough information to point eager students in the right
direction.


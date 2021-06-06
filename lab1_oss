# include <stdio.h>
# include <string.h>
int main( )
{
	FILE *filePointer ;
	char dataToBeWritten[50] = "Hello World-A Computer Science Sentence for beginners";
	filePointer = fopen("filehandling.c", "w") ;
	if ( filePointer == NULL )
	{
		printf( "filehndling.c file failed to open." ) ;
	}
	else
	{
		printf("The file is now opened.\n") ;
		if ( strlen ( dataToBeWritten ) > 0 )
		{
			fputs(dataToBeWritten, filePointer) ;
			fputs("\n", filePointer) ;
		}
		fclose(filePointer) ;
		printf("Data successfully written in file filehandling.c\n");
		printf("The file is now closed.") ;
	}
	FILE *fptr ;
    char dataToBeRead[50];
    fptr = fopen("filehandling.c", "r") ;
    if ( fptr == NULL )
    {
        printf( "filehandling.c file failed to open." ) ;
    }
    else
    {
        printf("The file is now opened.\n") ;
        while( fgets ( dataToBeRead, 50,fptr ) != NULL )
        {
            printf( "%s" , dataToBeRead ) ;
         }
        fclose(fptr) ;
        printf("Data successfully read from file filehandling.c\n");
        printf("The file is now closed.") ;
    }
	return 0;
}

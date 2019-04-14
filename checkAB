bool checkAB(char input[]) {
	char* t = input;
    
    if(*input =='\0')
        return 1;
    else if(*input=='a'){
        if(*(t+1)=='a')
            return checkAB(input+1);
        else if(*(t+1)=='b')
            return checkAB(input+1);
        else if(*(t+1)=='\0')
            return 1;
        else
            return 0;
    }
    
    else if(*input=='b'){
        if(*(t+1)=='b' && *(t+2)=='a')
            return checkAB(input+2);
        else if(*(t+1)=='b' && *(t+2)=='\0'){
             if(*(t-1)=='a')
                 return 1;
            else
                return 0;
        }
        else
            return 0;
    }

}

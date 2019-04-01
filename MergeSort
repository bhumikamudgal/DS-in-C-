void merge(int input[], int s, int mid, int e) {
    int temp[e-s+1];
    int i = s;
    int j = mid+1;
    //Let one part of array is from s to mid and another from mid+1 to end
    int k = 0;
    
    while(i<=mid && j<=e) {
        if(input[i]<=input[j]) {
            temp[k++] = input[i];
            i++;
        }
        else {
            temp[k++] = input[j];
            j++;
        }
    }
    
    while(i<=mid) {
        temp[k++] = input[i];
        i++;
    }
    
    while(j<=e) {
        temp[k++] = input[j];
        j++;
    }
    for(int l=s;l<=e;l++) {
        input[l] = temp[l-s];
    }
    
}

void mergeSort1(int input[],int s, int e) {
    if(s>=e)
        return;
    
    int mid = (s+e)/2;
    
    mergeSort1(input,s,mid);
    mergeSort1(input,mid+1,e);
    
    merge(input,s,mid,e);
}

void mergeSort(int input[], int size){
	// Write your code here
    mergeSort1(input,0,size-1);    
}

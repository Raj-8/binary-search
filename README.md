# binary-search


lo=0;int hi=2000000007;
while(lo<hi){
    int mid=(lo+hi+1)/2;
    int tot=0;
    for (int i = 0; i < n; i++) {
			tot += max(mid - a[i], 0LL);
		}
		if (tot <= x) {lo = mid;} 
		else {hi = mid - 1;}
}

cout<<lo<<endl;

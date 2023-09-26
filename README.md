# binary-search


while (lo < hi) {
		long long mid = lo + (hi - lo + 1) / 2;
		long long tot = 0;
		for (int i = 0; i < n; i++) {
			tot += max(mid - a[i], 0LL);
		}
		if (tot <= x) {lo = mid;} 
		else {hi = mid - 1;}
	}

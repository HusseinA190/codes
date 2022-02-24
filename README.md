# codes
problem solving codes
long long n;
	bool word = false;
	string x = "hate", y = "love", r1="that",r2="it", res="";
	cin>>n;
	if(n==1)
	{
		res = "I hate it";
		cout << res << endl;
	}
	else
	{
		for (int i = 0;i<n;i++)
		{
			if(!word)
			{
				if(i<n-1)
				{
					res += "I " + x + " " + r1+" ";
				}
				else if(i==n-1)
				{
					res += "I " + x + " " + r2;
				}
				word = !word;
			}
			else
			{
				if(i<n-1)
				{
					res += "I " + y + " " + r1+" ";
				}
				else if(i==n-1)
				{
					res += "I " + y + " " + r2;
				}
				word = !word;
			}

		}
		cout << res << endl;
	}

int l=1,r=n;

    while(l<r)
    {
        int mid=l+(r-1)/2;

        if(a[mid]==k)
        {
            cout << mid << endl;
            return;
        }
        else if(a[mid]<k)
        {
            l=mid;
        }
        else
        {
            r=mid-1;
        }
    }

    cout << -1 << endl;

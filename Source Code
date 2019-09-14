class Solution {
public:
    bool carPooling(vector<vector<int>>& trips, int capacity) {
        vector v(1001,0);int max1=0;
        for(int i=0;i<trips.size();i++)
        {
        v[trips[i][1]]+=trips[i][0];
        v[trips[i][2]]-=trips[i][0];
        max1=max(max1,trips[i][2]);
        }
        for(int i=2;i<max1;i++)
        {
        v[i]=v[i]+v[i-1];
        if(v[i]>capacity)
        return false;
        }
        return true;
            }
};

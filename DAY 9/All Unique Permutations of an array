class Solution {
  public:
    vector<vector<int>> uniquePerms(vector<int> &arr ,int n) {
        set<vector<int>>s1;
        vector<int>temp;
        sort(arr.begin(), arr.end());
        for(int i = 0; i < arr.size(); i++) temp.push_back(arr[i]);
        s1.insert(temp);
        string str = "";
        for(int i = 0; i < arr.size(); i++) str.push_back((char)arr[i]);
        string s = str;
        while(next_permutation(begin(str), end(str))) {
            if(s == str)    break;
            vector<int>a;
            for(int i = 0; i < str.length(); i++)
                a.push_back((int)str[i]);
            s1.insert(a);
        }
        vector<vector<int>>ans;
        for(auto it : s1)    ans.push_back(it);
        return ans;
    }
};

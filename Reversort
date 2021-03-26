#include<bits/stdc++.h>
using namespace std;
int reversort(vector<int> &arr){
    int cost = 0;
    for(int i=0; i<arr.size()-1; i++){
        int j = std::min_element(arr.begin()+i,arr.end()) - arr.begin();
        reverse(arr.begin()+i, arr.begin()+j+1);
        cost += j-i+1;
    }
    return cost;
}
int main(){
    int t; cin >> t;
    for(int c=0; c<t; c++){
        int n; cin >> n;
        vector<int> arr = vector<int>();
        for(int i=0; i<n; i++){
            int ai; cin >> ai;
            arr.push_back(ai);
        }
        cout << "Case #" << c+1 << ": " << reversort(arr) << endl;
    }
    return 0;
}

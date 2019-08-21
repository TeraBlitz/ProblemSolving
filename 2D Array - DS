/*
https://www.hackerrank.com/challenges/2d-array/problem?h_l=interview&playlist_slugs%5B%5D=interview-preparation-kit&playlist_slugs%5B%5D=arrays
*/


#include <bits/stdc++.h>

using namespace std;
///
/// My code
/// 
// Complete the hourglassSum function below.
int hourglassSum(vector<vector<int>> arr) 
{
    int resulTemp;
    int maxRes=-(9*7);

    for(int heigth=0;heigth<4;heigth++)
    {
        for(int width=0;width<4;width++)
        {
            resulTemp=
            arr[heigth][width]+arr[heigth][width+1]+arr[heigth][width+2]+
            arr[heigth+1][width+1]+
            arr[heigth+2][width]+arr[heigth+2][width+1]+arr[heigth+2][width+2];
            (resulTemp>maxRes)?(maxRes=resulTemp):(maxRes=maxRes);
        }
    }
    return maxRes;

}
///
///End of my code
///

int main()
{
    ofstream fout(getenv("OUTPUT_PATH"));

    vector<vector<int>> arr(6);
    for (int i = 0; i < 6; i++) {
        arr[i].resize(6);

        for (int j = 0; j < 6; j++) {
            cin >> arr[i][j];
        }

        cin.ignore(numeric_limits<streamsize>::max(), '\n');
    }

    int result = hourglassSum(arr);

    fout << result << "\n";

    fout.close();

    return 0;
}

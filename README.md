# 18CSC202J_OODP_CT1-446
##Input and Output
```
#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;


int main() {
    int a,b,c;
    std::cin>> a>>b>>c;
    std::cout << a+b+c;
    return 0;
}
```

##Variable Sized Arrays
```
#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;


int main() {
    int n, q;
    cin >> n >> q;

    vector<vector<int>> a(n);

    for (int i = 0; i < n; i++) {
        int k;
        cin >> k;
        a[i].resize(k);
        for (int j = 0; j < k; j++) {
            cin >> a[i][j];
        }
    }

    for (int q_num = 0; q_num < q; q_num++) {
        int i, j;
        cin >> i >> j;
        cout << a[i][j] << endl;
    }

    return 0;
}
```

##Functions
```
#include <iostream>
#include <cstdio>
using namespace std;

int max_of_four(int num1, int num2, int num3, int num4)
{
    int a;
    if(num1>num2 && num1>num3 && num1>num4){

  a=num1;

}

else if(num2>num3 && num2>num4){

a=num2;

}

else if(num3>num4){

a=num3;

}

else{

a=num4;

}
    return a;
}

int main() {
    
    int a, b, c, d;
    scanf("%d %d %d %d", &a, &b, &c, &d);
    int ans = max_of_four(a, b, c, d);
    printf("%d", ans);
    
    return 0;
}
```

##For Loop
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>



int main() 
{
      int a=0,b=0,n=0;
    scanf("%d",&a);
    scanf("%d",&b);

    for(n = a;n<=b;n++)
    {
       if(n == 1) {

        printf("one\n");

    }

    else if(n == 2) {

        printf("two\n");

    }

    else if(n == 3) {

        printf("three\n");

    }

    else if(n == 4) {

        printf("four\n");

    }

    else if(n == 5) {

        printf("five\n");

    }

    else if(n == 6) {

        printf("six\n");

    }

    else if(n == 7) {

        printf("seven\n");

    }

    else if(n == 8) {

        printf("eight\n");

    }

    else if(n == 9) {

        printf("nine\n");

    }

    else {

        if(n %2 ==0)
            printf("even\n");
        else
           printf("odd\n");

    }
    }
}
```







![[Pasted image 20250813115034.png]]
![[Pasted image 20250813115312.png]]
![[Pasted image 20250813115507.png]]
![[Pasted image 20250813115628.png]]
![[Pasted image 20250813115824.png]]
![[Pasted image 20250813120021.png]]
![[Pasted image 20250813120144.png]]
![[Pasted image 20250813120654.png]]
![[Pasted image 20250813120923.png]]
![[Pasted image 20250813143932.png]]
![[Pasted image 20250813144614.png]]
![[Pasted image 20250813145037.png]]
![[Pasted image 20250813145657.png]]
![[Pasted image 20250813150028.png]]
![[Pasted image 20250813152615.png]]
![[Pasted image 20250813154036.png]]
![[Pasted image 20250813162642.png]]
![[Pasted image 20250816094652.png]]
![[Pasted image 20250816095032.png]]
![[Pasted image 20250816100439.png]]
![[Pasted image 20250816100343.png]]
![[Pasted image 20250816100440.png]]
![[Pasted image 20250816100528.png]]
![[Pasted image 20250816100636.png]]
![[Pasted image 20250816101244.png]]
![[Pasted image 20250816101434.png]]
![[Pasted image 20250816105315.png]]
![[Pasted image 20250816105500.png]]
![[Pasted image 20250816105950.png]]
![[Pasted image 20250816110345.png]]
![[Pasted image 20250816110730.png]]
![[Pasted image 20250816112021.png]]
![[Pasted image 20250816113046.png]]
![[Pasted image 20250816113915.png]]
### Fixed Code:

```c++
#include <iostream>
using namespace std;
int gcd(int a, int b) {
	while (b != 0) {
		int temp = b;
        b = a % b;         
        a = temp;     
    }     
return a;
}  
long long lcm(int a, int b) {
	if (a == 0 || b == 0) return 0;   // handle zero case     
		return (1LL * a * b) / gcd(a, b); // use long long to avoid overflow }  
int main() {
	int x, y;     
	cin >> x >> y;     
	cout << lcm(x, y) << endl;     
	return 0; 
}
```
![[Pasted image 20250816115654.png]]

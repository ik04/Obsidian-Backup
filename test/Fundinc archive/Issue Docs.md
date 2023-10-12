## Import Csv Error in portfolio:
![[Pasted image 20231009100113.png]]

## Dealflow delete (bad code):
- it dosen't get rid of the recently deleted in the array 
- this is causing issues with the statistics cards
## Fix:
- just modified the function to parse only recently deleted not true ones in statistics cards

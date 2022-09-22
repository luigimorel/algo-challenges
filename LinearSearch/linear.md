Linear Search is defined as a sequential search algorithm that starts at one end and goes through each element of a list until the desired element is found, otherwise the search continues till the end of the data set. It is the easiest searching algorithm

```js
function search(arr, n, x) {
  for (let i = 0; i < n; i++) if (arr[i] == x) return i;

  return -1;
}

let arr = [1, 2, 3, 4, 5, 6];
let n = arr.length;
let x = 5;

const result = search(arr, n, x);
console.log(result);
```

````java
package LinearSearch;

class GFG {
    public static int search(int arr[], int x) {
        int N = arr.length;
        for (int i = 0; i < N; i++) {
            if (arr[i] == x)
                return i;
        }
        return -1;
    }

    // Driver's code
    public static void main(String args[]) {
        int arr[] = { 2, 3, 4, 10, 40 };
        int x = 10;

        // Function call
        int result = search(arr, x);
        if (result == -1)
            System.out.print(
                    "Element is not present in array");
        else
            System.out.print("Element is present at index "
                    + result);
    }
}```
````

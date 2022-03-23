Example taken from <https://developerinsider.co/big-o-notation-explained-with-examples/>

# O[1]

* Definition
    - constant time
    - only require one step

* Code
    void printFirstElementOfArray(int arr[]) {

        printf("First element of array = %d",arr[0]);

    }

# O[n]

* Definition
    - linear time
    - n is the number of items in array ( proportional )

* Code

    void printAllElementOfArray(int arr[], int size) {
        
        for (int i = 0; i < size; i++) {

            printf("%d\n", arr[i]);

        }

    }

# O[n^2]

* Definition
    - nested two loops, quadratic time
    - grow faster and faster
    - not sclable

* Code 

    void printAllPossibleOrderedPairs(int arr[], int size) {

        for (int i = 0; i < size; i++) {

            for (int j = 0; j < size; j++) {

                printf("%d = %d\n", arr[i], arr[j]);

            }

        }

    }


# O[2^n]

* Definition
    - recursive calculation
    - denotes an algorithm whose growth doubles with each addition to the input data set

* Code 

    int fibonacci(int num) {

        if (num <= 1) return num;
        
        return fibonacci(num - 2) + fibonacci(num - 1);
    }

# std::vector: 

* Complexity

    Random access O[1]

    Insert or removal of element at the end O[1]

    Insert or removal of element somewhere O[n]

# forward_list (SLL)

* Complexity

    Random access O[n]

    Insert or removal of element at front or end O[1]

    Insert or removal of element somewhere O[1] is the iterator is given or O[n] is traversing the list is require

# list (DLL)

* Complexity

    Random access O[n]

    Insert or removal of element at front or end O[1]

    Insert or removal of element somewhere O[1] is the iterator is given or O[n] is traversing the list is require




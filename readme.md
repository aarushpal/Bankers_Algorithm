# Author Details

- **Aarush Pal**
- **Aditya Goyal**
- **Arnav Kumar**
- **Course** : Operating Systems | University 5th semester project
- **Organization** : Manipal Institute of Technology, Manipal

# Bankers Algorithm

The banker’s algorithm is a resource allocation and deadlock avoidance algorithm that tests for safety by simulating the allocation for predetermined maximum possible amounts of all resources, then makes an “s-state” check to test for possible activities, before deciding whether allocation should be allowed to continue.

So in our project we are using this same algorithm to check that if our system is in a deadlock or a safe state.

Let ‘n’ be the number of processes in the system and ‘m’ be the number of resources types. We have arrays for Available, Max need , Allocation and Need.

Available Matrix:

- It is a 1-d array of size ‘m’ indicating the number of available resources of each type.
- Available[ j ] = k means there are ‘k’ instances of resource type Rj

Max need Matrix:

- It is a 2-d array of size ‘n\*m’ that defines the maximum demand of each process in a system.
- Max[ i, j ] = k means process Pi may request at most ‘k’ instances of resource type Rj.

Allocation Matrix:

- It is a 2-d array of size ‘n\*m’ that defines the number of resources of each type currently allocated to each process.
- Allocation[ i, j ] = k means process Pi is currently allocated ‘k’ instances of resource type Rj

Remaining Need Matrix:

- It is a 2-d array of size ‘n\*m’ that indicates the remaining resource need of each process.
- Need [ i, j ] = k means process Pi currently need ‘k’ instances of resource type Rj
- Need [ i, j ] = Max [ i, j ] – Allocation [ i, j ]
  Allocation specifies the resources currently allocated to process Pi and Needi specifies the additional resources that process Pi may still request to complete its task.

Banker’s algorithm consists of Safety algorithm and Resource request algorithm.

~ Thank you!

## Contributors

https://github.com/aarushpal

https://github.com/eddyhacks

https://github.com/Arnav10-coder

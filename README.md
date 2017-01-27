# CMU-18645-How-To-Write-Fast-Code

This is the course taught by Prof.Jike Chong and Prof. Ian Lane from CMU 
### Course content
- Multicore platforms 
  - OpenMP
  - SIMD
- Manycore platforms
  - CUDA
- Cloud platforms
  - Hadoop
  - Spark
  - AWS

### Projects
- Multicore Optimization for Matrix-to-Matrix Multiplication and K-means Clustering
  - Cache blocking
  - OpenMP pragma-based optimizations
  - Intrinsics Programming
- Manycore Optimization for Matrix-to-Matrix Multiplication and K-means Clustering
  - For Matrix-to-Matrix Multiplication, achieve 150 GFLOPS
  - For K-means Clustering, achieve 1.5x speedup
- Cloud Computing Framework 
  - NGramCount
  - HashtagSim


### Term project
Use Hadoop and Spark to implement a movie recommendation model with 10M stable benchmark rating dataset  
Data from [MovieLens](http://grouplens.org/datasets/movielens/)

#### 1. Local Machine
[use python](http://blog.csdn.net/ygrx/article/details/15501679)

how to run: 
> python userFC.py ../../ml-100k/u.data ../../ml-100k/u.item

The above method use cos distance to calculate similarity and use user-based model, but in order to compared with the distributed version that use concurrency matrix as similarity and item-based model, we rewrite the version as itemCF.py.
To run it:
> python itemCF.py ./ml-100k/u.data ./ml-100k/u.item ./ml-100k/u.user

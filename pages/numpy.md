- ```
  a = np.array([1., 2., 3.])
  b = np.array([4., 5., 6.])
  
  a.dot(b)
  
  lst = [[1, 2, 3], 
         [4, 5, 6]]
  ary2d = np.array(lst)
  ary2d.dtype
  
  int32_ary = ary2d.astype(np.int32)
  
  np.ones((3, 4), dtype=np.int)
  
  np.arange(4, 10)
  array([4, 5, 6, 7, 8, 9])
  
  np.arange(4, 10)
  array([4, 5, 6, 7, 8, 9])
  
  np.linspace(6., 15., num=10)
  array([ 6.,  7.,  8.,  9., 10., 11., 12., 13., 14., 15.])
  
  ary = np.array([[1, 2, 3],
                  [4, 5, 6]])
  ary[0, -2] # first row, second from last element
  ary[:, 0] # entire first column
  ary[:, :2] # first two columns
  
  np.add(ary, 1)
  
  ary = np.array([[1, 2, 3], 
                  [4, 5, 6]]) # rolling over the 1st axis, axis 0
  
  np.add.reduce(ary, axis=0)
  ary.sum(axis=0) # column sums
  array([5, 7, 9])
  
  np.add.reduce(ary, axis=1) # row sums
  ary.sum(axis=1) # row sums
  array([ 6, 15])
  
  np.mean (computes arithmetic mean or average)
  np.std (computes the standard deviation)
  np.var (computes variance)
  np.sort (sorts an array)
  np.argsort (returns indices that would sort an array)
  np.min (returns the minimum value of an array)
  np.max (returns the maximum value of an array)
  np.argmin (returns the index of the minimum value)
  np.argmax (returns the index of the maximum value)
  np.array_equal (checks if two arrays have the same shape and elements)
  
  
  ary = np.array([[1, 2, 3],
                  [4, 5, 6]])
  ary[:, [0, 2]] # first and and last column
  array([[1, 3],
         [4, 6]])
  
  (ary > 3) & (ary % 2 == 0)
  array([[False, False, False],
         [ True, False,  True]])
         
  np.random.rand(3)
  
  ary1d = np.array([1, 2, 3, 4, 5, 6])
  ary2d_view = ary1d.reshape(2, 3)
  ary2d_view
  
  ary1d.reshape(-1, 2)
  array([[1, 2],
         [3, 4],
         [5, 6]])
         
  ary1d = np.array([1, 2, 3, 4, 5, 6])
  ary2d_view = ary1d.reshape(2, 3)
  ary2d_view
  array([[1, 2, 3],
         [4, 5, 6]])
         
  ary1d.reshape(-1, 2)
  array([[1, 2],
         [3, 4],
         [5, 6]])
         
  ary = np.array([[[1, 2, 3],
                   [4, 5, 6]]])
  ary.reshape(-1)
  array([1, 2, 3, 4, 5, 6])
  
  ary = np.array([1, 2, 3])
  # stack along the first axis
  np.concatenate((ary, ary))
  array([1, 2, 3, 1, 2, 3])
  
  ary = np.array([[1, 2, 3]])
  # stack along the first axis (here: rows)
  np.concatenate((ary, ary), axis=0)
  array([[1, 2, 3],
         [1, 2, 3]])
  
  ary = np.array([1, 2, 3, 4, 5])
  mask = ary > 2
  mask
  
  ary[mask]
  array([3, 4, 5])
  
  row_vector = np.array([1, 2, 3])
  column_vector = np.array([1, 2, 3]).reshape(-1, 1)
  row_vector[:, np.newaxis]
  row_vector[:, None]
  
  matrix = np.array([[1, 2, 3], 
                     [4, 5, 6]])
                     
  ```
-
-
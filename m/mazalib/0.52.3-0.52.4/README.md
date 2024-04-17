# Comparing `tmp/mazalib-0.52.3.tar.gz` & `tmp/mazalib-0.52.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazalib-0.52.3.tar", last modified: Thu Mar 28 14:40:52 2024, max compression
+gzip compressed data, was "mazalib-0.52.4.tar", last modified: Wed Apr 17 15:14:08 2024, max compression
```

## Comparing `mazalib-0.52.3.tar` & `mazalib-0.52.4.tar`

### file list

```diff
@@ -1,1942 +1,1942 @@
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:52.089840 mazalib-0.52.3/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35821 2023-10-30 16:40:18.000000 mazalib-0.52.3/LICENSE.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1449 2024-03-28 14:40:52.089581 mazalib-0.52.3/PKG-INFO
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      800 2023-11-06 10:05:41.000000 mazalib-0.52.3/README.md
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2024-03-28 14:40:52.089937 mazalib-0.52.3/setup.cfg
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3261 2024-03-28 14:34:56.000000 mazalib-0.52.3/setup.py
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.054773 mazalib-0.52.3/src/
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.086958 mazalib-0.52.3/src/eigen3/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      185 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/.hg_archival.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      191 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/.hgeol
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      319 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/.hgignore
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1544 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/.hgtags
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26000 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1541 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/COPYING.BSD
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35821 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/COPYING.GPL
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    27032 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/COPYING.LGPL
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2246 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/COPYING.MINPACK
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17099 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/COPYING.MPL2
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      797 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/COPYING.README
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      601 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/CTestConfig.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      184 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/CTestCustom.cmake.in
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.112812 mazalib-0.52.3/src/eigen3/Eigen/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      713 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1252 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/Cholesky
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1948 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/CholmodSupport
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12243 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/Core
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      129 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/Dense.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       37 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/Eigen
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1883 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/Eigenvalues
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2008 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/Geometry
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      904 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/Householder
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2131 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/IterativeLinearSolvers
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      972 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/Jacobi
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1430 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/KLUSupport
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1483 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/LU
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1026 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/MetisSupport
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2521 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/OrderingMethods
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1800 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/PaStiXSupport
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1151 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/PardisoSupport
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1368 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/QR
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      985 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/QtAlignedMalloc
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1196 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/SPQRSupport
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1680 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/SVD
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      922 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/Sparse
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1272 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/SparseCholesky
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2309 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/SparseCore
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1864 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/SparseLU
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1231 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/SparseQR
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      824 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/StdDeque
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      752 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/StdList
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      830 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/StdVector
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2307 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/SuperLUSupport
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1422 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/UmfPackSupport
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.034147 mazalib-0.52.3/src/eigen3/Eigen/src/
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.116039 mazalib-0.52.3/src/eigen3/Eigen/src/Cholesky/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    25525 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Cholesky/LDLT.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19241 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Cholesky/LLT.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4073 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.117021 mazalib-0.52.3/src/eigen3/Eigen/src/CholmodSupport/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26123 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.202503 mazalib-0.52.3/src/eigen3/Eigen/src/Core/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19627 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/ArithmeticSequence.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17128 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Array.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8385 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/ArrayBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6984 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/ArrayWrapper.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2828 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Assign.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    41301 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/AssignEvaluator.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12666 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Assign_MKL.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14263 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/BandMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18852 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Block.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4463 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/BooleanRedux.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5885 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/CommaInitializer.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7165 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/ConditionEstimator.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    65712 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/CoreEvaluators.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4877 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/CoreIterators.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8131 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/CwiseBinaryOp.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    33932 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/CwiseNullaryOp.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8453 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/CwiseTernaryOp.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3980 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/CwiseUnaryOp.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5389 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/CwiseUnaryView.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    30534 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/DenseBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24905 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/DenseCoeffsBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22985 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/DenseStorage.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9967 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Diagonal.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15061 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/DiagonalMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1016 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/DiagonalProduct.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11969 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Dot.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5911 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/EigenBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4915 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/ForceAlignedAccess.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5914 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Fuzzy.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22314 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/GeneralProduct.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29503 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/GenericPacketMath.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11454 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/GlobalFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7673 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/IO.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8528 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/IndexedView.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3566 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Inverse.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7398 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Map.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11294 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/MapBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    54438 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/MathFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3199 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/MathFunctionsImpl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24843 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Matrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24339 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/MatrixBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2543 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/NestByValue.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3729 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/NoAlias.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10626 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/NumTraits.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9429 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/PartialReduxEvaluator.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21353 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/PermutationMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    49641 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/PlainObjectBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7524 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Product.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    54433 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/ProductEvaluators.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6579 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Random.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19176 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Redux.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13346 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Ref.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5773 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Replicate.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17453 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Reshaped.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4335 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/ReturnByValue.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7672 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Reverse.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6182 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Select.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15238 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/SelfAdjointView.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1744 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6985 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Solve.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9461 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/SolveTriangular.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6338 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/SolverBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9165 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/StableNorm.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14871 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/StlIterators.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3976 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Stride.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2833 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Swap.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15681 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Transpose.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13459 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Transpositions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    39038 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/TriangularMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3584 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/VectorBlock.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    34308 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/VectorwiseOp.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9613 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/Visitor.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.027010 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.210833 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19643 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX/Complex.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6061 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    49706 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2133 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.217841 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX512/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20075 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX512/Complex.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17800 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    73803 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1132 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.222405 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AltiVec/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17889 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2413 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    44416 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.224187 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/CUDA/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4347 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/CUDA/Complex.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.232727 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2018 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24629 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2255 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    27369 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/Half.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1795 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/Settings.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2564 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.237354 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/GPU/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2798 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    33043 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1498 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.025526 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/HIP/
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.238994 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/HIP/hcc/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      714 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.244039 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/MSA/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21729 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/MSA/Complex.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16546 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    38368 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.250373 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/NEON/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19549 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/NEON/Complex.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1348 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    32019 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1394 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.256083 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SSE/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20968 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SSE/Complex.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6494 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    51849 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3534 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.263624 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SYCL/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7019 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11685 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23733 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22550 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2711 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.268093 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/ZVector/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21077 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/ZVector/Complex.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8469 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    41889 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.275743 mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6863 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18792 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/BinaryFunctors.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8209 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/NullaryFunctors.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4536 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/StlFunctors.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      632 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/TernaryFunctors.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35610 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/UnaryFunctors.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.304146 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   115557 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20629 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16265 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7081 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5230 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22242 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6504 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5740 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/Parallelizer.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21898 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11865 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10220 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5327 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6313 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/SelfadjointProduct.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4198 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21459 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14184 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15072 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10826 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14947 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6874 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6030 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularSolverVector.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.326113 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19661 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/BlasUtil.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19139 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/ConfigureVectorization.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22362 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/Constants.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4887 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15599 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/ForwardDeclarations.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6711 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/IndexedViewHelper.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11167 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/IntegralConstant.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4405 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/MKL_support.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    46645 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/Macros.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    46766 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/Memory.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    25516 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/Meta.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       88 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/NonMPL2.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1055 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1483 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/ReshapedHelper.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10863 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/StaticAssert.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12280 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/SymbolicIndex.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    36539 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/XprHelper.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.344765 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12905 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17736 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4269 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23592 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/EigenSolver.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17594 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9942 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14713 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5733 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24297 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/RealQZ.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21636 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/RealSchur.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3727 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    34828 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4191 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23099 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.364032 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15232 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/AlignedBox.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8670 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/AngleAxis.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3753 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/EulerAngles.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21036 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Homogeneous.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12244 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Hyperplane.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9190 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/OrthoMethods.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10049 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/ParametrizedLine.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    33830 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Quaternion.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7076 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Rotation2D.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8269 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/RotationBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6905 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Scaling.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    63424 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Transform.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7981 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Translation.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6356 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Umeyama.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.365425 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/arch/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5993 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.369340 mazalib-0.52.3/src/eigen3/Eigen/src/Householder/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4894 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Householder/BlockHouseholder.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5541 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Householder/Householder.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24114 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Householder/HouseholderSequence.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.380049 mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6981 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7062 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9104 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15442 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15415 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13793 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7547 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4273 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.381322 mazalib-0.52.3/src/eigen3/Eigen/src/Jacobi/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16856 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/Jacobi/Jacobi.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.382719 mazalib-0.52.3/src/eigen3/Eigen/src/KLUSupport/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11892 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/KLUSupport/KLUSupport.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.389568 mazalib-0.52.3/src/eigen3/Eigen/src/LU/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3556 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/LU/Determinant.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    33188 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/LU/FullPivLU.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15519 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/LU/InverseImpl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22475 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/LU/PartialPivLU.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3638 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.390938 mazalib-0.52.3/src/eigen3/Eigen/src/LU/arch/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14000 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/LU/arch/Inverse_SSE.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.392462 mazalib-0.52.3/src/eigen3/Eigen/src/MetisSupport/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4725 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/MetisSupport/MetisSupport.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.396936 mazalib-0.52.3/src/eigen3/Eigen/src/OrderingMethods/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16540 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/OrderingMethods/Amd.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    63544 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5401 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/OrderingMethods/Ordering.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.398253 mazalib-0.52.3/src/eigen3/Eigen/src/PaStiXSupport/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22927 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.399686 mazalib-0.52.3/src/eigen3/Eigen/src/PardisoSupport/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20637 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.408399 mazalib-0.52.3/src/eigen3/Eigen/src/QR/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26172 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/QR/ColPivHouseholderQR.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4759 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24064 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    27481 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/QR/FullPivHouseholderQR.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15075 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/QR/HouseholderQR.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3061 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.409703 mazalib-0.52.3/src/eigen3/Eigen/src/SPQRSupport/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12161 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.416628 mazalib-0.52.3/src/eigen3/Eigen/src/SVD/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    55030 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SVD/BDCSVD.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    33798 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SVD/JacobiSVD.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5190 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14620 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SVD/SVDBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16371 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SVD/UpperBidiagonalization.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.419397 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCholesky/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24881 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6004 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.460205 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10914 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/AmbiVector.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9017 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/CompressedStorage.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13530 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2258 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11638 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseAssign.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24341 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseBlock.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6691 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseColEtree.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13976 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26156 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4887 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13598 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5946 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3178 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseDot.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1136 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseFuzzy.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12894 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseMap.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    58689 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17849 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7507 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparsePermutation.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7219 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseProduct.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1748 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseRedux.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15889 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseRef.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26371 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4548 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseSolverBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8902 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3267 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseTranspose.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6626 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseTriangularView.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7013 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseUtil.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15310 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseVector.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8381 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseView.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9972 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/TriangularSolver.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.482122 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    28727 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4369 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLUImpl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7828 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5084 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10335 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2129 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6893 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6763 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3788 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10497 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4307 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5853 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8708 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9286 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5116 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4681 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2972 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.483356 mazalib-0.52.3/src/eigen3/Eigen/src/SparseQR/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29925 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SparseQR/SparseQR.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.488706 mazalib-0.52.3/src/eigen3/Eigen/src/StlSupport/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5251 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/StlSupport/StdDeque.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4261 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/StlSupport/StdList.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5469 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/StlSupport/StdVector.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2893 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/StlSupport/details.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.489990 mazalib-0.52.3/src/eigen3/Eigen/src/SuperLUSupport/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35373 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.491516 mazalib-0.52.3/src/eigen3/Eigen/src/UmfPackSupport/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    25098 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.509300 mazalib-0.52.3/src/eigen3/Eigen/src/misc/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2995 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/misc/Image.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2821 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/misc/Kernel.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1803 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/misc/RealSvd2x2.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    31000 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/misc/blas.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7986 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/misc/lapack.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)  1074661 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/misc/lapacke.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      491 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/misc/lapacke_mangling.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.521579 mazalib-0.52.3/src/eigen3/Eigen/src/plugins/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13464 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20266 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    60448 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/plugins/BlockMethods.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4943 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6266 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12545 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/plugins/IndexedViewMethods.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6527 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3022 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7064 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/Eigen/src/plugins/ReshapedMethods.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1180 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/INSTALL
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      371 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/README.md
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/__init__.py
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.570995 mazalib-0.52.3/src/eigen3/bench/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4081 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/BenchSparseUtil.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4685 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/BenchTimer.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2621 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/BenchUtil.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2063 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/README.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29859 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/analyze-blocking-sizes.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1449 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/basicbench.cxxlist
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1142 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/basicbenchmark.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1732 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/basicbenchmark.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6532 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/benchBlasGemm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3676 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/benchCholesky.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6000 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/benchEigenSolver.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2921 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/benchFFT.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3732 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/benchGeometry.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5328 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/benchVecAdd.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11810 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/bench_gemm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      646 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/bench_multi_compilers.sh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12013 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/bench_norm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2243 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/bench_reverse.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      338 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/bench_sum.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      663 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/bench_unrolling
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22936 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/benchmark-blocking-sizes.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      829 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/benchmark.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      873 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/benchmarkSlice.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      676 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/benchmarkX.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      640 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/benchmarkXcwise.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1227 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/benchmark_suite
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.574991 mazalib-0.52.3/src/eigen3/bench/btl/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2976 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18449 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/COPYING
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6601 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/README
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.599078 mazalib-0.52.3/src/eigen3/bench/btl/actions/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3519 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_aat_product.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3499 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_ata_product.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3804 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_atv_product.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3498 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_axpby.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3479 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_axpy.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3330 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_cholesky.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3588 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_ger.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5831 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_hessenberg.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3275 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_lu_decomp.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3734 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_lu_solve.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4036 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_matrix_matrix_product.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4134 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_matrix_matrix_product_bis.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4142 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_matrix_vector_product.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3313 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_partial_lu.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3135 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_rot.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3830 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_symv.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3797 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_syr2.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3562 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_trisolve.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4226 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_trisolve_matrix.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4072 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/action_trmm.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      485 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/actions/basic_actions.hh
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.612450 mazalib-0.52.3/src/eigen3/bench/btl/cmake/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      983 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindACML.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1396 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindATLAS.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      846 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindBLAZE.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1132 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindBlitz.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      703 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindCBLAS.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      383 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindGMM.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1435 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindMKL.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      850 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindMTL4.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      639 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindOPENBLAS.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2432 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindPackageHandleStandardArgs.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      864 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindTvmet.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1346 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.626082 mazalib-0.52.3/src/eigen3/bench/btl/data/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      901 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/data/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1387 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/data/action_settings.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2311 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/data/gnuplot_common_settings.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2122 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/data/go_mean
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5488 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/data/mean.cxx
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1918 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/data/mk_gnuplot_script.sh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      981 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/data/mk_mean_script.sh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1796 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/data/mk_new_gnuplot.sh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      990 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/data/perlib_plot_settings.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3556 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/data/regularize.cxx
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5310 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/data/smooth.cxx
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1755 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/data/smooth_all.sh
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.630016 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4995 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/bench.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1969 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/bench_parameter.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6990 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/btl.hh
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.634054 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/init/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1532 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/init/init_function.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2359 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/init/init_matrix.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1453 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/init/init_vector.hh
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.638505 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/static/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2358 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/static/bench_static.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2014 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/static/intel_bench_fixed_size.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2279 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/static/static_size_generator.hh
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.650090 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2387 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/STL_perf_analyzer.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2600 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/STL_timer.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2067 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3041 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/portable_perf_analyzer.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3668 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3721 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/portable_timer.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3035 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/x86_perf_analyzer.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5540 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/x86_timer.hh
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.655511 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/utils/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1728 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/utils/size_lin_log.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1700 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/utils/size_log.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2835 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/utils/utilities.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2289 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/utils/xy_file.hh
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.040125 mazalib-0.52.3/src/eigen3/bench/btl/libs/
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.664514 mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1619 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35833 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/blas.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2974 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/blas_interface.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4958 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/blas_interface_impl.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1707 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/c_interface_base.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3033 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/main.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.668969 mazalib-0.52.3/src/eigen3/bench/btl/libs/STL/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       39 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/STL/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6046 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/STL/STL_interface.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1870 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/STL/main.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.673102 mazalib-0.52.3/src/eigen3/bench/btl/libs/blaze/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      488 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/blaze/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4263 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/blaze/blaze_interface.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1676 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/blaze/main.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.680088 mazalib-0.52.3/src/eigen3/bench/btl/libs/blitz/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      441 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/blitz/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5556 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/blitz/blitz_LU_solve_interface.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4276 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/blitz/blitz_interface.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2013 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/blitz/btl_blitz.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1431 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/blitz/btl_tiny_blitz.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3206 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/blitz/tiny_blitz_interface.hh
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.690149 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      787 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1710 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5319 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/eigen2_interface.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1843 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/main_adv.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1239 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/main_linear.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1419 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/main_matmat.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1492 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/main_vecmat.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.700627 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3357 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1710 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8429 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/eigen3_interface.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1843 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/main_adv.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1320 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/main_linear.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1413 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/main_matmat.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1483 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/main_vecmat.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.706498 mazalib-0.52.3/src/eigen3/bench/btl/libs/gmm/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      131 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/gmm/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5556 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/gmm/gmm_LU_solve_interface.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4318 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/gmm/gmm_interface.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2164 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/gmm/main.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.713787 mazalib-0.52.3/src/eigen3/bench/btl/libs/mtl4/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      165 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/mtl4/.kdbgrc.main
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      139 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/mtl4/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1989 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/mtl4/main.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5556 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4354 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/mtl4/mtl4_interface.hh
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.721192 mazalib-0.52.3/src/eigen3/bench/btl/libs/tensors/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2199 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/tensors/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      694 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/tensors/main_linear.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      645 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/tensors/main_matmat.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      645 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/tensors/main_vecmat.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3295 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/tensors/tensor_interface.hh
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.725246 mazalib-0.52.3/src/eigen3/bench/btl/libs/tvmet/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      148 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/tvmet/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1500 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/tvmet/main.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3121 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/tvmet/tvmet_interface.hh
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.729063 mazalib-0.52.3/src/eigen3/bench/btl/libs/ublas/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      187 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/ublas/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1829 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/ublas/main.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4482 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/btl/libs/ublas/ublas_interface.hh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3370 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/check_cache_queries.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6602 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/dense_solvers.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7438 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/eig33.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3433 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/geometry.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.750512 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6962 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/changesets.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      205 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/gemm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1449 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/gemm_common.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      184 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/gemm_settings.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      125 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/gemm_square_settings.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      205 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/gemv.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1450 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/gemv_common.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       90 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/gemv_settings.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      101 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/gemv_square_settings.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      217 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/gemvt.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2567 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/lazy_gemm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      147 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/lazy_gemm_settings.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      313 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/llt.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2805 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/make_plot.sh
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.759534 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/resources/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3852 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/resources/chart_footer.html
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14824 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/resources/chart_header.html
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       28 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/resources/footer.html
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      926 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/resources/header.html
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   151724 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/resources/s1.js
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   241320 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/resources/s2.js
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4261 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/run.sh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2103 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/runall.sh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      229 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/trmv_lo.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      241 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/trmv_lot.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      229 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/trmv_up.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      241 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/perf_monitoring/trmv_upt.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3375 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/product_threshold.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6253 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/quat_slerp.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1144 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/quatmul.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6476 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/sparse_cholesky.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5288 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/sparse_dense_product.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3143 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/sparse_lu.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9322 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/sparse_product.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3483 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/sparse_randomsetter.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14246 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/sparse_setter.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2451 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/sparse_transpose.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6334 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/sparse_trisolver.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.768467 mazalib-0.52.3/src/eigen3/bench/spbench/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3024 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/spbench/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4098 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/spbench/sp_solver.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1886 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/spbench/spbench.dtd
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3388 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/spbench/spbenchsolver.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18271 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/spbench/spbenchsolver.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3920 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/spbench/spbenchstyle.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2922 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/spbench/test_sparseLU.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6329 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/spmv.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.778698 mazalib-0.52.3/src/eigen3/bench/tensors/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2498 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/tensors/README
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1634 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/tensors/benchmark.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7071 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/tensors/benchmark_main.cc
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1428 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/tensors/contraction_benchmarks_cpu.cc
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19792 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/tensors/tensor_benchmarks.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6432 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/tensors/tensor_benchmarks_cpu.cc
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3458 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/tensors/tensor_benchmarks_fp16_gpu.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3448 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/tensors/tensor_benchmarks_gpu.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3394 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/tensors/tensor_benchmarks_sycl.cc
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       78 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/tensors/tensor_benchmarks_sycl_include_headers.cc
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1259 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/bench/vdw_new.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.798045 mazalib-0.52.3/src/eigen3/blas/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3711 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/BandTriangularSolver.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1744 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1652 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/GeneralRank1Update.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2089 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/PackedSelfadjointProduct.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3244 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/PackedTriangularMatrixVector.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3279 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/PackedTriangularSolverVector.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      189 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/README.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2225 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/Rank2Update.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4847 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/common.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      667 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/complex_double.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      666 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/complex_single.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1539 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/double.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.819627 mazalib-0.52.3/src/eigen3/blas/f2c/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15595 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/chbmv.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13464 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/chpmv.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2394 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/complexdots.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19592 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/ctbmv.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      123 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/d_cnjg.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      681 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/datatypes.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5183 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/drotm.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6486 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/drotmg.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10554 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/dsbmv.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8391 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/dspmv.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12085 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/dtbmv.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3093 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/lsame.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      111 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/r_cnjg.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5118 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/srotm.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6351 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/srotmg.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10578 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/ssbmv.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8367 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/sspmv.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12071 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/stbmv.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15632 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/zhbmv.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13498 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/zhpmv.c
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19620 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/f2c/ztbmv.c
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.820704 mazalib-0.52.3/src/eigen3/blas/fortran/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1022 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/fortran/complexdots.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5801 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/level1_cplx_impl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4036 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/level1_impl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4389 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/level1_real_impl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12583 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/level2_cplx_impl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    25725 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/level2_impl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10805 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/level2_real_impl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    38745 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/level3_impl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      785 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/single.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.849311 mazalib-0.52.3/src/eigen3/blas/testing/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1004 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    32834 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/cblat1.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1581 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/cblat2.dat
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   119936 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/cblat2.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1069 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/cblat3.dat
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   135042 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/cblat3.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    45885 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/dblat1.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1500 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/dblat2.dat
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   115511 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/dblat2.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      902 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/dblat3.dat
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   107135 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/dblat3.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1061 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/runblastest.sh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    44410 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/sblat1.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1500 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/sblat2.dat
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   115427 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/sblat2.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      902 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/sblat3.dat
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   107045 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/sblat3.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    32839 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/zblat1.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1581 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/zblat2.dat
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   120290 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/zblat2.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1069 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/zblat3.dat
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   135497 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/testing/zblat3.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      412 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/blas/xerbla.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.880959 mazalib-0.52.3/src/eigen3/cmake/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      825 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/Eigen3Config.cmake.in
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1427 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/Eigen3ConfigLegacy.cmake.in
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2883 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/EigenConfigureTesting.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1608 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/EigenDetermineOSVersion.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1855 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/EigenDetermineVSServicePack.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    28473 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/EigenTesting.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1240 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/EigenUninstall.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      521 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindAdolc.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    45226 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindBLAS.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13411 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindBLASEXT.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2661 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindCholmod.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9993 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindComputeCpp.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2922 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindEigen2.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3950 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindEigen3.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2876 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindFFTW.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3048 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindGLEW.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      575 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindGMP.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5205 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindGSL.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      932 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindGoogleHash.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12188 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindHWLOC.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1386 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindKLU.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10182 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindLAPACK.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2928 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindMPFR.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9227 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindMetis.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14873 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindPTSCOTCH.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23911 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindPastix.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1228 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindSPQR.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12379 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindScotch.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2258 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindStandardMathLibrary.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2396 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindSuperLU.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4897 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindTriSYCL.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1788 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/FindUmfpack.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      954 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/RegexUtils.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      183 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/UseEigen3.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2480 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/cmake/language_support.cmake
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.043262 mazalib-0.52.3/src/eigen3/debug/
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.882682 mazalib-0.52.3/src/eigen3/debug/gdb/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       23 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/debug/gdb/__init__.py
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9931 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/debug/gdb/printers.py
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.884632 mazalib-0.52.3/src/eigen3/debug/msvc/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11661 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/debug/msvc/eigen.natvis
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7566 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/debug/msvc/eigen_autoexp_part.dat
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.885489 mazalib-0.52.3/src/eigen3/demos/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      309 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/CMakeLists.txt
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.888996 mazalib-0.52.3/src/eigen3/demos/mandelbrot/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      507 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/mandelbrot/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      346 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/mandelbrot/README
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7722 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/mandelbrot/mandelbrot.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1959 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/mandelbrot/mandelbrot.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.892817 mazalib-0.52.3/src/eigen3/demos/mix_eigen_and_c/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      269 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/mix_eigen_and_c/README
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4343 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/mix_eigen_and_c/binary_library.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3415 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/mix_eigen_and_c/binary_library.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1681 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/mix_eigen_and_c/example.c
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.903843 mazalib-0.52.3/src/eigen3/demos/opengl/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      722 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/opengl/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      416 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/opengl/README
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6245 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/opengl/camera.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3553 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/opengl/camera.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4100 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/opengl/gpuhelper.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7384 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/opengl/gpuhelper.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4047 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/opengl/icosphere.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      899 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/opengl/icosphere.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19848 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/opengl/quaternion_demo.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2749 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/opengl/quaternion_demo.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1815 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/opengl/trackball.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      985 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/demos/opengl/trackball.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.965866 mazalib-0.52.3/src/eigen3/doc/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11391 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/AsciiQuickReference.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2477 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/B01_Experimental.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4967 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6461 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/ClassHierarchy.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18408 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/CoeffwiseMathFunctionsTable.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4543 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/CustomizingEigen_CustomScalar.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1371 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/CustomizingEigen_InheritingMatrix.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3744 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/CustomizingEigen_NullaryExpr.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3727 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/CustomizingEigen_Plugins.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5064 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/DenseDecompositionBenchmark.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    87484 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/Doxyfile.in
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8355 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/Eigen_Silly_Professor_64x64.png
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1944 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/FixedSizeVectorizable.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13675 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/FunctionsTakingEigenTypes.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5557 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/HiPerformance.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3911 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/InplaceDecomposition.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    31085 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/InsideEigenExample.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2860 2023-10-30 16:40:18.000000 mazalib-0.52.3/src/eigen3/doc/LeastSquares.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6953 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/Manual.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      777 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/MatrixfreeSolverExample.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5753 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/NewExpressionType.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1957 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/Overview.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1206 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/PassingByValue.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6402 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/Pitfalls.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13858 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/PreprocessorDirectives.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    30486 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/QuickReference.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6678 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/QuickStartGuide.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20134 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/SparseLinearSystems.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8583 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/SparseQuickReference.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3996 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/StlContainers.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4205 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/StorageOrders.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7229 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/StructHavingEigenMembers.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6290 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TemplateKeyword.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10506 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TopicAliasing.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5393 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TopicAssertions.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1970 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TopicCMakeGuide.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      185 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TopicEigenExpressionTemplates.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6411 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TopicLazyEvaluation.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9080 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TopicLinearAlgebraDecompositions.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3681 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TopicMultithreading.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      148 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TopicResizing.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      157 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TopicScalarTypes.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      106 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TopicVectorization.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7062 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialAdvancedInitialization.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8715 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialArrayClass.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8051 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialBlockOperations.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9973 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialGeometry.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11494 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialLinearAlgebra.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4074 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialMapClass.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10079 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialMatrixArithmetic.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13973 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialMatrixClass.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12272 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialReductionsVisitorsBroadcasting.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3063 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialReshape.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2208 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialSTL.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8453 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialSlicingIndexing.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20843 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialSparse.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       93 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/TutorialSparse_example_details.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8870 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/UnalignedArrayAssert.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6766 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/UsingBlasLapackBackends.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6226 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/UsingIntelMKL.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1885 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/UsingNVCC.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2980 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/WrongStackAlignment.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8206 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/eigen_navtree_hacks.js
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4817 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/eigendoxy.css
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1480 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/eigendoxy_footer.html.in
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2302 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/eigendoxy_header.html.in
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5515 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/eigendoxy_layout.xml.in
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1154 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/eigendoxy_tabs.css
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.048454 mazalib-0.52.3/src/eigen3/doc/examples/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       36 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/.krazy
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      637 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      796 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/CustomizingEigen_Inheritance.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      198 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Cwise_erf.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      199 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Cwise_erfc.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      201 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Cwise_lgamma.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      297 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/DenseBase_middleCols_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      297 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/DenseBase_middleRows_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      298 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/DenseBase_template_int_middleCols.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      298 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/DenseBase_template_int_middleRows.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      220 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/QuickStart_example.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      320 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/QuickStart_example2_dynamic.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      304 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/QuickStart_example2_fixed.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      699 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/TemplateKeyword_flexible.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      528 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/TemplateKeyword_simple.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1650 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/TutorialInplaceLU.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      645 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/TutorialLinAlgComputeTwice.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      385 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/TutorialLinAlgExComputeSolveError.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      398 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/TutorialLinAlgExSolveColPivHouseholderQR.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      372 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/TutorialLinAlgExSolveLDLT.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      364 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/TutorialLinAlgInverseDeterminant.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      620 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/TutorialLinAlgRankRevealing.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      420 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/TutorialLinAlgSVDSolve.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      552 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      393 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/TutorialLinAlgSetThreshold.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      490 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ArrayClass_accessors.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      423 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ArrayClass_addition.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      429 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ArrayClass_cwise_other.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      466 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ArrayClass_interop.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      617 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      253 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ArrayClass_mult.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      541 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_BlockOperations_block_assignment.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      407 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_BlockOperations_colrow.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      465 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_BlockOperations_corner.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      433 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_BlockOperations_print_block.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      362 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_BlockOperations_vector.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      419 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_PartialLU_solve.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      464 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_1nn.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      377 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      381 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple_rowwise.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      260 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_colwise.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      522 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      534 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      703 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      465 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_operatornorm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      257 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_rowwise.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      557 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      702 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_simple_example_dynamic_size.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      297 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_simple_example_fixed_size.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      764 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/class_Block.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      544 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/class_CwiseBinaryOp.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      580 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/class_CwiseUnaryOp.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      391 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/class_CwiseUnaryOp_ptrfun.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      724 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/class_FixedBlock.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      489 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/class_FixedReshaped.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      700 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/class_FixedVectorBlock.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      568 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/class_Reshaped.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      802 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/class_VectorBlock.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      436 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/function_taking_eigenbase.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      613 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/function_taking_ref.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      377 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/make_circulant.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      150 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/make_circulant.cpp.entry
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      980 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/make_circulant.cpp.evaluator
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      611 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/make_circulant.cpp.expression
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      154 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/make_circulant.cpp.main
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       89 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/make_circulant.cpp.preamble
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      624 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/make_circulant.cpp.traits
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1372 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/make_circulant2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4404 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/matrixfree_cg.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2520 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/nullary_indexing.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      493 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/tut_arithmetic_add_sub.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      408 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/tut_arithmetic_dot_cross.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      631 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/tut_arithmetic_matrix_mul.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      545 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/tut_arithmetic_redux_basic.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      370 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/tut_arithmetic_scalar_mul_div.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      361 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/tut_matrix_coefficient_accessors.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      507 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/tut_matrix_resize.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      241 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/examples/tut_matrix_resize_fixed_size.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       86 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/ftv2node.png
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      229 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/ftv2pnode.png
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.336772 mazalib-0.52.3/src/eigen3/doc/snippets/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       36 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/.krazy
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      215 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/AngleAxis_mimic_euler.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       63 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Array_initializer_list_23_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       63 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Array_initializer_list_vector_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      103 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Array_variadic_ctor_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      403 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/BiCGSTAB_simple.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      419 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/BiCGSTAB_step_by_step.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1671 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      332 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/ColPivHouseholderQR_solve.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      808 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/ComplexEigenSolver_compute.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      220 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/ComplexEigenSolver_eigenvalues.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      198 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/ComplexEigenSolver_eigenvectors.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      307 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/ComplexSchur_compute.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      267 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/ComplexSchur_matrixT.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      225 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/ComplexSchur_matrixU.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       47 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_abs.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       48 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_abs2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       57 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_acos.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       88 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_arg.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      236 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_array_power_array.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       57 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_asin.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       67 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_atan.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       66 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_boolean_and.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      110 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_boolean_not.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       66 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_boolean_or.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       65 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_boolean_xor.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       95 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_ceil.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       60 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_cos.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       66 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_cosh.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       46 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_cube.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       54 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_equal_equal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       45 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_exp.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       96 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_floor.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       53 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_greater.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       54 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_greater_equal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       49 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_inverse.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      109 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_isFinite.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      106 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_isInf.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      106 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_isNaN.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       53 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_less.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       54 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_less_equal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       45 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_log.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       49 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_log10.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       56 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_max.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       56 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_min.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       41 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_minus.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       48 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_minus_equal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       54 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_not_equal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       41 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_plus.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       48 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_plus_equal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       55 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_pow.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      145 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_product.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       51 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_quotient.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       96 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_round.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       87 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_scalar_power_array.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       47 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_sign.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       60 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_sin.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       66 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_sinh.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       58 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_slash_equal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       46 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_sqrt.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       48 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_square.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       60 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_tan.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       66 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_tanh.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       58 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Cwise_times_equal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      119 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/DenseBase_LinSpaced.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      428 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/DenseBase_LinSpacedInt.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      141 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/DenseBase_LinSpaced_seq_deprecated.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       63 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/DenseBase_setLinSpaced.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      374 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/DirectionWise_hnormalized.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      190 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/DirectionWise_replicate.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      183 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/DirectionWise_replicate_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      816 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      367 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/EigenSolver_compute.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      180 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/EigenSolver_eigenvalues.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      185 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/EigenSolver_eigenvectors.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      439 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/EigenSolver_pseudoEigenvectors.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      333 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/FullPivHouseholderQR_solve.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      378 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/FullPivLU_image.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      324 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/FullPivLU_kernel.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      424 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/FullPivLU_solve.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      463 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/GeneralizedEigenSolver.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      345 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/HessenbergDecomposition_compute.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      399 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/HessenbergDecomposition_matrixH.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      491 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/HessenbergDecomposition_packedMatrix.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      307 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/HouseholderQR_householderQ.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      366 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/HouseholderQR_solve.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1347 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/HouseholderSequence_HouseholderSequence.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      617 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/IOFormat.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      623 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/JacobiSVD_basic.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      240 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Jacobi_makeGivens.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      299 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Jacobi_makeJacobi.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      531 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/LLT_example.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      464 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/LLT_solve.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      196 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/LeastSquaresNormalEquations.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      181 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/LeastSquaresQR.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      169 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Map_general_stride.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      204 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Map_inner_stride.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      141 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Map_outer_stride.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      186 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Map_placement_new.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       96 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Map_simple.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      172 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_adjoint.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      530 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_all.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      214 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_applyOnTheLeft.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      301 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_applyOnTheRight.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       74 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_array.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      238 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_array_const.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       57 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_asDiagonal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      249 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_block_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      255 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_block_int_int_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      277 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_bottomLeftCorner_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      280 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_bottomRightCorner_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      248 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_bottomRows_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      122 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_cast.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       85 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_col.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      292 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_colwise.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      481 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_colwise_iterator_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      423 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_computeInverseAndDetWithCheck.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      329 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_computeInverseWithCheck.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       84 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_cwiseAbs.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       85 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_cwiseAbs2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      283 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_cwiseEqual.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       91 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_cwiseInverse.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       62 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_cwiseMax.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       62 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_cwiseMin.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      293 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_cwiseNotEqual.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      157 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_cwiseProduct.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       67 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_cwiseQuotient.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       84 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_cwiseSign.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       52 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_cwiseSqrt.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      192 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_diagonal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      275 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_diagonal_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      279 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_diagonal_template_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      163 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_eigenvalues.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      231 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_end_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      479 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_eval.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      279 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_fixedBlock_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      381 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_hnormalized.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      491 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_homogeneous.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       51 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_identity.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       43 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_identity_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      148 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_inverse.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      247 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_isDiagonal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      240 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_isIdentity.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      221 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_isOnes.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      299 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_isOrthogonal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      236 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_isUnitary.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      220 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_isZero.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      242 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_leftCols_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      132 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_noalias.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       77 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_ones.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       79 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_ones_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_ones_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      135 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_operatorNorm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      174 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_prod.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       43 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_random.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_random_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       40 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_random_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      174 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_replicate.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      167 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_replicate_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      295 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_reshaped_auto.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      181 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_reshaped_fixed.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      163 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_reshaped_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      291 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_reshaped_to_vector.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      415 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_reverse.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      245 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_rightCols_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       85 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_row.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      286 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_rowwise.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      249 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_segment_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      121 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_select.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      367 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_selfadjointView.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      303 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_set.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       86 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_setIdentity.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       75 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_setOnes.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       75 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_setRandom.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       75 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_setZero.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      231 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_start_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      254 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_bottomRows.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      235 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_end.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      269 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_int_block_int_int_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      280 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      307 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      283 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_int_bottomRightCorner.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      310 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_int_bottomRightCorner_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      271 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_int_topLeftCorner.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      298 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_int_topLeftCorner_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      274 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_int_topRightCorner.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      301 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_int_topRightCorner_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      248 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_leftCols.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      251 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_rightCols.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      249 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_segment.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      235 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_start.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      245 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_template_int_topRows.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      268 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_topLeftCorner_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      271 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_topRightCorner_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      239 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_topRows_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      422 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_transpose.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      582 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_triangularView.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       73 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_zero.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       75 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_zero_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_zero_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      164 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_Map_stride.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       63 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_initializer_list_23_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       40 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_initializer_list_vector_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      114 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_resize_NoChange_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      241 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_resize_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      114 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_resize_int_NoChange.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      416 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_resize_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       55 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_setConstant_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       58 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_setConstant_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       55 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_setIdentity_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       48 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_setOnes_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       51 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_setOnes_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       50 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_setRandom_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       53 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_setRandom_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       48 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_setZero_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       51 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_setZero_int_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      105 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Matrix_variadic_ctor_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      379 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/PartialPivLU_solve.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      268 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/PartialRedux_count.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      179 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/PartialRedux_maxCoeff.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      179 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/PartialRedux_minCoeff.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      172 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/PartialRedux_norm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      172 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/PartialRedux_prod.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      183 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/PartialRedux_squaredNorm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      167 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/PartialRedux_sum.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      836 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/RealQZ_compute.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      439 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/RealSchur_RealSchur_MatrixType.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      349 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/RealSchur_compute.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      369 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      833 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      842 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      372 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      405 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      184 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointEigenSolver_eigenvalues.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      197 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointEigenSolver_eigenvectors.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      435 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointEigenSolver_operatorInverseSqrt.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      371 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointEigenSolver_operatorSqrt.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      187 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointView_eigenvalues.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      160 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointView_operatorNorm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      169 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Slicing_arrayexpr.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      379 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Slicing_custom_padding_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      193 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Slicing_rawarray_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      166 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Slicing_stdvector_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      420 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/SparseMatrix_coeffs.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      274 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/TopicAliasing_block.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      277 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/TopicAliasing_block_correct.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      611 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/TopicAliasing_cwise.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       80 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/TopicAliasing_mult1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      240 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/TopicAliasing_mult2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       90 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/TopicAliasing_mult3.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      105 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/TopicAliasing_mult4.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      114 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/TopicAliasing_mult5.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      543 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/TopicStorageOrders_example.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      531 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Triangular_solve.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      454 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tridiagonalization_Tridiagonalization_MatrixType.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      401 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tridiagonalization_compute.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      485 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tridiagonalization_decomposeInPlace.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      565 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tridiagonalization_diagonal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      309 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tridiagonalization_householderCoefficients.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      402 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tridiagonalization_packedMatrix.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      137 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_Block.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      172 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_CommaTemporary.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      277 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_Join.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      279 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_LinSpaced.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      898 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      345 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_Zero.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      306 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_Map_rowmajor.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      917 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_Map_using.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      175 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_ReshapeMat2Mat.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      308 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_ReshapeMat2Vec.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      620 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_SlicingCol.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      182 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_SlicingVec.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       75 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_commainit_01.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      118 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_commainit_01b.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      222 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_commainit_02.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      119 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_range_for_loop_1d_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      151 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_range_for_loop_2d_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      252 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_reshaped_vs_resize_1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      378 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_reshaped_vs_resize_2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      152 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_solve_matrix_inverse.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      328 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_solve_multiple_rhs.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      381 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_solve_reuse_decomposition.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      265 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_solve_singular.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      281 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_solve_triangular.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      165 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_solve_triangular_inplace.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      205 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_std_sort.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      221 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_std_sort_rows_cxx11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      467 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/VectorwiseOp_homogeneous.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      546 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/Vectorwise_reverse.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      748 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/class_FullPivLU.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      526 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/compile_snippet.cpp.in
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      480 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/tut_arithmetic_redux_minmax.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      191 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/tut_arithmetic_transpose_aliasing.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      289 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/tut_arithmetic_transpose_conjugate.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      178 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/tut_arithmetic_transpose_inplace.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      198 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/snippets/tut_matrix_assignment_resizing.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.341835 mazalib-0.52.3/src/eigen3/doc/special_examples/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1176 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/special_examples/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1222 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/special_examples/Tutorial_sparse_example.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1620 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/special_examples/Tutorial_sparse_example_details.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      350 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/special_examples/random_cpp11.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2606 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/doc/tutorial.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      263 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/eigen3.pc.in
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.389887 mazalib-0.52.3/src/eigen3/failtest/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2493 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      259 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/bdcsvd_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      248 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/block_nonconst_ctor_on_const_xpr_0.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      248 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/block_nonconst_ctor_on_const_xpr_1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      277 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/block_nonconst_ctor_on_const_xpr_2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      278 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/block_on_const_type_actually_const_0.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      278 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/block_on_const_type_actually_const_1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      271 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/colpivqr_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      260 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/const_qualified_block_method_retval_0.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      255 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/const_qualified_block_method_retval_1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      254 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/const_qualified_diagonal_method_retval.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      256 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/const_qualified_transpose_method_retval.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      286 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/cwiseunaryview_nonconst_ctor_on_const_xpr.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      312 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/cwiseunaryview_on_const_type_actually_const.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      243 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/diagonal_nonconst_ctor_on_const_xpr.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      266 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/diagonal_on_const_type_actually_const.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      290 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/eigensolver_cplx.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      273 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/eigensolver_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      161 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/failtest_sanity_check.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      261 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/fullpivlu_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      272 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/fullpivqr_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      197 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/initializer_list_1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      238 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/initializer_list_2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      262 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/jacobisvd_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      264 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/ldlt_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      262 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/llt_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      239 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/map_nonconst_ctor_on_const_ptr_0.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      261 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/map_nonconst_ctor_on_const_ptr_1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      285 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/map_nonconst_ctor_on_const_ptr_2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      329 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/map_nonconst_ctor_on_const_ptr_3.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      336 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/map_nonconst_ctor_on_const_ptr_4.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      264 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/map_on_const_type_actually_const_0.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      256 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/map_on_const_type_actually_const_1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      264 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/partialpivlu_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      265 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/qr_int.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      281 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/ref_1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      228 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/ref_2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      246 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/ref_3.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      242 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/ref_4.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      254 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/ref_5.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      256 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/selfadjointview_nonconst_ctor_on_const_xpr.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      282 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/selfadjointview_on_const_type_actually_const.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      320 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/sparse_ref_1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      253 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/sparse_ref_2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      286 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/sparse_ref_3.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      250 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/sparse_ref_4.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      301 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/sparse_ref_5.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      306 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/sparse_storage_mismatch.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      231 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/swap_1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      223 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/swap_2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      226 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/ternary_1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      238 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/ternary_2.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      244 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/transpose_nonconst_ctor_on_const_xpr.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      270 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/transpose_on_const_type_actually_const.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      253 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/triangularview_nonconst_ctor_on_const_xpr.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      281 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/failtest/triangularview_on_const_type_actually_const.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.438217 mazalib-0.52.3/src/eigen3/lapack/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11422 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2277 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/cholesky.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2947 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/clacgv.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2437 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/cladiv.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6527 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/clarf.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24195 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/clarfb.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5547 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/clarfg.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10778 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/clarft.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      596 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/complex_double.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      595 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/complex_single.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3097 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/dladiv.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5448 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/dlamch.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2618 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/dlapy2.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2848 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/dlapy3.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6394 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/dlarf.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23511 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/dlarfb.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5142 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/dlarfg.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10548 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/dlarft.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      580 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/double.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1334 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/dsecnd_NONE.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1888 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/eigenvalues.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3075 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/ilaclc.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3118 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/ilaclr.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3070 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/iladlc.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3121 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/iladlr.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3059 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/ilaslc.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3109 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/ilaslr.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3080 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/ilazlc.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3131 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/ilazlr.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      906 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/lapack_common.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2744 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/lu.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1310 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/second_NONE.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      579 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/single.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3025 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/sladiv.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5453 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/slamch.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2594 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/slapy2.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2812 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/slapy3.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6344 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/slarf.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23490 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/slarfb.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5104 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/slarfg.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10509 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/slarft.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5029 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/svd.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2955 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/zlacgv.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2461 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/zladiv.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6510 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/zlarf.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24272 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/zlarfb.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5562 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/zlarfg.f
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10780 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/lapack/zlarft.f
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.448564 mazalib-0.52.3/src/eigen3/scripts/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      334 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/scripts/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      599 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/scripts/buildtests.in
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1615 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/scripts/cdashtesting.cmake.in
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      691 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/scripts/check.in
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       47 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/scripts/debug.in
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6616 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/scripts/eigen_gen_credits.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      762 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/scripts/eigen_gen_docs
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      333 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/scripts/eigen_gen_split_test_help.cmake
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1034 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/scripts/eigen_monitor_perf.sh
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       49 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/scripts/release.in
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2437 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/scripts/relicense.py
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      217 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/signature_of_eigen3_matrix_library
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.598725 mazalib-0.52.3/src/eigen3/test/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5665 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/AnnoyingScalar.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14389 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8887 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/adjoint.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22072 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/array_cwise.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13190 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/array_for_matrix.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      993 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/array_of_string.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2423 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/array_replicate.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6587 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/array_reverse.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2503 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/bandmatrix.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11407 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/basicstuff.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4516 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/bdcsvd.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1507 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/bicgstab.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15132 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/block.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5892 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/boostmultiprec.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      187 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/bug1213.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      155 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/bug1213.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      297 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/bug1213_main.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18872 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/cholesky.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3446 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/cholmod_support.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3037 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/commainitializer.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1577 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/conjugate_gradient.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5344 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/conservative_resize.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2660 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/constructor.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6565 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/corners.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2097 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/ctorleak.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5252 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/denseLM.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3881 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/dense_storage.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2341 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/determinant.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4220 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/diagonal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6871 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/diagonal_matrix_variadic_ctor.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7704 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/diagonalmatrices.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2291 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/dontalign.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4937 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/dynalloc.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2261 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/eigen2support.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6397 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/eigensolver_complex.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4149 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/eigensolver_generalized_real.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9706 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/eigensolver_generic.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11304 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/eigensolver_selfadjoint.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/evaluator_common.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21563 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/evaluators.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1965 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/exceptions.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5355 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/fastmath.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1925 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/first_aligned.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6089 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/geo_alignedbox.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3674 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/geo_eulerangles.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5595 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/geo_homogeneous.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7761 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/geo_hyperplane.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4971 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/geo_orthomethods.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5353 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/geo_parametrizedline.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11872 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/geo_quaternion.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26166 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/geo_transformations.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7254 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/gpu_basic.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5224 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/gpu_common.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11914 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/half_float.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2466 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/hessenberg.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6434 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/householder.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2692 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/incomplete_cholesky.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19079 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/indexed_view.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13127 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/initializer_list_construction.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3990 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/inplace_decomposition.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5937 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/integer_types.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4755 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/inverse.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1409 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/is_same_dense.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2813 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/jacobi.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5771 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/jacobisvd.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      987 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/klu_support.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6277 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/linearstructure.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1536 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/lscg.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9327 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/lu.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    33626 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/main.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8150 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/mapped_matrix.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7648 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/mapstaticmethods.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10354 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/mapstride.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7494 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/meta.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      776 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/metis_support.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1835 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/miscmatrices.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18088 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/mixingtypes.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      659 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/mpl2only.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1245 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/nestbyvalue.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4484 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/nesting_ops.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8928 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/nomalloc.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13147 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/nullary.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3302 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/num_dimensions.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1766 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/numext.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    38925 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/packetmath.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      984 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/pardiso_support.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1956 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/pastix_support.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7212 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/permutationmatrices.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3287 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/prec_inverse_4x4.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12139 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/product.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14926 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/product_extra.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4862 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/product_large.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4553 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/product_mmtr.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11197 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/product_notemporary.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3596 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/product_selfadjoint.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12234 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/product_small.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6258 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/product_symm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8002 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/product_syrk.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7058 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/product_trmm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4340 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/product_trmv.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6229 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/product_trsolve.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4803 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/qr.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14235 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/qr_colpivoting.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5759 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/qr_fullpivoting.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4777 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/qtvector.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4491 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/rand.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3196 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/real_qz.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8422 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/redux.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12060 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/ref.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10922 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/reshape.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1146 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/resize.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4424 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/rvalue_types.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3660 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/schur_complex.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4074 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/schur_real.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2494 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/selfadjoint.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2270 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/simplicial_cholesky.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2085 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sizeof.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2703 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sizeoverflow.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2200 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/smallvectors.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1752 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/solverbase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6500 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sparse.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4916 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sparseLM.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29569 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sparse_basic.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12423 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sparse_block.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10233 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sparse_permutations.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26049 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sparse_product.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6264 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sparse_ref.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19769 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sparse_solver.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5267 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sparse_solvers.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5250 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sparse_vector.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1836 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sparselu.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4736 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/sparseqr.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1820 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/special_numbers.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   165510 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/split_test_helper.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1905 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/spqr_support.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10374 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/stable_norm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4390 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/stddeque.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4896 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/stddeque_overload.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4362 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/stdlist.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6044 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/stdlist_overload.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5274 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/stdvector.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5175 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/stdvector_overload.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16845 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/stl_iterators.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      979 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/superlu_support.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19275 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/svd_common.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4168 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/svd_fill.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3034 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/swap.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2826 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/symbolic_index.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12210 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/triangular.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2072 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/type_alias.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6042 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/umeyama.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1205 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/umfpack_support.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6045 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/unalignedassert.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2625 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/unalignedcount.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1759 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/upperbidiagonalization.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21414 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/vectorization_logic.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11787 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/vectorwiseop.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4135 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/visitor.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3845 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/test/zerosized.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.600488 mazalib-0.52.3/src/eigen3/unsupported/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      272 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/CMakeLists.txt
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.624443 mazalib-0.52.3/src/eigen3/unsupported/Eigen/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4403 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/AdolcForward
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6454 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/AlignedVector3
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      960 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/ArpackSupport
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1227 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/AutoDiff
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5618 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/BVH
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      635 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CMakeLists.txt
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.628578 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      315 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4759 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/Tensor
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1309 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/TensorSymmetry
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2205 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/ThreadPool
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.048341 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.755077 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    64351 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/README.md
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21825 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12891 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6116 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMaxSycl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10877 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    57454 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12682 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    50233 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlockV2.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    43466 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22995 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16716 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    46416 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2748 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      231 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    64859 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24002 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24756 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    71697 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17980 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    49791 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29339 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8856 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13645 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4981 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      221 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3531 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12393 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    36824 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15544 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7910 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18240 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8884 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    40663 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    31651 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16503 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    25072 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15665 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8070 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8505 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15029 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11457 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1349 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3907 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1195 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2639 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    28554 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26365 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9399 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2798 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9304 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8658 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2881 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15064 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8612 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    47194 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26691 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11823 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13524 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    50912 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      227 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35222 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10007 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15325 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17970 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11500 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18419 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5246 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14524 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4024 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSycl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8991 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclConvertToDeviceExpression.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26700 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExprConstructor.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15800 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractAccessor.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24014 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractFunctors.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16137 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclFunctors.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8058 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclLeafCount.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11408 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclPlaceHolderExpr.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4439 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclRun.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9995 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclTuple.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10513 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10200 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7801 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    30215 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.759573 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11150 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9322 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13359 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.761141 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21715 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.774711 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2180 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9370 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17189 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9602 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      797 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1249 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11783 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1728 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      735 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.779617 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/util/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23218 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4231 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8416 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4332 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1169 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/EulerAngles
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14535 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/FFT
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1472 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/IterativeSolvers
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      980 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/KroneckerProduct
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1287 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/LevenbergMarquardt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7869 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/MPRealSupport
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18423 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/MatrixFunctions
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      616 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/MoreVectorization
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6103 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/NonLinearOptimization
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1835 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/NumericalDiff
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19394 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/OpenGLSupport
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4932 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/Polynomials
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      969 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/Skyline
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1377 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/SparseExtra
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2221 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/SpecialFunctions
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1031 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/Splines
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.053300 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.783225 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/AutoDiff/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3258 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29909 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9249 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.785470 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/BVH/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13269 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9389 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/BVH/KdBVH.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.786587 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Eigenvalues/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29865 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.789949 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/EulerAngles/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      180 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/EulerAngles/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15722 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11925 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.792594 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/FFT/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9532 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12693 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.800985 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5581 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18280 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10544 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2610 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5508 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12664 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6046 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.802074 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/KroneckerProduct/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10535 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.809041 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2246 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2527 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6850 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5199 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6993 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13693 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.817178 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17065 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23240 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17930 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24127 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14483 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2224 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.818343 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MoreVectorization/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3130 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.831953 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20429 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22792 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1930 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1985 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3404 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2304 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9409 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3355 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1111 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3182 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1411 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.833117 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NumericalDiff/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4150 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.836608 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Polynomials/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8113 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Polynomials/Companion.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16111 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4949 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.844442 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11717 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    31967 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7957 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11148 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8225 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3242 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.852367 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4382 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    41395 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14148 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8708 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7815 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12168 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.869259 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10301 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12998 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2610 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    71584 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5424 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7861 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12030 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2957 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    59028 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3792 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.052992 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.870978 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11233 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/GpuSpecialFunctions.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.875961 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Splines/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18814 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Splines/Spline.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16853 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4405 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1926 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/README.txt
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.877337 mazalib-0.52.3/src/eigen3/unsupported/bench/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4029 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/bench/bench_svd.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.880972 mazalib-0.52.3/src/eigen3/unsupported/doc/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      118 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      858 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/Overview.dox
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5460 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/eigendoxy_layout.xml.in
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.898527 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2158 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/BVH_Example.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      687 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1893 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/EulerAngles.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2640 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/FFT.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      372 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/MatrixExponential.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      492 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/MatrixFunction.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      390 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/MatrixLogarithm.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      380 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/MatrixPower.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      441 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/MatrixPower_optimal.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      528 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/MatrixSine.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      544 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/MatrixSinh.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      450 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/MatrixSquareRoot.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2445 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/PolynomialSolver1.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      655 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/examples/PolynomialUtils1.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:51.899542 mazalib-0.52.3/src/eigen3/unsupported/doc/snippets/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1163 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/doc/snippets/CMakeLists.txt
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:52.029614 mazalib-0.52.3/src/eigen3/unsupported/test/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7412 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/BVH.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13045 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/CMakeLists.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9919 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/EulerAngles.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       49 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/FFT.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9495 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/FFTW.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    66446 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/NonLinearOptimization.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2976 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/NumericalDiff.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2392 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/alignedvector3.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11379 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/autodiff.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3044 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/autodiff_scalar.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16779 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/bessel_functions.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4132 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_eventcount.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1916 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_maxsizevector.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19097 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_meta.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5164 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_non_blocking_thread_pool.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7259 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_runqueue.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9444 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_argmax.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9139 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_argmax_gpu.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9843 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_argmax_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10077 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_assign.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23668 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_block_access.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    30298 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_block_eval.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16430 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_block_io.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5852 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_broadcast_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9540 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_broadcasting.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17638 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_builtins_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2499 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_cast_float16_gpu.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3114 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_casts.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13475 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_chipping.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26697 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_chipping_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2075 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_comparisons.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2938 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6822 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_complex_gpu.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4767 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_concatenation.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8591 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_concatenation_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1722 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_const.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7568 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_contract_gpu.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12913 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_contract_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23634 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_contraction.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5531 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_convolution.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20502 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_convolution_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2618 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_custom_index.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3322 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_custom_op.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6773 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_custom_op_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13891 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_device.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3287 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_device_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2666 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_dimension.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1039 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_empty.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    31406 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_executor.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10692 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_expr.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14021 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_fft.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7513 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_fixed_size.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2246 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_forced_eval.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3431 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2357 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_generator.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5879 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_generator_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    60089 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_gpu.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6096 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_ifft.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    36846 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_image_patch.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    63203 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_image_patch_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19037 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_index_list.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2190 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_inflation.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5237 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_inflation_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4276 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_intdiv.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3413 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_io.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1700 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_layout_swap.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4856 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      992 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_lvalue.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8289 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_map.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1039 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_math.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1554 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_mixed_indices.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16867 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_morphing.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11272 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_morphing_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1996 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_move.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1681 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_notification.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2996 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_of_complex.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2535 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_of_const_values.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22284 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_of_float16_gpu.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3918 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_of_strings.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2745 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_padding.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5834 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_padding_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5671 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_patch.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9634 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_patch_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2232 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_random.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2441 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_random_gpu.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15797 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_reduction.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5564 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_reduction_gpu.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7986 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_reduction_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6970 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_ref.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5475 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_reverse.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8666 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_reverse_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1548 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_roundings.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3088 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_scan.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2654 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_scan_gpu.cu
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6504 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_shuffling.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4227 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_shuffling_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9951 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_simple.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3143 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_striding.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7277 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_striding_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1977 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_sugar.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11350 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    59897 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_symmetry.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4386 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_thread_local.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26212 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_thread_pool.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5275 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_trace.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5886 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_uint128.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4719 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_volume_patch.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12209 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1310 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/dgmres.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3963 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/forward_adolc.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1276 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/gmres.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9327 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/kronecker_product.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    56981 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/levenberg_marquardt.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4558 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/matrix_exponential.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6653 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/matrix_function.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2173 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/matrix_functions.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7382 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/matrix_power.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1081 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/matrix_square_root.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1702 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/minres.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:52.030811 mazalib-0.52.3/src/eigen3/unsupported/test/mpreal/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   121580 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/mpreal/mpreal.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2448 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/mpreal_support.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10929 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/openglsupport.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7718 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/polynomialsolver.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3695 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/polynomialutils.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7378 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/sparse_extra.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21638 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/special_functions.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8810 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/eigen3/unsupported/test/splines.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.057373 mazalib-0.52.3/src/mazalib/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17957 2024-03-09 14:30:24.000000 mazalib-0.52.3/src/mazalib/mazalib.cpp
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:52.036753 mazalib-0.52.3/src/mazalib.egg-info/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1449 2024-03-28 14:40:49.000000 mazalib-0.52.3/src/mazalib.egg-info/PKG-INFO
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    84583 2024-03-28 14:40:49.000000 mazalib-0.52.3/src/mazalib.egg-info/SOURCES.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)        1 2024-03-28 14:40:49.000000 mazalib-0.52.3/src/mazalib.egg-info/dependency_links.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      208 2024-03-28 14:40:49.000000 mazalib-0.52.3/src/mazalib.egg-info/entry_points.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)        6 2024-03-28 14:40:49.000000 mazalib-0.52.3/src/mazalib.egg-info/requires.txt
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       28 2024-03-28 14:40:49.000000 mazalib-0.52.3/src/mazalib.egg-info/top_level.txt
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:52.037548 mazalib-0.52.3/src/segmentation/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/segmentation/__init__.py
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:52.082661 mazalib-0.52.3/src/segmentation/include/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1039 2023-10-22 16:19:07.000000 mazalib-0.52.3/src/segmentation/include/BinaryIO.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1577 2023-10-22 18:31:46.000000 mazalib-0.52.3/src/segmentation/include/CACSegmentation.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      464 2023-10-17 22:32:20.000000 mazalib-0.52.3/src/segmentation/include/Config.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2665 2023-10-22 17:25:22.000000 mazalib-0.52.3/src/segmentation/include/DenoiseParameters.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11817 2023-10-27 18:53:57.000000 mazalib-0.52.3/src/segmentation/include/DynamicArray.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      727 2023-10-22 16:40:40.000000 mazalib-0.52.3/src/segmentation/include/ExpectedMaximized.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3090 2023-10-17 22:32:20.000000 mazalib-0.52.3/src/segmentation/include/Grid.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    34871 2024-02-16 13:59:27.000000 mazalib-0.52.3/src/segmentation/include/HessianSegmentation.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6256 2023-10-17 22:32:20.000000 mazalib-0.52.3/src/segmentation/include/IntegralImage.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4958 2023-10-22 17:38:45.000000 mazalib-0.52.3/src/segmentation/include/IterativeNonLocalMeansCPU.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3117 2024-03-28 14:16:36.000000 mazalib-0.52.3/src/segmentation/include/KrigingSegmentation.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2265 2024-02-15 13:48:10.000000 mazalib-0.52.3/src/segmentation/include/LatticeModel.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2867 2023-10-17 22:32:20.000000 mazalib-0.52.3/src/segmentation/include/LogFile.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16800 2024-02-16 13:59:27.000000 mazalib-0.52.3/src/segmentation/include/MRFSegmentation.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      865 2023-10-17 22:32:20.000000 mazalib-0.52.3/src/segmentation/include/MRFUtils.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5807 2023-10-17 22:32:20.000000 mazalib-0.52.3/src/segmentation/include/NelderMead.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11440 2023-10-22 17:26:14.000000 mazalib-0.52.3/src/segmentation/include/NewCACSegmentation.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1213 2023-10-22 17:38:57.000000 mazalib-0.52.3/src/segmentation/include/NoiseLevel.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      783 2023-10-22 17:13:57.000000 mazalib-0.52.3/src/segmentation/include/NonLocalMeans.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1899 2023-10-22 17:42:50.000000 mazalib-0.52.3/src/segmentation/include/Point.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2424 2024-03-09 11:11:31.000000 mazalib-0.52.3/src/segmentation/include/Point3d.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      715 2023-10-27 18:11:54.000000 mazalib-0.52.3/src/segmentation/include/RandomNumbers.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13861 2023-10-22 14:19:52.000000 mazalib-0.52.3/src/segmentation/include/RegionGrowthSegmentation.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5297 2024-02-13 11:25:07.000000 mazalib-0.52.3/src/segmentation/include/Variation.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    42272 2023-10-27 18:11:46.000000 mazalib-0.52.3/src/segmentation/include/threshold.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7849 2023-10-22 18:19:36.000000 mazalib-0.52.3/src/segmentation/include/util.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10339 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/segmentation/include/var_2d.h
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12673 2023-10-30 16:40:19.000000 mazalib-0.52.3/src/segmentation/include/var_3d.h
-drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-03-28 14:40:50.073117 mazalib-0.52.3/src/segmentation/src/
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11189 2023-10-22 18:31:38.000000 mazalib-0.52.3/src/segmentation/src/CACSegmentation.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2513 2023-10-22 16:40:00.000000 mazalib-0.52.3/src/segmentation/src/ExpectedMaximized.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9675 2020-09-29 10:07:48.000000 mazalib-0.52.3/src/segmentation/src/Grid.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2555 2020-09-29 10:07:48.000000 mazalib-0.52.3/src/segmentation/src/HessianSegmentation.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      872 2020-09-29 10:07:48.000000 mazalib-0.52.3/src/segmentation/src/IntegralImage.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)   105044 2023-10-22 17:23:50.000000 mazalib-0.52.3/src/segmentation/src/IterativeNonLocalMeansCPU.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13772 2024-03-28 14:16:40.000000 mazalib-0.52.3/src/segmentation/src/KrigingSegmentation.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7402 2024-02-15 17:05:48.000000 mazalib-0.52.3/src/segmentation/src/LatticeModel.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)      183 2021-01-18 05:35:22.000000 mazalib-0.52.3/src/segmentation/src/LogFile.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14065 2020-09-29 10:07:48.000000 mazalib-0.52.3/src/segmentation/src/MRFSegmentation.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)       33 2020-09-29 10:07:48.000000 mazalib-0.52.3/src/segmentation/src/NewCACSegmentation.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14464 2023-10-22 17:14:57.000000 mazalib-0.52.3/src/segmentation/src/NoiseLevel.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1898 2023-10-22 17:24:03.000000 mazalib-0.52.3/src/segmentation/src/NonLocalMeans.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2231 2020-09-29 10:07:48.000000 mazalib-0.52.3/src/segmentation/src/RandomNumbers.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1016 2024-02-13 11:32:43.000000 mazalib-0.52.3/src/segmentation/src/Variation.cpp
--rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3513 2023-10-22 18:20:20.000000 mazalib-0.52.3/src/segmentation/src/threshold.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.516465 mazalib-0.52.4/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35821 2023-10-30 16:40:18.000000 mazalib-0.52.4/LICENSE.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4543 2024-04-17 15:14:08.515603 mazalib-0.52.4/PKG-INFO
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3897 2024-04-17 15:11:28.000000 mazalib-0.52.4/README.md
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2024-04-17 15:14:08.516838 mazalib-0.52.4/setup.cfg
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2975 2024-04-17 15:14:00.000000 mazalib-0.52.4/setup.py
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.506137 mazalib-0.52.4/src/
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.539914 mazalib-0.52.4/src/eigen3/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      185 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/.hg_archival.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      191 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/.hgeol
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      319 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/.hgignore
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1544 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/.hgtags
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26000 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1541 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/COPYING.BSD
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35821 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/COPYING.GPL
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    27032 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/COPYING.LGPL
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2246 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/COPYING.MINPACK
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17099 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/COPYING.MPL2
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      797 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/COPYING.README
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      601 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/CTestConfig.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      184 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/CTestCustom.cmake.in
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.566828 mazalib-0.52.4/src/eigen3/Eigen/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      713 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1252 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/Cholesky
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1948 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/CholmodSupport
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12243 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/Core
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      129 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/Dense.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       37 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/Eigen
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1883 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/Eigenvalues
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2008 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/Geometry
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      904 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/Householder
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2131 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/IterativeLinearSolvers
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      972 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/Jacobi
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1430 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/KLUSupport
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1483 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/LU
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1026 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/MetisSupport
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2521 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/OrderingMethods
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1800 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/PaStiXSupport
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1151 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/PardisoSupport
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1368 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/QR
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      985 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/QtAlignedMalloc
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1196 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/SPQRSupport
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1680 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/SVD
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      922 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/Sparse
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1272 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/SparseCholesky
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2309 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/SparseCore
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1864 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/SparseLU
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1231 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/SparseQR
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      824 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/StdDeque
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      752 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/StdList
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      830 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/StdVector
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2307 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/SuperLUSupport
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1422 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/UmfPackSupport
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.484579 mazalib-0.52.4/src/eigen3/Eigen/src/
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.570130 mazalib-0.52.4/src/eigen3/Eigen/src/Cholesky/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    25525 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Cholesky/LDLT.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19241 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Cholesky/LLT.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4073 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.571104 mazalib-0.52.4/src/eigen3/Eigen/src/CholmodSupport/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26123 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.661351 mazalib-0.52.4/src/eigen3/Eigen/src/Core/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19627 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/ArithmeticSequence.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17128 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Array.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8385 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/ArrayBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6984 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/ArrayWrapper.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2828 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Assign.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    41301 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/AssignEvaluator.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12666 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Assign_MKL.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14263 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/BandMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18852 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Block.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4463 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/BooleanRedux.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5885 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/CommaInitializer.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7165 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/ConditionEstimator.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    65712 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/CoreEvaluators.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4877 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/CoreIterators.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8131 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/CwiseBinaryOp.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    33932 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/CwiseNullaryOp.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8453 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/CwiseTernaryOp.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3980 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/CwiseUnaryOp.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5389 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/CwiseUnaryView.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    30534 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/DenseBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24905 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/DenseCoeffsBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22985 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/DenseStorage.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9967 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Diagonal.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15061 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/DiagonalMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1016 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/DiagonalProduct.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11969 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Dot.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5911 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/EigenBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4915 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/ForceAlignedAccess.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5914 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Fuzzy.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22314 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/GeneralProduct.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29503 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/GenericPacketMath.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11454 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/GlobalFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7673 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/IO.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8528 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/IndexedView.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3566 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Inverse.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7398 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Map.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11294 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/MapBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    54438 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/MathFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3199 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/MathFunctionsImpl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24843 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Matrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24339 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/MatrixBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2543 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/NestByValue.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3729 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/NoAlias.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10626 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/NumTraits.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9429 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/PartialReduxEvaluator.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21353 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/PermutationMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    49641 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/PlainObjectBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7524 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Product.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    54433 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/ProductEvaluators.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6579 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Random.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19176 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Redux.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13346 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Ref.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5773 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Replicate.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17453 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Reshaped.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4335 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/ReturnByValue.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7672 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Reverse.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6182 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Select.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15238 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/SelfAdjointView.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1744 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6985 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Solve.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9461 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/SolveTriangular.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6338 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/SolverBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9165 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/StableNorm.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14871 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/StlIterators.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3976 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Stride.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2833 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Swap.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15681 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Transpose.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13459 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Transpositions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    39038 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/TriangularMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3584 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/VectorBlock.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    34308 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/VectorwiseOp.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9613 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/Visitor.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.476341 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.667184 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19643 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX/Complex.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6061 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    49706 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2133 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.672684 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX512/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20075 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX512/Complex.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17800 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    73803 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1132 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.676152 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AltiVec/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17889 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2413 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    44416 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.677612 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/CUDA/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4347 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/CUDA/Complex.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.684730 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2018 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24629 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2255 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    27369 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/Half.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1795 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/Settings.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2564 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.688470 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/GPU/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2798 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    33043 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1498 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.474711 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/HIP/
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.689679 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/HIP/hcc/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      714 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.693503 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/MSA/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21729 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/MSA/Complex.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16546 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    38368 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.698498 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/NEON/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19549 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/NEON/Complex.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1348 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    32019 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1394 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.703560 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SSE/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20968 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SSE/Complex.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6494 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    51849 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3534 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.709629 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SYCL/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7019 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11685 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23733 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22550 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2711 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.713469 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/ZVector/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21077 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/ZVector/Complex.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8469 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    41889 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.720229 mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6863 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18792 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/BinaryFunctors.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8209 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/NullaryFunctors.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4536 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/StlFunctors.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      632 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/TernaryFunctors.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35610 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/UnaryFunctors.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.745463 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   115557 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20629 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16265 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7081 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5230 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22242 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6504 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5740 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/Parallelizer.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21898 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11865 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10220 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5327 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6313 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/SelfadjointProduct.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4198 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21459 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14184 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15072 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10826 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14947 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6874 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6030 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularSolverVector.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.765582 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19661 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/BlasUtil.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19139 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/ConfigureVectorization.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22362 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/Constants.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4887 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15599 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/ForwardDeclarations.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6711 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/IndexedViewHelper.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11167 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/IntegralConstant.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4405 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/MKL_support.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    46645 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/Macros.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    46766 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/Memory.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    25516 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/Meta.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       88 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/NonMPL2.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1055 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1483 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/ReshapedHelper.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10863 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/StaticAssert.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12280 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/SymbolicIndex.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    36539 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/XprHelper.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.781982 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12905 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17736 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4269 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23592 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/EigenSolver.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17594 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9942 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14713 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5733 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24297 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/RealQZ.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21636 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/RealSchur.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3727 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    34828 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4191 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23099 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.797494 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15232 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/AlignedBox.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8670 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/AngleAxis.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3753 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/EulerAngles.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21036 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Homogeneous.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12244 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Hyperplane.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9190 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/OrthoMethods.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10049 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/ParametrizedLine.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    33830 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Quaternion.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7076 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Rotation2D.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8269 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/RotationBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6905 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Scaling.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    63424 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Transform.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7981 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Translation.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6356 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Umeyama.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.798605 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/arch/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5993 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.801696 mazalib-0.52.4/src/eigen3/Eigen/src/Householder/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4894 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Householder/BlockHouseholder.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5541 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Householder/Householder.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24114 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Householder/HouseholderSequence.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.811353 mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6981 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7062 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9104 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15442 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15415 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13793 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7547 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4273 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.812502 mazalib-0.52.4/src/eigen3/Eigen/src/Jacobi/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16856 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/Jacobi/Jacobi.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.813951 mazalib-0.52.4/src/eigen3/Eigen/src/KLUSupport/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11892 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/KLUSupport/KLUSupport.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.819910 mazalib-0.52.4/src/eigen3/Eigen/src/LU/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3556 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/LU/Determinant.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    33188 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/LU/FullPivLU.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15519 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/LU/InverseImpl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22475 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/LU/PartialPivLU.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3638 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.820946 mazalib-0.52.4/src/eigen3/Eigen/src/LU/arch/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14000 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/LU/arch/Inverse_SSE.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.822069 mazalib-0.52.4/src/eigen3/Eigen/src/MetisSupport/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4725 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/MetisSupport/MetisSupport.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.825822 mazalib-0.52.4/src/eigen3/Eigen/src/OrderingMethods/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16540 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/OrderingMethods/Amd.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    63544 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5401 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/OrderingMethods/Ordering.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.827221 mazalib-0.52.4/src/eigen3/Eigen/src/PaStiXSupport/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22927 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.828574 mazalib-0.52.4/src/eigen3/Eigen/src/PardisoSupport/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20637 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.835423 mazalib-0.52.4/src/eigen3/Eigen/src/QR/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26172 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/QR/ColPivHouseholderQR.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4759 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24064 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    27481 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/QR/FullPivHouseholderQR.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15075 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/QR/HouseholderQR.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3061 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.836393 mazalib-0.52.4/src/eigen3/Eigen/src/SPQRSupport/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12161 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.842471 mazalib-0.52.4/src/eigen3/Eigen/src/SVD/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    55030 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SVD/BDCSVD.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    33798 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SVD/JacobiSVD.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5190 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14620 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SVD/SVDBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16371 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SVD/UpperBidiagonalization.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.844732 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCholesky/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24881 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6004 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.885342 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10914 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/AmbiVector.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9017 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/CompressedStorage.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13530 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2258 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11638 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseAssign.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24341 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseBlock.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6691 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseColEtree.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13976 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26156 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4887 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13598 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5946 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3178 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseDot.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1136 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseFuzzy.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12894 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseMap.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    58689 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17849 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7507 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparsePermutation.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7219 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseProduct.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1748 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseRedux.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15889 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseRef.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26371 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4548 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseSolverBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8902 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3267 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseTranspose.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6626 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseTriangularView.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7013 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseUtil.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15310 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseVector.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8381 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseView.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9972 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/TriangularSolver.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.903850 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    28727 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4369 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLUImpl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7828 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5084 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10335 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2129 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6893 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6763 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3788 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10497 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4307 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5853 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8708 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9286 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5116 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4681 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2972 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.904970 mazalib-0.52.4/src/eigen3/Eigen/src/SparseQR/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29925 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SparseQR/SparseQR.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.909605 mazalib-0.52.4/src/eigen3/Eigen/src/StlSupport/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5251 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/StlSupport/StdDeque.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4261 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/StlSupport/StdList.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5469 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/StlSupport/StdVector.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2893 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/StlSupport/details.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.910601 mazalib-0.52.4/src/eigen3/Eigen/src/SuperLUSupport/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35373 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.911768 mazalib-0.52.4/src/eigen3/Eigen/src/UmfPackSupport/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    25098 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.925759 mazalib-0.52.4/src/eigen3/Eigen/src/misc/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2995 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/misc/Image.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2821 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/misc/Kernel.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1803 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/misc/RealSvd2x2.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    31000 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/misc/blas.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7986 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/misc/lapack.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)  1074661 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/misc/lapacke.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      491 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/misc/lapacke_mangling.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.935061 mazalib-0.52.4/src/eigen3/Eigen/src/plugins/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13464 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20266 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    60448 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/plugins/BlockMethods.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4943 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6266 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12545 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/plugins/IndexedViewMethods.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6527 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3022 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7064 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/Eigen/src/plugins/ReshapedMethods.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1180 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/INSTALL
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      371 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/README.md
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/__init__.py
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.973307 mazalib-0.52.4/src/eigen3/bench/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4081 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/BenchSparseUtil.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4685 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/BenchTimer.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2621 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/BenchUtil.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2063 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/README.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29859 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/analyze-blocking-sizes.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1449 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/basicbench.cxxlist
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1142 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/basicbenchmark.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1732 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/basicbenchmark.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6532 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/benchBlasGemm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3676 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/benchCholesky.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6000 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/benchEigenSolver.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2921 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/benchFFT.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3732 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/benchGeometry.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5328 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/benchVecAdd.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11810 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/bench_gemm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      646 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/bench_multi_compilers.sh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12013 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/bench_norm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2243 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/bench_reverse.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      338 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/bench_sum.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      663 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/bench_unrolling
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22936 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/benchmark-blocking-sizes.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      829 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/benchmark.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      873 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/benchmarkSlice.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      676 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/benchmarkX.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      640 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/benchmarkXcwise.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1227 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/benchmark_suite
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.976163 mazalib-0.52.4/src/eigen3/bench/btl/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2976 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18449 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/COPYING
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6601 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/README
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.997832 mazalib-0.52.4/src/eigen3/bench/btl/actions/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3519 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_aat_product.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3499 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_ata_product.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3804 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_atv_product.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3498 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_axpby.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3479 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_axpy.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3330 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_cholesky.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3588 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_ger.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5831 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_hessenberg.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3275 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_lu_decomp.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3734 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_lu_solve.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4036 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_matrix_matrix_product.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4134 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_matrix_matrix_product_bis.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4142 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_matrix_vector_product.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3313 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_partial_lu.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3135 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_rot.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3830 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_symv.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3797 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_syr2.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3562 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_trisolve.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4226 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_trisolve_matrix.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4072 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/action_trmm.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      485 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/actions/basic_actions.hh
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.010422 mazalib-0.52.4/src/eigen3/bench/btl/cmake/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      983 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindACML.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1396 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindATLAS.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      846 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindBLAZE.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1132 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindBlitz.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      703 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindCBLAS.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      383 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindGMM.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1435 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindMKL.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      850 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindMTL4.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      639 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindOPENBLAS.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2432 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindPackageHandleStandardArgs.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      864 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindTvmet.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1346 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.022808 mazalib-0.52.4/src/eigen3/bench/btl/data/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      901 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/data/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1387 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/data/action_settings.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2311 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/data/gnuplot_common_settings.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2122 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/data/go_mean
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5488 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/data/mean.cxx
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1918 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/data/mk_gnuplot_script.sh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      981 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/data/mk_mean_script.sh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1796 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/data/mk_new_gnuplot.sh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      990 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/data/perlib_plot_settings.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3556 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/data/regularize.cxx
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5310 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/data/smooth.cxx
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1755 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/data/smooth_all.sh
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.026034 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4995 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/bench.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1969 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/bench_parameter.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6990 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/btl.hh
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.029259 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/init/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1532 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/init/init_function.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2359 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/init/init_matrix.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1453 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/init/init_vector.hh
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.032729 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/static/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2358 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/static/bench_static.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2014 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/static/intel_bench_fixed_size.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2279 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/static/static_size_generator.hh
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.041771 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2387 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/STL_perf_analyzer.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2600 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/STL_timer.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2067 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3041 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/portable_perf_analyzer.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3668 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3721 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/portable_timer.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3035 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/x86_perf_analyzer.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5540 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/x86_timer.hh
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.046476 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/utils/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1728 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/utils/size_lin_log.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1700 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/utils/size_log.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2835 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/utils/utilities.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2289 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/utils/xy_file.hh
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.490205 mazalib-0.52.4/src/eigen3/bench/btl/libs/
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.053962 mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1619 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35833 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/blas.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2974 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/blas_interface.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4958 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/blas_interface_impl.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1707 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/c_interface_base.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3033 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/main.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.057491 mazalib-0.52.4/src/eigen3/bench/btl/libs/STL/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       39 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/STL/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6046 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/STL/STL_interface.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1870 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/STL/main.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.061188 mazalib-0.52.4/src/eigen3/bench/btl/libs/blaze/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      488 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/blaze/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4263 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/blaze/blaze_interface.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1676 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/blaze/main.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.069074 mazalib-0.52.4/src/eigen3/bench/btl/libs/blitz/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      441 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/blitz/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5556 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/blitz/blitz_LU_solve_interface.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4276 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/blitz/blitz_interface.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2013 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/blitz/btl_blitz.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1431 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/blitz/btl_tiny_blitz.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3206 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/blitz/tiny_blitz_interface.hh
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.078939 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      787 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1710 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5319 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/eigen2_interface.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1843 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/main_adv.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1239 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/main_linear.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1419 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/main_matmat.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1492 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/main_vecmat.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.088635 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3357 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1710 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8429 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/eigen3_interface.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1843 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/main_adv.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1320 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/main_linear.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1413 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/main_matmat.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1483 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/main_vecmat.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.094086 mazalib-0.52.4/src/eigen3/bench/btl/libs/gmm/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      131 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/gmm/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5556 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/gmm/gmm_LU_solve_interface.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4318 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/gmm/gmm_interface.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2164 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/gmm/main.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.099607 mazalib-0.52.4/src/eigen3/bench/btl/libs/mtl4/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      165 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/mtl4/.kdbgrc.main
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      139 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/mtl4/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1989 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/mtl4/main.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5556 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4354 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/mtl4/mtl4_interface.hh
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.107206 mazalib-0.52.4/src/eigen3/bench/btl/libs/tensors/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2199 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/tensors/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      694 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/tensors/main_linear.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      645 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/tensors/main_matmat.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      645 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/tensors/main_vecmat.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3295 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/tensors/tensor_interface.hh
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.111461 mazalib-0.52.4/src/eigen3/bench/btl/libs/tvmet/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      148 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/tvmet/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1500 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/tvmet/main.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3121 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/tvmet/tvmet_interface.hh
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.115541 mazalib-0.52.4/src/eigen3/bench/btl/libs/ublas/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      187 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/ublas/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1829 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/ublas/main.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4482 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/btl/libs/ublas/ublas_interface.hh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3370 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/check_cache_queries.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6602 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/dense_solvers.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7438 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/eig33.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3433 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/geometry.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.138581 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6962 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/changesets.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      205 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/gemm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1449 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/gemm_common.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      184 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/gemm_settings.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      125 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/gemm_square_settings.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      205 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/gemv.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1450 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/gemv_common.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       90 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/gemv_settings.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      101 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/gemv_square_settings.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      217 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/gemvt.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2567 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/lazy_gemm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      147 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/lazy_gemm_settings.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      313 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/llt.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2805 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/make_plot.sh
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.146690 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/resources/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3852 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/resources/chart_footer.html
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14824 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/resources/chart_header.html
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       28 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/resources/footer.html
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      926 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/resources/header.html
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   151724 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/resources/s1.js
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   241320 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/resources/s2.js
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4261 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/run.sh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2103 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/runall.sh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      229 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/trmv_lo.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      241 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/trmv_lot.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      229 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/trmv_up.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      241 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/perf_monitoring/trmv_upt.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3375 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/product_threshold.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6253 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/quat_slerp.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1144 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/quatmul.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6476 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/sparse_cholesky.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5288 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/sparse_dense_product.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3143 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/sparse_lu.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9322 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/sparse_product.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3483 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/sparse_randomsetter.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14246 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/sparse_setter.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2451 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/sparse_transpose.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6334 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/sparse_trisolver.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.155993 mazalib-0.52.4/src/eigen3/bench/spbench/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3024 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/spbench/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4098 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/spbench/sp_solver.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1886 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/spbench/spbench.dtd
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3388 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/spbench/spbenchsolver.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18271 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/spbench/spbenchsolver.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3920 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/spbench/spbenchstyle.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2922 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/spbench/test_sparseLU.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6329 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/spmv.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.166739 mazalib-0.52.4/src/eigen3/bench/tensors/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2498 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/tensors/README
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1634 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/tensors/benchmark.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7071 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/tensors/benchmark_main.cc
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1428 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/tensors/contraction_benchmarks_cpu.cc
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19792 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/tensors/tensor_benchmarks.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6432 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/tensors/tensor_benchmarks_cpu.cc
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3458 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/tensors/tensor_benchmarks_fp16_gpu.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3448 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/tensors/tensor_benchmarks_gpu.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3394 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/tensors/tensor_benchmarks_sycl.cc
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       78 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/tensors/tensor_benchmarks_sycl_include_headers.cc
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1259 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/bench/vdw_new.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.186001 mazalib-0.52.4/src/eigen3/blas/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3711 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/BandTriangularSolver.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1744 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1652 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/GeneralRank1Update.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2089 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/PackedSelfadjointProduct.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3244 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/PackedTriangularMatrixVector.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3279 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/PackedTriangularSolverVector.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      189 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/README.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2225 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/Rank2Update.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4847 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/common.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      667 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/complex_double.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      666 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/complex_single.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1539 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/double.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.206575 mazalib-0.52.4/src/eigen3/blas/f2c/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15595 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/chbmv.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13464 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/chpmv.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2394 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/complexdots.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19592 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/ctbmv.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      123 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/d_cnjg.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      681 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/datatypes.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5183 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/drotm.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6486 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/drotmg.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10554 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/dsbmv.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8391 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/dspmv.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12085 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/dtbmv.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3093 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/lsame.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      111 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/r_cnjg.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5118 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/srotm.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6351 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/srotmg.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10578 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/ssbmv.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8367 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/sspmv.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12071 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/stbmv.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15632 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/zhbmv.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13498 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/zhpmv.c
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19620 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/f2c/ztbmv.c
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.207597 mazalib-0.52.4/src/eigen3/blas/fortran/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1022 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/fortran/complexdots.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5801 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/level1_cplx_impl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4036 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/level1_impl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4389 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/level1_real_impl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12583 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/level2_cplx_impl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    25725 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/level2_impl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10805 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/level2_real_impl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    38745 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/level3_impl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      785 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/single.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.234776 mazalib-0.52.4/src/eigen3/blas/testing/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1004 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    32834 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/cblat1.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1581 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/cblat2.dat
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   119936 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/cblat2.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1069 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/cblat3.dat
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   135042 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/cblat3.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    45885 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/dblat1.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1500 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/dblat2.dat
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   115511 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/dblat2.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      902 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/dblat3.dat
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   107135 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/dblat3.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1061 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/runblastest.sh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    44410 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/sblat1.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1500 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/sblat2.dat
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   115427 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/sblat2.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      902 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/sblat3.dat
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   107045 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/sblat3.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    32839 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/zblat1.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1581 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/zblat2.dat
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   120290 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/zblat2.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1069 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/zblat3.dat
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   135497 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/testing/zblat3.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      412 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/blas/xerbla.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.267488 mazalib-0.52.4/src/eigen3/cmake/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      825 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/Eigen3Config.cmake.in
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1427 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/Eigen3ConfigLegacy.cmake.in
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2883 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/EigenConfigureTesting.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1608 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/EigenDetermineOSVersion.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1855 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/EigenDetermineVSServicePack.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    28473 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/EigenTesting.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1240 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/EigenUninstall.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      521 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindAdolc.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    45226 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindBLAS.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13411 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindBLASEXT.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2661 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindCholmod.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9993 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindComputeCpp.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2922 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindEigen2.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3950 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindEigen3.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2876 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindFFTW.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3048 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindGLEW.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      575 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindGMP.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5205 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindGSL.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      932 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindGoogleHash.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12188 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindHWLOC.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1386 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindKLU.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10182 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindLAPACK.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2928 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindMPFR.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9227 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindMetis.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14873 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindPTSCOTCH.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23911 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindPastix.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1228 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindSPQR.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12379 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindScotch.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2258 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindStandardMathLibrary.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2396 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindSuperLU.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4897 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindTriSYCL.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1788 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/FindUmfpack.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      954 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/RegexUtils.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      183 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/UseEigen3.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2480 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/cmake/language_support.cmake
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.493260 mazalib-0.52.4/src/eigen3/debug/
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.269333 mazalib-0.52.4/src/eigen3/debug/gdb/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       23 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/debug/gdb/__init__.py
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9931 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/debug/gdb/printers.py
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.271357 mazalib-0.52.4/src/eigen3/debug/msvc/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11661 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/debug/msvc/eigen.natvis
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7566 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/debug/msvc/eigen_autoexp_part.dat
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.275337 mazalib-0.52.4/src/eigen3/demos/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      309 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/CMakeLists.txt
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.279065 mazalib-0.52.4/src/eigen3/demos/mandelbrot/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      507 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/mandelbrot/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      346 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/mandelbrot/README
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7722 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/mandelbrot/mandelbrot.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1959 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/mandelbrot/mandelbrot.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.282995 mazalib-0.52.4/src/eigen3/demos/mix_eigen_and_c/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      269 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/mix_eigen_and_c/README
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4343 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/mix_eigen_and_c/binary_library.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3415 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/mix_eigen_and_c/binary_library.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1681 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/mix_eigen_and_c/example.c
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.301250 mazalib-0.52.4/src/eigen3/demos/opengl/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      722 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/opengl/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      416 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/opengl/README
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6245 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/opengl/camera.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3553 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/opengl/camera.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4100 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/opengl/gpuhelper.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7384 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/opengl/gpuhelper.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4047 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/opengl/icosphere.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      899 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/opengl/icosphere.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19848 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/opengl/quaternion_demo.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2749 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/opengl/quaternion_demo.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1815 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/opengl/trackball.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      985 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/demos/opengl/trackball.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.374209 mazalib-0.52.4/src/eigen3/doc/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11391 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/AsciiQuickReference.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2477 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/B01_Experimental.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4967 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6461 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/ClassHierarchy.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18408 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/CoeffwiseMathFunctionsTable.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4543 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/CustomizingEigen_CustomScalar.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1371 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/CustomizingEigen_InheritingMatrix.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3744 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/CustomizingEigen_NullaryExpr.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3727 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/CustomizingEigen_Plugins.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5064 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/DenseDecompositionBenchmark.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    87484 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/Doxyfile.in
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8355 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/Eigen_Silly_Professor_64x64.png
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1944 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/FixedSizeVectorizable.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13675 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/FunctionsTakingEigenTypes.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5557 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/HiPerformance.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3911 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/InplaceDecomposition.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    31085 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/InsideEigenExample.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2860 2023-10-30 16:40:18.000000 mazalib-0.52.4/src/eigen3/doc/LeastSquares.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6953 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/Manual.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      777 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/MatrixfreeSolverExample.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5753 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/NewExpressionType.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1957 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/Overview.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1206 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/PassingByValue.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6402 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/Pitfalls.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13858 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/PreprocessorDirectives.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    30486 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/QuickReference.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6678 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/QuickStartGuide.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20134 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/SparseLinearSystems.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8583 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/SparseQuickReference.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3996 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/StlContainers.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4205 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/StorageOrders.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7229 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/StructHavingEigenMembers.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6290 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TemplateKeyword.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10506 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TopicAliasing.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5393 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TopicAssertions.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1970 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TopicCMakeGuide.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      185 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TopicEigenExpressionTemplates.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6411 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TopicLazyEvaluation.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9080 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TopicLinearAlgebraDecompositions.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3681 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TopicMultithreading.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      148 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TopicResizing.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      157 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TopicScalarTypes.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      106 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TopicVectorization.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7062 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialAdvancedInitialization.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8715 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialArrayClass.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8051 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialBlockOperations.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9973 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialGeometry.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11494 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialLinearAlgebra.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4074 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialMapClass.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10079 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialMatrixArithmetic.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13973 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialMatrixClass.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12272 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialReductionsVisitorsBroadcasting.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3063 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialReshape.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2208 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialSTL.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8453 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialSlicingIndexing.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20843 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialSparse.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       93 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/TutorialSparse_example_details.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8870 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/UnalignedArrayAssert.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6766 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/UsingBlasLapackBackends.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6226 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/UsingIntelMKL.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1885 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/UsingNVCC.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2980 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/WrongStackAlignment.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8206 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/eigen_navtree_hacks.js
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4817 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/eigendoxy.css
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1480 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/eigendoxy_footer.html.in
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2302 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/eigendoxy_header.html.in
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5515 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/eigendoxy_layout.xml.in
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1154 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/eigendoxy_tabs.css
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.453519 mazalib-0.52.4/src/eigen3/doc/examples/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       36 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/.krazy
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      637 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      796 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/CustomizingEigen_Inheritance.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      198 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Cwise_erf.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      199 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Cwise_erfc.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      201 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Cwise_lgamma.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      297 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/DenseBase_middleCols_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      297 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/DenseBase_middleRows_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      298 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/DenseBase_template_int_middleCols.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      298 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/DenseBase_template_int_middleRows.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      220 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/QuickStart_example.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      320 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/QuickStart_example2_dynamic.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      304 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/QuickStart_example2_fixed.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      699 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/TemplateKeyword_flexible.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      528 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/TemplateKeyword_simple.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1650 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/TutorialInplaceLU.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      645 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/TutorialLinAlgComputeTwice.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      385 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/TutorialLinAlgExComputeSolveError.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      398 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/TutorialLinAlgExSolveColPivHouseholderQR.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      372 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/TutorialLinAlgExSolveLDLT.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      364 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/TutorialLinAlgInverseDeterminant.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      620 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/TutorialLinAlgRankRevealing.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      420 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/TutorialLinAlgSVDSolve.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      552 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      393 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/TutorialLinAlgSetThreshold.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      490 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ArrayClass_accessors.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      423 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ArrayClass_addition.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      429 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ArrayClass_cwise_other.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      466 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ArrayClass_interop.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      617 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      253 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ArrayClass_mult.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      541 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_BlockOperations_block_assignment.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      407 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_BlockOperations_colrow.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      465 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_BlockOperations_corner.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      433 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_BlockOperations_print_block.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      362 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_BlockOperations_vector.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      419 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_PartialLU_solve.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      464 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_1nn.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      377 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      381 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple_rowwise.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      260 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_colwise.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      522 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      534 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      703 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      465 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_operatornorm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      257 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_rowwise.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      557 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      702 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_simple_example_dynamic_size.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      297 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_simple_example_fixed_size.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      764 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/class_Block.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      544 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/class_CwiseBinaryOp.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      580 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/class_CwiseUnaryOp.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      391 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/class_CwiseUnaryOp_ptrfun.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      724 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/class_FixedBlock.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      489 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/class_FixedReshaped.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      700 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/class_FixedVectorBlock.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      568 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/class_Reshaped.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      802 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/class_VectorBlock.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      436 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/function_taking_eigenbase.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      613 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/function_taking_ref.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      377 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/make_circulant.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      150 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/make_circulant.cpp.entry
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      980 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/make_circulant.cpp.evaluator
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      611 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/make_circulant.cpp.expression
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      154 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/make_circulant.cpp.main
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       89 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/make_circulant.cpp.preamble
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      624 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/make_circulant.cpp.traits
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1372 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/make_circulant2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4404 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/matrixfree_cg.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2520 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/nullary_indexing.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      493 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/tut_arithmetic_add_sub.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      408 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/tut_arithmetic_dot_cross.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      631 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/tut_arithmetic_matrix_mul.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      545 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/tut_arithmetic_redux_basic.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      370 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/tut_arithmetic_scalar_mul_div.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      361 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/tut_matrix_coefficient_accessors.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      507 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/tut_matrix_resize.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      241 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/examples/tut_matrix_resize_fixed_size.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       86 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/ftv2node.png
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      229 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/ftv2pnode.png
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.753977 mazalib-0.52.4/src/eigen3/doc/snippets/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       36 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/.krazy
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      215 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/AngleAxis_mimic_euler.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       63 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Array_initializer_list_23_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       63 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Array_initializer_list_vector_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      103 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Array_variadic_ctor_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      403 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/BiCGSTAB_simple.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      419 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/BiCGSTAB_step_by_step.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1671 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      332 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/ColPivHouseholderQR_solve.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      808 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/ComplexEigenSolver_compute.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      220 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/ComplexEigenSolver_eigenvalues.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      198 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/ComplexEigenSolver_eigenvectors.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      307 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/ComplexSchur_compute.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      267 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/ComplexSchur_matrixT.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      225 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/ComplexSchur_matrixU.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       47 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_abs.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       48 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_abs2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       57 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_acos.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       88 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_arg.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      236 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_array_power_array.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       57 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_asin.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       67 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_atan.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       66 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_boolean_and.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      110 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_boolean_not.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       66 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_boolean_or.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       65 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_boolean_xor.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       95 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_ceil.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       60 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_cos.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       66 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_cosh.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       46 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_cube.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       54 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_equal_equal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       45 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_exp.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       96 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_floor.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       53 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_greater.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       54 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_greater_equal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       49 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_inverse.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      109 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_isFinite.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      106 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_isInf.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      106 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_isNaN.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       53 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_less.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       54 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_less_equal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       45 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_log.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       49 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_log10.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       56 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_max.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       56 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_min.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       41 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_minus.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       48 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_minus_equal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       54 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_not_equal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       41 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_plus.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       48 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_plus_equal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       55 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_pow.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      145 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_product.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       51 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_quotient.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       96 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_round.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       87 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_scalar_power_array.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       47 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_sign.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       60 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_sin.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       66 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_sinh.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       58 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_slash_equal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       46 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_sqrt.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       48 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_square.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       60 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_tan.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       66 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_tanh.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       58 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Cwise_times_equal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      119 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/DenseBase_LinSpaced.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      428 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/DenseBase_LinSpacedInt.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      141 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/DenseBase_LinSpaced_seq_deprecated.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       63 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/DenseBase_setLinSpaced.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      374 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/DirectionWise_hnormalized.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      190 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/DirectionWise_replicate.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      183 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/DirectionWise_replicate_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      816 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      367 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/EigenSolver_compute.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      180 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/EigenSolver_eigenvalues.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      185 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/EigenSolver_eigenvectors.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      439 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/EigenSolver_pseudoEigenvectors.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      333 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/FullPivHouseholderQR_solve.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      378 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/FullPivLU_image.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      324 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/FullPivLU_kernel.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      424 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/FullPivLU_solve.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      463 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/GeneralizedEigenSolver.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      345 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/HessenbergDecomposition_compute.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      399 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/HessenbergDecomposition_matrixH.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      491 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/HessenbergDecomposition_packedMatrix.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      307 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/HouseholderQR_householderQ.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      366 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/HouseholderQR_solve.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1347 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/HouseholderSequence_HouseholderSequence.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      617 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/IOFormat.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      623 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/JacobiSVD_basic.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      240 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Jacobi_makeGivens.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      299 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Jacobi_makeJacobi.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      531 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/LLT_example.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      464 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/LLT_solve.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      196 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/LeastSquaresNormalEquations.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      181 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/LeastSquaresQR.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      169 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Map_general_stride.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      204 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Map_inner_stride.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      141 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Map_outer_stride.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      186 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Map_placement_new.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       96 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Map_simple.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      172 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_adjoint.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      530 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_all.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      214 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_applyOnTheLeft.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      301 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_applyOnTheRight.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       74 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_array.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      238 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_array_const.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       57 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_asDiagonal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      249 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_block_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      255 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_block_int_int_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      277 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_bottomLeftCorner_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      280 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_bottomRightCorner_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      248 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_bottomRows_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      122 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_cast.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       85 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_col.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      292 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_colwise.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      481 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_colwise_iterator_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      423 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_computeInverseAndDetWithCheck.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      329 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_computeInverseWithCheck.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       84 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_cwiseAbs.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       85 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_cwiseAbs2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      283 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_cwiseEqual.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       91 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_cwiseInverse.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       62 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_cwiseMax.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       62 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_cwiseMin.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      293 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_cwiseNotEqual.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      157 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_cwiseProduct.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       67 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_cwiseQuotient.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       84 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_cwiseSign.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       52 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_cwiseSqrt.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      192 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_diagonal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      275 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_diagonal_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      279 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_diagonal_template_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      163 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_eigenvalues.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      231 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_end_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      479 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_eval.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      279 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_fixedBlock_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      381 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_hnormalized.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      491 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_homogeneous.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       51 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_identity.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       43 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_identity_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      148 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_inverse.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      247 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_isDiagonal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      240 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_isIdentity.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      221 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_isOnes.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      299 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_isOrthogonal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      236 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_isUnitary.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      220 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_isZero.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      242 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_leftCols_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      132 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_noalias.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       77 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_ones.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       79 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_ones_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_ones_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      135 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_operatorNorm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      174 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_prod.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       43 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_random.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_random_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       40 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_random_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      174 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_replicate.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      167 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_replicate_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      295 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_reshaped_auto.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      181 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_reshaped_fixed.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      163 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_reshaped_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      291 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_reshaped_to_vector.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      415 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_reverse.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      245 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_rightCols_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       85 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_row.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      286 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_rowwise.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      249 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_segment_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      121 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_select.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      367 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_selfadjointView.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      303 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_set.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       86 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_setIdentity.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       75 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_setOnes.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       75 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_setRandom.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       75 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_setZero.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      231 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_start_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      254 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_bottomRows.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      235 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_end.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      269 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_int_block_int_int_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      280 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      307 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      283 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_int_bottomRightCorner.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      310 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_int_bottomRightCorner_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      271 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_int_topLeftCorner.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      298 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_int_topLeftCorner_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      274 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_int_topRightCorner.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      301 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_int_topRightCorner_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      248 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_leftCols.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      251 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_rightCols.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      249 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_segment.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      235 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_start.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      245 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_template_int_topRows.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      268 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_topLeftCorner_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      271 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_topRightCorner_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      239 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_topRows_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      422 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_transpose.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      582 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_triangularView.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       73 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_zero.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       75 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_zero_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       38 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_zero_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      164 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_Map_stride.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       63 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_initializer_list_23_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       40 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_initializer_list_vector_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      114 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_resize_NoChange_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      241 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_resize_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      114 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_resize_int_NoChange.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      416 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_resize_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       55 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_setConstant_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       58 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_setConstant_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       55 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_setIdentity_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       48 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_setOnes_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       51 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_setOnes_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       50 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_setRandom_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       53 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_setRandom_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       48 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_setZero_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       51 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_setZero_int_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      105 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Matrix_variadic_ctor_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      379 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/PartialPivLU_solve.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      268 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/PartialRedux_count.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      179 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/PartialRedux_maxCoeff.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      179 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/PartialRedux_minCoeff.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      172 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/PartialRedux_norm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      172 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/PartialRedux_prod.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      183 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/PartialRedux_squaredNorm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      167 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/PartialRedux_sum.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      836 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/RealQZ_compute.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      439 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/RealSchur_RealSchur_MatrixType.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      349 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/RealSchur_compute.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      369 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      833 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      842 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      372 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      405 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      184 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointEigenSolver_eigenvalues.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      197 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointEigenSolver_eigenvectors.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      435 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointEigenSolver_operatorInverseSqrt.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      371 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointEigenSolver_operatorSqrt.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      187 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointView_eigenvalues.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      160 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointView_operatorNorm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      169 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Slicing_arrayexpr.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      379 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Slicing_custom_padding_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      193 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Slicing_rawarray_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      166 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Slicing_stdvector_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      420 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/SparseMatrix_coeffs.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      274 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/TopicAliasing_block.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      277 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/TopicAliasing_block_correct.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      611 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/TopicAliasing_cwise.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       80 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/TopicAliasing_mult1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      240 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/TopicAliasing_mult2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       90 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/TopicAliasing_mult3.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      105 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/TopicAliasing_mult4.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      114 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/TopicAliasing_mult5.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      543 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/TopicStorageOrders_example.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      531 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Triangular_solve.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      454 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tridiagonalization_Tridiagonalization_MatrixType.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      401 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tridiagonalization_compute.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      485 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tridiagonalization_decomposeInPlace.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      565 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tridiagonalization_diagonal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      309 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tridiagonalization_householderCoefficients.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      402 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tridiagonalization_packedMatrix.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      137 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_Block.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      172 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_CommaTemporary.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      277 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_Join.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      279 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_LinSpaced.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      898 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      345 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_Zero.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      306 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_Map_rowmajor.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      917 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_Map_using.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      175 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_ReshapeMat2Mat.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      308 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_ReshapeMat2Vec.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      620 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_SlicingCol.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      182 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_SlicingVec.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       75 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_commainit_01.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      118 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_commainit_01b.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      222 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_commainit_02.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      119 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_range_for_loop_1d_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      151 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_range_for_loop_2d_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      252 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_reshaped_vs_resize_1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      378 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_reshaped_vs_resize_2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      152 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_solve_matrix_inverse.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      328 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_solve_multiple_rhs.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      381 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_solve_reuse_decomposition.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      265 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_solve_singular.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      281 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_solve_triangular.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      165 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_solve_triangular_inplace.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      205 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_std_sort.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      221 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_std_sort_rows_cxx11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      467 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/VectorwiseOp_homogeneous.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      546 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/Vectorwise_reverse.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      748 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/class_FullPivLU.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      526 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/compile_snippet.cpp.in
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      480 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/tut_arithmetic_redux_minmax.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      191 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/tut_arithmetic_transpose_aliasing.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      289 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/tut_arithmetic_transpose_conjugate.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      178 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/tut_arithmetic_transpose_inplace.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      198 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/snippets/tut_matrix_assignment_resizing.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.758626 mazalib-0.52.4/src/eigen3/doc/special_examples/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1176 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/special_examples/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1222 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/special_examples/Tutorial_sparse_example.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1620 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/special_examples/Tutorial_sparse_example_details.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      350 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/special_examples/random_cpp11.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2606 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/doc/tutorial.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      263 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/eigen3.pc.in
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.814164 mazalib-0.52.4/src/eigen3/failtest/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2493 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      259 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/bdcsvd_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      248 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/block_nonconst_ctor_on_const_xpr_0.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      248 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/block_nonconst_ctor_on_const_xpr_1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      277 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/block_nonconst_ctor_on_const_xpr_2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      278 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/block_on_const_type_actually_const_0.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      278 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/block_on_const_type_actually_const_1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      271 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/colpivqr_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      260 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/const_qualified_block_method_retval_0.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      255 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/const_qualified_block_method_retval_1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      254 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/const_qualified_diagonal_method_retval.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      256 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/const_qualified_transpose_method_retval.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      286 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/cwiseunaryview_nonconst_ctor_on_const_xpr.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      312 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/cwiseunaryview_on_const_type_actually_const.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      243 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/diagonal_nonconst_ctor_on_const_xpr.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      266 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/diagonal_on_const_type_actually_const.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      290 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/eigensolver_cplx.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      273 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/eigensolver_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      161 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/failtest_sanity_check.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      261 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/fullpivlu_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      272 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/fullpivqr_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      197 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/initializer_list_1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      238 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/initializer_list_2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      262 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/jacobisvd_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      264 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/ldlt_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      262 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/llt_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      239 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/map_nonconst_ctor_on_const_ptr_0.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      261 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/map_nonconst_ctor_on_const_ptr_1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      285 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/map_nonconst_ctor_on_const_ptr_2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      329 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/map_nonconst_ctor_on_const_ptr_3.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      336 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/map_nonconst_ctor_on_const_ptr_4.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      264 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/map_on_const_type_actually_const_0.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      256 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/map_on_const_type_actually_const_1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      264 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/partialpivlu_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      265 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/qr_int.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      281 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/ref_1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      228 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/ref_2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      246 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/ref_3.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      242 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/ref_4.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      254 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/ref_5.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      256 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/selfadjointview_nonconst_ctor_on_const_xpr.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      282 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/selfadjointview_on_const_type_actually_const.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      320 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/sparse_ref_1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      253 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/sparse_ref_2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      286 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/sparse_ref_3.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      250 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/sparse_ref_4.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      301 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/sparse_ref_5.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      306 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/sparse_storage_mismatch.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      231 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/swap_1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      223 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/swap_2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      226 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/ternary_1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      238 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/ternary_2.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      244 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/transpose_nonconst_ctor_on_const_xpr.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      270 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/transpose_on_const_type_actually_const.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      253 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/triangularview_nonconst_ctor_on_const_xpr.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      281 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/failtest/triangularview_on_const_type_actually_const.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.864695 mazalib-0.52.4/src/eigen3/lapack/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11422 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2277 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/cholesky.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2947 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/clacgv.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2437 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/cladiv.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6527 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/clarf.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24195 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/clarfb.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5547 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/clarfg.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10778 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/clarft.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      596 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/complex_double.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      595 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/complex_single.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3097 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/dladiv.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5448 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/dlamch.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2618 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/dlapy2.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2848 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/dlapy3.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6394 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/dlarf.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23511 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/dlarfb.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5142 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/dlarfg.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10548 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/dlarft.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      580 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/double.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1334 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/dsecnd_NONE.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1888 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/eigenvalues.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3075 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/ilaclc.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3118 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/ilaclr.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3070 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/iladlc.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3121 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/iladlr.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3059 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/ilaslc.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3109 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/ilaslr.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3080 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/ilazlc.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3131 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/ilazlr.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      906 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/lapack_common.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2744 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/lu.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1310 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/second_NONE.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      579 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/single.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3025 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/sladiv.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5453 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/slamch.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2594 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/slapy2.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2812 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/slapy3.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6344 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/slarf.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23490 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/slarfb.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5104 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/slarfg.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10509 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/slarft.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5029 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/svd.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2955 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/zlacgv.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2461 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/zladiv.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6510 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/zlarf.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24272 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/zlarfb.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5562 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/zlarfg.f
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10780 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/lapack/zlarft.f
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:07.875846 mazalib-0.52.4/src/eigen3/scripts/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      334 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/scripts/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      599 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/scripts/buildtests.in
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1615 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/scripts/cdashtesting.cmake.in
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      691 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/scripts/check.in
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       47 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/scripts/debug.in
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6616 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/scripts/eigen_gen_credits.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      762 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/scripts/eigen_gen_docs
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      333 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/scripts/eigen_gen_split_test_help.cmake
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1034 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/scripts/eigen_monitor_perf.sh
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       49 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/scripts/release.in
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2437 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/scripts/relicense.py
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      217 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/signature_of_eigen3_matrix_library
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.043912 mazalib-0.52.4/src/eigen3/test/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5665 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/AnnoyingScalar.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14389 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8887 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/adjoint.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22072 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/array_cwise.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13190 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/array_for_matrix.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      993 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/array_of_string.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2423 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/array_replicate.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6587 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/array_reverse.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2503 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/bandmatrix.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11407 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/basicstuff.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4516 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/bdcsvd.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1507 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/bicgstab.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15132 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/block.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5892 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/boostmultiprec.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      187 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/bug1213.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      155 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/bug1213.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      297 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/bug1213_main.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18872 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/cholesky.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3446 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/cholmod_support.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3037 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/commainitializer.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1577 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/conjugate_gradient.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5344 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/conservative_resize.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2660 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/constructor.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6565 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/corners.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2097 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/ctorleak.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5252 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/denseLM.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3881 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/dense_storage.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2341 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/determinant.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4220 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/diagonal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6871 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/diagonal_matrix_variadic_ctor.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7704 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/diagonalmatrices.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2291 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/dontalign.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4937 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/dynalloc.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2261 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/eigen2support.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6397 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/eigensolver_complex.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4149 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/eigensolver_generalized_real.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9706 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/eigensolver_generic.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11304 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/eigensolver_selfadjoint.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/evaluator_common.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21563 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/evaluators.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1965 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/exceptions.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5355 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/fastmath.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1925 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/first_aligned.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6089 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/geo_alignedbox.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3674 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/geo_eulerangles.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5595 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/geo_homogeneous.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7761 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/geo_hyperplane.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4971 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/geo_orthomethods.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5353 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/geo_parametrizedline.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11872 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/geo_quaternion.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26166 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/geo_transformations.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7254 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/gpu_basic.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5224 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/gpu_common.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11914 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/half_float.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2466 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/hessenberg.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6434 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/householder.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2692 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/incomplete_cholesky.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19079 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/indexed_view.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13127 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/initializer_list_construction.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3990 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/inplace_decomposition.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5937 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/integer_types.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4755 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/inverse.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1409 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/is_same_dense.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2813 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/jacobi.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5771 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/jacobisvd.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      987 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/klu_support.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6277 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/linearstructure.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1536 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/lscg.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9327 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/lu.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    33626 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/main.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8150 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/mapped_matrix.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7648 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/mapstaticmethods.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10354 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/mapstride.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7494 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/meta.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      776 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/metis_support.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1835 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/miscmatrices.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18088 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/mixingtypes.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      659 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/mpl2only.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1245 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/nestbyvalue.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4484 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/nesting_ops.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8928 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/nomalloc.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13147 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/nullary.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3302 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/num_dimensions.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1766 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/numext.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    38925 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/packetmath.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      984 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/pardiso_support.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1956 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/pastix_support.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7212 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/permutationmatrices.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3287 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/prec_inverse_4x4.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12139 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/product.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14926 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/product_extra.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4862 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/product_large.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4553 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/product_mmtr.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11197 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/product_notemporary.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3596 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/product_selfadjoint.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12234 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/product_small.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6258 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/product_symm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8002 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/product_syrk.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7058 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/product_trmm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4340 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/product_trmv.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6229 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/product_trsolve.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4803 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/qr.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14235 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/qr_colpivoting.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5759 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/qr_fullpivoting.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4777 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/qtvector.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4491 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/rand.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3196 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/real_qz.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8422 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/redux.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12060 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/ref.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10922 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/reshape.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1146 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/resize.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4424 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/rvalue_types.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3660 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/schur_complex.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4074 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/schur_real.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2494 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/selfadjoint.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2270 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/simplicial_cholesky.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2085 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sizeof.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2703 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sizeoverflow.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2200 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/smallvectors.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1752 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/solverbase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6500 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sparse.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4916 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sparseLM.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29569 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sparse_basic.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12423 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sparse_block.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10233 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sparse_permutations.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26049 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sparse_product.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6264 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sparse_ref.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19769 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sparse_solver.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5267 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sparse_solvers.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5250 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sparse_vector.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1836 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sparselu.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4736 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/sparseqr.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1820 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/special_numbers.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   165510 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/split_test_helper.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1905 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/spqr_support.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10374 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/stable_norm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4390 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/stddeque.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4896 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/stddeque_overload.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4362 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/stdlist.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6044 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/stdlist_overload.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5274 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/stdvector.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5175 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/stdvector_overload.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16845 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/stl_iterators.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      979 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/superlu_support.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19275 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/svd_common.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4168 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/svd_fill.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3034 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/swap.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2826 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/symbolic_index.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12210 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/triangular.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2072 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/type_alias.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6042 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/umeyama.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1205 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/umfpack_support.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6045 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/unalignedassert.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2625 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/unalignedcount.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1759 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/upperbidiagonalization.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21414 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/vectorization_logic.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11787 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/vectorwiseop.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4135 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/visitor.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3845 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/test/zerosized.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.045500 mazalib-0.52.4/src/eigen3/unsupported/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      272 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/CMakeLists.txt
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.068633 mazalib-0.52.4/src/eigen3/unsupported/Eigen/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4403 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/AdolcForward
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6454 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/AlignedVector3
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      960 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/ArpackSupport
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1227 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/AutoDiff
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5618 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/BVH
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      635 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CMakeLists.txt
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.073183 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      315 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4759 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/Tensor
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1309 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/TensorSymmetry
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2205 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/ThreadPool
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.498725 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.181084 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    64351 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/README.md
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21825 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12891 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6116 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMaxSycl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10877 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    57454 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12682 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    50233 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlockV2.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    43466 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22995 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16716 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    46416 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2748 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      231 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    64859 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24002 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24756 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    71697 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17980 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    49791 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29339 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8856 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13645 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4981 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      221 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3531 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12393 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    36824 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15544 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7910 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18240 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8884 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    40663 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    31651 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16503 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    25072 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15665 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8070 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8505 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15029 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11457 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1349 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3907 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1195 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2639 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    28554 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26365 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9399 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2798 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9304 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8658 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2881 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15064 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8612 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    47194 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26691 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11823 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13524 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    50912 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      227 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    35222 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10007 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15325 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17970 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11500 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18419 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5246 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14524 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4024 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSycl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8991 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclConvertToDeviceExpression.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26700 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExprConstructor.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15800 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractAccessor.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24014 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractFunctors.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16137 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclFunctors.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8058 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclLeafCount.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11408 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclPlaceHolderExpr.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4439 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclRun.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9995 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclTuple.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10513 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10200 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7801 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    30215 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.185647 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11150 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9322 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13359 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.187127 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21715 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.199629 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2180 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9370 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17189 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9602 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      797 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1249 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11783 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1728 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      735 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.204916 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/util/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23218 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4231 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8416 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4332 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1169 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/EulerAngles
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14535 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/FFT
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1472 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/IterativeSolvers
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      980 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/KroneckerProduct
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1287 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/LevenbergMarquardt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7869 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/MPRealSupport
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18423 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/MatrixFunctions
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      616 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/MoreVectorization
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6103 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/NonLinearOptimization
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1835 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/NumericalDiff
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19394 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/OpenGLSupport
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4932 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/Polynomials
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      969 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/Skyline
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1377 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/SparseExtra
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2221 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/SpecialFunctions
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1031 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/Splines
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.504463 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.208443 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/AutoDiff/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3258 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29909 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9249 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.211051 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/BVH/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13269 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9389 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/BVH/KdBVH.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.212551 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Eigenvalues/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    29865 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.216378 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/EulerAngles/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      180 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/EulerAngles/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15722 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11925 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.218824 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/FFT/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9532 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12693 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.227357 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5581 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18280 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10544 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2610 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5508 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12664 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6046 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.228581 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/KroneckerProduct/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10535 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.235420 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2246 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2527 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6850 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5199 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6993 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13693 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.243045 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17065 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23240 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17930 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    24127 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14483 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2224 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.244231 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MoreVectorization/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3130 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.257827 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20429 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22792 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1930 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1985 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3404 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2304 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9409 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3355 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1111 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3182 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1411 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.260319 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NumericalDiff/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4150 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.264632 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Polynomials/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8113 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Polynomials/Companion.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16111 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4949 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.273930 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11717 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    31967 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7957 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11148 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8225 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3242 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.283852 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4382 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    41395 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14148 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8708 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7815 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12168 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.297735 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10301 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12998 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2610 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    71584 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5424 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7861 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12030 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2957 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    59028 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3792 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.504201 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.299193 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11233 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/GpuSpecialFunctions.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.303334 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Splines/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    18814 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Splines/Spline.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16853 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4405 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1926 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/README.txt
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.304665 mazalib-0.52.4/src/eigen3/unsupported/bench/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4029 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/bench/bench_svd.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.307685 mazalib-0.52.4/src/eigen3/unsupported/doc/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      118 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      858 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/Overview.dox
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5460 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/eigendoxy_layout.xml.in
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.324226 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2158 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/BVH_Example.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      687 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1893 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/EulerAngles.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2640 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/FFT.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      372 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/MatrixExponential.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      492 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/MatrixFunction.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      390 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/MatrixLogarithm.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      380 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/MatrixPower.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      441 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/MatrixPower_optimal.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      528 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/MatrixSine.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      544 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/MatrixSinh.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      450 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/MatrixSquareRoot.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2445 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/PolynomialSolver1.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      655 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/examples/PolynomialUtils1.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.325487 mazalib-0.52.4/src/eigen3/unsupported/doc/snippets/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1163 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/doc/snippets/CMakeLists.txt
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.472647 mazalib-0.52.4/src/eigen3/unsupported/test/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7412 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/BVH.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13045 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/CMakeLists.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9919 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/EulerAngles.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       49 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/FFT.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9495 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/FFTW.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    66446 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/NonLinearOptimization.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2976 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/NumericalDiff.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2392 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/alignedvector3.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11379 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/autodiff.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3044 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/autodiff_scalar.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16779 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/bessel_functions.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4132 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_eventcount.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1916 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_maxsizevector.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19097 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_meta.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5164 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_non_blocking_thread_pool.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7259 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_runqueue.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9444 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_argmax.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9139 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_argmax_gpu.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9843 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_argmax_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10077 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_assign.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23668 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_block_access.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    30298 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_block_eval.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16430 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_block_io.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5852 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_broadcast_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9540 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_broadcasting.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17638 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_builtins_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2499 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_cast_float16_gpu.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3114 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_casts.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13475 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_chipping.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26697 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_chipping_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2075 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_comparisons.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2938 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6822 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_complex_gpu.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4767 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_concatenation.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8591 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_concatenation_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1722 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_const.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7568 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_contract_gpu.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12913 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_contract_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    23634 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_contraction.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5531 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_convolution.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    20502 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_convolution_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2618 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_custom_index.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3322 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_custom_op.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6773 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_custom_op_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13891 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_device.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3287 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_device_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2666 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_dimension.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1039 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_empty.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    31406 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_executor.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10692 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_expr.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14021 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_fft.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7513 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_fixed_size.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2246 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_forced_eval.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3431 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2357 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_generator.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5879 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_generator_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    60089 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_gpu.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6096 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_ifft.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    36846 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_image_patch.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    63203 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_image_patch_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    19037 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_index_list.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2190 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_inflation.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5237 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_inflation_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4276 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_intdiv.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3413 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_io.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1700 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_layout_swap.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4856 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      992 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_lvalue.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8289 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_map.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1039 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_math.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1554 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_mixed_indices.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16867 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_morphing.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11272 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_morphing_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1996 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_move.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1681 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_notification.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2996 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_of_complex.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2535 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_of_const_values.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    22284 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_of_float16_gpu.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3918 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_of_strings.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2745 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_padding.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5834 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_padding_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5671 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_patch.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9634 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_patch_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2232 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_random.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2441 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_random_gpu.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    15797 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_reduction.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5564 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_reduction_gpu.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7986 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_reduction_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6970 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_ref.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5475 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_reverse.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8666 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_reverse_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1548 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_roundings.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3088 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_scan.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2654 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_scan_gpu.cu
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6504 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_shuffling.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4227 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_shuffling_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9951 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_simple.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3143 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_striding.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7277 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_striding_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1977 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_sugar.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11350 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    59897 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_symmetry.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4386 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_thread_local.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    26212 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_thread_pool.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5275 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_trace.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5886 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_uint128.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4719 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_volume_patch.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12209 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1310 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/dgmres.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3963 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/forward_adolc.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1276 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/gmres.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9327 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/kronecker_product.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    56981 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/levenberg_marquardt.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4558 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/matrix_exponential.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6653 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/matrix_function.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2173 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/matrix_functions.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7382 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/matrix_power.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1081 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/matrix_square_root.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1702 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/minres.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.473879 mazalib-0.52.4/src/eigen3/unsupported/test/mpreal/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   121580 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/mpreal/mpreal.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2448 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/mpreal_support.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10929 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/openglsupport.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7718 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/polynomialsolver.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3695 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/polynomialutils.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7378 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/sparse_extra.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    21638 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/special_functions.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     8810 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/eigen3/unsupported/test/splines.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.509331 mazalib-0.52.4/src/mazalib/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    17957 2024-03-09 14:30:24.000000 mazalib-0.52.4/src/mazalib/mazalib.cpp
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.479750 mazalib-0.52.4/src/mazalib.egg-info/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4543 2024-04-17 15:14:05.000000 mazalib-0.52.4/src/mazalib.egg-info/PKG-INFO
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    84583 2024-04-17 15:14:06.000000 mazalib-0.52.4/src/mazalib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)        1 2024-04-17 15:14:05.000000 mazalib-0.52.4/src/mazalib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      208 2024-04-17 15:14:05.000000 mazalib-0.52.4/src/mazalib.egg-info/entry_points.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)        6 2024-04-17 15:14:05.000000 mazalib-0.52.4/src/mazalib.egg-info/requires.txt
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       28 2024-04-17 15:14:05.000000 mazalib-0.52.4/src/mazalib.egg-info/top_level.txt
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.480481 mazalib-0.52.4/src/segmentation/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/segmentation/__init__.py
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:08.507284 mazalib-0.52.4/src/segmentation/include/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1039 2023-10-22 16:19:07.000000 mazalib-0.52.4/src/segmentation/include/BinaryIO.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1577 2023-10-22 18:31:46.000000 mazalib-0.52.4/src/segmentation/include/CACSegmentation.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      464 2023-10-17 22:32:20.000000 mazalib-0.52.4/src/segmentation/include/Config.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2665 2023-10-22 17:25:22.000000 mazalib-0.52.4/src/segmentation/include/DenoiseParameters.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11817 2023-10-27 18:53:57.000000 mazalib-0.52.4/src/segmentation/include/DynamicArray.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      727 2023-10-22 16:40:40.000000 mazalib-0.52.4/src/segmentation/include/ExpectedMaximized.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3090 2023-10-17 22:32:20.000000 mazalib-0.52.4/src/segmentation/include/Grid.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    34871 2024-02-16 13:59:27.000000 mazalib-0.52.4/src/segmentation/include/HessianSegmentation.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     6256 2023-10-17 22:32:20.000000 mazalib-0.52.4/src/segmentation/include/IntegralImage.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     4958 2023-10-22 17:38:45.000000 mazalib-0.52.4/src/segmentation/include/IterativeNonLocalMeansCPU.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3117 2024-03-28 14:16:36.000000 mazalib-0.52.4/src/segmentation/include/KrigingSegmentation.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2265 2024-02-15 13:48:10.000000 mazalib-0.52.4/src/segmentation/include/LatticeModel.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2867 2023-10-17 22:32:20.000000 mazalib-0.52.4/src/segmentation/include/LogFile.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    16800 2024-02-16 13:59:27.000000 mazalib-0.52.4/src/segmentation/include/MRFSegmentation.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      865 2023-10-17 22:32:20.000000 mazalib-0.52.4/src/segmentation/include/MRFUtils.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5807 2023-10-17 22:32:20.000000 mazalib-0.52.4/src/segmentation/include/NelderMead.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11440 2023-10-22 17:26:14.000000 mazalib-0.52.4/src/segmentation/include/NewCACSegmentation.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1213 2023-10-22 17:38:57.000000 mazalib-0.52.4/src/segmentation/include/NoiseLevel.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      783 2023-10-22 17:13:57.000000 mazalib-0.52.4/src/segmentation/include/NonLocalMeans.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1899 2023-10-22 17:42:50.000000 mazalib-0.52.4/src/segmentation/include/Point.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2424 2024-03-09 11:11:31.000000 mazalib-0.52.4/src/segmentation/include/Point3d.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      715 2023-10-27 18:11:54.000000 mazalib-0.52.4/src/segmentation/include/RandomNumbers.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13861 2023-10-22 14:19:52.000000 mazalib-0.52.4/src/segmentation/include/RegionGrowthSegmentation.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     5297 2024-02-13 11:25:07.000000 mazalib-0.52.4/src/segmentation/include/Variation.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    42272 2023-10-27 18:11:46.000000 mazalib-0.52.4/src/segmentation/include/threshold.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7849 2023-10-22 18:19:36.000000 mazalib-0.52.4/src/segmentation/include/util.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    10339 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/segmentation/include/var_2d.h
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    12673 2023-10-30 16:40:19.000000 mazalib-0.52.4/src/segmentation/include/var_3d.h
+drwxrwxrwx   0 andrey    (1000) andrey    (1000)        0 2024-04-17 15:14:06.525034 mazalib-0.52.4/src/segmentation/src/
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    11189 2023-10-22 18:31:38.000000 mazalib-0.52.4/src/segmentation/src/CACSegmentation.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2513 2023-10-22 16:40:00.000000 mazalib-0.52.4/src/segmentation/src/ExpectedMaximized.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     9675 2020-09-29 10:07:48.000000 mazalib-0.52.4/src/segmentation/src/Grid.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2555 2020-09-29 10:07:48.000000 mazalib-0.52.4/src/segmentation/src/HessianSegmentation.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      872 2020-09-29 10:07:48.000000 mazalib-0.52.4/src/segmentation/src/IntegralImage.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)   105044 2023-10-22 17:23:50.000000 mazalib-0.52.4/src/segmentation/src/IterativeNonLocalMeansCPU.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    13772 2024-03-28 14:16:40.000000 mazalib-0.52.4/src/segmentation/src/KrigingSegmentation.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     7402 2024-02-15 17:05:48.000000 mazalib-0.52.4/src/segmentation/src/LatticeModel.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)      183 2021-01-18 05:35:22.000000 mazalib-0.52.4/src/segmentation/src/LogFile.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14065 2020-09-29 10:07:48.000000 mazalib-0.52.4/src/segmentation/src/MRFSegmentation.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)       33 2020-09-29 10:07:48.000000 mazalib-0.52.4/src/segmentation/src/NewCACSegmentation.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)    14464 2023-10-22 17:14:57.000000 mazalib-0.52.4/src/segmentation/src/NoiseLevel.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1898 2023-10-22 17:24:03.000000 mazalib-0.52.4/src/segmentation/src/NonLocalMeans.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     2231 2020-09-29 10:07:48.000000 mazalib-0.52.4/src/segmentation/src/RandomNumbers.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     1016 2024-02-13 11:32:43.000000 mazalib-0.52.4/src/segmentation/src/Variation.cpp
+-rwxrwxrwx   0 andrey    (1000) andrey    (1000)     3513 2023-10-22 18:20:20.000000 mazalib-0.52.4/src/segmentation/src/threshold.cpp
```

### Comparing `mazalib-0.52.3/LICENSE.txt` & `mazalib-0.52.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/setup.py` & `mazalib-0.52.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,64 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 import os
-import glob
-from sys import argv
-import pathlib
-isST=True
 from setuptools import setup, Extension, find_packages
-from os import listdir
-from os.path import isfile, join
-import platform
-systemName=platform.system()
-import sys
-is_64bits = sys.maxsize > 2**32
+import pip
 
 from setuptools.command.build_ext import build_ext as build_ext_orig
 
 
-version='0.52.3'
+version='0.52.4'
 libName="mazalib"
 
 file_dir_path = os.path.dirname(os.path.realpath(__file__))
 
 def package_files(directory):
     return [os.path.join(p,f) for p,d,files in os.walk(directory) for f in files]
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 short_description = "Cross-platform 2d/3d image segmentation C++ library"
 
 language="c++"
 extra_compile_args=['-O3', '-w', '-std=c++11']
-# extra_link_args=['-std=c++11','_GLIBCXX_USE_CXX11_ABI=0']
-# extraFlags=['-fpermissive','-std=c++11']
 installRequiresList=['numpy']
 entry_points_Command={'main_library': ['kriging = mazalib:kriging',
                                        'mrf = mazalib:mrf',
                                        'rgs = mazalib:rgs',
                                        'hessian = mazalib:hessian',
                                        'windowedHessian = mazalib:windowedHessian',
                                        'nlm = mazalib:nlm',
                                        'unsharp = mazalib:unsharp',
 									   'cac = mazalib:cac']}
 license='GPLv3'
 author='Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina, Andrey A. Ananev'
-author_email='mathieu.gravey@unil.ch'
+author_email='andrey.ananev@phystech.edu'
 
 classifiers=[
 			'Development Status :: 3 - Alpha',
 			'Intended Audience :: Science/Research',
 			'Intended Audience :: Education',
 			'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
 			'Programming Language :: C++',
 			'Programming Language :: Python :: 3 :: Only'
-			# 'Operating System :: OS Independent',
 		]
 
 packages=find_packages('src',include=['mazalib*']) + ['segmentation', 'eigen3']
 
 eigen_path=os.path.join(file_dir_path,"src","eigen3","")
 eigen_package_files=package_files(eigen_path)
 
 
 
 os.environ["CXX"]='g++'
 os.environ["CC"]='gcc'
 
+pip.main(['install', 'numpy'])
+
 class get_numpy_include(object):
     """Defer numpy.get_include() until after numpy is installed."""
 
     def __str__(self):
         import numpy
         return numpy.get_include()
 
@@ -78,21 +68,21 @@
 						extra_compile_args=extra_compile_args,
 						include_dirs=["./src/segmentation/include/", "./src/eigen3/", get_numpy_include()])
 setup(
 	name=libName,
 	version=version,
 	description=short_description,
 	long_description=long_description,
+    long_description_content_type="text/markdown",
 	author=author,
 	author_email=author_email,
 	license=license,
 	packages=packages,
 	package_dir={'': 'src'},
 	package_data={'segmentation': ['./src/*.cpp', './include/*.h'],
 					'eigen3': eigen_package_files},
 	classifiers=classifiers,
-	# ext_package = libName,
 	ext_modules=[mazalib_module],
 	setup_requires=installRequiresList,
 	install_requires=installRequiresList,
 	entry_points=entry_points_Command
 )
```

### Comparing `mazalib-0.52.3/src/eigen3/.hgtags` & `mazalib-0.52.4/src/eigen3/.hgtags`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/COPYING.BSD` & `mazalib-0.52.4/src/eigen3/COPYING.BSD`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/COPYING.GPL` & `mazalib-0.52.4/src/eigen3/COPYING.GPL`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/COPYING.LGPL` & `mazalib-0.52.4/src/eigen3/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/COPYING.MINPACK` & `mazalib-0.52.4/src/eigen3/COPYING.MINPACK`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/COPYING.MPL2` & `mazalib-0.52.4/src/eigen3/COPYING.MPL2`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/COPYING.README` & `mazalib-0.52.4/src/eigen3/COPYING.README`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/CTestConfig.cmake` & `mazalib-0.52.4/src/eigen3/CTestConfig.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/Cholesky` & `mazalib-0.52.4/src/eigen3/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/CholmodSupport` & `mazalib-0.52.4/src/eigen3/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/Core` & `mazalib-0.52.4/src/eigen3/Eigen/Core`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/Eigenvalues` & `mazalib-0.52.4/src/eigen3/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/Geometry` & `mazalib-0.52.4/src/eigen3/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/Householder` & `mazalib-0.52.4/src/eigen3/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/IterativeLinearSolvers` & `mazalib-0.52.4/src/eigen3/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/Jacobi` & `mazalib-0.52.4/src/eigen3/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/KLUSupport` & `mazalib-0.52.4/src/eigen3/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/LU` & `mazalib-0.52.4/src/eigen3/Eigen/LU`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/MetisSupport` & `mazalib-0.52.4/src/eigen3/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/OrderingMethods` & `mazalib-0.52.4/src/eigen3/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/PaStiXSupport` & `mazalib-0.52.4/src/eigen3/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/PardisoSupport` & `mazalib-0.52.4/src/eigen3/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/QR` & `mazalib-0.52.4/src/eigen3/Eigen/QR`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/QtAlignedMalloc` & `mazalib-0.52.4/src/eigen3/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/SPQRSupport` & `mazalib-0.52.4/src/eigen3/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/SVD` & `mazalib-0.52.4/src/eigen3/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/Sparse` & `mazalib-0.52.4/src/eigen3/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/SparseCholesky` & `mazalib-0.52.4/src/eigen3/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/SparseCore` & `mazalib-0.52.4/src/eigen3/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/SparseLU` & `mazalib-0.52.4/src/eigen3/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/SparseQR` & `mazalib-0.52.4/src/eigen3/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/StdDeque` & `mazalib-0.52.4/src/eigen3/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/StdList` & `mazalib-0.52.4/src/eigen3/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/StdVector` & `mazalib-0.52.4/src/eigen3/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/SuperLUSupport` & `mazalib-0.52.4/src/eigen3/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/UmfPackSupport` & `mazalib-0.52.4/src/eigen3/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Cholesky/LDLT.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Cholesky/LLT.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/ArithmeticSequence.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Array.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/ArrayBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/ArrayWrapper.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Assign.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/AssignEvaluator.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Assign_MKL.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/BandMatrix.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Block.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/BooleanRedux.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/CommaInitializer.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/ConditionEstimator.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/CoreEvaluators.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/CoreIterators.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/CwiseBinaryOp.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/CwiseNullaryOp.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/CwiseTernaryOp.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/CwiseUnaryOp.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/CwiseUnaryView.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/DenseBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/DenseCoeffsBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/DenseStorage.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Diagonal.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/DiagonalMatrix.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/DiagonalProduct.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Dot.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/EigenBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/ForceAlignedAccess.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Fuzzy.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/GeneralProduct.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/GenericPacketMath.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/GlobalFunctions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/IO.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/IndexedView.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Inverse.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Map.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/MapBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/MathFunctions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/MathFunctionsImpl.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Matrix.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/MatrixBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/NestByValue.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/NoAlias.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/NumTraits.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/PartialReduxEvaluator.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/PermutationMatrix.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/PlainObjectBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Product.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/ProductEvaluators.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Random.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Redux.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Ref.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Replicate.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Reshaped.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/ReturnByValue.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Reverse.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Select.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/SelfAdjointView.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Solve.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/SolveTriangular.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/SolverBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/StableNorm.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/StlIterators.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Stride.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Swap.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Transpose.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Transpositions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/TriangularMatrix.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/VectorBlock.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/VectorwiseOp.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/Visitor.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX/Complex.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX512/Complex.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/CUDA/Complex.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/Half.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/Settings.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/MSA/Complex.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/NEON/Complex.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SSE/Complex.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/ZVector/Complex.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/BinaryFunctors.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/NullaryFunctors.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/StlFunctors.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/TernaryFunctors.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/functors/UnaryFunctors.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/Parallelizer.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/SelfadjointProduct.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/products/TriangularSolverVector.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/BlasUtil.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/ConfigureVectorization.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/Constants.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/ForwardDeclarations.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/IndexedViewHelper.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/IntegralConstant.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/MKL_support.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/Macros.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/Memory.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/Meta.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/ReshapedHelper.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/StaticAssert.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/SymbolicIndex.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Core/util/XprHelper.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/EigenSolver.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/RealQZ.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/RealSchur.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/AlignedBox.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/AngleAxis.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/EulerAngles.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Homogeneous.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Hyperplane.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/OrthoMethods.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/ParametrizedLine.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Quaternion.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Rotation2D.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/RotationBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Scaling.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Transform.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Translation.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/Umeyama.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Geometry/arch/Geometry_SSE.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Householder/BlockHouseholder.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Householder/Householder.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Householder/HouseholderSequence.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/Jacobi/Jacobi.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/KLUSupport/KLUSupport.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/LU/Determinant.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/LU/FullPivLU.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/LU/InverseImpl.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/LU/PartialPivLU.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/LU/arch/Inverse_SSE.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/MetisSupport/MetisSupport.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/OrderingMethods/Amd.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/OrderingMethods/Ordering.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/QR/ColPivHouseholderQR.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/QR/FullPivHouseholderQR.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/QR/HouseholderQR.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SVD/BDCSVD.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SVD/JacobiSVD.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SVD/SVDBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SVD/UpperBidiagonalization.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/AmbiVector.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/CompressedStorage.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseAssign.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseBlock.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseColEtree.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseDot.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseFuzzy.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseMap.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseMatrix.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparsePermutation.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseProduct.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseRedux.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseRef.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseSolverBase.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseTranspose.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseTriangularView.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseUtil.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseVector.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/SparseView.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseCore/TriangularSolver.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLUImpl.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SparseQR/SparseQR.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/StlSupport/StdDeque.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/StlSupport/StdList.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/StlSupport/StdVector.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/StlSupport/details.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/misc/Image.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/misc/Kernel.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/misc/RealSvd2x2.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/misc/blas.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/misc/lapack.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/misc/lapacke.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/plugins/BlockMethods.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/plugins/IndexedViewMethods.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/Eigen/src/plugins/ReshapedMethods.h` & `mazalib-0.52.4/src/eigen3/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/INSTALL` & `mazalib-0.52.4/src/eigen3/INSTALL`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/BenchSparseUtil.h` & `mazalib-0.52.4/src/eigen3/bench/BenchSparseUtil.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/BenchTimer.h` & `mazalib-0.52.4/src/eigen3/bench/BenchTimer.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/BenchUtil.h` & `mazalib-0.52.4/src/eigen3/bench/BenchUtil.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/README.txt` & `mazalib-0.52.4/src/eigen3/bench/README.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/analyze-blocking-sizes.cpp` & `mazalib-0.52.4/src/eigen3/bench/analyze-blocking-sizes.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/basicbench.cxxlist` & `mazalib-0.52.4/src/eigen3/bench/basicbench.cxxlist`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/basicbenchmark.cpp` & `mazalib-0.52.4/src/eigen3/bench/basicbenchmark.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/basicbenchmark.h` & `mazalib-0.52.4/src/eigen3/bench/basicbenchmark.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/benchBlasGemm.cpp` & `mazalib-0.52.4/src/eigen3/bench/benchBlasGemm.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/benchCholesky.cpp` & `mazalib-0.52.4/src/eigen3/bench/benchCholesky.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/benchEigenSolver.cpp` & `mazalib-0.52.4/src/eigen3/bench/benchEigenSolver.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/benchFFT.cpp` & `mazalib-0.52.4/src/eigen3/bench/benchFFT.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/benchGeometry.cpp` & `mazalib-0.52.4/src/eigen3/bench/benchGeometry.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/benchVecAdd.cpp` & `mazalib-0.52.4/src/eigen3/bench/benchVecAdd.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/bench_gemm.cpp` & `mazalib-0.52.4/src/eigen3/bench/bench_gemm.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/bench_multi_compilers.sh` & `mazalib-0.52.4/src/eigen3/bench/bench_multi_compilers.sh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/bench_norm.cpp` & `mazalib-0.52.4/src/eigen3/bench/bench_norm.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/bench_reverse.cpp` & `mazalib-0.52.4/src/eigen3/bench/bench_reverse.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/bench_unrolling` & `mazalib-0.52.4/src/eigen3/bench/bench_unrolling`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/benchmark-blocking-sizes.cpp` & `mazalib-0.52.4/src/eigen3/bench/benchmark-blocking-sizes.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/benchmark.cpp` & `mazalib-0.52.4/src/eigen3/bench/benchmark.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/benchmarkSlice.cpp` & `mazalib-0.52.4/src/eigen3/bench/benchmarkSlice.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/benchmarkX.cpp` & `mazalib-0.52.4/src/eigen3/bench/benchmarkX.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/benchmarkXcwise.cpp` & `mazalib-0.52.4/src/eigen3/bench/benchmarkXcwise.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/benchmark_suite` & `mazalib-0.52.4/src/eigen3/bench/benchmark_suite`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/bench/btl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/COPYING` & `mazalib-0.52.4/src/eigen3/bench/btl/COPYING`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/README` & `mazalib-0.52.4/src/eigen3/bench/btl/README`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_aat_product.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_aat_product.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_ata_product.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_ata_product.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_atv_product.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_atv_product.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_axpby.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_axpby.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_axpy.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_axpy.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_cholesky.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_cholesky.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_ger.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_ger.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_hessenberg.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_hessenberg.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_lu_decomp.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_lu_decomp.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_lu_solve.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_lu_solve.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_matrix_matrix_product.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_matrix_matrix_product.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_matrix_matrix_product_bis.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_matrix_matrix_product_bis.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_matrix_vector_product.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_matrix_vector_product.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_partial_lu.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_partial_lu.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_rot.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_rot.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_symv.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_symv.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_syr2.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_syr2.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_trisolve.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_trisolve.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_trisolve_matrix.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_trisolve_matrix.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/actions/action_trmm.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/actions/action_trmm.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindACML.cmake` & `mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindACML.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindATLAS.cmake` & `mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindATLAS.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindBLAZE.cmake` & `mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindBLAZE.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindBlitz.cmake` & `mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindBlitz.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindCBLAS.cmake` & `mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindCBLAS.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindMKL.cmake` & `mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindMKL.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindMTL4.cmake` & `mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindMTL4.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindOPENBLAS.cmake` & `mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindOPENBLAS.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindPackageHandleStandardArgs.cmake` & `mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/cmake/FindTvmet.cmake` & `mazalib-0.52.4/src/eigen3/bench/btl/cmake/FindTvmet.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake` & `mazalib-0.52.4/src/eigen3/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/data/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/bench/btl/data/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/data/action_settings.txt` & `mazalib-0.52.4/src/eigen3/bench/btl/data/action_settings.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/data/gnuplot_common_settings.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/data/gnuplot_common_settings.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/data/go_mean` & `mazalib-0.52.4/src/eigen3/bench/btl/data/go_mean`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/data/mean.cxx` & `mazalib-0.52.4/src/eigen3/bench/btl/data/mean.cxx`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/data/mk_gnuplot_script.sh` & `mazalib-0.52.4/src/eigen3/bench/btl/data/mk_gnuplot_script.sh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/data/mk_mean_script.sh` & `mazalib-0.52.4/src/eigen3/bench/btl/data/mk_mean_script.sh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/data/mk_new_gnuplot.sh` & `mazalib-0.52.4/src/eigen3/bench/btl/data/mk_new_gnuplot.sh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/data/perlib_plot_settings.txt` & `mazalib-0.52.4/src/eigen3/bench/btl/data/perlib_plot_settings.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/data/regularize.cxx` & `mazalib-0.52.4/src/eigen3/bench/btl/data/regularize.cxx`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/data/smooth.cxx` & `mazalib-0.52.4/src/eigen3/bench/btl/data/smooth.cxx`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/data/smooth_all.sh` & `mazalib-0.52.4/src/eigen3/bench/btl/data/smooth_all.sh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/bench.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/bench.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/bench_parameter.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/bench_parameter.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/btl.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/btl.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/init/init_function.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/init/init_function.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/init/init_matrix.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/init/init_matrix.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/init/init_vector.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/init/init_vector.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/static/bench_static.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/static/bench_static.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/static/intel_bench_fixed_size.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/static/intel_bench_fixed_size.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/static/static_size_generator.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/static/static_size_generator.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/STL_perf_analyzer.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/STL_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/STL_timer.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/STL_timer.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/portable_perf_analyzer.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/portable_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/portable_timer.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/portable_timer.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/x86_perf_analyzer.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/x86_perf_analyzer.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/timers/x86_timer.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/timers/x86_timer.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/utils/size_lin_log.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/utils/size_lin_log.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/utils/size_log.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/utils/size_log.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/utils/utilities.h` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/utils/utilities.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/generic_bench/utils/xy_file.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/generic_bench/utils/xy_file.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/blas.h` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/blas.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/blas_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/blas_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/blas_interface_impl.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/blas_interface_impl.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/c_interface_base.h` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/c_interface_base.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/BLAS/main.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/BLAS/main.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/STL/STL_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/STL/STL_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/STL/main.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/STL/main.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/blaze/blaze_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/blaze/blaze_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/blaze/main.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/blaze/main.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/blitz/blitz_LU_solve_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/blitz/blitz_LU_solve_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/blitz/blitz_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/blitz/blitz_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/blitz/btl_blitz.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/blitz/btl_blitz.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/blitz/btl_tiny_blitz.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/blitz/btl_tiny_blitz.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/blitz/tiny_blitz_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/blitz/tiny_blitz_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/eigen2_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/eigen2_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/main_adv.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/main_adv.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/main_linear.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/main_linear.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/main_matmat.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/main_matmat.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen2/main_vecmat.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen2/main_vecmat.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/eigen3_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/eigen3_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/main_adv.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/main_adv.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/main_linear.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/main_linear.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/main_matmat.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/main_matmat.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/eigen3/main_vecmat.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/eigen3/main_vecmat.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/gmm/gmm_LU_solve_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/gmm/gmm_LU_solve_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/gmm/gmm_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/gmm/gmm_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/gmm/main.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/gmm/main.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/mtl4/main.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/mtl4/main.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/mtl4/mtl4_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/mtl4/mtl4_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/tensors/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/tensors/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/tensors/main_linear.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/tensors/main_linear.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/tensors/main_matmat.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/tensors/main_matmat.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/tensors/main_vecmat.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/tensors/main_vecmat.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/tensors/tensor_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/tensors/tensor_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/tvmet/main.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/tvmet/main.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/tvmet/tvmet_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/tvmet/tvmet_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/ublas/main.cpp` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/ublas/main.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/btl/libs/ublas/ublas_interface.hh` & `mazalib-0.52.4/src/eigen3/bench/btl/libs/ublas/ublas_interface.hh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/check_cache_queries.cpp` & `mazalib-0.52.4/src/eigen3/bench/check_cache_queries.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/dense_solvers.cpp` & `mazalib-0.52.4/src/eigen3/bench/dense_solvers.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/eig33.cpp` & `mazalib-0.52.4/src/eigen3/bench/eig33.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/geometry.cpp` & `mazalib-0.52.4/src/eigen3/bench/geometry.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/perf_monitoring/changesets.txt` & `mazalib-0.52.4/src/eigen3/bench/perf_monitoring/changesets.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/perf_monitoring/gemm_common.h` & `mazalib-0.52.4/src/eigen3/bench/perf_monitoring/gemm_common.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/perf_monitoring/gemv_common.h` & `mazalib-0.52.4/src/eigen3/bench/perf_monitoring/gemv_common.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/perf_monitoring/lazy_gemm.cpp` & `mazalib-0.52.4/src/eigen3/bench/perf_monitoring/lazy_gemm.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/perf_monitoring/make_plot.sh` & `mazalib-0.52.4/src/eigen3/bench/perf_monitoring/make_plot.sh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/perf_monitoring/resources/chart_footer.html` & `mazalib-0.52.4/src/eigen3/bench/perf_monitoring/resources/chart_footer.html`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/perf_monitoring/resources/chart_header.html` & `mazalib-0.52.4/src/eigen3/bench/perf_monitoring/resources/chart_header.html`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/perf_monitoring/resources/header.html` & `mazalib-0.52.4/src/eigen3/bench/perf_monitoring/resources/header.html`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/perf_monitoring/resources/s1.js` & `mazalib-0.52.4/src/eigen3/bench/perf_monitoring/resources/s1.js`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/perf_monitoring/resources/s2.js` & `mazalib-0.52.4/src/eigen3/bench/perf_monitoring/resources/s2.js`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/perf_monitoring/run.sh` & `mazalib-0.52.4/src/eigen3/bench/perf_monitoring/run.sh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/perf_monitoring/runall.sh` & `mazalib-0.52.4/src/eigen3/bench/perf_monitoring/runall.sh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/product_threshold.cpp` & `mazalib-0.52.4/src/eigen3/bench/product_threshold.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/quat_slerp.cpp` & `mazalib-0.52.4/src/eigen3/bench/quat_slerp.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/quatmul.cpp` & `mazalib-0.52.4/src/eigen3/bench/quatmul.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/sparse_cholesky.cpp` & `mazalib-0.52.4/src/eigen3/bench/sparse_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/sparse_dense_product.cpp` & `mazalib-0.52.4/src/eigen3/bench/sparse_dense_product.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/sparse_lu.cpp` & `mazalib-0.52.4/src/eigen3/bench/sparse_lu.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/sparse_product.cpp` & `mazalib-0.52.4/src/eigen3/bench/sparse_product.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/sparse_randomsetter.cpp` & `mazalib-0.52.4/src/eigen3/bench/sparse_randomsetter.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/sparse_setter.cpp` & `mazalib-0.52.4/src/eigen3/bench/sparse_setter.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/sparse_transpose.cpp` & `mazalib-0.52.4/src/eigen3/bench/sparse_transpose.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/sparse_trisolver.cpp` & `mazalib-0.52.4/src/eigen3/bench/sparse_trisolver.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/spbench/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/bench/spbench/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/spbench/sp_solver.cpp` & `mazalib-0.52.4/src/eigen3/bench/spbench/sp_solver.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/spbench/spbench.dtd` & `mazalib-0.52.4/src/eigen3/bench/spbench/spbench.dtd`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/spbench/spbenchsolver.cpp` & `mazalib-0.52.4/src/eigen3/bench/spbench/spbenchsolver.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/spbench/spbenchsolver.h` & `mazalib-0.52.4/src/eigen3/bench/spbench/spbenchsolver.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/spbench/spbenchstyle.h` & `mazalib-0.52.4/src/eigen3/bench/spbench/spbenchstyle.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/spbench/test_sparseLU.cpp` & `mazalib-0.52.4/src/eigen3/bench/spbench/test_sparseLU.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/spmv.cpp` & `mazalib-0.52.4/src/eigen3/bench/spmv.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/tensors/README` & `mazalib-0.52.4/src/eigen3/bench/tensors/README`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/tensors/benchmark.h` & `mazalib-0.52.4/src/eigen3/bench/tensors/benchmark.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/tensors/benchmark_main.cc` & `mazalib-0.52.4/src/eigen3/bench/tensors/benchmark_main.cc`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/tensors/contraction_benchmarks_cpu.cc` & `mazalib-0.52.4/src/eigen3/bench/tensors/contraction_benchmarks_cpu.cc`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/tensors/tensor_benchmarks.h` & `mazalib-0.52.4/src/eigen3/bench/tensors/tensor_benchmarks.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/tensors/tensor_benchmarks_cpu.cc` & `mazalib-0.52.4/src/eigen3/bench/tensors/tensor_benchmarks_cpu.cc`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/tensors/tensor_benchmarks_fp16_gpu.cu` & `mazalib-0.52.4/src/eigen3/bench/tensors/tensor_benchmarks_fp16_gpu.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/tensors/tensor_benchmarks_gpu.cu` & `mazalib-0.52.4/src/eigen3/bench/tensors/tensor_benchmarks_gpu.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/tensors/tensor_benchmarks_sycl.cc` & `mazalib-0.52.4/src/eigen3/bench/tensors/tensor_benchmarks_sycl.cc`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/bench/vdw_new.cpp` & `mazalib-0.52.4/src/eigen3/bench/vdw_new.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/BandTriangularSolver.h` & `mazalib-0.52.4/src/eigen3/blas/BandTriangularSolver.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/blas/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/GeneralRank1Update.h` & `mazalib-0.52.4/src/eigen3/blas/GeneralRank1Update.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/PackedSelfadjointProduct.h` & `mazalib-0.52.4/src/eigen3/blas/PackedSelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/PackedTriangularMatrixVector.h` & `mazalib-0.52.4/src/eigen3/blas/PackedTriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/PackedTriangularSolverVector.h` & `mazalib-0.52.4/src/eigen3/blas/PackedTriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/Rank2Update.h` & `mazalib-0.52.4/src/eigen3/blas/Rank2Update.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/common.h` & `mazalib-0.52.4/src/eigen3/blas/common.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/complex_double.cpp` & `mazalib-0.52.4/src/eigen3/blas/complex_double.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/complex_single.cpp` & `mazalib-0.52.4/src/eigen3/blas/complex_single.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/double.cpp` & `mazalib-0.52.4/src/eigen3/blas/double.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/chbmv.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/chbmv.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/chpmv.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/chpmv.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/complexdots.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/complexdots.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/ctbmv.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/ctbmv.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/datatypes.h` & `mazalib-0.52.4/src/eigen3/blas/f2c/datatypes.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/drotm.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/drotm.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/drotmg.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/drotmg.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/dsbmv.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/dsbmv.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/dspmv.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/dspmv.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/dtbmv.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/dtbmv.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/lsame.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/lsame.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/srotm.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/srotm.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/srotmg.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/srotmg.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/ssbmv.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/ssbmv.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/sspmv.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/sspmv.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/stbmv.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/stbmv.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/zhbmv.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/zhbmv.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/zhpmv.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/zhpmv.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/f2c/ztbmv.c` & `mazalib-0.52.4/src/eigen3/blas/f2c/ztbmv.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/fortran/complexdots.f` & `mazalib-0.52.4/src/eigen3/blas/fortran/complexdots.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/level1_cplx_impl.h` & `mazalib-0.52.4/src/eigen3/blas/level1_cplx_impl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/level1_impl.h` & `mazalib-0.52.4/src/eigen3/blas/level1_impl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/level1_real_impl.h` & `mazalib-0.52.4/src/eigen3/blas/level1_real_impl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/level2_cplx_impl.h` & `mazalib-0.52.4/src/eigen3/blas/level2_cplx_impl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/level2_impl.h` & `mazalib-0.52.4/src/eigen3/blas/level2_impl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/level2_real_impl.h` & `mazalib-0.52.4/src/eigen3/blas/level2_real_impl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/level3_impl.h` & `mazalib-0.52.4/src/eigen3/blas/level3_impl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/single.cpp` & `mazalib-0.52.4/src/eigen3/blas/single.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/blas/testing/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/cblat1.f` & `mazalib-0.52.4/src/eigen3/blas/testing/cblat1.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/cblat2.dat` & `mazalib-0.52.4/src/eigen3/blas/testing/cblat2.dat`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/cblat2.f` & `mazalib-0.52.4/src/eigen3/blas/testing/cblat2.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/cblat3.dat` & `mazalib-0.52.4/src/eigen3/blas/testing/cblat3.dat`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/cblat3.f` & `mazalib-0.52.4/src/eigen3/blas/testing/cblat3.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/dblat1.f` & `mazalib-0.52.4/src/eigen3/blas/testing/dblat1.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/dblat2.dat` & `mazalib-0.52.4/src/eigen3/blas/testing/dblat2.dat`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/dblat2.f` & `mazalib-0.52.4/src/eigen3/blas/testing/dblat2.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/dblat3.dat` & `mazalib-0.52.4/src/eigen3/blas/testing/dblat3.dat`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/dblat3.f` & `mazalib-0.52.4/src/eigen3/blas/testing/dblat3.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/runblastest.sh` & `mazalib-0.52.4/src/eigen3/blas/testing/runblastest.sh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/sblat1.f` & `mazalib-0.52.4/src/eigen3/blas/testing/sblat1.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/sblat2.dat` & `mazalib-0.52.4/src/eigen3/blas/testing/sblat2.dat`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/sblat2.f` & `mazalib-0.52.4/src/eigen3/blas/testing/sblat2.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/sblat3.dat` & `mazalib-0.52.4/src/eigen3/blas/testing/sblat3.dat`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/sblat3.f` & `mazalib-0.52.4/src/eigen3/blas/testing/sblat3.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/zblat1.f` & `mazalib-0.52.4/src/eigen3/blas/testing/zblat1.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/zblat2.dat` & `mazalib-0.52.4/src/eigen3/blas/testing/zblat2.dat`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/zblat2.f` & `mazalib-0.52.4/src/eigen3/blas/testing/zblat2.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/zblat3.dat` & `mazalib-0.52.4/src/eigen3/blas/testing/zblat3.dat`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/blas/testing/zblat3.f` & `mazalib-0.52.4/src/eigen3/blas/testing/zblat3.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/Eigen3Config.cmake.in` & `mazalib-0.52.4/src/eigen3/cmake/Eigen3Config.cmake.in`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/Eigen3ConfigLegacy.cmake.in` & `mazalib-0.52.4/src/eigen3/cmake/Eigen3ConfigLegacy.cmake.in`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/EigenConfigureTesting.cmake` & `mazalib-0.52.4/src/eigen3/cmake/EigenConfigureTesting.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/EigenDetermineOSVersion.cmake` & `mazalib-0.52.4/src/eigen3/cmake/EigenDetermineOSVersion.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/EigenDetermineVSServicePack.cmake` & `mazalib-0.52.4/src/eigen3/cmake/EigenDetermineVSServicePack.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/EigenTesting.cmake` & `mazalib-0.52.4/src/eigen3/cmake/EigenTesting.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/EigenUninstall.cmake` & `mazalib-0.52.4/src/eigen3/cmake/EigenUninstall.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindAdolc.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindAdolc.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindBLAS.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindBLAS.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindBLASEXT.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindBLASEXT.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindCholmod.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindCholmod.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindComputeCpp.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindComputeCpp.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindEigen2.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindEigen2.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindEigen3.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindFFTW.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindFFTW.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindGLEW.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindGLEW.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindGMP.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindGSL.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindGSL.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindGoogleHash.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindGoogleHash.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindHWLOC.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindHWLOC.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindKLU.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindKLU.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindLAPACK.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindLAPACK.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindMPFR.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindMPFR.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindMetis.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindMetis.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindPTSCOTCH.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindPTSCOTCH.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindPastix.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindPastix.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindSPQR.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindSPQR.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindScotch.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindScotch.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindStandardMathLibrary.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindStandardMathLibrary.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindSuperLU.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindSuperLU.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindTriSYCL.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindTriSYCL.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/FindUmfpack.cmake` & `mazalib-0.52.4/src/eigen3/cmake/FindUmfpack.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/RegexUtils.cmake` & `mazalib-0.52.4/src/eigen3/cmake/RegexUtils.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/cmake/language_support.cmake` & `mazalib-0.52.4/src/eigen3/cmake/language_support.cmake`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/debug/gdb/printers.py` & `mazalib-0.52.4/src/eigen3/debug/gdb/printers.py`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/debug/msvc/eigen.natvis` & `mazalib-0.52.4/src/eigen3/debug/msvc/eigen.natvis`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/debug/msvc/eigen_autoexp_part.dat` & `mazalib-0.52.4/src/eigen3/debug/msvc/eigen_autoexp_part.dat`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/mandelbrot/mandelbrot.cpp` & `mazalib-0.52.4/src/eigen3/demos/mandelbrot/mandelbrot.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/mandelbrot/mandelbrot.h` & `mazalib-0.52.4/src/eigen3/demos/mandelbrot/mandelbrot.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/mix_eigen_and_c/binary_library.cpp` & `mazalib-0.52.4/src/eigen3/demos/mix_eigen_and_c/binary_library.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/mix_eigen_and_c/binary_library.h` & `mazalib-0.52.4/src/eigen3/demos/mix_eigen_and_c/binary_library.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/mix_eigen_and_c/example.c` & `mazalib-0.52.4/src/eigen3/demos/mix_eigen_and_c/example.c`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/opengl/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/demos/opengl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/opengl/camera.cpp` & `mazalib-0.52.4/src/eigen3/demos/opengl/camera.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/opengl/camera.h` & `mazalib-0.52.4/src/eigen3/demos/opengl/camera.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/opengl/gpuhelper.cpp` & `mazalib-0.52.4/src/eigen3/demos/opengl/gpuhelper.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/opengl/gpuhelper.h` & `mazalib-0.52.4/src/eigen3/demos/opengl/gpuhelper.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/opengl/icosphere.cpp` & `mazalib-0.52.4/src/eigen3/demos/opengl/icosphere.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/opengl/icosphere.h` & `mazalib-0.52.4/src/eigen3/demos/opengl/icosphere.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/opengl/quaternion_demo.cpp` & `mazalib-0.52.4/src/eigen3/demos/opengl/quaternion_demo.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/opengl/quaternion_demo.h` & `mazalib-0.52.4/src/eigen3/demos/opengl/quaternion_demo.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/opengl/trackball.cpp` & `mazalib-0.52.4/src/eigen3/demos/opengl/trackball.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/demos/opengl/trackball.h` & `mazalib-0.52.4/src/eigen3/demos/opengl/trackball.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/AsciiQuickReference.txt` & `mazalib-0.52.4/src/eigen3/doc/AsciiQuickReference.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/B01_Experimental.dox` & `mazalib-0.52.4/src/eigen3/doc/B01_Experimental.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/ClassHierarchy.dox` & `mazalib-0.52.4/src/eigen3/doc/ClassHierarchy.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/CoeffwiseMathFunctionsTable.dox` & `mazalib-0.52.4/src/eigen3/doc/CoeffwiseMathFunctionsTable.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/CustomizingEigen_CustomScalar.dox` & `mazalib-0.52.4/src/eigen3/doc/CustomizingEigen_CustomScalar.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/CustomizingEigen_InheritingMatrix.dox` & `mazalib-0.52.4/src/eigen3/doc/CustomizingEigen_InheritingMatrix.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/CustomizingEigen_NullaryExpr.dox` & `mazalib-0.52.4/src/eigen3/doc/CustomizingEigen_NullaryExpr.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/CustomizingEigen_Plugins.dox` & `mazalib-0.52.4/src/eigen3/doc/CustomizingEigen_Plugins.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/DenseDecompositionBenchmark.dox` & `mazalib-0.52.4/src/eigen3/doc/DenseDecompositionBenchmark.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/Doxyfile.in` & `mazalib-0.52.4/src/eigen3/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/Eigen_Silly_Professor_64x64.png` & `mazalib-0.52.4/src/eigen3/doc/Eigen_Silly_Professor_64x64.png`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/FixedSizeVectorizable.dox` & `mazalib-0.52.4/src/eigen3/doc/FixedSizeVectorizable.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/FunctionsTakingEigenTypes.dox` & `mazalib-0.52.4/src/eigen3/doc/FunctionsTakingEigenTypes.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/HiPerformance.dox` & `mazalib-0.52.4/src/eigen3/doc/HiPerformance.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/InplaceDecomposition.dox` & `mazalib-0.52.4/src/eigen3/doc/InplaceDecomposition.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/InsideEigenExample.dox` & `mazalib-0.52.4/src/eigen3/doc/InsideEigenExample.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/LeastSquares.dox` & `mazalib-0.52.4/src/eigen3/doc/LeastSquares.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/Manual.dox` & `mazalib-0.52.4/src/eigen3/doc/Manual.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/MatrixfreeSolverExample.dox` & `mazalib-0.52.4/src/eigen3/doc/MatrixfreeSolverExample.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/NewExpressionType.dox` & `mazalib-0.52.4/src/eigen3/doc/NewExpressionType.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/Overview.dox` & `mazalib-0.52.4/src/eigen3/doc/Overview.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/PassingByValue.dox` & `mazalib-0.52.4/src/eigen3/doc/PassingByValue.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/Pitfalls.dox` & `mazalib-0.52.4/src/eigen3/doc/Pitfalls.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/PreprocessorDirectives.dox` & `mazalib-0.52.4/src/eigen3/doc/PreprocessorDirectives.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/QuickReference.dox` & `mazalib-0.52.4/src/eigen3/doc/QuickReference.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/QuickStartGuide.dox` & `mazalib-0.52.4/src/eigen3/doc/QuickStartGuide.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/SparseLinearSystems.dox` & `mazalib-0.52.4/src/eigen3/doc/SparseLinearSystems.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/SparseQuickReference.dox` & `mazalib-0.52.4/src/eigen3/doc/SparseQuickReference.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/StlContainers.dox` & `mazalib-0.52.4/src/eigen3/doc/StlContainers.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/StorageOrders.dox` & `mazalib-0.52.4/src/eigen3/doc/StorageOrders.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/StructHavingEigenMembers.dox` & `mazalib-0.52.4/src/eigen3/doc/StructHavingEigenMembers.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TemplateKeyword.dox` & `mazalib-0.52.4/src/eigen3/doc/TemplateKeyword.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TopicAliasing.dox` & `mazalib-0.52.4/src/eigen3/doc/TopicAliasing.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TopicAssertions.dox` & `mazalib-0.52.4/src/eigen3/doc/TopicAssertions.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TopicCMakeGuide.dox` & `mazalib-0.52.4/src/eigen3/doc/TopicCMakeGuide.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TopicLazyEvaluation.dox` & `mazalib-0.52.4/src/eigen3/doc/TopicLazyEvaluation.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TopicLinearAlgebraDecompositions.dox` & `mazalib-0.52.4/src/eigen3/doc/TopicLinearAlgebraDecompositions.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TopicMultithreading.dox` & `mazalib-0.52.4/src/eigen3/doc/TopicMultithreading.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialAdvancedInitialization.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialAdvancedInitialization.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialArrayClass.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialArrayClass.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialBlockOperations.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialBlockOperations.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialGeometry.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialGeometry.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialLinearAlgebra.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialLinearAlgebra.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialMapClass.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialMapClass.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialMatrixArithmetic.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialMatrixArithmetic.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialMatrixClass.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialMatrixClass.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialReductionsVisitorsBroadcasting.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialReductionsVisitorsBroadcasting.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialReshape.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialReshape.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialSTL.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialSTL.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialSlicingIndexing.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialSlicingIndexing.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/TutorialSparse.dox` & `mazalib-0.52.4/src/eigen3/doc/TutorialSparse.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/UnalignedArrayAssert.dox` & `mazalib-0.52.4/src/eigen3/doc/UnalignedArrayAssert.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/UsingBlasLapackBackends.dox` & `mazalib-0.52.4/src/eigen3/doc/UsingBlasLapackBackends.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/UsingIntelMKL.dox` & `mazalib-0.52.4/src/eigen3/doc/UsingIntelMKL.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/UsingNVCC.dox` & `mazalib-0.52.4/src/eigen3/doc/UsingNVCC.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/WrongStackAlignment.dox` & `mazalib-0.52.4/src/eigen3/doc/WrongStackAlignment.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/eigen_navtree_hacks.js` & `mazalib-0.52.4/src/eigen3/doc/eigen_navtree_hacks.js`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/eigendoxy.css` & `mazalib-0.52.4/src/eigen3/doc/eigendoxy.css`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/eigendoxy_footer.html.in` & `mazalib-0.52.4/src/eigen3/doc/eigendoxy_footer.html.in`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/eigendoxy_header.html.in` & `mazalib-0.52.4/src/eigen3/doc/eigendoxy_header.html.in`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/eigendoxy_layout.xml.in` & `mazalib-0.52.4/src/eigen3/doc/eigendoxy_layout.xml.in`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/eigendoxy_tabs.css` & `mazalib-0.52.4/src/eigen3/doc/eigendoxy_tabs.css`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/doc/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/CustomizingEigen_Inheritance.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/CustomizingEigen_Inheritance.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/TemplateKeyword_flexible.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/TemplateKeyword_flexible.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/TemplateKeyword_simple.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/TemplateKeyword_simple.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/TutorialInplaceLU.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/TutorialInplaceLU.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/TutorialLinAlgComputeTwice.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/TutorialLinAlgComputeTwice.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/TutorialLinAlgRankRevealing.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/TutorialLinAlgRankRevealing.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_BlockOperations_block_assignment.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_BlockOperations_block_assignment.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/Tutorial_simple_example_dynamic_size.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/Tutorial_simple_example_dynamic_size.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/class_Block.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/class_Block.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/class_CwiseBinaryOp.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/class_CwiseBinaryOp.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/class_CwiseUnaryOp.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/class_CwiseUnaryOp.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/class_FixedBlock.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/class_FixedBlock.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/class_FixedVectorBlock.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/class_FixedVectorBlock.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/class_Reshaped.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/class_Reshaped.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/class_VectorBlock.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/class_VectorBlock.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/function_taking_ref.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/function_taking_ref.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/make_circulant.cpp.evaluator` & `mazalib-0.52.4/src/eigen3/doc/examples/make_circulant.cpp.evaluator`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/make_circulant.cpp.expression` & `mazalib-0.52.4/src/eigen3/doc/examples/make_circulant.cpp.expression`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/make_circulant.cpp.traits` & `mazalib-0.52.4/src/eigen3/doc/examples/make_circulant.cpp.traits`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/make_circulant2.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/make_circulant2.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/matrixfree_cg.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/matrixfree_cg.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/nullary_indexing.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/nullary_indexing.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/tut_arithmetic_matrix_mul.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/tut_arithmetic_matrix_mul.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/examples/tut_arithmetic_redux_basic.cpp` & `mazalib-0.52.4/src/eigen3/doc/examples/tut_arithmetic_redux_basic.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/doc/snippets/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/ComplexEigenSolver_compute.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/ComplexEigenSolver_compute.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/HouseholderSequence_HouseholderSequence.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/HouseholderSequence_HouseholderSequence.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/IOFormat.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/IOFormat.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/JacobiSVD_basic.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/JacobiSVD_basic.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/LLT_example.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/LLT_example.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_all.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_all.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/MatrixBase_triangularView.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/MatrixBase_triangularView.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/RealQZ_compute.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/RealQZ_compute.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/TopicAliasing_cwise.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/TopicAliasing_cwise.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/TopicStorageOrders_example.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/TopicStorageOrders_example.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/Triangular_solve.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/Triangular_solve.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/Tridiagonalization_diagonal.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/Tridiagonalization_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_Map_using.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_Map_using.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/Tutorial_SlicingCol.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/Tutorial_SlicingCol.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/Vectorwise_reverse.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/Vectorwise_reverse.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/class_FullPivLU.cpp` & `mazalib-0.52.4/src/eigen3/doc/snippets/class_FullPivLU.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/snippets/compile_snippet.cpp.in` & `mazalib-0.52.4/src/eigen3/doc/snippets/compile_snippet.cpp.in`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/special_examples/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/doc/special_examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/special_examples/Tutorial_sparse_example.cpp` & `mazalib-0.52.4/src/eigen3/doc/special_examples/Tutorial_sparse_example.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/special_examples/Tutorial_sparse_example_details.cpp` & `mazalib-0.52.4/src/eigen3/doc/special_examples/Tutorial_sparse_example_details.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/doc/tutorial.cpp` & `mazalib-0.52.4/src/eigen3/doc/tutorial.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/failtest/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/failtest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/lapack/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/cholesky.cpp` & `mazalib-0.52.4/src/eigen3/lapack/cholesky.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/clacgv.f` & `mazalib-0.52.4/src/eigen3/lapack/clacgv.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/cladiv.f` & `mazalib-0.52.4/src/eigen3/lapack/cladiv.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/clarf.f` & `mazalib-0.52.4/src/eigen3/lapack/clarf.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/clarfb.f` & `mazalib-0.52.4/src/eigen3/lapack/clarfb.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/clarfg.f` & `mazalib-0.52.4/src/eigen3/lapack/clarfg.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/clarft.f` & `mazalib-0.52.4/src/eigen3/lapack/clarft.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/complex_double.cpp` & `mazalib-0.52.4/src/eigen3/lapack/complex_double.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/complex_single.cpp` & `mazalib-0.52.4/src/eigen3/lapack/complex_single.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/dladiv.f` & `mazalib-0.52.4/src/eigen3/lapack/dladiv.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/dlamch.f` & `mazalib-0.52.4/src/eigen3/lapack/dlamch.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/dlapy2.f` & `mazalib-0.52.4/src/eigen3/lapack/dlapy2.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/dlapy3.f` & `mazalib-0.52.4/src/eigen3/lapack/dlapy3.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/dlarf.f` & `mazalib-0.52.4/src/eigen3/lapack/dlarf.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/dlarfb.f` & `mazalib-0.52.4/src/eigen3/lapack/dlarfb.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/dlarfg.f` & `mazalib-0.52.4/src/eigen3/lapack/dlarfg.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/dlarft.f` & `mazalib-0.52.4/src/eigen3/lapack/dlarft.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/double.cpp` & `mazalib-0.52.4/src/eigen3/lapack/double.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/dsecnd_NONE.f` & `mazalib-0.52.4/src/eigen3/lapack/dsecnd_NONE.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/eigenvalues.cpp` & `mazalib-0.52.4/src/eigen3/lapack/eigenvalues.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/ilaclc.f` & `mazalib-0.52.4/src/eigen3/lapack/ilaclc.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/ilaclr.f` & `mazalib-0.52.4/src/eigen3/lapack/ilaclr.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/iladlc.f` & `mazalib-0.52.4/src/eigen3/lapack/iladlc.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/iladlr.f` & `mazalib-0.52.4/src/eigen3/lapack/iladlr.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/ilaslc.f` & `mazalib-0.52.4/src/eigen3/lapack/ilaslc.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/ilaslr.f` & `mazalib-0.52.4/src/eigen3/lapack/ilaslr.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/ilazlc.f` & `mazalib-0.52.4/src/eigen3/lapack/ilazlc.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/ilazlr.f` & `mazalib-0.52.4/src/eigen3/lapack/ilazlr.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/lapack_common.h` & `mazalib-0.52.4/src/eigen3/lapack/lapack_common.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/lu.cpp` & `mazalib-0.52.4/src/eigen3/lapack/lu.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/second_NONE.f` & `mazalib-0.52.4/src/eigen3/lapack/second_NONE.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/single.cpp` & `mazalib-0.52.4/src/eigen3/lapack/single.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/sladiv.f` & `mazalib-0.52.4/src/eigen3/lapack/sladiv.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/slamch.f` & `mazalib-0.52.4/src/eigen3/lapack/slamch.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/slapy2.f` & `mazalib-0.52.4/src/eigen3/lapack/slapy2.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/slapy3.f` & `mazalib-0.52.4/src/eigen3/lapack/slapy3.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/slarf.f` & `mazalib-0.52.4/src/eigen3/lapack/slarf.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/slarfb.f` & `mazalib-0.52.4/src/eigen3/lapack/slarfb.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/slarfg.f` & `mazalib-0.52.4/src/eigen3/lapack/slarfg.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/slarft.f` & `mazalib-0.52.4/src/eigen3/lapack/slarft.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/svd.cpp` & `mazalib-0.52.4/src/eigen3/lapack/svd.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/zlacgv.f` & `mazalib-0.52.4/src/eigen3/lapack/zlacgv.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/zladiv.f` & `mazalib-0.52.4/src/eigen3/lapack/zladiv.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/zlarf.f` & `mazalib-0.52.4/src/eigen3/lapack/zlarf.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/zlarfb.f` & `mazalib-0.52.4/src/eigen3/lapack/zlarfb.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/zlarfg.f` & `mazalib-0.52.4/src/eigen3/lapack/zlarfg.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/lapack/zlarft.f` & `mazalib-0.52.4/src/eigen3/lapack/zlarft.f`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/scripts/buildtests.in` & `mazalib-0.52.4/src/eigen3/scripts/buildtests.in`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/scripts/cdashtesting.cmake.in` & `mazalib-0.52.4/src/eigen3/scripts/cdashtesting.cmake.in`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/scripts/check.in` & `mazalib-0.52.4/src/eigen3/scripts/check.in`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/scripts/eigen_gen_credits.cpp` & `mazalib-0.52.4/src/eigen3/scripts/eigen_gen_credits.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/scripts/eigen_gen_docs` & `mazalib-0.52.4/src/eigen3/scripts/eigen_gen_docs`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/scripts/eigen_monitor_perf.sh` & `mazalib-0.52.4/src/eigen3/scripts/eigen_monitor_perf.sh`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/scripts/relicense.py` & `mazalib-0.52.4/src/eigen3/scripts/relicense.py`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/AnnoyingScalar.h` & `mazalib-0.52.4/src/eigen3/test/AnnoyingScalar.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/adjoint.cpp` & `mazalib-0.52.4/src/eigen3/test/adjoint.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/array_cwise.cpp` & `mazalib-0.52.4/src/eigen3/test/array_cwise.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/array_for_matrix.cpp` & `mazalib-0.52.4/src/eigen3/test/array_for_matrix.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/array_of_string.cpp` & `mazalib-0.52.4/src/eigen3/test/array_of_string.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/array_replicate.cpp` & `mazalib-0.52.4/src/eigen3/test/array_replicate.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/array_reverse.cpp` & `mazalib-0.52.4/src/eigen3/test/array_reverse.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/bandmatrix.cpp` & `mazalib-0.52.4/src/eigen3/test/bandmatrix.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/basicstuff.cpp` & `mazalib-0.52.4/src/eigen3/test/basicstuff.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/bdcsvd.cpp` & `mazalib-0.52.4/src/eigen3/test/bdcsvd.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/bicgstab.cpp` & `mazalib-0.52.4/src/eigen3/test/bicgstab.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/block.cpp` & `mazalib-0.52.4/src/eigen3/test/block.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/boostmultiprec.cpp` & `mazalib-0.52.4/src/eigen3/test/boostmultiprec.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/cholesky.cpp` & `mazalib-0.52.4/src/eigen3/test/cholesky.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/cholmod_support.cpp` & `mazalib-0.52.4/src/eigen3/test/cholmod_support.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/commainitializer.cpp` & `mazalib-0.52.4/src/eigen3/test/commainitializer.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/conjugate_gradient.cpp` & `mazalib-0.52.4/src/eigen3/test/conjugate_gradient.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/conservative_resize.cpp` & `mazalib-0.52.4/src/eigen3/test/conservative_resize.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/constructor.cpp` & `mazalib-0.52.4/src/eigen3/test/constructor.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/corners.cpp` & `mazalib-0.52.4/src/eigen3/test/corners.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/ctorleak.cpp` & `mazalib-0.52.4/src/eigen3/test/ctorleak.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/denseLM.cpp` & `mazalib-0.52.4/src/eigen3/test/denseLM.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/dense_storage.cpp` & `mazalib-0.52.4/src/eigen3/test/dense_storage.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/determinant.cpp` & `mazalib-0.52.4/src/eigen3/test/determinant.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/diagonal.cpp` & `mazalib-0.52.4/src/eigen3/test/diagonal.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/diagonal_matrix_variadic_ctor.cpp` & `mazalib-0.52.4/src/eigen3/test/diagonal_matrix_variadic_ctor.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/diagonalmatrices.cpp` & `mazalib-0.52.4/src/eigen3/test/diagonalmatrices.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/dontalign.cpp` & `mazalib-0.52.4/src/eigen3/test/dontalign.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/dynalloc.cpp` & `mazalib-0.52.4/src/eigen3/test/dynalloc.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/eigen2support.cpp` & `mazalib-0.52.4/src/eigen3/test/eigen2support.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/eigensolver_complex.cpp` & `mazalib-0.52.4/src/eigen3/test/eigensolver_complex.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/eigensolver_generalized_real.cpp` & `mazalib-0.52.4/src/eigen3/test/eigensolver_generalized_real.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/eigensolver_generic.cpp` & `mazalib-0.52.4/src/eigen3/test/eigensolver_generic.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/eigensolver_selfadjoint.cpp` & `mazalib-0.52.4/src/eigen3/test/eigensolver_selfadjoint.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/evaluators.cpp` & `mazalib-0.52.4/src/eigen3/test/evaluators.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/exceptions.cpp` & `mazalib-0.52.4/src/eigen3/test/exceptions.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/fastmath.cpp` & `mazalib-0.52.4/src/eigen3/test/fastmath.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/first_aligned.cpp` & `mazalib-0.52.4/src/eigen3/test/first_aligned.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/geo_alignedbox.cpp` & `mazalib-0.52.4/src/eigen3/test/geo_alignedbox.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/geo_eulerangles.cpp` & `mazalib-0.52.4/src/eigen3/test/geo_eulerangles.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/geo_homogeneous.cpp` & `mazalib-0.52.4/src/eigen3/test/geo_homogeneous.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/geo_hyperplane.cpp` & `mazalib-0.52.4/src/eigen3/test/geo_hyperplane.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/geo_orthomethods.cpp` & `mazalib-0.52.4/src/eigen3/test/geo_orthomethods.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/geo_parametrizedline.cpp` & `mazalib-0.52.4/src/eigen3/test/geo_parametrizedline.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/geo_quaternion.cpp` & `mazalib-0.52.4/src/eigen3/test/geo_quaternion.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/geo_transformations.cpp` & `mazalib-0.52.4/src/eigen3/test/geo_transformations.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/gpu_basic.cu` & `mazalib-0.52.4/src/eigen3/test/gpu_basic.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/gpu_common.h` & `mazalib-0.52.4/src/eigen3/test/gpu_common.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/half_float.cpp` & `mazalib-0.52.4/src/eigen3/test/half_float.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/hessenberg.cpp` & `mazalib-0.52.4/src/eigen3/test/hessenberg.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/householder.cpp` & `mazalib-0.52.4/src/eigen3/test/householder.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/incomplete_cholesky.cpp` & `mazalib-0.52.4/src/eigen3/test/incomplete_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/indexed_view.cpp` & `mazalib-0.52.4/src/eigen3/test/indexed_view.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/initializer_list_construction.cpp` & `mazalib-0.52.4/src/eigen3/test/initializer_list_construction.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/inplace_decomposition.cpp` & `mazalib-0.52.4/src/eigen3/test/inplace_decomposition.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/integer_types.cpp` & `mazalib-0.52.4/src/eigen3/test/integer_types.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/inverse.cpp` & `mazalib-0.52.4/src/eigen3/test/inverse.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/is_same_dense.cpp` & `mazalib-0.52.4/src/eigen3/test/is_same_dense.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/jacobi.cpp` & `mazalib-0.52.4/src/eigen3/test/jacobi.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/jacobisvd.cpp` & `mazalib-0.52.4/src/eigen3/test/jacobisvd.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/klu_support.cpp` & `mazalib-0.52.4/src/eigen3/test/klu_support.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/linearstructure.cpp` & `mazalib-0.52.4/src/eigen3/test/linearstructure.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/lscg.cpp` & `mazalib-0.52.4/src/eigen3/test/lscg.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/lu.cpp` & `mazalib-0.52.4/src/eigen3/test/lu.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/main.h` & `mazalib-0.52.4/src/eigen3/test/main.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/mapped_matrix.cpp` & `mazalib-0.52.4/src/eigen3/test/mapped_matrix.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/mapstaticmethods.cpp` & `mazalib-0.52.4/src/eigen3/test/mapstaticmethods.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/mapstride.cpp` & `mazalib-0.52.4/src/eigen3/test/mapstride.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/meta.cpp` & `mazalib-0.52.4/src/eigen3/test/meta.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/metis_support.cpp` & `mazalib-0.52.4/src/eigen3/test/metis_support.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/miscmatrices.cpp` & `mazalib-0.52.4/src/eigen3/test/miscmatrices.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/mixingtypes.cpp` & `mazalib-0.52.4/src/eigen3/test/mixingtypes.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/mpl2only.cpp` & `mazalib-0.52.4/src/eigen3/test/mpl2only.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/nestbyvalue.cpp` & `mazalib-0.52.4/src/eigen3/test/nestbyvalue.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/nesting_ops.cpp` & `mazalib-0.52.4/src/eigen3/test/nesting_ops.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/nomalloc.cpp` & `mazalib-0.52.4/src/eigen3/test/nomalloc.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/nullary.cpp` & `mazalib-0.52.4/src/eigen3/test/nullary.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/num_dimensions.cpp` & `mazalib-0.52.4/src/eigen3/test/num_dimensions.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/numext.cpp` & `mazalib-0.52.4/src/eigen3/test/numext.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/packetmath.cpp` & `mazalib-0.52.4/src/eigen3/test/packetmath.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/pardiso_support.cpp` & `mazalib-0.52.4/src/eigen3/test/pardiso_support.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/pastix_support.cpp` & `mazalib-0.52.4/src/eigen3/test/pastix_support.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/permutationmatrices.cpp` & `mazalib-0.52.4/src/eigen3/test/permutationmatrices.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/prec_inverse_4x4.cpp` & `mazalib-0.52.4/src/eigen3/test/prec_inverse_4x4.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/product.h` & `mazalib-0.52.4/src/eigen3/test/product.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/product_extra.cpp` & `mazalib-0.52.4/src/eigen3/test/product_extra.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/product_large.cpp` & `mazalib-0.52.4/src/eigen3/test/product_large.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/product_mmtr.cpp` & `mazalib-0.52.4/src/eigen3/test/product_mmtr.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/product_notemporary.cpp` & `mazalib-0.52.4/src/eigen3/test/product_notemporary.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/product_selfadjoint.cpp` & `mazalib-0.52.4/src/eigen3/test/product_selfadjoint.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/product_small.cpp` & `mazalib-0.52.4/src/eigen3/test/product_small.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/product_symm.cpp` & `mazalib-0.52.4/src/eigen3/test/product_symm.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/product_syrk.cpp` & `mazalib-0.52.4/src/eigen3/test/product_syrk.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/product_trmm.cpp` & `mazalib-0.52.4/src/eigen3/test/product_trmm.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/product_trmv.cpp` & `mazalib-0.52.4/src/eigen3/test/product_trmv.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/product_trsolve.cpp` & `mazalib-0.52.4/src/eigen3/test/product_trsolve.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/qr.cpp` & `mazalib-0.52.4/src/eigen3/test/qr.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/qr_colpivoting.cpp` & `mazalib-0.52.4/src/eigen3/test/qr_colpivoting.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/qr_fullpivoting.cpp` & `mazalib-0.52.4/src/eigen3/test/qr_fullpivoting.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/qtvector.cpp` & `mazalib-0.52.4/src/eigen3/test/qtvector.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/rand.cpp` & `mazalib-0.52.4/src/eigen3/test/rand.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/real_qz.cpp` & `mazalib-0.52.4/src/eigen3/test/real_qz.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/redux.cpp` & `mazalib-0.52.4/src/eigen3/test/redux.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/ref.cpp` & `mazalib-0.52.4/src/eigen3/test/ref.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/reshape.cpp` & `mazalib-0.52.4/src/eigen3/test/reshape.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/resize.cpp` & `mazalib-0.52.4/src/eigen3/test/resize.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/rvalue_types.cpp` & `mazalib-0.52.4/src/eigen3/test/rvalue_types.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/schur_complex.cpp` & `mazalib-0.52.4/src/eigen3/test/schur_complex.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/schur_real.cpp` & `mazalib-0.52.4/src/eigen3/test/schur_real.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/selfadjoint.cpp` & `mazalib-0.52.4/src/eigen3/test/selfadjoint.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/simplicial_cholesky.cpp` & `mazalib-0.52.4/src/eigen3/test/simplicial_cholesky.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sizeof.cpp` & `mazalib-0.52.4/src/eigen3/test/sizeof.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sizeoverflow.cpp` & `mazalib-0.52.4/src/eigen3/test/sizeoverflow.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/smallvectors.cpp` & `mazalib-0.52.4/src/eigen3/test/smallvectors.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/solverbase.h` & `mazalib-0.52.4/src/eigen3/test/solverbase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sparse.h` & `mazalib-0.52.4/src/eigen3/test/sparse.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sparseLM.cpp` & `mazalib-0.52.4/src/eigen3/test/sparseLM.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sparse_basic.cpp` & `mazalib-0.52.4/src/eigen3/test/sparse_basic.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sparse_block.cpp` & `mazalib-0.52.4/src/eigen3/test/sparse_block.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sparse_permutations.cpp` & `mazalib-0.52.4/src/eigen3/test/sparse_permutations.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sparse_product.cpp` & `mazalib-0.52.4/src/eigen3/test/sparse_product.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sparse_ref.cpp` & `mazalib-0.52.4/src/eigen3/test/sparse_ref.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sparse_solver.h` & `mazalib-0.52.4/src/eigen3/test/sparse_solver.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sparse_solvers.cpp` & `mazalib-0.52.4/src/eigen3/test/sparse_solvers.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sparse_vector.cpp` & `mazalib-0.52.4/src/eigen3/test/sparse_vector.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sparselu.cpp` & `mazalib-0.52.4/src/eigen3/test/sparselu.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/sparseqr.cpp` & `mazalib-0.52.4/src/eigen3/test/sparseqr.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/special_numbers.cpp` & `mazalib-0.52.4/src/eigen3/test/special_numbers.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/split_test_helper.h` & `mazalib-0.52.4/src/eigen3/test/split_test_helper.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/spqr_support.cpp` & `mazalib-0.52.4/src/eigen3/test/spqr_support.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/stable_norm.cpp` & `mazalib-0.52.4/src/eigen3/test/stable_norm.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/stddeque.cpp` & `mazalib-0.52.4/src/eigen3/test/stddeque.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/stddeque_overload.cpp` & `mazalib-0.52.4/src/eigen3/test/stddeque_overload.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/stdlist.cpp` & `mazalib-0.52.4/src/eigen3/test/stdlist.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/stdlist_overload.cpp` & `mazalib-0.52.4/src/eigen3/test/stdlist_overload.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/stdvector.cpp` & `mazalib-0.52.4/src/eigen3/test/stdvector.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/stdvector_overload.cpp` & `mazalib-0.52.4/src/eigen3/test/stdvector_overload.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/stl_iterators.cpp` & `mazalib-0.52.4/src/eigen3/test/stl_iterators.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/superlu_support.cpp` & `mazalib-0.52.4/src/eigen3/test/superlu_support.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/svd_common.h` & `mazalib-0.52.4/src/eigen3/test/svd_common.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/svd_fill.h` & `mazalib-0.52.4/src/eigen3/test/svd_fill.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/swap.cpp` & `mazalib-0.52.4/src/eigen3/test/swap.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/symbolic_index.cpp` & `mazalib-0.52.4/src/eigen3/test/symbolic_index.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/triangular.cpp` & `mazalib-0.52.4/src/eigen3/test/triangular.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/type_alias.cpp` & `mazalib-0.52.4/src/eigen3/test/type_alias.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/umeyama.cpp` & `mazalib-0.52.4/src/eigen3/test/umeyama.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/umfpack_support.cpp` & `mazalib-0.52.4/src/eigen3/test/umfpack_support.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/unalignedassert.cpp` & `mazalib-0.52.4/src/eigen3/test/unalignedassert.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/unalignedcount.cpp` & `mazalib-0.52.4/src/eigen3/test/unalignedcount.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/upperbidiagonalization.cpp` & `mazalib-0.52.4/src/eigen3/test/upperbidiagonalization.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/vectorization_logic.cpp` & `mazalib-0.52.4/src/eigen3/test/vectorization_logic.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/vectorwiseop.cpp` & `mazalib-0.52.4/src/eigen3/test/vectorwiseop.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/visitor.cpp` & `mazalib-0.52.4/src/eigen3/test/visitor.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/test/zerosized.cpp` & `mazalib-0.52.4/src/eigen3/test/zerosized.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/AdolcForward` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/AdolcForward`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/AlignedVector3` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/AlignedVector3`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/ArpackSupport` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/ArpackSupport`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/AutoDiff` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/AutoDiff`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/BVH` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/BVH`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/Tensor` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/Tensor`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/TensorSymmetry` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/TensorSymmetry`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/ThreadPool` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/ThreadPool`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/README.md` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/README.md`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMaxSycl.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMaxSycl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlockV2.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlockV2.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSycl.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSycl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclConvertToDeviceExpression.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclConvertToDeviceExpression.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExprConstructor.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExprConstructor.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractAccessor.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractAccessor.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractFunctors.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclExtractFunctors.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclFunctors.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclFunctors.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclLeafCount.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclLeafCount.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclPlaceHolderExpr.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclPlaceHolderExpr.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclRun.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclRun.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclTuple.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorSyclTuple.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/EulerAngles` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/EulerAngles`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/FFT` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/FFT`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/IterativeSolvers` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/IterativeSolvers`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/KroneckerProduct` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/KroneckerProduct`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/LevenbergMarquardt` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/LevenbergMarquardt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/MPRealSupport` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/MPRealSupport`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/MatrixFunctions` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/MatrixFunctions`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/MoreVectorization` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/MoreVectorization`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/NonLinearOptimization` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/NonLinearOptimization`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/NumericalDiff` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/NumericalDiff`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/OpenGLSupport` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/OpenGLSupport`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/Polynomials` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/Polynomials`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/Skyline` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/Skyline`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/SparseExtra` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/SparseExtra`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/SpecialFunctions` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/SpecialFunctions`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/Splines` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/Splines`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/BVH/KdBVH.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/BVH/KdBVH.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Polynomials/Companion.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Polynomials/Companion.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/GpuSpecialFunctions.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/GpuSpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Splines/Spline.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Splines/Spline.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h` & `mazalib-0.52.4/src/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/README.txt` & `mazalib-0.52.4/src/eigen3/unsupported/README.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/bench/bench_svd.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/bench/bench_svd.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/doc/Overview.dox` & `mazalib-0.52.4/src/eigen3/unsupported/doc/Overview.dox`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/doc/eigendoxy_layout.xml.in` & `mazalib-0.52.4/src/eigen3/unsupported/doc/eigendoxy_layout.xml.in`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/doc/examples/BVH_Example.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/doc/examples/BVH_Example.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/doc/examples/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/unsupported/doc/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/doc/examples/EulerAngles.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/doc/examples/EulerAngles.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/doc/examples/FFT.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/doc/examples/FFT.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/doc/examples/MatrixSine.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/doc/examples/MatrixSine.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/doc/examples/MatrixSinh.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/doc/examples/MatrixSinh.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/doc/examples/PolynomialSolver1.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/doc/examples/PolynomialSolver1.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/doc/examples/PolynomialUtils1.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/doc/examples/PolynomialUtils1.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/doc/snippets/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/unsupported/doc/snippets/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/BVH.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/BVH.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/CMakeLists.txt` & `mazalib-0.52.4/src/eigen3/unsupported/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/EulerAngles.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/EulerAngles.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/FFTW.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/FFTW.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/NonLinearOptimization.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/NonLinearOptimization.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/NumericalDiff.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/NumericalDiff.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/alignedvector3.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/alignedvector3.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/autodiff.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/autodiff.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/autodiff_scalar.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/autodiff_scalar.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/bessel_functions.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/bessel_functions.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_eventcount.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_eventcount.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_maxsizevector.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_maxsizevector.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_meta.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_meta.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_non_blocking_thread_pool.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_non_blocking_thread_pool.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_runqueue.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_runqueue.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_argmax.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_argmax.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_argmax_gpu.cu` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_argmax_gpu.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_argmax_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_argmax_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_assign.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_assign.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_block_access.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_block_access.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_block_eval.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_block_eval.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_block_io.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_block_io.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_broadcast_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_broadcast_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_broadcasting.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_broadcasting.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_builtins_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_builtins_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_cast_float16_gpu.cu` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_cast_float16_gpu.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_casts.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_casts.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_chipping.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_chipping.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_chipping_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_chipping_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_comparisons.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_comparisons.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_complex_gpu.cu` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_complex_gpu.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_concatenation.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_concatenation.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_concatenation_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_concatenation_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_const.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_const.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_contract_gpu.cu` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_contract_gpu.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_contract_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_contract_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_contraction.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_contraction.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_convolution.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_convolution.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_convolution_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_convolution_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_custom_index.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_custom_index.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_custom_op.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_custom_op.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_custom_op_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_custom_op_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_device.cu` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_device.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_device_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_device_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_dimension.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_dimension.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_empty.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_empty.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_executor.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_executor.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_expr.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_expr.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_fft.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_fft.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_fixed_size.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_fixed_size.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_forced_eval.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_forced_eval.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_generator.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_generator.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_generator_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_generator_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_gpu.cu` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_gpu.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_ifft.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_ifft.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_image_patch.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_image_patch.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_image_patch_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_image_patch_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_index_list.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_index_list.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_inflation.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_inflation.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_inflation_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_inflation_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_intdiv.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_intdiv.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_io.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_io.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_layout_swap.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_layout_swap.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_lvalue.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_lvalue.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_map.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_map.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_math.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_math.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_mixed_indices.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_mixed_indices.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_morphing.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_morphing.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_morphing_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_morphing_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_move.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_move.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_notification.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_notification.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_of_complex.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_of_complex.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_of_const_values.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_of_const_values.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_of_float16_gpu.cu` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_of_float16_gpu.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_of_strings.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_of_strings.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_padding.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_padding.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_padding_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_padding_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_patch.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_patch.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_patch_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_patch_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_random.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_random.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_random_gpu.cu` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_random_gpu.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_reduction.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_reduction.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_reduction_gpu.cu` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_reduction_gpu.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_reduction_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_reduction_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_ref.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_ref.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_reverse.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_reverse.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_reverse_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_reverse_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_roundings.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_roundings.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_scan.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_scan.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_scan_gpu.cu` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_scan_gpu.cu`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_shuffling.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_shuffling.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_shuffling_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_shuffling_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_simple.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_simple.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_striding.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_striding.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_striding_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_striding_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_sugar.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_sugar.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_symmetry.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_symmetry.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_thread_local.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_thread_local.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_thread_pool.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_thread_pool.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_trace.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_trace.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_uint128.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_uint128.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_volume_patch.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_volume_patch.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/dgmres.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/dgmres.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/forward_adolc.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/forward_adolc.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/gmres.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/gmres.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/kronecker_product.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/kronecker_product.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/levenberg_marquardt.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/levenberg_marquardt.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/matrix_exponential.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/matrix_exponential.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/matrix_function.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/matrix_function.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/matrix_functions.h` & `mazalib-0.52.4/src/eigen3/unsupported/test/matrix_functions.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/matrix_power.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/matrix_power.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/matrix_square_root.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/matrix_square_root.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/minres.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/minres.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/mpreal/mpreal.h` & `mazalib-0.52.4/src/eigen3/unsupported/test/mpreal/mpreal.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/mpreal_support.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/mpreal_support.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/openglsupport.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/openglsupport.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/polynomialsolver.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/polynomialsolver.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/polynomialutils.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/polynomialutils.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/sparse_extra.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/sparse_extra.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/special_functions.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/special_functions.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/eigen3/unsupported/test/splines.cpp` & `mazalib-0.52.4/src/eigen3/unsupported/test/splines.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/mazalib/mazalib.cpp` & `mazalib-0.52.4/src/mazalib/mazalib.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/mazalib.egg-info/SOURCES.txt` & `mazalib-0.52.4/src/mazalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/BinaryIO.h` & `mazalib-0.52.4/src/segmentation/include/BinaryIO.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/CACSegmentation.h` & `mazalib-0.52.4/src/segmentation/include/CACSegmentation.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/DenoiseParameters.h` & `mazalib-0.52.4/src/segmentation/include/DenoiseParameters.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/DynamicArray.h` & `mazalib-0.52.4/src/segmentation/include/DynamicArray.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/ExpectedMaximized.h` & `mazalib-0.52.4/src/segmentation/include/ExpectedMaximized.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/Grid.h` & `mazalib-0.52.4/src/segmentation/include/Grid.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/HessianSegmentation.h` & `mazalib-0.52.4/src/segmentation/include/HessianSegmentation.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/IntegralImage.h` & `mazalib-0.52.4/src/segmentation/include/IntegralImage.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/IterativeNonLocalMeansCPU.h` & `mazalib-0.52.4/src/segmentation/include/IterativeNonLocalMeansCPU.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/KrigingSegmentation.h` & `mazalib-0.52.4/src/segmentation/include/KrigingSegmentation.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/LatticeModel.h` & `mazalib-0.52.4/src/segmentation/include/LatticeModel.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/LogFile.h` & `mazalib-0.52.4/src/segmentation/include/LogFile.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/MRFSegmentation.h` & `mazalib-0.52.4/src/segmentation/include/MRFSegmentation.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/MRFUtils.h` & `mazalib-0.52.4/src/segmentation/include/MRFUtils.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/NelderMead.h` & `mazalib-0.52.4/src/segmentation/include/NelderMead.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/NewCACSegmentation.h` & `mazalib-0.52.4/src/segmentation/include/NewCACSegmentation.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/NoiseLevel.h` & `mazalib-0.52.4/src/segmentation/include/NoiseLevel.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/NonLocalMeans.h` & `mazalib-0.52.4/src/segmentation/include/NonLocalMeans.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/Point.h` & `mazalib-0.52.4/src/segmentation/include/Point.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/Point3d.h` & `mazalib-0.52.4/src/segmentation/include/Point3d.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/RandomNumbers.h` & `mazalib-0.52.4/src/segmentation/include/RandomNumbers.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/RegionGrowthSegmentation.h` & `mazalib-0.52.4/src/segmentation/include/RegionGrowthSegmentation.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/Variation.h` & `mazalib-0.52.4/src/segmentation/include/Variation.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/threshold.h` & `mazalib-0.52.4/src/segmentation/include/threshold.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/util.h` & `mazalib-0.52.4/src/segmentation/include/util.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/var_2d.h` & `mazalib-0.52.4/src/segmentation/include/var_2d.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/include/var_3d.h` & `mazalib-0.52.4/src/segmentation/include/var_3d.h`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/CACSegmentation.cpp` & `mazalib-0.52.4/src/segmentation/src/CACSegmentation.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/ExpectedMaximized.cpp` & `mazalib-0.52.4/src/segmentation/src/ExpectedMaximized.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/Grid.cpp` & `mazalib-0.52.4/src/segmentation/src/Grid.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/HessianSegmentation.cpp` & `mazalib-0.52.4/src/segmentation/src/HessianSegmentation.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/IntegralImage.cpp` & `mazalib-0.52.4/src/segmentation/src/IntegralImage.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/IterativeNonLocalMeansCPU.cpp` & `mazalib-0.52.4/src/segmentation/src/IterativeNonLocalMeansCPU.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/KrigingSegmentation.cpp` & `mazalib-0.52.4/src/segmentation/src/KrigingSegmentation.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/LatticeModel.cpp` & `mazalib-0.52.4/src/segmentation/src/LatticeModel.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/MRFSegmentation.cpp` & `mazalib-0.52.4/src/segmentation/src/MRFSegmentation.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/NoiseLevel.cpp` & `mazalib-0.52.4/src/segmentation/src/NoiseLevel.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/NonLocalMeans.cpp` & `mazalib-0.52.4/src/segmentation/src/NonLocalMeans.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/RandomNumbers.cpp` & `mazalib-0.52.4/src/segmentation/src/RandomNumbers.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/Variation.cpp` & `mazalib-0.52.4/src/segmentation/src/Variation.cpp`

 * *Files identical despite different names*

### Comparing `mazalib-0.52.3/src/segmentation/src/threshold.cpp` & `mazalib-0.52.4/src/segmentation/src/threshold.cpp`

 * *Files identical despite different names*


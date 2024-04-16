# Comparing `tmp/pyDatabases-0.0.5.tar.gz` & `tmp/pydatabases-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDatabases-0.0.5.tar", last modified: Thu Mar  9 15:06:01 2023, max compression
+gzip compressed data, was "pydatabases-0.1.0.tar", last modified: Tue Apr 16 22:36:50 2024, max compression
```

## Comparing `pyDatabases-0.0.5.tar` & `pydatabases-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 15:06:01.092119 pyDatabases-0.0.5/
--rw-rw-rw-   0        0        0     1089 2022-11-24 10:36:30.000000 pyDatabases-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      548 2023-03-09 15:06:01.091649 pyDatabases-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       68 2022-09-12 12:33:52.000000 pyDatabases-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-09 15:06:01.053221 pyDatabases-0.0.5/pyDatabases/
--rw-rw-rw-   0        0        0       61 2022-11-24 10:37:47.000000 pyDatabases-0.0.5/pyDatabases/__init__.py
--rw-rw-rw-   0        0        0    13781 2023-03-09 15:04:07.000000 pyDatabases-0.0.5/pyDatabases/_mixedTools.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:06:01.079151 pyDatabases-0.0.5/pyDatabases/gpyDB/
--rw-rw-rw-   0        0        0       39 2022-11-24 13:26:56.000000 pyDatabases-0.0.5/pyDatabases/gpyDB/__init__.py
--rw-rw-rw-   0        0        0    15876 2023-01-05 13:19:50.000000 pyDatabases-0.0.5/pyDatabases/gpyDB/_database.py
--rw-rw-rw-   0        0        0     9819 2023-01-05 13:19:51.000000 pyDatabases-0.0.5/pyDatabases/gpyDB/gpyDB.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:06:01.082293 pyDatabases-0.0.5/pyDatabases/gpyDB_wheels/
--rw-rw-rw-   0        0        0       56 2022-11-24 16:06:41.000000 pyDatabases-0.0.5/pyDatabases/gpyDB_wheels/__init__.py
--rw-rw-rw-   0        0        0    19834 2023-01-05 12:48:59.000000 pyDatabases-0.0.5/pyDatabases/gpyDB_wheels/gpyDB_wheels.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:06:01.086138 pyDatabases-0.0.5/pyDatabases/simpleDB/
--rw-rw-rw-   0        0        0       23 2023-03-09 13:13:57.000000 pyDatabases-0.0.5/pyDatabases/simpleDB/__init__.py
--rw-rw-rw-   0        0        0     3200 2023-03-09 13:33:11.000000 pyDatabases-0.0.5/pyDatabases/simpleDB/simpleDB.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:06:01.088156 pyDatabases-0.0.5/pyDatabases/simpleDB_wheels/
--rw-rw-rw-   0        0        0       30 2022-09-13 11:42:48.000000 pyDatabases-0.0.5/pyDatabases/simpleDB_wheels/__init__.py
--rw-rw-rw-   0        0        0     5291 2023-03-09 15:04:09.000000 pyDatabases-0.0.5/pyDatabases/simpleDB_wheels/simpleDB_wheels.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:06:01.072194 pyDatabases-0.0.5/pyDatabases.egg-info/
--rw-rw-rw-   0        0        0      548 2023-03-09 15:06:01.000000 pyDatabases-0.0.5/pyDatabases.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2023-03-09 15:06:01.000000 pyDatabases-0.0.5/pyDatabases.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 15:06:01.000000 pyDatabases-0.0.5/pyDatabases.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-03-09 15:06:01.000000 pyDatabases-0.0.5/pyDatabases.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-09 15:06:01.000000 pyDatabases-0.0.5/pyDatabases.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-09 15:06:01.092119 pyDatabases-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-03-09 15:05:15.000000 pyDatabases-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 22:36:50.385957 pydatabases-0.1.0/
+-rw-rw-rw-   0        0        0     1089 2022-11-24 10:36:30.000000 pydatabases-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      761 2024-04-16 22:36:50.384589 pydatabases-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-16 22:31:17.000000 pydatabases-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 22:36:50.308069 pydatabases-0.1.0/pyDatabases/
+-rw-rw-rw-   0        0        0       34 2024-04-15 19:36:01.000000 pydatabases-0.1.0/pyDatabases/__init__.py
+-rw-rw-rw-   0        0        0    12902 2024-04-16 12:46:37.000000 pydatabases-0.1.0/pyDatabases/auxfuncs.py
+drwxrwxrwx   0        0        0        0 2024-04-16 22:36:50.356879 pydatabases-0.1.0/pyDatabases/gpyDB/
+-rw-rw-rw-   0        0        0      101 2024-04-16 22:30:11.000000 pydatabases-0.1.0/pyDatabases/gpyDB/__init__.py
+-rw-rw-rw-   0        0        0    20423 2024-04-16 11:41:37.000000 pydatabases-0.1.0/pyDatabases/gpyDB/database.py
+-rw-rw-rw-   0        0        0    23887 2024-04-16 22:23:52.000000 pydatabases-0.1.0/pyDatabases/gpyDB/gpyDB.py
+drwxrwxrwx   0        0        0        0 2024-04-16 22:36:50.372523 pydatabases-0.1.0/pyDatabases/simpleDB/
+-rw-rw-rw-   0        0        0       23 2024-04-05 12:13:25.000000 pydatabases-0.1.0/pyDatabases/simpleDB/__init__.py
+-rw-rw-rw-   0        0        0     6339 2024-04-15 19:40:03.000000 pydatabases-0.1.0/pyDatabases/simpleDB/simpleDB.py
+drwxrwxrwx   0        0        0        0 2024-04-16 22:36:50.382919 pydatabases-0.1.0/pyDatabases.egg-info/
+-rw-rw-rw-   0        0        0      761 2024-04-16 22:36:50.000000 pydatabases-0.1.0/pyDatabases.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-04-16 22:36:50.000000 pydatabases-0.1.0/pyDatabases.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 22:36:50.000000 pydatabases-0.1.0/pyDatabases.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-16 22:36:50.000000 pydatabases-0.1.0/pyDatabases.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 22:36:50.000000 pydatabases-0.1.0/pyDatabases.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 22:36:50.386795 pydatabases-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-04-16 22:32:56.000000 pydatabases-0.1.0/setup.py
```

### Comparing `pyDatabases-0.0.5/LICENSE` & `pydatabases-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDatabases-0.0.5/pyDatabases/_mixedTools.py` & `pydatabases-0.1.0/pyDatabases/auxfuncs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import itertools, numpy as np, pandas as pd
 from collections.abc import Iterable
 from six import string_types
 _numtypes = (int,float,np.generic)
 _adj_admissable_types = (pd.Index, pd.Series, pd.DataFrame)
 
-# Content:
-# 0. Small auxiliary functions
-# 1. cartesianProductIndex: Creates sparse, cartesian product from iterator of indices.
-# 2. OrdSet: A small class that works like an ordered set.
-# 3. adj: A small class used to subset and adjust pandas-like symbols.
-# 4. adjMultiIndexDB, adjMultiIndex: A couple of classes that helps broadcasting pandas symbols defined over different indices.
+def tryIntIdx(idx):
+	return idx.set_levels([tryIntIdx1d(i) for i in idx.levels])
+
+def tryIntIdx1d(idx):
+	try:
+		return idx.astype(int)
+	except ValueError:
+		return idx
 
-### -------- 	0: Small, auxiliary functions    -------- ###
 def tryint(x):
 	try:
 		return int(x)
 	except ValueError:
 		return x
 
 def ifInt(x):
@@ -106,14 +107,18 @@
 	if is_iterable(by):
 		return x.groupby([k for k in x.index.names if k not in by])
 	else:
 		return x.groupby([k for k in x.index.names if k != by])
 def pdSum(x,sumby):
 	return pdGb(x, sumby).sum() if isinstance(x.index, pd.MultiIndex) else sum(x)
 
+def readSetsFromDb(db, types = None):
+	""" Read sets from database symbols """
+	[db.addOrMerge(set_, getIndex(symbol).get_level_values(set_).unique()) for symbol in db.getTypes(noneInit(types,['var'])).values() for set_ in getIndex(symbol).names];
+
 class OrdSet:
 	def __init__(self,i=None):
 		self.v = list(dict.fromkeys(noneInit(i,[])))
 
 	def __iter__(self):
 		return iter(self.v)
 
@@ -131,25 +136,51 @@
 
 	def __sub__(self,o):
 		return OrdSet([x for x in self.v if x not in o])
 
 	def union(self,*args):
 		return OrdSet(self.__add__([x for l in args for x in l]))
 
-	def intersection(self,*args):
-		return OrdSet([x for l in self.union(args) for x in l if x in self.v])
+	@staticmethod
+	def intersection_(s, ss):
+		s.v = [x for x in s if x in ss]
+		return s
+
+	def intersection(self, *args):
+		out = self.copy()
+		[OrdSet.intersection_(out, x) for x in args]
+		return out
+
+	@staticmethod
+	def partition(s, ss):
+		overlap = OrdSet.intersection(s, ss)
+		return (overlap, s-overlap, ss-overlap)
 
 	def update(self,*args):
 		self.v = self.union(*args).v
 
 	def copy(self):
 		return OrdSet(self.v.copy())
 
 class adj:
 	@staticmethod
+	def rc_AdjGpy(s, c = None, alias = None, lag = None, pm = True, **kwargs):
+		if c is None:
+			return adj.AdjGpy(s,alias=alias, lag = lag)
+		else:
+			copy = s.copy()
+			copy.vals = adj.rc_pd(s=s,c=c,alias=alias,lag=lag,pm=pm)
+			return copy
+	@staticmethod
+	def AdjGpy(symbol, alias = None, lag = None):
+		copy = symbol.copy()
+		copy.vals = adj.rc_AdjPd(symbol.vals, alias=alias, lag = lag)
+		return copy
+
+	@staticmethod
 	def rc_AdjPd(symbol, alias = None, lag = None):
 		if isinstance(symbol, pd.Index):
 			return adj.AdjAliasInd(adj.AdjLagInd(symbol, lag=lag), alias = alias)
 		elif isinstance(symbol, pd.Series):
 			return symbol.to_frame().set_index(adj.AdjAliasInd(adj.AdjLagInd(symbol.index, lag=lag), alias=alias),verify_integrity=False).iloc[:,0]
 		elif isinstance(symbol, pd.DataFrame):
 			return symbol.set_index(adj.AdjAliasInd(adj.AdjLagInd(symbol.index, lag=lag), alias=alias),verify_integrity=False)
@@ -256,92 +287,76 @@
 			return sum(l)>0
 		elif k == 'not' and isinstance(l,(list,set)):
 			return ~l[0]
 		elif k == 'not':
 			return ~l
 
 ### -------- 	4: Broadcasting methods    -------- ###
-class adjMultiIndexDB:
-	@staticmethod
-	def bc(db,x,symbols,fill_value=0, sort_levels=None):
-		v = adjMultiIndexDB.sparsedomain(db,[x]+symbols if is_iterable(symbols) else [x+symbols]).add(x,fill_value=fill_value).rename(x.name)
-		return v if sort_levels is None else v.reorder_levels(sort_levels)
-	@staticmethod
-	def mergeDomains(symbols,db,c=None,sort_levels=None):
-		v = adjMultiIndexDB.sparsedomain(db,symbols, c = ('and', symbols) if c is None else c).dropna().index
-		return v if sort_levels is None else v.reorder_levels(sort_levels)
-	@staticmethod
-	def sparsedomain(db, vlist, c=None):
-		return pd.Series(0, index = adj.rc_pdInd(adjMultiIndexDB.initindex_fromproduct(db,domains_vlist(vlist)), c))
-	@staticmethod	
-	def initindex_fromproduct(db, domains):
-		return pd.MultiIndex.from_product([db.get(s) for s in domains]) if len(domains)>1 else db.get(domains[0])
-
 class adjMultiIndex:
 	@staticmethod
 	def bc(x,y,fill_value = 0):
 		""" Broadcast domain of 'x' to conform with domain of 'y'. """
 		y, y_dom, x_dom = getIndex(y), getDomains(y), getDomains(x)
 		if y_dom:
 			if not x_dom:
 				return pd.Series(x, index = y)
 			elif set(x_dom).intersection(set(y_dom)):
-				return x.add(pd.Series(0, index = y),fill_value=fill_value) if (set(x_dom)-set(y_dom)) else pd.Series(0, index = y).add(x,fill_value=fill_value)
+				return x.add(pd.Series(y, index = y), fill_value =fill_value) if (set(x_dom)-set(y_dom)) else pd.Series(0, index = y).add(x,fill_value=fill_value)
 			else:
 				return pd.Series(0, index = cartesianProductIndex([getIndex(x),y])).add(x,fill_value=fill_value)
 		else:
 			return x
+
 	@staticmethod
 	def bcAdd(x,y,fill_value = 0):
 		""" broadcast domain of 'x' to conform with domain of 'y' and add"""
 		y_dom, x_dom = getDomains(y), getDomains(x)
 		if y_dom:
 			if not x_dom:
 				return y+x
 			elif set(x_dom).intersection(set(y_dom)):
 				return x.add(y, fill_value = fill_value) if (set(x_dom)-set(y_dom)) else y.add(x, fill_value=fill_value)
 			else:
 				return pd.Series(0, index = cartesianProductIndex([getIndex(x),getIndex(y)])).add(x,fill_value=fill_value).add(y, fill_value=fill_value)
 		else:
 			return x+y
+
+	@staticmethod
+	def applyMultIdx(idx, mapping):
+		return pd.Series(0, index = idx).add(pd.Series(0, index = adj.rc_pd(mapping, idx))).dropna().index.reorder_levels(idx.names+[k for k in mapping.names if k not in idx.names])
+
+	@staticmethod
+	def applyMultSrs(s, mapping):
+		if s.empty:
+			return pd.Series([], index = pd.MultiIndex.from_tuples([], names = s.index.names + [k for k in mapping.names if k not in s.index.names]))
+		else:
+			return s.add(pd.Series(0, index = adj.rc_pd(mapping,s)))
+
 	@staticmethod
 	def applyMult(symbol, mapping):
-		""" Apply 'mapping' to a symbol using multiindex """
-		if isinstance(symbol,pd.Index):
-			try: 
-				return (pd.Series(0, index = symbol).add(pd.Series(0, index = adj.rc_pd(mapping,symbol)))).dropna().index.reorder_levels(symbol.names+[k for k in mapping.names if k not in symbol.names])
-			except KeyError:
-				return adhocFix_pandasRemovesIndexLevels(symbol,mapping)
-		elif isinstance(symbol,pd.Series):
-			if symbol.empty:
-				return pd.Series([], index = pd.MultiIndex.from_tuples([], names = symbol.index.names + [k for k in mapping.names if k not in symbol.index.names]))
-			else:
-				s = symbol.add(pd.Series(0, index = adj.rc_pd(mapping,symbol)))
-				try: 
-					return s.reorder_levels(symbol.index.names+[k for k in mapping.names if k not in symbol.index.names])
-				except KeyError:
-					s.index = adhocFix_pandasRemovesIndexLevels(s.index, mapping)
-					return s
+		return adjMultiIndex.applyMultIdx(symbol, mapping) if isinstance(symbol, pd.Index) else adjMultiIndex.applyMultSrs(symbol, mapping)
+
 	@staticmethod
 	def grid(v0,vT,index,gridtype='linear',phi=1):
 		""" If v0, vT are 1d numpy arrays, returns 2d array. If scalars, returns 1d arrays. """
 		if gridtype == 'linear':
 			return np.linspace(v0,vT,len(index))
 		elif gridtype=='polynomial':
 			return np.array([v0+(vT-v0)*((i-1)/(len(index)-1))**phi for i in range(1,len(index)+1)])
+
 	@staticmethod
-	def addGrid(v0,vT,index,name,gridtype = 'linear', phi = 1,sort_levels=None, sort_index = False):
+	def addGrid(v0,vT,index,name,gridtype = 'linear', phi = 1, sort_levels=None, sort_index = False):
 		""" NB: Make sure that v0 and vT are sorted similarly (if they are defined over indices, that is) """
 		if sort_index:
 			v0 = v0.sort_index()
 			vT = vT.sort_index()
 		if isinstance(v0,pd.Series):
 			return pd.DataFrame(adjMultiIndex.grid(v0,vT,index,gridtype=gridtype,phi=phi).T, index = v0.index, columns = index).stack().rename(name).reorder_levels(index.names+v0.index.names if sort_levels is None else sort_levels)
 		else:
 			return pd.Series(adjMultiIndex.grid(v0,vT,index,gridtype=gridtype,phi=phi), index = index,name=name)
 
-def adhocFix_pandasRemovesIndexLevels(symbol, mapping):
-	""" When multiindices are matched, redundant index levels are dropped automatically - this keeps them """
-	s1,s2 = pd.Series(0, index = symbol), pd.Series(0, index = adj.rc_pd(mapping,symbol))
-	x,y = s1.add(s2).dropna().index, s2.add(s1).dropna().index
-	x_df, y_df = x.to_frame().set_index(list(set(x.names).intersection(y.names))), y.to_frame().set_index(list(set(x.names).intersection(y.names)))
-	return pd.MultiIndex.from_frame(pd.concat([x_df, y_df], axis =1).reset_index())
+def emptyCopy(obj):
+	class Empty(obj.__class__):
+		def __init__(self): pass
+	newcopy = Empty()
+	newcopy.__class__ = obj.__class__
+	return newcopy
```

### Comparing `pyDatabases-0.0.5/pyDatabases/simpleDB_wheels/simpleDB_wheels.py` & `pydatabases-0.1.0/pyDatabases/simpleDB/simpleDB.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,125 @@
-from pyDatabases._mixedTools import *
-from pyDatabases.simpleDB.simpleDB import SimpleDB, type_
+from pyDatabases.auxfuncs import *
+from pyDatabases.auxfuncs import _numtypes
+from copy import deepcopy
 import openpyxl,io
 
-# 1: Read methods:
-class read:
+def type_(s):
+	if isinstance(s, pd.Index):
+		return 'set'
+	elif isinstance(s, pd.Series):
+		return 'variable'
+	elif isinstance(s,_numtypes):
+		return 'scalar'
+	else:
+		return 'other'
+
+def mergeVals(s1,s2):
+	if isinstance(s1,pd.Series):
+		return s1.combine_first(s2)
+	elif isinstance(s1,pd.Index):
+		return s1.union(s2)
+	else:
+		return s1
+
+def symbols_(db_i):
+	""" return dictionary of symbols """
+	return db_i.symbols if isinstance(db_i, SimpleDB) else db_i
+
+class SimpleDB:
+	""" Collection of data """
+	def __init__(self,name='name',symbols=None,alias=None):
+		self.name = name
+		self.symbols = noneInit(symbols,{})
+		self.updateAlias(alias=alias)
+
+	def updateAlias(self,alias=None):
+		self.alias = self.alias.union(pd.MultiIndex.from_tuples(noneInit(alias,[]), names = ['from','to'])) if hasattr(self,'alias') else pd.MultiIndex.from_tuples(noneInit(alias,[]), names = ['from','to'])
+
+	def __iter__(self):
+		return iter(self.symbols.values())
+
+	def __len__(self):
+		return len(self.symbols)
+
+	def __getitem__(self,item):
+		try:
+			return self.symbols[item]
+		except KeyError:
+			try:
+				return self.symbols[self.getAlias(item)].rename(item)
+			except TypeError:
+				raise KeyError(f"Symbol {item} not in database")
+
+	def __setitem__(self,item,value):
+		if item in self.symbols:
+			if not is_iterable(value) and is_iterable(self[item]):
+				value = pd.Series(value,index=self[item].index,name=self[item].name)
+		self.symbols[item] = value
+
+	def __delitem__(self,item):
+		del(self.symbols[item])
+
+	def copy(self):
+		obj = type(self).__new__(self.__class__,None)
+		obj.__dict__.update(deepcopy(self.__dict__).items())
+		return obj
+
+	def getTypes(self,types=['variable']):
+		return {k:v for k,v in self.symbols.items() if type_(v) in types}
+
+	def variableDomains(self,set_,types=['variable']):
+		""" Return 'types' defined over 'set_'"""
+		return {k:v for k,v in self.getTypes(types).items() if set_ in getDomains(v)}
+
+	@property
+	def aliasDict(self):
+		return {k: self.alias.get_level_values(1)[self.alias.get_level_values(0) == k] for k in self.alias.get_level_values(0).unique()}
+
+	@property
+	def aliasDict0(self):
+		return {key: self.aliasDict[key].insert(0,key) for key in self.aliasDict}
+
+	def getAlias(self,x,index_=0):
+		if x in self.alias.get_level_values(0):
+			return self.aliasDict0[x][index_]
+		elif x in self.alias.get_level_values(1):
+			return self.aliasDict0[self.alias.get_level_values(0)[self.alias.get_level_values(1)==x][0]][index_]
+		elif x in self.getTypes(['set']) and index_==0:
+			return x
+		else:
+			raise TypeError(f"{x} is not aliased")
+
+	def addOrMerge(self, name, symbol, priority = 'first'):
+		if name in self.symbols:
+			self[name] = mergeVals(self.symbols[name],symbol) if priority == 'first' else mergeVals(symbol, self.symbols[name])
+		else:
+			self[name] = symbol
+
+	def mergeDbs(self, dbOther, priority='first'):
+		""" Merge all symbols in two databases """
+		[self.addOrMerge(name, symbol, priority=priority) for name,symbol in symbols_(dbOther).items()];
+
+class ReadFromExcel:
 	@staticmethod
 	def dbFromWB(workbook, kwargs, spliton='/'):
 		""" 'read' should be a dictionary with keys = method, value = list of sheets to apply this to."""
-		wb = read.simpleLoad(workbook) if isinstance(workbook,str) else workbook
+		wb = ReadFromExcel.simpleLoad(workbook) if isinstance(workbook,str) else workbook
 		db = SimpleDB()
-		[db.mergeDbs(getattr(read, function)(wb[sheet],spliton=spliton)) for function,sheets in kwargs.items() for sheet in sheets];
+		[db.mergeDbs(getattr(ReadFromExcel, function)(wb[sheet],spliton=spliton)) for function,sheets in kwargs.items() for sheet in sheets];
 		return db
 
 	@staticmethod
 	def simpleLoad(workbook):
 		with open(workbook,"rb") as file:
 			in_mem_file = io.BytesIO(file.read())
 		return openpyxl.load_workbook(in_mem_file,read_only=True,data_only=True)
 
-	def sheetnames_from_wb(self, wb):
+	@staticmethod
+	def sheetnames_from_wb(wb):
 		return (sheet.title for sheet in wb._sheets)
 
 	@staticmethod
 	def sets(sheet, **kwargs):
 		""" Return a dictionary with keys = set names and values = pandas objects. na entries are removed. 
 			The name of each set is defined as the first entry in each column. """
 		pd_sheet = pd.DataFrame(sheet.values)
@@ -39,15 +136,15 @@
 		pd_temp.columns = [x.split(spliton)[1] for x in pd_temp.iloc[0,:]]
 		return pd.MultiIndex.from_frame(pd_temp.dropna().iloc[1:,:])
 
 	@staticmethod
 	def maps(sheet,spliton='/'):
 		pd_sheet = pd.DataFrame(sheet.values)
 		pd_sheet.columns = [x.split(spliton)[0] for x in pd_sheet.iloc[0,:]]
-		return {col: read.aux_map(pd_sheet,col,spliton) for col in set(pd_sheet.columns)}
+		return {col: ReadFromExcel.aux_map(pd_sheet,col,spliton) for col in set(pd_sheet.columns)}
 
 	@staticmethod
 	def aux_var(sheet,col,spliton):
 		pd_temp = sheet[col].dropna()
 		pd_temp.columns = [x.split(spliton)[1] for x in pd_temp.iloc[0,:]]
 		if pd_temp.shape[1]==2:
 			index = pd.Index(pd_temp.iloc[1:,0])
@@ -55,64 +152,22 @@
 			index = pd.MultiIndex.from_frame(pd_temp.iloc[1:,:-1])
 		return pd.Series(pd_temp.iloc[1:,-1].values,index=index,name=col)
 
 	@staticmethod
 	def variables(sheet,spliton='/'):
 		pd_sheet = pd.DataFrame(sheet.values)
 		pd_sheet.columns = [x.split(spliton)[0] for x in pd_sheet.iloc[0,:]]
-		return {col: read.aux_var(pd_sheet,col,spliton) for col in set(pd_sheet.columns)}
+		return {col: ReadFromExcel.aux_var(pd_sheet,col,spliton) for col in set(pd_sheet.columns)}
 
 	@staticmethod
 	def scalars(sheet,**kwargs):
 		pd_sheet = pd.DataFrame(sheet.values)
 		return {pd_sheet.iloc[i,0]: pd_sheet.iloc[i,1] for i in range(pd_sheet.shape[0])}
 
 	@staticmethod
 	def variable2D(sheet,spliton='/',**kwargs):
 		""" Read in 2d variable arranged in matrix; Note, only reads 1 variable per sheet."""
 		pd_sheet = pd.DataFrame(sheet.values)
 		domains = pd_sheet.iloc[0,0].split(spliton)
 		var = pd.DataFrame(pd_sheet.iloc[1:,1:].values, index = pd.Index(pd_sheet.iloc[1:,0],name=domains[1]), columns = pd.Index(pd_sheet.iloc[0,1:], name = domains[2])).stack()
 		var.name = domains[0]
 		return {domains[0]: var}
-
-# 2: 
-def readSets(db, types = None):
-	""" Read sets from database symbols """
-	[db.addOrMerge(set_, getIndex(symbol).get_level_values(set_).unique()) for symbol in db.getTypes(noneInit(types,['variable'])).values() for set_ in getIndex(symbol).names];
-
-# 3: Broadcasting-like methods
-def applyMult(symbol, mapping):
-	""" Apply 'mapping' to a symbol using multiindex """
-	if isinstance(symbol,pd.Index):
-		return (pd.Series(0, index = symbol).add(pd.Series(0, index = rc_pd(mapping,symbol)))).dropna().index.reorder_levels(symbol.names+[k for k in mapping.names if k not in symbol.names])
-	elif isinstance(symbol,pd.Series):
-		if symbol.empty:
-			return pd.Series([], index = pd.MultiIndex.from_tuples([], names = symbol.index.names + [k for k in mapping.names if k not in symbol.index.names]))
-		else: 
-			return symbol.add(pd.Series(0, index = rc_pd(mapping,symbol))).reorder_levels(symbol.index.names+[k for k in mapping.names if k not in symbol.index.names])
-
-def appendIndexWithCopy(index, copyLevel, newLevel):
-	if is_iterable(copyLevel):
-		return pd.MultiIndex.from_frame(index.to_frame(index=False).assign(**{newLevel[i]: index.get_level_values(copyLevel[i]) for i in range(len(copyLevel))}))
-	else: 
-		return pd.MultiIndex.from_frame(index.to_frame(index=False).assign(**{newLevel: index.get_level_values(copyLevel)}))
-
-def broadcast(x,y,fill_value=0):
-	""" y is a index or None, x is a scalar or series."""
-	if type_(y) == 'set':
-		if getDomains(y):
-			if not getDomains(x):
-				return pd.Series(x, index = y)
-			elif set(getDomains(x)).intersection(set(getDomains(y))):
-				if set(getDomains(x))-set(getDomains(y)):
-					return x.add(pd.Series(0, index = y), fill_value=fill_value)
-				else:
-					return pd.Series(0, index=y).add(x,fill_value=fill_value)
-			else:
-				return pd.Series(0, index = cartesianProductIndex([database.getIndex(x),y])).add(x,fill_value=fill_value)
-		else:
-			return x
-	else:
-		b = broadcast(x, getIndex(y),fill_value=fill_value)
-		return b.add(y,fill_value=fill_value) if isinstance(b,pd.Series) else x+y
-
```


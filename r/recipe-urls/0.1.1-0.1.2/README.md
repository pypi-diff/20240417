# Comparing `tmp/recipe_urls-0.1.1.tar.gz` & `tmp/recipe_urls-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recipe_urls-0.1.1.tar", last modified: Tue Apr 16 22:02:31 2024, max compression
+gzip compressed data, was "recipe_urls-0.1.2.tar", last modified: Tue Apr 16 22:09:47 2024, max compression
```

## Comparing `recipe_urls-0.1.1.tar` & `recipe_urls-0.1.2.tar`

### file list

```diff
@@ -1,235 +1,238 @@
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:02:31.606646 recipe_urls-0.1.1/
--rw-r--r--   0 mkayeterry   (501) staff       (20)     6148 2024-04-16 16:01:33.000000 recipe_urls-0.1.1/.DS_Store
--rw-r--r--   0 mkayeterry   (501) staff       (20)       24 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/.gitignore
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1069 2024-04-01 22:10:57.000000 recipe_urls-0.1.1/LICENSE
--rw-r--r--   0 mkayeterry   (501) staff       (20)     4551 2024-04-16 22:02:31.606400 recipe_urls-0.1.1/PKG-INFO
--rw-r--r--   0 mkayeterry   (501) staff       (20)     3606 2024-04-16 21:56:08.000000 recipe_urls-0.1.1/README.md
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1073 2024-04-16 21:59:08.000000 recipe_urls-0.1.1/pyproject.toml
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:02:31.564245 recipe_urls-0.1.1/recipe_urls/
--rw-r--r--   0 mkayeterry   (501) staff       (20)     6148 2024-04-16 16:01:38.000000 recipe_urls-0.1.1/recipe_urls/.DS_Store
--rw-r--r--   0 mkayeterry   (501) staff       (20)    11850 2024-04-16 21:59:02.000000 recipe_urls-0.1.1/recipe_urls/__init__.py
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:02:31.603856 recipe_urls-0.1.1/recipe_urls/__pycache__/
--rw-r--r--   0 mkayeterry   (501) staff       (20)     8945 2024-04-16 16:25:22.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1892 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/_abstract.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2741 2024-04-16 20:46:05.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/_utils.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2003 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/abuelascounter.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2098 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/acouplecooks.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1671 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/addapinch.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1782 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/afghankitchenrecipes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1703 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/allrecipes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2256 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/ambitiouskitchen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2164 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/archanaskitchen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1994 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/averiecooks.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1717 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/bakingmischief.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1755 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/bakingsense.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1744 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/barefootcontessa.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1584 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/base_scraper.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1646 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/bbc.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1750 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/bettycrocker.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1916 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/bigoven.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1707 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/bluejeanchef.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1703 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/bonappetit.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1682 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/bongeats.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2028 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/bowlofdelicious.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2007 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/budgetbytes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2010 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/carlsbadcravings.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1984 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/castironketo.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1698 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/cdkitchen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1973 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/chefsavvy.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1995 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/closetcooking.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1713 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/cookieandkate.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1721 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/cookpad.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1651 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/copykat.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1741 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/countryliving.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1993 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/creativecanning.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1974 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/davidlebovitz.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1680 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/delish.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2029 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/domesticateme.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1971 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/downshiftology.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2035 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/eatingbirdfood.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1990 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/eatingwell.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2100 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/eatliverun.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2076 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/eatsmarter.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1693 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/eatwell101.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1725 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/eatwhattonight.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1975 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/elavegan.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1710 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/epicurious.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2066 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/errenskitchen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2022 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/ethanchlebowski.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2044 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/farmhouseonboone.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1732 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/fifteenspatulas.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1773 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/finedininglovers.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1942 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/fitmencook.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2027 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/fitslowcookerqueen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1648 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/food.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1660 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/food52.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2011 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/foodandwine.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1726 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/foodnetwork.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1716 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/foodrepublic.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2008 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/forksoverknives.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1990 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/forktospoon.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2008 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/gimmesomeoven.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2015 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/gonnawantseconds.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2062 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/goodfooddiscoveries.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1747 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/goodhousekeeping.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1762 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/greatbritishchefs.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1693 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/grimgrains.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2089 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/halfbakedharvest.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1989 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/handletheheat.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2096 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/headbangerskitchen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1738 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/heatherchristo.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1651 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/heb.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1702 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/hellofresh.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1750 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/hersheyland.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1952 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/hostthetoast.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1913 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/imworthy.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2048 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/indianhealthyrecipes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2038 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/insanelygoodrecipes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2016 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/inspiralized.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1980 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/izzycooking.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1731 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/jamieoliver.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2010 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/jimcooksfoodgood.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2027 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/joyfoodsunshine.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1700 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/justataste.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1948 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/justbento.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2131 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/justonecookbook.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1767 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/kingarthurbaking.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2054 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/leanandgreenrecipes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2053 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/lifestyleofafoodie.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2012 2024-04-04 16:22:13.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/littlespicejar.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2057 2024-04-04 16:40:16.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/livelytable.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2010 2024-04-04 19:29:31.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/lovingitvegan.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1737 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/ninjatestkitchen.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1685 2024-04-01 22:06:07.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/nytimes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1982 2024-04-04 19:32:04.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/ohsheglows.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1727 2024-04-12 20:09:17.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/onceuponachef.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2056 2024-04-12 20:18:36.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/paleorunningmomma.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2028 2024-04-12 20:32:55.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/persnicketyplates.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1712 2024-04-16 14:21:04.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/pickuplimes.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1921 2024-04-12 20:33:23.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/pinchofyum.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1985 2024-04-16 14:22:53.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/platingpixels.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2046 2024-04-16 14:37:50.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/rachlmansfield.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2122 2024-04-16 14:47:26.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/rainbowplantlife.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2009 2024-04-16 14:58:24.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/reciperunner.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2129 2024-04-16 15:05:11.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/sallysbakingaddiction.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2019 2024-04-16 15:11:06.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/simpleveganista.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1942 2024-04-16 15:16:27.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/simplyquinoa.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2024 2024-04-16 15:28:00.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/simplywhisked.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     2012 2024-04-16 15:32:14.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/southernliving.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1974 2024-04-16 15:48:41.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/tasteofhome.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1649 2024-04-16 15:50:33.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/tasty.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)      919 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1654 2024-04-16 15:55:58.000000 recipe_urls-0.1.1/recipe_urls/__pycache__/yummly.cpython-310.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1298 2024-04-16 21:18:48.000000 recipe_urls-0.1.1/recipe_urls/_abstract.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     3849 2024-04-16 20:45:56.000000 recipe_urls-0.1.1/recipe_urls/_utils.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1421 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/abuelascounter.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1702 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/acouplecooks.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1143 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/addapinch.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1199 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/afghankitchenrecipes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1170 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/allrecipes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1959 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/ambitiouskitchen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1804 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/archanaskitchen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1404 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/averiecooks.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1163 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/bakingmischief.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1216 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/bakingsense.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1180 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/barefootcontessa.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1144 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/bbc.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1204 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/bettycrocker.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1327 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/bigoven.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1163 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/bluejeanchef.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1166 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/bonappetit.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1155 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/bongeats.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1450 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/bowlofdelicious.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1500 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/budgetbytes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1404 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/carlsbadcravings.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1409 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/castironketo.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1170 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/cdkitchen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1463 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/chefsavvy.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1416 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/closetcooking.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1169 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/cookieandkate.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1132 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/copykat.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1189 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/countryliving.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1387 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/creativecanning.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1363 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/davidlebovitz.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1163 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/delish.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1526 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/domesticateme.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1343 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/downshiftology.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1525 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/eatingbirdfood.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1474 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/eatingwell.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1764 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/eatliverun.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1612 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/eatsmarter.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1159 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/eatwell101.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1171 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/eatwhattonight.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1516 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/elavegan.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1173 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/epicurious.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1593 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/errenskitchen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1396 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/ethanchlebowski.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1492 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/farmhouseonboone.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1174 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/fifteenspatulas.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1206 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/finedininglovers.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1339 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/fitmencook.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1418 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/fitslowcookerqueen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1148 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/food.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1143 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/food52.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1424 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/foodandwine.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1187 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/foodnetwork.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1169 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/foodrepublic.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1371 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/forksoverknives.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1483 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/forktospoon.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1445 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/gimmesomeoven.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1405 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/gonnawantseconds.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1463 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/goodfooddiscoveries.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1201 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/goodhousekeeping.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1193 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/greatbritishchefs.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1568 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/halfbakedharvest.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1426 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/handletheheat.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1528 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/headbangerskitchen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1184 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/heatherchristo.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1168 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/hellofresh.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1203 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/hersheyland.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1337 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/hostthetoast.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1322 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/imworthy.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1396 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/indianhealthyrecipes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1414 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/insanelygoodrecipes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1490 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/inspiralized.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1429 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/izzycooking.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1189 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/jamieoliver.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1399 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/jimcooksfoodgood.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1452 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/joyfoodsunshine.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1166 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/justataste.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1348 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/justbento.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1721 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/justonecookbook.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1200 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/kingarthurbaking.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1405 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/leanandgreenrecipes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1475 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/lifestyleofafoodie.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1473 2024-04-04 16:22:06.000000 recipe_urls-0.1.1/recipe_urls/littlespicejar.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1640 2024-04-04 16:40:12.000000 recipe_urls-0.1.1/recipe_urls/livelytable.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1492 2024-04-04 19:16:48.000000 recipe_urls-0.1.1/recipe_urls/lovingitvegan.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1173 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/ninjatestkitchen.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1163 2024-04-01 22:04:35.000000 recipe_urls-0.1.1/recipe_urls/nytimes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1500 2024-04-04 19:31:59.000000 recipe_urls-0.1.1/recipe_urls/ohsheglows.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1178 2024-04-04 19:36:45.000000 recipe_urls-0.1.1/recipe_urls/onceuponachef.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1484 2024-04-12 20:18:31.000000 recipe_urls-0.1.1/recipe_urls/paleorunningmomma.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1394 2024-04-12 20:24:05.000000 recipe_urls-0.1.1/recipe_urls/persnicketyplates.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1170 2024-04-16 14:17:37.000000 recipe_urls-0.1.1/recipe_urls/pickuplimes.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1392 2024-04-16 14:22:48.000000 recipe_urls-0.1.1/recipe_urls/platingpixels.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1536 2024-04-16 14:34:49.000000 recipe_urls-0.1.1/recipe_urls/rachlmansfield.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1675 2024-04-16 14:47:20.000000 recipe_urls-0.1.1/recipe_urls/rainbowplantlife.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1481 2024-04-16 14:54:23.000000 recipe_urls-0.1.1/recipe_urls/reciperunner.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1622 2024-04-16 15:05:05.000000 recipe_urls-0.1.1/recipe_urls/sallysbakingaddiction.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1443 2024-04-16 15:11:01.000000 recipe_urls-0.1.1/recipe_urls/simpleveganista.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1475 2024-04-16 15:23:57.000000 recipe_urls-0.1.1/recipe_urls/simplywhisked.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1375 2024-04-16 15:36:30.000000 recipe_urls-0.1.1/recipe_urls/tasteofhome.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     1137 2024-04-16 15:50:26.000000 recipe_urls-0.1.1/recipe_urls/tasty.py
--rw-r--r--   0 mkayeterry   (501) staff       (20)     5570 2024-04-16 20:49:32.000000 recipe_urls-0.1.1/recipe_urls/testing.py
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:02:31.605739 recipe_urls-0.1.1/recipe_urls.egg-info/
--rw-r--r--   0 mkayeterry   (501) staff       (20)     4551 2024-04-16 22:02:31.000000 recipe_urls-0.1.1/recipe_urls.egg-info/PKG-INFO
--rw-r--r--   0 mkayeterry   (501) staff       (20)     9200 2024-04-16 22:02:31.000000 recipe_urls-0.1.1/recipe_urls.egg-info/SOURCES.txt
--rw-r--r--   0 mkayeterry   (501) staff       (20)        1 2024-04-16 22:02:31.000000 recipe_urls-0.1.1/recipe_urls.egg-info/dependency_links.txt
--rw-r--r--   0 mkayeterry   (501) staff       (20)       75 2024-04-16 22:02:31.000000 recipe_urls-0.1.1/recipe_urls.egg-info/requires.txt
--rw-r--r--   0 mkayeterry   (501) staff       (20)       12 2024-04-16 22:02:31.000000 recipe_urls-0.1.1/recipe_urls.egg-info/top_level.txt
--rw-r--r--   0 mkayeterry   (501) staff       (20)       38 2024-04-16 22:02:31.606699 recipe_urls-0.1.1/setup.cfg
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:02:31.604189 recipe_urls-0.1.1/tests/
-drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:02:31.605226 recipe_urls-0.1.1/tests/__pycache__/
--rw-r--r--   0 mkayeterry   (501) staff       (20)    25473 2024-04-16 20:23:46.000000 recipe_urls-0.1.1/tests/__pycache__/test_get_site_origin.cpython-310-pytest-8.1.1.pyc
--rw-r--r--   0 mkayeterry   (501) staff       (20)    33786 2024-04-16 20:23:36.000000 recipe_urls-0.1.1/tests/test_get_site_origin.py
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:09:47.903607 recipe_urls-0.1.2/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     6148 2024-04-16 16:01:33.000000 recipe_urls-0.1.2/.DS_Store
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       24 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/.gitignore
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1069 2024-04-01 22:10:57.000000 recipe_urls-0.1.2/LICENSE
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     4521 2024-04-16 22:09:47.903361 recipe_urls-0.1.2/PKG-INFO
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     3576 2024-04-16 22:07:26.000000 recipe_urls-0.1.2/README.md
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:09:47.798679 recipe_urls-0.1.2/dist/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   231966 2024-04-16 22:08:43.000000 recipe_urls-0.1.2/dist/recipe_urls-0.1.1-py3-none-any.whl
+-rw-r--r--   0 mkayeterry   (501) staff       (20)   314217 2024-04-16 22:08:41.000000 recipe_urls-0.1.2/dist/recipe_urls-0.1.1.tar.gz
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1073 2024-04-16 22:09:07.000000 recipe_urls-0.1.2/pyproject.toml
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:09:47.845714 recipe_urls-0.1.2/recipe_urls/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     6148 2024-04-16 16:01:38.000000 recipe_urls-0.1.2/recipe_urls/.DS_Store
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    11850 2024-04-16 22:09:11.000000 recipe_urls-0.1.2/recipe_urls/__init__.py
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:09:47.900848 recipe_urls-0.1.2/recipe_urls/__pycache__/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     8945 2024-04-16 16:25:22.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1892 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/_abstract.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2741 2024-04-16 20:46:05.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/_utils.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2003 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/abuelascounter.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2098 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/acouplecooks.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1671 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/addapinch.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1782 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/afghankitchenrecipes.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1703 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/allrecipes.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2256 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/ambitiouskitchen.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2164 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/archanaskitchen.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1994 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/averiecooks.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1717 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/bakingmischief.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1755 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/bakingsense.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1744 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/barefootcontessa.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1584 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/base_scraper.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1646 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/bbc.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1750 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/bettycrocker.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1916 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/bigoven.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1707 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/bluejeanchef.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1703 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/bonappetit.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1682 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/bongeats.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2028 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/bowlofdelicious.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2007 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/budgetbytes.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2010 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/carlsbadcravings.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1984 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/castironketo.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1698 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/cdkitchen.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1973 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/chefsavvy.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1995 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/closetcooking.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1713 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/cookieandkate.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1721 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/cookpad.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1651 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/copykat.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1741 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/countryliving.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1993 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/creativecanning.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1974 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/davidlebovitz.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1680 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/delish.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2029 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/domesticateme.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1971 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/downshiftology.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2035 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/eatingbirdfood.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1990 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/eatingwell.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2100 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/eatliverun.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2076 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/eatsmarter.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1693 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/eatwell101.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1725 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/eatwhattonight.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1975 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/elavegan.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1710 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/epicurious.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2066 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/errenskitchen.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2022 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/ethanchlebowski.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2044 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/farmhouseonboone.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1732 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/fifteenspatulas.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1773 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/finedininglovers.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1942 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/fitmencook.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2027 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/fitslowcookerqueen.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1648 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/food.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1660 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/food52.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2011 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/foodandwine.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1726 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/foodnetwork.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1716 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/foodrepublic.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2008 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/forksoverknives.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1990 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/forktospoon.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2008 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/gimmesomeoven.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2015 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/gonnawantseconds.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2062 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/goodfooddiscoveries.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1747 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/goodhousekeeping.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1762 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/greatbritishchefs.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1693 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/grimgrains.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2089 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/halfbakedharvest.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1989 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/handletheheat.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2096 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/headbangerskitchen.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1738 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/heatherchristo.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1651 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/heb.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1702 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/hellofresh.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1750 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/hersheyland.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1952 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/hostthetoast.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1913 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/imworthy.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2048 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/indianhealthyrecipes.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2038 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/insanelygoodrecipes.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2016 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/inspiralized.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1980 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/izzycooking.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1731 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/jamieoliver.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2010 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/jimcooksfoodgood.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2027 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/joyfoodsunshine.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1700 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/justataste.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1948 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/justbento.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2131 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/justonecookbook.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1767 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/kingarthurbaking.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2054 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/leanandgreenrecipes.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2053 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/lifestyleofafoodie.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2012 2024-04-04 16:22:13.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/littlespicejar.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2057 2024-04-04 16:40:16.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/livelytable.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2010 2024-04-04 19:29:31.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/lovingitvegan.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1737 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/ninjatestkitchen.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1685 2024-04-01 22:06:07.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/nytimes.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1982 2024-04-04 19:32:04.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/ohsheglows.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1727 2024-04-12 20:09:17.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/onceuponachef.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2056 2024-04-12 20:18:36.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/paleorunningmomma.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2028 2024-04-12 20:32:55.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/persnicketyplates.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1712 2024-04-16 14:21:04.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/pickuplimes.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1921 2024-04-12 20:33:23.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/pinchofyum.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1985 2024-04-16 14:22:53.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/platingpixels.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2046 2024-04-16 14:37:50.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/rachlmansfield.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2122 2024-04-16 14:47:26.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/rainbowplantlife.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2009 2024-04-16 14:58:24.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/reciperunner.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2129 2024-04-16 15:05:11.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/sallysbakingaddiction.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2019 2024-04-16 15:11:06.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/simpleveganista.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1942 2024-04-16 15:16:27.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/simplyquinoa.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2024 2024-04-16 15:28:00.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/simplywhisked.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     2012 2024-04-16 15:32:14.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/southernliving.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1974 2024-04-16 15:48:41.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/tasteofhome.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1649 2024-04-16 15:50:33.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/tasty.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)      919 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1654 2024-04-16 15:55:58.000000 recipe_urls-0.1.2/recipe_urls/__pycache__/yummly.cpython-310.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1298 2024-04-16 21:18:48.000000 recipe_urls-0.1.2/recipe_urls/_abstract.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     3849 2024-04-16 20:45:56.000000 recipe_urls-0.1.2/recipe_urls/_utils.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1421 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/abuelascounter.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1702 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/acouplecooks.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1143 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/addapinch.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1199 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/afghankitchenrecipes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1170 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/allrecipes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1959 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/ambitiouskitchen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1804 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/archanaskitchen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1404 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/averiecooks.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1163 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/bakingmischief.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1216 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/bakingsense.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1180 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/barefootcontessa.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1144 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/bbc.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1204 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/bettycrocker.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1327 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/bigoven.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1163 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/bluejeanchef.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1166 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/bonappetit.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1155 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/bongeats.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1450 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/bowlofdelicious.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1500 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/budgetbytes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1404 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/carlsbadcravings.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1409 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/castironketo.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1170 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/cdkitchen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1463 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/chefsavvy.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1416 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/closetcooking.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1169 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/cookieandkate.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1132 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/copykat.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1189 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/countryliving.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1387 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/creativecanning.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1363 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/davidlebovitz.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1163 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/delish.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1526 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/domesticateme.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1343 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/downshiftology.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1525 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/eatingbirdfood.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1474 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/eatingwell.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1764 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/eatliverun.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1612 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/eatsmarter.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1159 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/eatwell101.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1171 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/eatwhattonight.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1516 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/elavegan.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1173 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/epicurious.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1593 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/errenskitchen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1396 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/ethanchlebowski.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1492 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/farmhouseonboone.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1174 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/fifteenspatulas.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1206 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/finedininglovers.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1339 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/fitmencook.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1418 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/fitslowcookerqueen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1148 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/food.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1143 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/food52.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1424 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/foodandwine.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1187 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/foodnetwork.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1169 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/foodrepublic.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1371 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/forksoverknives.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1483 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/forktospoon.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1445 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/gimmesomeoven.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1405 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/gonnawantseconds.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1463 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/goodfooddiscoveries.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1201 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/goodhousekeeping.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1193 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/greatbritishchefs.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1568 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/halfbakedharvest.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1426 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/handletheheat.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1528 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/headbangerskitchen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1184 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/heatherchristo.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1168 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/hellofresh.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1203 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/hersheyland.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1337 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/hostthetoast.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1322 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/imworthy.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1396 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/indianhealthyrecipes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1414 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/insanelygoodrecipes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1490 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/inspiralized.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1429 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/izzycooking.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1189 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/jamieoliver.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1399 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/jimcooksfoodgood.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1452 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/joyfoodsunshine.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1166 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/justataste.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1348 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/justbento.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1721 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/justonecookbook.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1200 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/kingarthurbaking.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1405 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/leanandgreenrecipes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1475 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/lifestyleofafoodie.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1473 2024-04-04 16:22:06.000000 recipe_urls-0.1.2/recipe_urls/littlespicejar.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1640 2024-04-04 16:40:12.000000 recipe_urls-0.1.2/recipe_urls/livelytable.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1492 2024-04-04 19:16:48.000000 recipe_urls-0.1.2/recipe_urls/lovingitvegan.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1173 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/ninjatestkitchen.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1163 2024-04-01 22:04:35.000000 recipe_urls-0.1.2/recipe_urls/nytimes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1500 2024-04-04 19:31:59.000000 recipe_urls-0.1.2/recipe_urls/ohsheglows.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1178 2024-04-04 19:36:45.000000 recipe_urls-0.1.2/recipe_urls/onceuponachef.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1484 2024-04-12 20:18:31.000000 recipe_urls-0.1.2/recipe_urls/paleorunningmomma.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1394 2024-04-12 20:24:05.000000 recipe_urls-0.1.2/recipe_urls/persnicketyplates.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1170 2024-04-16 14:17:37.000000 recipe_urls-0.1.2/recipe_urls/pickuplimes.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1392 2024-04-16 14:22:48.000000 recipe_urls-0.1.2/recipe_urls/platingpixels.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1536 2024-04-16 14:34:49.000000 recipe_urls-0.1.2/recipe_urls/rachlmansfield.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1675 2024-04-16 14:47:20.000000 recipe_urls-0.1.2/recipe_urls/rainbowplantlife.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1481 2024-04-16 14:54:23.000000 recipe_urls-0.1.2/recipe_urls/reciperunner.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1622 2024-04-16 15:05:05.000000 recipe_urls-0.1.2/recipe_urls/sallysbakingaddiction.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1443 2024-04-16 15:11:01.000000 recipe_urls-0.1.2/recipe_urls/simpleveganista.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1475 2024-04-16 15:23:57.000000 recipe_urls-0.1.2/recipe_urls/simplywhisked.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1375 2024-04-16 15:36:30.000000 recipe_urls-0.1.2/recipe_urls/tasteofhome.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     1137 2024-04-16 15:50:26.000000 recipe_urls-0.1.2/recipe_urls/tasty.py
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     5570 2024-04-16 20:49:32.000000 recipe_urls-0.1.2/recipe_urls/testing.py
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:09:47.902714 recipe_urls-0.1.2/recipe_urls.egg-info/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     4521 2024-04-16 22:09:47.000000 recipe_urls-0.1.2/recipe_urls.egg-info/PKG-INFO
+-rw-r--r--   0 mkayeterry   (501) staff       (20)     9270 2024-04-16 22:09:47.000000 recipe_urls-0.1.2/recipe_urls.egg-info/SOURCES.txt
+-rw-r--r--   0 mkayeterry   (501) staff       (20)        1 2024-04-16 22:09:47.000000 recipe_urls-0.1.2/recipe_urls.egg-info/dependency_links.txt
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       75 2024-04-16 22:09:47.000000 recipe_urls-0.1.2/recipe_urls.egg-info/requires.txt
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       12 2024-04-16 22:09:47.000000 recipe_urls-0.1.2/recipe_urls.egg-info/top_level.txt
+-rw-r--r--   0 mkayeterry   (501) staff       (20)       38 2024-04-16 22:09:47.903660 recipe_urls-0.1.2/setup.cfg
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:09:47.901121 recipe_urls-0.1.2/tests/
+drwxr-xr-x   0 mkayeterry   (501) staff       (20)        0 2024-04-16 22:09:47.902173 recipe_urls-0.1.2/tests/__pycache__/
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    25473 2024-04-16 20:23:46.000000 recipe_urls-0.1.2/tests/__pycache__/test_get_site_origin.cpython-310-pytest-8.1.1.pyc
+-rw-r--r--   0 mkayeterry   (501) staff       (20)    33786 2024-04-16 20:23:36.000000 recipe_urls-0.1.2/tests/test_get_site_origin.py
```

### Comparing `recipe_urls-0.1.1/.DS_Store` & `recipe_urls-0.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/LICENSE` & `recipe_urls-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/PKG-INFO` & `recipe_urls-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recipe_urls
-Version: 0.1.1
+Version: 0.1.2
 Summary: Scrapes all recipe URLs from provided base URL.
 Author-email: Melissa Terry <mkayeterry@gmail.com>
 License: MIT License
 Keywords: recipe,scraper,URLs,links
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 Requires-Dist: beautifulsoup4>=4.11.1
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pip-tools; extra == "test"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 
-# recipe-urls (Under Development)
+# recipe-urls
 
 ## Overview
 
 `recipe-urls` is a Python package designed to gather recipe URLs from a given base URL.
 
 ## Installation
 
@@ -51,15 +51,15 @@
 
 for base_url in base_urls:
 
     scrape = scrape_urls(base_url)
     compiled_recipe_links.extend(scrape)
 ```
 
-## Supported Websites (So Far!)
+## Supported Websites
 
 - https://abuelascounter.com
 - https://www.acouplecooks.com
 - https://addapinch.com
 - https://www.afghankitchenrecipes.com
 - https://www.allrecipes.com
 - https://www.ambitiouskitchen.com
```

### Comparing `recipe_urls-0.1.1/README.md` & `recipe_urls-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# recipe-urls (Under Development)
+# recipe-urls
 
 ## Overview
 
 `recipe-urls` is a Python package designed to gather recipe URLs from a given base URL.
 
 ## Installation
 
@@ -24,15 +24,15 @@
 
 for base_url in base_urls:
 
     scrape = scrape_urls(base_url)
     compiled_recipe_links.extend(scrape)
 ```
 
-## Supported Websites (So Far!)
+## Supported Websites
 
 - https://abuelascounter.com
 - https://www.acouplecooks.com
 - https://addapinch.com
 - https://www.afghankitchenrecipes.com
 - https://www.allrecipes.com
 - https://www.ambitiouskitchen.com
```

### Comparing `recipe_urls-0.1.1/pyproject.toml` & `recipe_urls-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "recipe_urls"
 authors = [
   {name = "Melissa Terry", email = "mkayeterry@gmail.com"},
 ]
-version = "0.1.1"
+version = "0.1.2"
 description = "Scrapes all recipe URLs from provided base URL."
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
```

### Comparing `recipe_urls-0.1.1/recipe_urls/.DS_Store` & `recipe_urls-0.1.2/recipe_urls/.DS_Store`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__init__.py` & `recipe_urls-0.1.2/recipe_urls/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 from typing import Optional
 import httpx
 
 from recipe_urls._abstract import AbstractScraper
 from recipe_urls._utils import get_site_origin
```

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/__init__.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/_abstract.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/_abstract.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/_utils.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/abuelascounter.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/abuelascounter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/acouplecooks.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/acouplecooks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/addapinch.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/addapinch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/afghankitchenrecipes.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/afghankitchenrecipes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/allrecipes.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/allrecipes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/ambitiouskitchen.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/ambitiouskitchen.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/archanaskitchen.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/archanaskitchen.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/averiecooks.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/averiecooks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/bakingmischief.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/bakingmischief.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/bakingsense.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/bakingsense.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/barefootcontessa.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/barefootcontessa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/base_scraper.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/base_scraper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/bbc.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/bbc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/bettycrocker.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/bettycrocker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/bigoven.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/bigoven.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/bluejeanchef.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/bluejeanchef.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/bonappetit.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/bonappetit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/bongeats.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/bongeats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/bowlofdelicious.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/bowlofdelicious.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/budgetbytes.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/budgetbytes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/carlsbadcravings.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/carlsbadcravings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/castironketo.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/castironketo.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/cdkitchen.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/cdkitchen.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/chefsavvy.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/chefsavvy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/closetcooking.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/closetcooking.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/cookieandkate.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/cookieandkate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/cookpad.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/cookpad.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/copykat.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/copykat.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/countryliving.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/countryliving.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/creativecanning.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/creativecanning.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/davidlebovitz.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/davidlebovitz.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/delish.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/delish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/domesticateme.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/domesticateme.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/downshiftology.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/downshiftology.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/eatingbirdfood.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/eatingbirdfood.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/eatingwell.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/eatingwell.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/eatliverun.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/eatliverun.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/eatsmarter.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/eatsmarter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/eatwell101.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/eatwell101.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/eatwhattonight.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/eatwhattonight.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/elavegan.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/elavegan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/epicurious.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/epicurious.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/errenskitchen.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/errenskitchen.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/ethanchlebowski.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/ethanchlebowski.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/farmhouseonboone.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/farmhouseonboone.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/fifteenspatulas.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/fifteenspatulas.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/finedininglovers.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/finedininglovers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/fitmencook.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/fitmencook.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/fitslowcookerqueen.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/fitslowcookerqueen.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/food.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/food.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/food52.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/food52.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/foodandwine.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/foodandwine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/foodnetwork.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/foodnetwork.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/foodrepublic.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/foodrepublic.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/forksoverknives.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/forksoverknives.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/forktospoon.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/forktospoon.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/gimmesomeoven.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/gimmesomeoven.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/gonnawantseconds.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/gonnawantseconds.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/goodfooddiscoveries.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/goodfooddiscoveries.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/goodhousekeeping.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/goodhousekeeping.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/greatbritishchefs.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/greatbritishchefs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/grimgrains.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/grimgrains.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/halfbakedharvest.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/halfbakedharvest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/handletheheat.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/handletheheat.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/headbangerskitchen.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/headbangerskitchen.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/heatherchristo.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/heatherchristo.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/heb.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/heb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/hellofresh.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/hellofresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/hersheyland.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/hersheyland.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/hostthetoast.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/hostthetoast.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/imworthy.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/imworthy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/indianhealthyrecipes.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/indianhealthyrecipes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/insanelygoodrecipes.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/insanelygoodrecipes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/inspiralized.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/inspiralized.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/izzycooking.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/izzycooking.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/jamieoliver.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/jamieoliver.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/jimcooksfoodgood.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/jimcooksfoodgood.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/joyfoodsunshine.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/joyfoodsunshine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/justataste.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/justataste.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/justbento.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/justbento.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/justonecookbook.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/justonecookbook.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/kingarthurbaking.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/kingarthurbaking.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/leanandgreenrecipes.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/leanandgreenrecipes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/lifestyleofafoodie.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/lifestyleofafoodie.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/littlespicejar.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/littlespicejar.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/livelytable.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/livelytable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/lovingitvegan.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/lovingitvegan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/ninjatestkitchen.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/ninjatestkitchen.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/nytimes.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/nytimes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/ohsheglows.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/ohsheglows.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/onceuponachef.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/onceuponachef.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/paleorunningmomma.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/paleorunningmomma.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/persnicketyplates.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/persnicketyplates.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/pickuplimes.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/pickuplimes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/pinchofyum.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/pinchofyum.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/platingpixels.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/platingpixels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/rachlmansfield.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/rachlmansfield.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/rainbowplantlife.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/rainbowplantlife.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/reciperunner.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/reciperunner.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/sallysbakingaddiction.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/sallysbakingaddiction.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/simpleveganista.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/simpleveganista.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/simplyquinoa.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/simplyquinoa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/simplywhisked.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/simplywhisked.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/southernliving.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/southernliving.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/tasteofhome.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/tasteofhome.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/tasty.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/tasty.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/utils.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/__pycache__/yummly.cpython-310.pyc` & `recipe_urls-0.1.2/recipe_urls/__pycache__/yummly.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/_abstract.py` & `recipe_urls-0.1.2/recipe_urls/_abstract.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/_utils.py` & `recipe_urls-0.1.2/recipe_urls/_utils.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/abuelascounter.py` & `recipe_urls-0.1.2/recipe_urls/abuelascounter.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/acouplecooks.py` & `recipe_urls-0.1.2/recipe_urls/acouplecooks.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/addapinch.py` & `recipe_urls-0.1.2/recipe_urls/addapinch.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/afghankitchenrecipes.py` & `recipe_urls-0.1.2/recipe_urls/afghankitchenrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/allrecipes.py` & `recipe_urls-0.1.2/recipe_urls/allrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/ambitiouskitchen.py` & `recipe_urls-0.1.2/recipe_urls/ambitiouskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/archanaskitchen.py` & `recipe_urls-0.1.2/recipe_urls/archanaskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/averiecooks.py` & `recipe_urls-0.1.2/recipe_urls/averiecooks.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/bakingmischief.py` & `recipe_urls-0.1.2/recipe_urls/bakingmischief.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/bakingsense.py` & `recipe_urls-0.1.2/recipe_urls/bakingsense.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/barefootcontessa.py` & `recipe_urls-0.1.2/recipe_urls/barefootcontessa.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/bbc.py` & `recipe_urls-0.1.2/recipe_urls/bbc.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/bettycrocker.py` & `recipe_urls-0.1.2/recipe_urls/bettycrocker.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/bigoven.py` & `recipe_urls-0.1.2/recipe_urls/bigoven.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/bluejeanchef.py` & `recipe_urls-0.1.2/recipe_urls/bluejeanchef.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/bonappetit.py` & `recipe_urls-0.1.2/recipe_urls/bonappetit.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/bongeats.py` & `recipe_urls-0.1.2/recipe_urls/bongeats.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/bowlofdelicious.py` & `recipe_urls-0.1.2/recipe_urls/bowlofdelicious.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/budgetbytes.py` & `recipe_urls-0.1.2/recipe_urls/budgetbytes.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/carlsbadcravings.py` & `recipe_urls-0.1.2/recipe_urls/carlsbadcravings.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/castironketo.py` & `recipe_urls-0.1.2/recipe_urls/castironketo.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/cdkitchen.py` & `recipe_urls-0.1.2/recipe_urls/cdkitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/chefsavvy.py` & `recipe_urls-0.1.2/recipe_urls/chefsavvy.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/closetcooking.py` & `recipe_urls-0.1.2/recipe_urls/closetcooking.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/cookieandkate.py` & `recipe_urls-0.1.2/recipe_urls/cookieandkate.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/copykat.py` & `recipe_urls-0.1.2/recipe_urls/copykat.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/countryliving.py` & `recipe_urls-0.1.2/recipe_urls/countryliving.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/creativecanning.py` & `recipe_urls-0.1.2/recipe_urls/creativecanning.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/davidlebovitz.py` & `recipe_urls-0.1.2/recipe_urls/davidlebovitz.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/delish.py` & `recipe_urls-0.1.2/recipe_urls/delish.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/domesticateme.py` & `recipe_urls-0.1.2/recipe_urls/domesticateme.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/downshiftology.py` & `recipe_urls-0.1.2/recipe_urls/downshiftology.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/eatingbirdfood.py` & `recipe_urls-0.1.2/recipe_urls/eatingbirdfood.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/eatingwell.py` & `recipe_urls-0.1.2/recipe_urls/eatingwell.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/eatliverun.py` & `recipe_urls-0.1.2/recipe_urls/eatliverun.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/eatsmarter.py` & `recipe_urls-0.1.2/recipe_urls/eatsmarter.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/eatwell101.py` & `recipe_urls-0.1.2/recipe_urls/eatwell101.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/eatwhattonight.py` & `recipe_urls-0.1.2/recipe_urls/eatwhattonight.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/elavegan.py` & `recipe_urls-0.1.2/recipe_urls/elavegan.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/epicurious.py` & `recipe_urls-0.1.2/recipe_urls/epicurious.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/errenskitchen.py` & `recipe_urls-0.1.2/recipe_urls/errenskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/ethanchlebowski.py` & `recipe_urls-0.1.2/recipe_urls/ethanchlebowski.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/farmhouseonboone.py` & `recipe_urls-0.1.2/recipe_urls/farmhouseonboone.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/fifteenspatulas.py` & `recipe_urls-0.1.2/recipe_urls/fifteenspatulas.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/finedininglovers.py` & `recipe_urls-0.1.2/recipe_urls/finedininglovers.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/fitmencook.py` & `recipe_urls-0.1.2/recipe_urls/fitmencook.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/fitslowcookerqueen.py` & `recipe_urls-0.1.2/recipe_urls/fitslowcookerqueen.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/food.py` & `recipe_urls-0.1.2/recipe_urls/food.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/food52.py` & `recipe_urls-0.1.2/recipe_urls/food52.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/foodandwine.py` & `recipe_urls-0.1.2/recipe_urls/foodandwine.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/foodnetwork.py` & `recipe_urls-0.1.2/recipe_urls/foodnetwork.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/foodrepublic.py` & `recipe_urls-0.1.2/recipe_urls/foodrepublic.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/forksoverknives.py` & `recipe_urls-0.1.2/recipe_urls/forksoverknives.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/forktospoon.py` & `recipe_urls-0.1.2/recipe_urls/forktospoon.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/gimmesomeoven.py` & `recipe_urls-0.1.2/recipe_urls/gimmesomeoven.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/gonnawantseconds.py` & `recipe_urls-0.1.2/recipe_urls/gonnawantseconds.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/goodfooddiscoveries.py` & `recipe_urls-0.1.2/recipe_urls/goodfooddiscoveries.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/goodhousekeeping.py` & `recipe_urls-0.1.2/recipe_urls/goodhousekeeping.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/greatbritishchefs.py` & `recipe_urls-0.1.2/recipe_urls/greatbritishchefs.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/halfbakedharvest.py` & `recipe_urls-0.1.2/recipe_urls/halfbakedharvest.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/handletheheat.py` & `recipe_urls-0.1.2/recipe_urls/handletheheat.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/headbangerskitchen.py` & `recipe_urls-0.1.2/recipe_urls/headbangerskitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/heatherchristo.py` & `recipe_urls-0.1.2/recipe_urls/heatherchristo.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/hellofresh.py` & `recipe_urls-0.1.2/recipe_urls/hellofresh.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/hersheyland.py` & `recipe_urls-0.1.2/recipe_urls/hersheyland.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/hostthetoast.py` & `recipe_urls-0.1.2/recipe_urls/hostthetoast.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/imworthy.py` & `recipe_urls-0.1.2/recipe_urls/imworthy.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/indianhealthyrecipes.py` & `recipe_urls-0.1.2/recipe_urls/indianhealthyrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/insanelygoodrecipes.py` & `recipe_urls-0.1.2/recipe_urls/insanelygoodrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/inspiralized.py` & `recipe_urls-0.1.2/recipe_urls/inspiralized.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/izzycooking.py` & `recipe_urls-0.1.2/recipe_urls/izzycooking.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/jamieoliver.py` & `recipe_urls-0.1.2/recipe_urls/jamieoliver.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/jimcooksfoodgood.py` & `recipe_urls-0.1.2/recipe_urls/jimcooksfoodgood.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/joyfoodsunshine.py` & `recipe_urls-0.1.2/recipe_urls/joyfoodsunshine.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/justataste.py` & `recipe_urls-0.1.2/recipe_urls/justataste.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/justbento.py` & `recipe_urls-0.1.2/recipe_urls/justbento.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/justonecookbook.py` & `recipe_urls-0.1.2/recipe_urls/justonecookbook.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/kingarthurbaking.py` & `recipe_urls-0.1.2/recipe_urls/kingarthurbaking.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/leanandgreenrecipes.py` & `recipe_urls-0.1.2/recipe_urls/leanandgreenrecipes.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/lifestyleofafoodie.py` & `recipe_urls-0.1.2/recipe_urls/lifestyleofafoodie.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/littlespicejar.py` & `recipe_urls-0.1.2/recipe_urls/littlespicejar.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/livelytable.py` & `recipe_urls-0.1.2/recipe_urls/livelytable.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/lovingitvegan.py` & `recipe_urls-0.1.2/recipe_urls/lovingitvegan.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/ninjatestkitchen.py` & `recipe_urls-0.1.2/recipe_urls/ninjatestkitchen.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/nytimes.py` & `recipe_urls-0.1.2/recipe_urls/nytimes.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/ohsheglows.py` & `recipe_urls-0.1.2/recipe_urls/ohsheglows.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/onceuponachef.py` & `recipe_urls-0.1.2/recipe_urls/onceuponachef.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/paleorunningmomma.py` & `recipe_urls-0.1.2/recipe_urls/paleorunningmomma.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/persnicketyplates.py` & `recipe_urls-0.1.2/recipe_urls/persnicketyplates.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/pickuplimes.py` & `recipe_urls-0.1.2/recipe_urls/pickuplimes.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/platingpixels.py` & `recipe_urls-0.1.2/recipe_urls/platingpixels.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/rachlmansfield.py` & `recipe_urls-0.1.2/recipe_urls/rachlmansfield.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/rainbowplantlife.py` & `recipe_urls-0.1.2/recipe_urls/rainbowplantlife.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/reciperunner.py` & `recipe_urls-0.1.2/recipe_urls/reciperunner.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/sallysbakingaddiction.py` & `recipe_urls-0.1.2/recipe_urls/sallysbakingaddiction.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/simpleveganista.py` & `recipe_urls-0.1.2/recipe_urls/simpleveganista.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/simplywhisked.py` & `recipe_urls-0.1.2/recipe_urls/simplywhisked.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/tasteofhome.py` & `recipe_urls-0.1.2/recipe_urls/tasteofhome.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/tasty.py` & `recipe_urls-0.1.2/recipe_urls/tasty.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls/testing.py` & `recipe_urls-0.1.2/recipe_urls/testing.py`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/recipe_urls.egg-info/PKG-INFO` & `recipe_urls-0.1.2/recipe_urls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recipe_urls
-Version: 0.1.1
+Version: 0.1.2
 Summary: Scrapes all recipe URLs from provided base URL.
 Author-email: Melissa Terry <mkayeterry@gmail.com>
 License: MIT License
 Keywords: recipe,scraper,URLs,links
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 Requires-Dist: beautifulsoup4>=4.11.1
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pip-tools; extra == "test"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 
-# recipe-urls (Under Development)
+# recipe-urls
 
 ## Overview
 
 `recipe-urls` is a Python package designed to gather recipe URLs from a given base URL.
 
 ## Installation
 
@@ -51,15 +51,15 @@
 
 for base_url in base_urls:
 
     scrape = scrape_urls(base_url)
     compiled_recipe_links.extend(scrape)
 ```
 
-## Supported Websites (So Far!)
+## Supported Websites
 
 - https://abuelascounter.com
 - https://www.acouplecooks.com
 - https://addapinch.com
 - https://www.afghankitchenrecipes.com
 - https://www.allrecipes.com
 - https://www.ambitiouskitchen.com
```

### Comparing `recipe_urls-0.1.1/recipe_urls.egg-info/SOURCES.txt` & `recipe_urls-0.1.2/recipe_urls.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .DS_Store
 .gitignore
 LICENSE
 README.md
 pyproject.toml
+dist/recipe_urls-0.1.1-py3-none-any.whl
+dist/recipe_urls-0.1.1.tar.gz
 recipe_urls/.DS_Store
 recipe_urls/__init__.py
 recipe_urls/_abstract.py
 recipe_urls/_utils.py
 recipe_urls/abuelascounter.py
 recipe_urls/acouplecooks.py
 recipe_urls/addapinch.py
```

### Comparing `recipe_urls-0.1.1/tests/__pycache__/test_get_site_origin.cpython-310-pytest-8.1.1.pyc` & `recipe_urls-0.1.2/tests/__pycache__/test_get_site_origin.cpython-310-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `recipe_urls-0.1.1/tests/test_get_site_origin.py` & `recipe_urls-0.1.2/tests/test_get_site_origin.py`

 * *Files identical despite different names*


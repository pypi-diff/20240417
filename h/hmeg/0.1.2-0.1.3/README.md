# Comparing `tmp/hmeg-0.1.2.tar.gz` & `tmp/hmeg-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmeg-0.1.2.tar", max compression
+gzip compressed data, was "hmeg-0.1.3.tar", max compression
```

## Comparing `hmeg-0.1.2.tar` & `hmeg-0.1.3.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0     1066 2024-03-01 07:41:02.775209 hmeg-0.1.2/LICENSE
--rw-r--r--   0        0        0     4437 2024-04-06 02:54:50.998893 hmeg-0.1.2/README.md
--rw-r--r--   0        0        0      137 2024-03-31 04:16:50.659172 hmeg-0.1.2/hmeg/__init__.py
--rw-r--r--   0        0        0     2345 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/entities.py
--rw-r--r--   0        0        0     1566 2024-04-04 12:43:38.812500 hmeg-0.1.2/hmeg/exercise_generator.py
--rw-r--r--   0        0        0     1500 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/ab.toml
--rw-r--r--   0        0        0     1782 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/cd.toml
--rw-r--r--   0        0        0     1897 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/efg.toml
--rw-r--r--   0        0        0     1384 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/h.toml
--rw-r--r--   0        0        0     1631 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/ikl.toml
--rw-r--r--   0        0        0     1809 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/mn.toml
--rw-r--r--   0        0        0     1216 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/opr.toml
--rw-r--r--   0        0        0     3075 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/stu.toml
--rw-r--r--   0        0        0     2146 2024-04-01 23:25:07.107024 hmeg-0.1.2/hmeg/miniphrase/wy.toml
--rw-r--r--   0        0        0     1682 2024-04-02 00:34:59.871652 hmeg-0.1.2/hmeg/registry.py
--rw-r--r--   0        0        0      290 2024-03-10 07:44:10.147484 hmeg-0.1.2/hmeg/topics/1_basic_present_tense.toml
--rw-r--r--   0        0        0      296 2024-03-10 07:44:10.147484 hmeg-0.1.2/hmeg/topics/1_from_a_to_b_from_c_until_d.toml
--rw-r--r--   0        0        0      325 2024-03-24 12:49:15.051567 hmeg-0.1.2/hmeg/topics/1_have_dont_have_there_is_there_isnt.toml
--rw-r--r--   0        0        0      290 2024-03-10 07:44:10.147484 hmeg-0.1.2/hmeg/topics/1_i_want_to.toml
--rw-r--r--   0        0        0      415 2024-03-10 07:44:10.147484 hmeg-0.1.2/hmeg/topics/1_negative_sentenses.toml
--rw-r--r--   0        0        0      233 2024-03-10 07:44:10.151485 hmeg-0.1.2/hmeg/topics/1_past_tense.toml
--rw-r--r--   0        0        0      161 2024-03-10 07:44:10.151485 hmeg-0.1.2/hmeg/topics/1_please_give_me.toml
--rw-r--r--   0        0        0      224 2024-03-24 12:49:15.051567 hmeg-0.1.2/hmeg/topics/1_this_is.toml
--rw-r--r--   0        0        0      165 2024-03-10 07:44:10.151485 hmeg-0.1.2/hmeg/topics/1_topic_subject_particle.toml
--rw-r--r--   0        0        0      327 2024-03-10 07:44:10.151485 hmeg-0.1.2/hmeg/topics/1_what_do_you_want_to_do.toml
--rw-r--r--   0        0        0      230 2024-03-14 13:30:47.048412 hmeg-0.1.2/hmeg/topics/2_and_and_then_therefore_so.toml
--rw-r--r--   0        0        0      154 2024-03-14 13:33:59.925728 hmeg-0.1.2/hmeg/topics/2_and_with.toml
--rw-r--r--   0        0        0      288 2024-03-14 13:39:48.992097 hmeg-0.1.2/hmeg/topics/2_but_however.toml
--rw-r--r--   0        0        0      250 2024-03-14 13:49:14.375934 hmeg-0.1.2/hmeg/topics/2_can_cannot.toml
--rw-r--r--   0        0        0      152 2024-03-15 14:01:09.329766 hmeg-0.1.2/hmeg/topics/2_dont_do_it.toml
--rw-r--r--   0        0        0      242 2024-03-14 13:27:05.334892 hmeg-0.1.2/hmeg/topics/2_future_tense.toml
--rw-r--r--   0        0        0      281 2024-03-21 21:46:08.368116 hmeg-0.1.2/hmeg/topics/2_have_to_should_must.toml
--rw-r--r--   0        0        0      185 2024-03-15 13:48:12.447505 hmeg-0.1.2/hmeg/topics/2_if_in_case.toml
--rw-r--r--   0        0        0      138 2024-03-15 13:50:12.715855 hmeg-0.1.2/hmeg/topics/2_imperative.toml
--rw-r--r--   0        0        0      183 2024-03-15 13:59:28.597472 hmeg-0.1.2/hmeg/topics/2_particles_for_method_way.toml
--rw-r--r--   0        0        0      173 2024-04-02 00:34:59.871652 hmeg-0.1.2/hmeg/topics/2_please_do_it_for_me.toml
--rw-r--r--   0        0        0      251 2024-03-14 13:46:29.870818 hmeg-0.1.2/hmeg/topics/2_present_progressive.toml
--rw-r--r--   0        0        0      294 2024-03-14 13:51:21.940821 hmeg-0.1.2/hmeg/topics/2_to_be_good_poor_at.toml
--rw-r--r--   0        0        0      288 2024-03-14 13:56:35.319010 hmeg-0.1.2/hmeg/topics/2_to_like.toml
--rw-r--r--   0        0        0      152 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_after_ing.toml
--rw-r--r--   0        0        0      209 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_approximately_about.toml
--rw-r--r--   0        0        0      156 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_before_ing.toml
--rw-r--r--   0        0        0      167 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_but_still_nevertheless.toml
--rw-r--r--   0        0        0      166 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_even_if_even_though.toml
--rw-r--r--   0        0        0      284 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_in_front_of_behind.toml
--rw-r--r--   0        0        0      215 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_in_order_to_for_the_sake_of.toml
--rw-r--r--   0        0        0      204 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_linking_verbs_고.toml
--rw-r--r--   0        0        0      165 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_linking_verbs_여서.toml
--rw-r--r--   0        0        0      256 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_linking_words_는데.toml
--rw-r--r--   0        0        0      339 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_maybe_i_might.toml
--rw-r--r--   0        0        0      289 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_nothing_but_only.toml
--rw-r--r--   0        0        0      241 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_shall_we_i_wonder.toml
--rw-r--r--   0        0        0      198 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_to_look_like_seem_like.toml
--rw-r--r--   0        0        0      166 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_too_much_very.toml
--rw-r--r--   0        0        0      159 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_verb_ending_네요.toml
--rw-r--r--   0        0        0      371 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_well_then_in_that_case.toml
--rw-r--r--   0        0        0      284 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_among_between.toml
--rw-r--r--   0        0        0      168 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_do_you_want_to.toml
--rw-r--r--   0        0        0      511 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_i_think_past_future.toml
--rw-r--r--   0        0        0      293 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_it_cant_be.toml
--rw-r--r--   0        0        0      439 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_it_is_ok_to.toml
--rw-r--r--   0        0        0      281 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_less_not_completely.toml
--rw-r--r--   0        0        0      314 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_most_best.toml
--rw-r--r--   0        0        0      190 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_much_more_much_less.toml
--rw-r--r--   0        0        0      343 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_the_more_the_more.toml
--rw-r--r--   0        0        0      224 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_to_become_adj.toml
--rw-r--r--   0        0        0      371 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_to_gradually_get_to_do.toml
--rw-r--r--   0        0        0      339 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_to_try_doing_something.toml
--rw-r--r--   0        0        0      247 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_verb_ending_지_죠.toml
--rw-r--r--   0        0        0      413 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_you_should_not.toml
--rw-r--r--   0        0        0      354 2024-03-10 07:43:30.163214 hmeg-0.1.2/hmeg/topics/9_while.toml
--rw-r--r--   0        0        0     3195 2024-04-01 23:25:07.107024 hmeg-0.1.2/hmeg/utils.py
--rw-r--r--   0        0        0     3943 2024-03-30 12:01:08.301249 hmeg-0.1.2/hmeg/vocabs/minilex.toml
--rw-r--r--   0        0        0     4953 2024-04-01 23:25:07.107024 hmeg-0.1.2/hmeg/vocabulary.py
--rw-r--r--   0        0        0      482 2024-04-06 02:56:59.567357 hmeg-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 hmeg-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-01 07:41:02.775209 hmeg-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4437 2024-04-06 02:58:35.143708 hmeg-0.1.3/README.md
+-rw-r--r--   0        0        0      137 2024-03-31 04:16:50.659172 hmeg-0.1.3/hmeg/__init__.py
+-rw-r--r--   0        0        0     2782 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/entities.py
+-rw-r--r--   0        0        0     1652 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/exercise_generator.py
+-rw-r--r--   0        0        0     1500 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/ab.toml
+-rw-r--r--   0        0        0     1782 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/cd.toml
+-rw-r--r--   0        0        0     1897 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/efg.toml
+-rw-r--r--   0        0        0     1384 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/h.toml
+-rw-r--r--   0        0        0     1631 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/ikl.toml
+-rw-r--r--   0        0        0     1809 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/mn.toml
+-rw-r--r--   0        0        0     1216 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/opr.toml
+-rw-r--r--   0        0        0     3075 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/stu.toml
+-rw-r--r--   0        0        0     2146 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/miniphrase/wy.toml
+-rw-r--r--   0        0        0     2327 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/registry.py
+-rw-r--r--   0        0        0      290 2024-03-10 07:44:10.147484 hmeg-0.1.3/hmeg/topics/1_basic_present_tense.toml
+-rw-r--r--   0        0        0      296 2024-03-10 07:44:10.147484 hmeg-0.1.3/hmeg/topics/1_from_a_to_b_from_c_until_d.toml
+-rw-r--r--   0        0        0      325 2024-03-24 12:49:15.051567 hmeg-0.1.3/hmeg/topics/1_have_dont_have_there_is_there_isnt.toml
+-rw-r--r--   0        0        0      290 2024-03-10 07:44:10.147484 hmeg-0.1.3/hmeg/topics/1_i_want_to.toml
+-rw-r--r--   0        0        0      415 2024-03-10 07:44:10.147484 hmeg-0.1.3/hmeg/topics/1_negative_sentenses.toml
+-rw-r--r--   0        0        0      233 2024-03-10 07:44:10.151485 hmeg-0.1.3/hmeg/topics/1_past_tense.toml
+-rw-r--r--   0        0        0      161 2024-03-10 07:44:10.151485 hmeg-0.1.3/hmeg/topics/1_please_give_me.toml
+-rw-r--r--   0        0        0      224 2024-03-24 12:49:15.051567 hmeg-0.1.3/hmeg/topics/1_this_is.toml
+-rw-r--r--   0        0        0      165 2024-03-10 07:44:10.151485 hmeg-0.1.3/hmeg/topics/1_topic_subject_particle.toml
+-rw-r--r--   0        0        0      327 2024-03-10 07:44:10.151485 hmeg-0.1.3/hmeg/topics/1_what_do_you_want_to_do.toml
+-rw-r--r--   0        0        0      230 2024-03-14 13:30:47.048412 hmeg-0.1.3/hmeg/topics/2_and_and_then_therefore_so.toml
+-rw-r--r--   0        0        0      154 2024-03-14 13:33:59.925728 hmeg-0.1.3/hmeg/topics/2_and_with.toml
+-rw-r--r--   0        0        0      288 2024-03-14 13:39:48.992097 hmeg-0.1.3/hmeg/topics/2_but_however.toml
+-rw-r--r--   0        0        0      250 2024-03-14 13:49:14.375934 hmeg-0.1.3/hmeg/topics/2_can_cannot.toml
+-rw-r--r--   0        0        0      152 2024-03-15 14:01:09.329766 hmeg-0.1.3/hmeg/topics/2_dont_do_it.toml
+-rw-r--r--   0        0        0      242 2024-03-14 13:27:05.334892 hmeg-0.1.3/hmeg/topics/2_future_tense.toml
+-rw-r--r--   0        0        0      281 2024-03-21 21:46:08.368116 hmeg-0.1.3/hmeg/topics/2_have_to_should_must.toml
+-rw-r--r--   0        0        0      185 2024-03-15 13:48:12.447505 hmeg-0.1.3/hmeg/topics/2_if_in_case.toml
+-rw-r--r--   0        0        0      138 2024-03-15 13:50:12.715855 hmeg-0.1.3/hmeg/topics/2_imperative.toml
+-rw-r--r--   0        0        0      183 2024-03-15 13:59:28.597472 hmeg-0.1.3/hmeg/topics/2_particles_for_method_way.toml
+-rw-r--r--   0        0        0      173 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/2_please_do_it_for_me.toml
+-rw-r--r--   0        0        0      251 2024-03-14 13:46:29.870818 hmeg-0.1.3/hmeg/topics/2_present_progressive.toml
+-rw-r--r--   0        0        0      294 2024-03-14 13:51:21.940821 hmeg-0.1.3/hmeg/topics/2_to_be_good_poor_at.toml
+-rw-r--r--   0        0        0      288 2024-03-14 13:56:35.319010 hmeg-0.1.3/hmeg/topics/2_to_like.toml
+-rw-r--r--   0        0        0      152 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_after_ing.toml
+-rw-r--r--   0        0        0      209 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_approximately_about.toml
+-rw-r--r--   0        0        0      156 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_before_ing.toml
+-rw-r--r--   0        0        0      167 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_but_still_nevertheless.toml
+-rw-r--r--   0        0        0      166 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_even_if_even_though.toml
+-rw-r--r--   0        0        0      284 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_in_front_of_behind.toml
+-rw-r--r--   0        0        0      215 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_in_order_to_for_the_sake_of.toml
+-rw-r--r--   0        0        0      204 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_linking_verbs_고.toml
+-rw-r--r--   0        0        0      165 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_linking_verbs_여서.toml
+-rw-r--r--   0        0        0      256 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_linking_words_는데.toml
+-rw-r--r--   0        0        0      339 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_maybe_i_might.toml
+-rw-r--r--   0        0        0      289 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_nothing_but_only.toml
+-rw-r--r--   0        0        0      241 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_shall_we_i_wonder.toml
+-rw-r--r--   0        0        0      198 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_to_look_like_seem_like.toml
+-rw-r--r--   0        0        0      166 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_too_much_very.toml
+-rw-r--r--   0        0        0      159 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_verb_ending_네요.toml
+-rw-r--r--   0        0        0      371 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_well_then_in_that_case.toml
+-rw-r--r--   0        0        0      284 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/4_among_between.toml
+-rw-r--r--   0        0        0      168 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/4_do_you_want_to.toml
+-rw-r--r--   0        0        0      511 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/4_i_think_past_future.toml
+-rw-r--r--   0        0        0      293 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/4_it_cant_be.toml
+-rw-r--r--   0        0        0      439 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/4_it_is_ok_to.toml
+-rw-r--r--   0        0        0      281 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/4_less_not_completely.toml
+-rw-r--r--   0        0        0      314 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_most_best.toml
+-rw-r--r--   0        0        0      190 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_much_more_much_less.toml
+-rw-r--r--   0        0        0      343 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_the_more_the_more.toml
+-rw-r--r--   0        0        0      224 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_to_become_adj.toml
+-rw-r--r--   0        0        0      371 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_to_gradually_get_to_do.toml
+-rw-r--r--   0        0        0      339 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_to_try_doing_something.toml
+-rw-r--r--   0        0        0      247 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_verb_ending_지_죠.toml
+-rw-r--r--   0        0        0      413 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_you_should_not.toml
+-rw-r--r--   0        0        0      354 2024-03-10 07:43:30.163214 hmeg-0.1.3/hmeg/topics/9_while.toml
+-rw-r--r--   0        0        0     5504 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/usecases.py
+-rw-r--r--   0        0        0     2673 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/vocabs/minilex.toml
+-rw-r--r--   0        0        0     1037 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/vocabs/nanolex.toml
+-rw-r--r--   0        0        0     5598 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/vocabulary.py
+-rw-r--r--   0        0        0      500 2024-04-17 14:36:28.371952 hmeg-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 hmeg-0.1.3/PKG-INFO
```

### Comparing `hmeg-0.1.2/LICENSE` & `hmeg-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.2/README.md` & `hmeg-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.2/hmeg/entities.py` & `hmeg-0.1.3/hmeg/entities.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,11 +50,28 @@
             VocabularyPlaceholders.VerbSingular3rd,
             VocabularyPlaceholders.VerbPast,
             VocabularyPlaceholders.VerbProgressive,
         ]
 
 
 @dataclasses.dataclass
+class TopicLevelInfo:
+    resource_name: str
+    level: int
+
+
+@dataclasses.dataclass
 class GrammarDescription:
     name: str
     links: list[str]
     exercises: list[str]
+    levels: list[TopicLevelInfo]
+
+    @staticmethod
+    def from_dict(d: dict) -> GrammarDescription:
+        res = GrammarDescription(
+            name=d["name"],
+            links=d["links"],
+            exercises=d["exercises"],
+            levels=[TopicLevelInfo(**level_descr) for level_descr in d.get("levels", [])],
+        )
+        return res
```

### Comparing `hmeg-0.1.2/hmeg/exercise_generator.py` & `hmeg-0.1.3/hmeg/exercise_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import random
 
 from nltk.parse.generate import generate
 from nltk import CFG
+import os
 
 from .registry import GrammarRegistry
-from .utils import apply_vocabulary
+from .usecases import apply_vocabulary
 from .vocabulary import Vocabulary
 
 
-DEFAULT_VOCABULARY_FILE = "hmeg/vocabs/minilex.toml"
+cur_dir = os.path.split(os.path.realpath(__file__))[0]
+DEFAULT_VOCABULARY_FILE = os.path.join(cur_dir, "vocabs/minilex.toml")
 
 
 class ExerciseGenerator:
     @staticmethod
     def generate_exercises(topic_name: str, num: int, vocab: Vocabulary | None = None) -> list[str]:
         """
         Generates list of random translation exercises for the given topic.
```

### Comparing `hmeg-0.1.2/hmeg/miniphrase/ab.toml` & `hmeg-0.1.3/hmeg/miniphrase/ab.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.2/hmeg/miniphrase/cd.toml` & `hmeg-0.1.3/hmeg/miniphrase/cd.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.2/hmeg/miniphrase/efg.toml` & `hmeg-0.1.3/hmeg/miniphrase/efg.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.2/hmeg/miniphrase/h.toml` & `hmeg-0.1.3/hmeg/miniphrase/h.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.2/hmeg/miniphrase/ikl.toml` & `hmeg-0.1.3/hmeg/miniphrase/ikl.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.2/hmeg/miniphrase/mn.toml` & `hmeg-0.1.3/hmeg/miniphrase/mn.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.2/hmeg/miniphrase/opr.toml` & `hmeg-0.1.3/hmeg/miniphrase/opr.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.2/hmeg/miniphrase/stu.toml` & `hmeg-0.1.3/hmeg/miniphrase/stu.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.2/hmeg/miniphrase/wy.toml` & `hmeg-0.1.3/hmeg/miniphrase/wy.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.2/hmeg/registry.py` & `hmeg-0.1.3/hmeg/registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,31 @@
     def get_registered_topics() -> list[str]:
         """
         Returns names of registered topics.
         """
         return list(GrammarRegistry.topics)
 
     @staticmethod
+    def get_registered_levels() -> dict[str, list[int]]:
+        """
+        Returns information about registered levels for topics.
+        The levels are grouped by the resource and sorted in the ascending order.
+        """
+        res = dict()
+        for topic in GrammarRegistry.topics.values():
+            for level_descr in topic.levels:
+                if level_descr.resource_name not in res:
+                    res[level_descr.resource_name] = list()
+                res[level_descr.resource_name].append(level_descr.level)
+
+        for key in res:
+            res[key] = sorted(set(res[key]))
+        return res
+
+    @staticmethod
     def find_topics(topic_name: str) -> list[str]:
         """
         Find registered topic that fully or partially matches the provided name.
 
         Args
         ----
         topic_name: str,
```

### Comparing `hmeg-0.1.2/hmeg/vocabulary.py` & `hmeg-0.1.3/hmeg/vocabulary.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     'hurt': 'hurts',
     'look for': 'looks for',
     'name': 'names',
 }
 
 
 class Vocabulary:
-    vocab_file: str  # file with the current vocabulary
+    vocab_file: str | None  # file with the current vocabulary
+    name: str | None
     adjectives: list[str]
     adverbs: list[str]
     nouns: list[str]
     verbs: list[str]
     weekdays: list[str] = [
         "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"
     ]
@@ -59,29 +60,45 @@
         "teacher", "wife", "woman"
     ]
     places = [
         "airport", "apartment", "country", "flat", "home", "house", "road", "room",
         "school", "shop", "side", "street", "town", "work", "bathroom"
     ]
 
-    def __init__(self, vocab_file: str):
+    def __init__(self, vocab_file: str | None = None):
         self.vocab_file = vocab_file
+        self.name = None
+        self.adjectives = []
+        self.adverbs = []
+        self.nouns = []
+        self.verbs = []
         self._load()
 
     @staticmethod
     def load(vocab_file: str) -> Vocabulary:
         return Vocabulary(vocab_file)
 
     def _load(self):
+        if self.vocab_file is None:
+            return
+
         with open(self.vocab_file, "r") as f:
             vocab_dict = toml.loads(f.read())
-            self.adjectives = vocab_dict.get("adjectives") or []
-            self.adverbs = vocab_dict.get("adverbs") or []
-            self.nouns = vocab_dict.get("nouns") or []
-            self.verbs = vocab_dict.get("verbs") or []
+
+        if "import" in vocab_dict:
+            import_dir = os.path.split(self.vocab_file)[0]
+            import_vocab = Vocabulary.load(os.path.join(import_dir, vocab_dict["import"]))
+        else:
+            import_vocab = Vocabulary()
+
+        self.name = vocab_dict.get("name")
+        self.adjectives = sorted(set(import_vocab.adjectives + (vocab_dict.get("adjectives") or [])))
+        self.adverbs = sorted(set(import_vocab.adverbs + (vocab_dict.get("adverbs") or [])))
+        self.nouns = sorted(set(import_vocab.nouns + (vocab_dict.get("nouns") or [])))
+        self.verbs = sorted(set(import_vocab.verbs + (vocab_dict.get("verbs") or [])))
 
     def random_verb(self) -> str:
         return random.choice(self.verbs)
 
     def random_verb_singular_3rd(self) -> str:
         cur_verb = conj.conjugate(self.random_verb())
         conj_verb = verbs_singular_3rd.get(
```

### Comparing `hmeg-0.1.2/PKG-INFO` & `hmeg-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: hmeg
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generator of exercises for practicing speaking for language learning.
 Home-page: https://github.com/yurytsoy/hmeg
 License: MIT
 Author: Yury Choi
 Author-email: yurytsoy@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fire (>=0.6.0,<0.7.0)
 Requires-Dist: inflect (>=7.0.0,<8.0.0)
 Requires-Dist: mlconjug3 (>=3.11.0,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/yurytsoy/hmeg
 Description-Content-Type: text/markdown
 
 # hmeg
 
 Help me, Erik Gunnemark -- library for generation of exercises for practicing of some basic speaking constructs.
```


# Changelog

Changelog for ghacupha commons-chain.

    ## Unreleased
                ### GitHub #23469   

            **Apply contributions by Matthew Sgarlata, #23469**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142814 13f79535-47bb-0310-9956-ffa450edef68

            [ec3419ff7e8b64f](https://github.com/ghacupha/commons-chain/commit/ec3419ff7e8b64f) Ted Nathan Husted *2003-09-29 15:44:40*


                ### GitHub #31807   

            **Adjust the example chain configuration file to reflect the default**

                * behavior of expecting a &lt;catalog&gt; outermost element, which will register
                * the included chains and commands into the default catalog for this app.
                * PR:  Bugzilla #31807
                * Submitted by:  Sean Schofield &lt;sean.schofield AT gmail.com&gt;
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142904 13f79535-47bb-0310-9956-ffa450edef68

            [cd91132db57f9da](https://github.com/ghacupha/commons-chain/commit/cd91132db57f9da) Craig R. McClanahan *2004-10-21 05:14:45*


                ### GitHub #31844   

            **Now that we have CatalogFactory, make LookupCommand leverage it by expecting**

                * a Catalog name instead of a Catalog instance.  If not specified, the default
                * Catalog for this application will be consulted.
                * PR: Bugzilla #31844
                * Submitted By:  Sean Schofield &lt;sean DOT schofield AT gmail.com&gt;
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142905 13f79535-47bb-0310-9956-ffa450edef68

            [1c620766f45bd1c](https://github.com/ghacupha/commons-chain/commit/1c620766f45bd1c) Craig R. McClanahan *2004-10-22 18:06:47*


                ### GitHub #32655   

            **Bug #32655: Code fragment incorrect.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142917 13f79535-47bb-0310-9956-ffa450edef68

            [99ba10484555e71](https://github.com/ghacupha/commons-chain/commit/99ba10484555e71) Martin Cooper *2004-12-12 16:40:15*


                ### GitHub #32881   

            **Implement enhanced lookup for commands that takes "catalog:command" argument**

                * as a single string.
                * PR:  Bugzilla #32881
                * Submitted By:  Joe Germuska &lt;joe AT germuska.com&gt;
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142918 13f79535-47bb-0310-9956-ffa450edef68

            [5055af741f79c50](https://github.com/ghacupha/commons-chain/commit/5055af741f79c50) Craig R. McClanahan *2004-12-31 02:28:07*


                ### GitHub #34409   

            **Make ContextBase live up to the Serializable contract that it inherits**

                * by virtue of extending HashMap, and add a unit test to prove it works.
                * Fixed in nightly build 20050417.
                * However, this unit test pointed out a problem with the design of the
                * concrete WebContext subclasses (ServletWebContext, PortletWebContext,
                * FacesWebContext).  It is not going to be possible to make these classes
                * Serializable because the underlying container objects they wrap are not
                * Serializable -- and there is no way to un-inherit the &quot;implements Serializable&quot;
                * characteristic of the ContextBase base class.
                * PR:  Bugzilla #34409
                * Submitted By:  Jeff Ramsdale &lt;jramsdale AT solutionsiq.com&gt;
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@161600 13f79535-47bb-0310-9956-ffa450edef68

            [fcb67fbb0e3e712](https://github.com/ghacupha/commons-chain/commit/fcb67fbb0e3e712) Craig R. McClanahan *2005-04-16 19:55:37*


                ### Jira CHAIN-100   

            **CHAIN-100 - Add Maven PMD Plugin to the site build**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1496197 13f79535-47bb-0310-9956-ffa450edef68

            [af7681f58b4121e](https://github.com/ghacupha/commons-chain/commit/af7681f58b4121e) Benedikt Ritter *2013-06-24 20:26:35*


                ### Jira CHAIN-106   

            **[CHAIN-106] JavaDoc report contains JavaDocs of cookbook examples**

                * initial attempt of excluding undesired apidocs be published
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1500836 13f79535-47bb-0310-9956-ffa450edef68

            [56233d45b9fa799](https://github.com/ghacupha/commons-chain/commit/56233d45b9fa799) Simone Tripodi *2013-07-08 16:53:54*


                ### Jira CHAIN-108   

            **CHAIN-108 - Build fails with Java 6; assigning variables helps the compiler to figure out typed arguments**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1500972 13f79535-47bb-0310-9956-ffa450edef68

            [70f701134c33c4f](https://github.com/ghacupha/commons-chain/commit/70f701134c33c4f) Benedikt Ritter *2013-07-08 21:31:39*


                ### Jira CHAIN-11   

            **Modify DispatchCommand so that it will compile using JDK 1.3 (remove JDK 1.4 method).**

                * JIRA Issue: CHAIN-11
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@409125 13f79535-47bb-0310-9956-ffa450edef68

            [fd6ce1ba69d08ea](https://github.com/ghacupha/commons-chain/commit/fd6ce1ba69d08ea) Niall Pemberton *2006-05-24 10:38:54*


                ### Jira CHAIN-12   

            **Further fix for CHAIN-12 - Using JDK 1.4.2_10 ContextBase can be serialized, but JDK 1.4.2_11 (and 1.3.1_04) fail trying to serialize - thanks to Dennis Lundberg for spotting this.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@412150 13f79535-47bb-0310-9956-ffa450edef68

            [35aff8d3da335ca](https://github.com/ghacupha/commons-chain/commit/35aff8d3da335ca) Niall Pemberton *2006-06-06 15:31:50*


                ### Jira CHAIN-28   

            **CHAIN-28 - Provide a Map of Cookies in the WebContext**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@411948 13f79535-47bb-0310-9956-ffa450edef68

            [483cbe0865dd08c](https://github.com/ghacupha/commons-chain/commit/483cbe0865dd08c) Niall Pemberton *2006-06-05 23:29:02*


                ### Jira CHAIN-29   

            **Fix for CHAIN-29 - Remove static Log instances**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@411893 13f79535-47bb-0310-9956-ffa450edef68

            [b8bd19ebcb61670](https://github.com/ghacupha/commons-chain/commit/b8bd19ebcb61670) Niall Pemberton *2006-06-05 18:59:05*


                ### Jira CHAIN-30   

            **Fix for CHAIN-30 - ServletSessionScopeMap always forces a Session to be Created**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@412789 13f79535-47bb-0310-9956-ffa450edef68

            [1ba75151c667c0b](https://github.com/ghacupha/commons-chain/commit/1ba75151c667c0b) Niall Pemberton *2006-06-08 16:19:14*


                ### Jira CHAIN-31   

            **Fix for CHAIN-31 -  Portlet Map implementations' entry Set should contain Map.Entry elements**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@412719 13f79535-47bb-0310-9956-ffa450edef68

            [6512e6703ca336d](https://github.com/ghacupha/commons-chain/commit/6512e6703ca336d) Niall Pemberton *2006-06-08 10:49:18*


                ### Jira CHAIN-32   

            **CHAIN-32 Improve instantiation performance of ContextBase subclasses. Thanks to Joshua Graham.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@416980 13f79535-47bb-0310-9956-ffa450edef68

            [864041291c63c77](https://github.com/ghacupha/commons-chain/commit/864041291c63c77) Niall Pemberton *2006-06-25 03:13:17*


                ### Jira CHAIN-33   

            **CHAIN-33 - Upgrade to Digester 1.8 to fix bug loading webapp resources**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@482967 13f79535-47bb-0310-9956-ffa450edef68

            [3d9f67d276a5908](https://github.com/ghacupha/commons-chain/commit/3d9f67d276a5908) Niall Pemberton *2006-12-06 08:43:48*


                ### Jira CHAIN-34   

            **CHAIN-34 - JavaDoc fix for ContextBase - thanks to Mark Vedder**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@499247 13f79535-47bb-0310-9956-ffa450edef68

            [91b94fe73e5029b](https://github.com/ghacupha/commons-chain/commit/91b94fe73e5029b) Niall Pemberton *2007-01-24 04:09:44*


                ### Jira CHAIN-36   

            **CHAIN-36 - Add Example webapp for Servlet Mapper Commands**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@532952 13f79535-47bb-0310-9956-ffa450edef68

            [e11a8f0c4f19eca](https://github.com/ghacupha/commons-chain/commit/e11a8f0c4f19eca) Niall Pemberton *2007-04-27 04:00:53*


                ### Jira CHAIN-4   

            **Fix for CHAIN-4 - Update servlet implementation classes to be aware of CatalogFactory - thanks to Joe Germuska**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@532951 13f79535-47bb-0310-9956-ffa450edef68

            [bae0be6cb3d53b2](https://github.com/ghacupha/commons-chain/commit/bae0be6cb3d53b2) Niall Pemberton *2007-04-27 03:59:00*


                ### Jira CHAIN-41   

            **CHAIN-41 fix bad ant buildfile. Code now depends on digester1.8; the pom.xml had been updated but not the build.xml.**

                * Thanks to Isaac Shabtay for the report.
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@600302 13f79535-47bb-0310-9956-ffa450edef68

            [df621d959854032](https://github.com/ghacupha/commons-chain/commit/df621d959854032) Simon Kitching *2007-12-02 14:50:55*


                ### Jira CHAIN-42   

            **CHAIN-42 - Various scope mappers use incorrect equalization - thanks to Isaac Shabtay for the patch**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658355 13f79535-47bb-0310-9956-ffa450edef68

            [6bca26c304a613c](https://github.com/ghacupha/commons-chain/commit/6bca26c304a613c) Niall Pemberton *2008-05-20 17:25:51*


                ### Jira CHAIN-43   

            **CHAIN-43 - ChainListener URL translation does not work as expected - thanks to Ales Dolecek**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658426 13f79535-47bb-0310-9956-ffa450edef68

            [6a8797d09c43dc4](https://github.com/ghacupha/commons-chain/commit/6a8797d09c43dc4) Niall Pemberton *2008-05-20 20:55:38*


                ### Jira CHAIN-44   

            **Fix CHAIN-44 - CatalogFactory instance varibale prevents ChainProcessor from being serializable**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@661360 13f79535-47bb-0310-9956-ffa450edef68

            [16df0d7ed957b21](https://github.com/ghacupha/commons-chain/commit/16df0d7ed957b21) Niall Pemberton *2008-05-29 15:31:29*


                ### Jira CHAIN-47   

            **CHAIN-47**

                * Refactored ServletWebContext and WebContext to an interface.
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1366094 13f79535-47bb-0310-9956-ffa450edef68

            [9056f326728677d](https://github.com/ghacupha/commons-chain/commit/9056f326728677d) Elijah Zupancic *2012-07-26 17:29:31*


                ### Jira CHAIN-53   

            **[CHAIN-53] warkaround for old version of javac that raise "type parameters of <T>T cannot be determined; no unique maximal instance exists for type variable T with upper bounds T,java.lang.Object" error**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1169757 13f79535-47bb-0310-9956-ffa450edef68

            [5ef3b2d7628b060](https://github.com/ghacupha/commons-chain/commit/5ef3b2d7628b060) Simone Tripodi *2011-09-12 14:16:47*

            **added the CHAIN-53 issue**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164531 13f79535-47bb-0310-9956-ffa450edef68

            [4496c72a81de95d](https://github.com/ghacupha/commons-chain/commit/4496c72a81de95d) Simone Tripodi *2011-09-02 13:40:44*

            **[CHAIN-53] Global Update of Chain - Generics, JDK 1.5, Update Dependency Versions - patch submitted by Elijah Zupancic**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1162332 13f79535-47bb-0310-9956-ffa450edef68

            [495e5f7ccfcad46](https://github.com/ghacupha/commons-chain/commit/495e5f7ccfcad46) Simone Tripodi *2011-08-27 12:34:14*


                ### Jira CHAIN-54   

            **[CHAIN-54] upgrate JUnit dependency to latest released version and adapt tests**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1170348 13f79535-47bb-0310-9956-ffa450edef68

            [3896471c981382d](https://github.com/ghacupha/commons-chain/commit/3896471c981382d) Simone Tripodi *2011-09-13 21:03:29*


                ### Jira CHAIN-55   

            **[CHAIN-55] split the huge project in submodules.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295177 13f79535-47bb-0310-9956-ffa450edef68

            [2e2d3e8e83dd5c4](https://github.com/ghacupha/commons-chain/commit/2e2d3e8e83dd5c4) Simone Tripodi *2012-02-29 16:19:22*

            **part of [CHAIN-55] prepared new assembly descriptors to grab non artifacts files from the right location (not integrated in the reactor yet)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295050 13f79535-47bb-0310-9956-ffa450edef68

            [6a8a0d523483ab2](https://github.com/ghacupha/commons-chain/commit/6a8a0d523483ab2) Simone Tripodi *2012-02-29 10:03:53*

            **part of [CHAIN-55] added the binaries distribution package module (not integrated in the reactor yet)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295042 13f79535-47bb-0310-9956-ffa450edef68

            [b0750b49a91e406](https://github.com/ghacupha/commons-chain/commit/b0750b49a91e406) Simone Tripodi *2012-02-29 09:51:24*

            **part of [CHAIN-55] fixed future parent pom reference (not integrated in the reactor yet)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295040 13f79535-47bb-0310-9956-ffa450edef68

            [e4d4e31049b2c8e](https://github.com/ghacupha/commons-chain/commit/e4d4e31049b2c8e) Simone Tripodi *2012-02-29 09:48:30*

            **part of [CHAIN-55] created the distribution packages empty submodule directory (not included in the reactor yet)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295030 13f79535-47bb-0310-9956-ffa450edef68

            [f6963a7c43dcc13](https://github.com/ghacupha/commons-chain/commit/f6963a7c43dcc13) Simone Tripodi *2012-02-29 09:27:15*

            **part of [CHAIN-55] created the empty submodules directories (not included in the reactor yet)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295022 13f79535-47bb-0310-9956-ffa450edef68

            [bb8b3a6ddcb68d5](https://github.com/ghacupha/commons-chain/commit/bb8b3a6ddcb68d5) Simone Tripodi *2012-02-29 09:10:18*

            **dropped Ant stuff, preparation for [CHAIN-55] (project will be splitted in submodules)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1294384 13f79535-47bb-0310-9956-ffa450edef68

            [b284b06256158db](https://github.com/ghacupha/commons-chain/commit/b284b06256158db) Simone Tripodi *2012-02-27 23:04:12*


                ### Jira CHAIN-56   

            **added CHAIN-56 in the changelist**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165082 13f79535-47bb-0310-9956-ffa450edef68

            [4fcb1118173bb31](https://github.com/ghacupha/commons-chain/commit/4fcb1118173bb31) Simone Tripodi *2011-09-04 18:52:18*

            **[CHAIN-56] clever Context with generic type auto-cast feature**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165075 13f79535-47bb-0310-9956-ffa450edef68

            [575ca905ae623a2](https://github.com/ghacupha/commons-chain/commit/575ca905ae623a2) Simone Tripodi *2011-09-04 17:02:05*


                ### Jira CHAIN-57   

            **CHAIN-57 Chain 2.0 does not build on older JDKs**

                * Alternate solution, not requiring unchecked cast:
                * Give the Java 1.5 compiler a bit of help resolving the generic
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1169769 13f79535-47bb-0310-9956-ffa450edef68

            [8c0a5a9ef94a424](https://github.com/ghacupha/commons-chain/commit/8c0a5a9ef94a424) Sebastian Bazley *2011-09-12 14:33:15*


                ### Jira CHAIN-58   

            **[CHAIN-58] Update Chain Context interface to use K,V generics - patch submitted by Elijah Zupancic**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1243699 13f79535-47bb-0310-9956-ffa450edef68

            [a0a63b5f27f56ee](https://github.com/ghacupha/commons-chain/commit/a0a63b5f27f56ee) Simone Tripodi *2012-02-13 21:19:07*


                ### Jira CHAIN-59   

            **[CHAIN-59] move layout dir to standard maven**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1173817 13f79535-47bb-0310-9956-ffa450edef68

            [ff8b7a8c1447aff](https://github.com/ghacupha/commons-chain/commit/ff8b7a8c1447aff) Simone Tripodi *2011-09-21 20:00:30*


                ### Jira CHAIN-60   

            **[CHAIN-60] In certain build configurations unit tests fail with the following message: testDefault: Correct command count expected:<17> but was:<19> - patch contributed by Elijah Zupancic**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1178379 13f79535-47bb-0310-9956-ffa450edef68

            [876a8564a931c4b](https://github.com/ghacupha/commons-chain/commit/876a8564a931c4b) Simone Tripodi *2011-10-03 11:42:37*


                ### Jira CHAIN-61   

            **[CHAIN-61] Chain 2.0 trunk build is throwing many warnings as a result of generification changes (Contributed by Elijah Zupancic)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1189035 13f79535-47bb-0310-9956-ffa450edef68

            [9c85fc0cacaee6d](https://github.com/ghacupha/commons-chain/commit/9c85fc0cacaee6d) Simone Tripodi *2011-10-26 06:18:03*


                ### Jira CHAIN-65   

            **dropped empty packages left when applied [CHAIN-65]**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1294383 13f79535-47bb-0310-9956-ffa450edef68

            [7cade28931dd750](https://github.com/ghacupha/commons-chain/commit/7cade28931dd750) Simone Tripodi *2012-02-27 23:02:53*

            **[CHAIN-65] Rename package org.apache.commons.chain to org.apache.commons.chain2 for v2 of chain - patch provided by Elijah Zupancic**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1294379 13f79535-47bb-0310-9956-ffa450edef68

            [7cfdf537bdba675](https://github.com/ghacupha/commons-chain/commit/7cfdf537bdba675) Simone Tripodi *2012-02-27 22:55:46*


                ### Jira CHAIN-66   

            **[CHAIN-66] Updated Chain documentation to include new changes to the API - patch provided by Elijah Zupancic**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1327509 13f79535-47bb-0310-9956-ffa450edef68

            [e0a3efe13f6e551](https://github.com/ghacupha/commons-chain/commit/e0a3efe13f6e551) Simone Tripodi *2012-04-18 13:41:56*


                ### Jira CHAIN-67   

            **[CHAIN-67] Refactor of explicit Exception throws to a RuntimeException type - patch submitted by Elijah Zupancic**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1297032 13f79535-47bb-0310-9956-ffa450edef68

            [4ec00f53a40b8d0](https://github.com/ghacupha/commons-chain/commit/4ec00f53a40b8d0) Simone Tripodi *2012-03-05 12:35:10*


                ### Jira CHAIN-68   

            **CHAIN-68/69 are bugs, not improvements**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363266 13f79535-47bb-0310-9956-ffa450edef68

            [409d41cd6a8fc60](https://github.com/ghacupha/commons-chain/commit/409d41cd6a8fc60) Simone Tripodi *2012-07-19 08:58:18*

            **[CHAIN-68] SNAPSHOT tomcat plugin breaks the build - patch provided by Elijah Zupancic**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1328084 13f79535-47bb-0310-9956-ffa450edef68

            [99192e1b97dd9d1](https://github.com/ghacupha/commons-chain/commit/99192e1b97dd9d1) Simone Tripodi *2012-04-19 19:26:03*


                ### Jira CHAIN-69   

            **[CHAIN-69] Fixed Checkstyle / PMD Warnings - patch submitted by Elijah Zupancic**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1355373 13f79535-47bb-0310-9956-ffa450edef68

            [06dd90d4750d817](https://github.com/ghacupha/commons-chain/commit/06dd90d4750d817) Simone Tripodi *2012-06-29 13:29:34*


                ### Jira CHAIN-70   

            **[CHAIN-70] Add a small EDSL to simplify Catalog setup**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1365025 13f79535-47bb-0310-9956-ffa450edef68

            [250fd0c7cc703e1](https://github.com/ghacupha/commons-chain/commit/250fd0c7cc703e1) Simone Tripodi *2012-07-24 12:57:56*

            **[CHAIN-70] Add a small EDSL to simplify Chain setup and execution**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363265 13f79535-47bb-0310-9956-ffa450edef68

            [f509b1749bc1e04](https://github.com/ghacupha/commons-chain/commit/f509b1749bc1e04) Simone Tripodi *2012-07-19 08:56:32*


                ### Jira CHAIN-71   

            **CHAIN-71**

                * Removed methods and code paths that were marked deprecated in chain 1.xx.
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1364104 13f79535-47bb-0310-9956-ffa450edef68

            [2dfe3de988d60aa](https://github.com/ghacupha/commons-chain/commit/2dfe3de988d60aa) Elijah Zupancic *2012-07-21 14:25:54*


                ### Jira CHAIN-72   

            **CHAIN-72 - configuration façade APIs**

                * XmlConfigParser must implement the ConfigParser interface
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1486526 13f79535-47bb-0310-9956-ffa450edef68

            [58a9926aec60ea8](https://github.com/ghacupha/commons-chain/commit/58a9926aec60ea8) Simone Tripodi *2013-05-27 07:22:45*

            **CHAIN-72 - configuration façade APIs**

                * still better separation between configuration APIs and XML implementation
                * configuration exception moved to configuration package
                * XML related classes moved in proper config.xml subpackage
                * configuration exception moved to the configuration package/module
                * registry throws a runtime exception rather than a configuration exception
                * trivial: updated ignore list
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1486478 13f79535-47bb-0310-9956-ffa450edef68

            [85a087bd111b4ce](https://github.com/ghacupha/commons-chain/commit/85a087bd111b4ce) Simone Tripodi *2013-05-26 21:21:21*

            **CHAIN-72**

                * Refactored configuration module into a facade. We now have two modules - configuration-api which is the
                * facade that is compiled against and configuration-xml which is an implementation that allows xml based
                * configuration.
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1366118 13f79535-47bb-0310-9956-ffa450edef68

            [777e23f168d1192](https://github.com/ghacupha/commons-chain/commit/777e23f168d1192) Elijah Zupancic *2012-07-26 18:04:57*


                ### Jira CHAIN-74   

            **fixed boken tests (on Continuum) after introduced [CHAIN-74]**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1365107 13f79535-47bb-0310-9956-ffa450edef68

            [9e8f2e2669553ea](https://github.com/ghacupha/commons-chain/commit/9e8f2e2669553ea) Simone Tripodi *2012-07-24 15:04:08*

            **[CHAIN-74] Improve Chain/Catalog use of Generics**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1365049 13f79535-47bb-0310-9956-ffa450edef68

            [126ea0412096a66](https://github.com/ghacupha/commons-chain/commit/126ea0412096a66) Simone Tripodi *2012-07-24 13:40:08*


                ### Jira CHAIN-75   

            **CHAIN-75 Updated serialVersionUID field in chain classes to a format based on the current date**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1365262 13f79535-47bb-0310-9956-ffa450edef68

            [3f01aca052713b2](https://github.com/ghacupha/commons-chain/commit/3f01aca052713b2) Elijah Zupancic *2012-07-24 19:56:21*


                ### Jira CHAIN-78   

            **[CHAIN-78] #comment updated to parent 28, props to Steve Westwood #resolve**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1457300 13f79535-47bb-0310-9956-ffa450edef68

            [4545e2c6543521f](https://github.com/ghacupha/commons-chain/commit/4545e2c6543521f) Simone Tripodi *2013-03-16 20:03:18*


                ### Jira CHAIN-79   

            **[CHAIN-79] #comment APIs extracted from default implementation module #resolve**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1457657 13f79535-47bb-0310-9956-ffa450edef68

            [e341c25ca10aa70](https://github.com/ghacupha/commons-chain/commit/e341c25ca10aa70) Simone Tripodi *2013-03-18 06:42:27*


                ### Jira CHAIN-80   

            **[CHAIN-80] NPE when submitting null commands map to CatalogBase - patch submitted by Steve Westwood**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1461601 13f79535-47bb-0310-9956-ffa450edef68

            [df502f5c53dfe18](https://github.com/ghacupha/commons-chain/commit/df502f5c53dfe18) Simone Tripodi *2013-03-27 14:23:12*


                ### Jira CHAIN-83   

            **CHAIN-83 was an update and not an add**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493360 13f79535-47bb-0310-9956-ffa450edef68

            [d0d3a6a00f5a150](https://github.com/ghacupha/commons-chain/commit/d0d3a6a00f5a150) Benedikt Ritter *2013-06-15 14:07:34*

            **CHAIN-83 - Rename o.a.c.chain2.generic package to o.a.c.chain2.base - remove old generic directories**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493346 13f79535-47bb-0310-9956-ffa450edef68

            [97c228e1cb2f3ce](https://github.com/ghacupha/commons-chain/commit/97c228e1cb2f3ce) Benedikt Ritter *2013-06-15 12:07:58*

            **CHAIN-83 - Rename o.a.c.chain2.generic package to o.a.c.chain2.base**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493342 13f79535-47bb-0310-9956-ffa450edef68

            [8fd1246a773fbab](https://github.com/ghacupha/commons-chain/commit/8fd1246a773fbab) Benedikt Ritter *2013-06-15 11:53:34*


                ### Jira CHAIN-86   

            **CHAIN-86 - Make CatalogFactory an interface (missing this file on the last commit)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1509003 13f79535-47bb-0310-9956-ffa450edef68

            [42f75b8b9246ed5](https://github.com/ghacupha/commons-chain/commit/42f75b8b9246ed5) Benedikt Ritter *2013-07-31 19:43:20*

            **CHAIN-86 - Make CatalogFactory an interface**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1508999 13f79535-47bb-0310-9956-ffa450edef68

            [9bdac08b1f5052a](https://github.com/ghacupha/commons-chain/commit/9bdac08b1f5052a) Benedikt Ritter *2013-07-31 19:37:11*


                ### Jira CHAIN-87   

            **CHAIN-87 - Change method signature of ConfigParser.parse(URL)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492853 13f79535-47bb-0310-9956-ffa450edef68

            [e57653951414be4](https://github.com/ghacupha/commons-chain/commit/e57653951414be4) Benedikt Ritter *2013-06-13 20:32:14*


                ### Jira CHAIN-88   

            **CHAIN-88 - Refactor tests in class ContextBaseTestCase - Thanks to Stephan Köninger**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493355 13f79535-47bb-0310-9956-ffa450edef68

            [103d4ecb3fca476](https://github.com/ghacupha/commons-chain/commit/103d4ecb3fca476) Benedikt Ritter *2013-06-15 13:56:11*


                ### Jira CHAIN-89   

            **CHAIN-89 - Combine XmlConfigParserTestCase and XmlConfigParser2TestCase into a parameterized test case - add issue to changes.xml**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493200 13f79535-47bb-0310-9956-ffa450edef68

            [cd73e7eac7866a8](https://github.com/ghacupha/commons-chain/commit/cd73e7eac7866a8) Benedikt Ritter *2013-06-14 18:48:32*

            **CHAIN-89 - Combine XmlConfigParserTestCase and XmlConfigParser2TestCase into a parameterized test case - move loading of config to setUp()**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493199 13f79535-47bb-0310-9956-ffa450edef68

            [22cf74a0fd1de23](https://github.com/ghacupha/commons-chain/commit/22cf74a0fd1de23) Benedikt Ritter *2013-06-14 18:45:38*

            **CHAIN-89 - Combine XmlConfigParserTestCase and XmlConfigParser2TestCase into a parameterized test case - initial refactoring to parameterized test case**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493195 13f79535-47bb-0310-9956-ffa450edef68

            [21acba33b661d8b](https://github.com/ghacupha/commons-chain/commit/21acba33b661d8b) Benedikt Ritter *2013-06-14 18:41:09*


                ### Jira CHAIN-90   

            **CHAIN-90 - Create test for o.a.c.chain.generic.CopyCommand**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493246 13f79535-47bb-0310-9956-ffa450edef68

            [34afd19b99c251a](https://github.com/ghacupha/commons-chain/commit/34afd19b99c251a) Benedikt Ritter *2013-06-14 21:04:41*


                ### Jira CHAIN-91   

            **CHAIN-91 - Split up CopyCommand**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1495718 13f79535-47bb-0310-9956-ffa450edef68

            [4037f37ecdffb0c](https://github.com/ghacupha/commons-chain/commit/4037f37ecdffb0c) Benedikt Ritter *2013-06-22 12:35:21*


                ### Jira CHAIN-92   

            **CHAIN-92 - Create a new module containing common test code and utilities; add issue to list of changes**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493554 13f79535-47bb-0310-9956-ffa450edef68

            [4d2ee522257c128](https://github.com/ghacupha/commons-chain/commit/4d2ee522257c128) Benedikt Ritter *2013-06-16 17:57:21*

            **CHAIN-92 - Create a new module containing common test code and utilities; create a matcher for checkCommandCount in test module**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493547 13f79535-47bb-0310-9956-ffa450edef68

            [6ddf7bf845b1fee](https://github.com/ghacupha/commons-chain/commit/6ddf7bf845b1fee) Benedikt Ritter *2013-06-16 17:49:49*

            **CHAIN-92 - Create a new module containing common test code and utilities; remove now obsolete dependency to chain2-base test-jar**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493535 13f79535-47bb-0310-9956-ffa450edef68

            [3dfa1ca2df2fea5](https://github.com/ghacupha/commons-chain/commit/3dfa1ca2df2fea5) Benedikt Ritter *2013-06-16 17:10:35*

            **CHAIN-92 - Create a new module containing common test code and utilities; move common commands used in tests to new module**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493534 13f79535-47bb-0310-9956-ffa450edef68

            [45638155e0516ea](https://github.com/ghacupha/commons-chain/commit/45638155e0516ea) Benedikt Ritter *2013-06-16 17:09:33*

            **CHAIN-92 - Create a new module containing common test code and utilities; initial check in of new module and a matcher implementation that substitutes checkExecuteLog(String)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493532 13f79535-47bb-0310-9956-ffa450edef68

            [3415b14e99d6978](https://github.com/ghacupha/commons-chain/commit/3415b14e99d6978) Benedikt Ritter *2013-06-16 17:03:19*


                ### Jira CHAIN-93   

            **CHAIN-93 - Create test case for o.a.c.chain2.base.RemoveCommand**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1494269 13f79535-47bb-0310-9956-ffa450edef68

            [bd9df4fb8d8cea9](https://github.com/ghacupha/commons-chain/commit/bd9df4fb8d8cea9) Benedikt Ritter *2013-06-18 19:45:59*


                ### Jira CHAIN-94   

            **CHAIN-94 - Refactor tests in class TestContextTestCase. Thanks to Jonas Sprenger**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497528 13f79535-47bb-0310-9956-ffa450edef68

            [35996d391baf1e1](https://github.com/ghacupha/commons-chain/commit/35996d391baf1e1) Benedikt Ritter *2013-06-27 19:47:43*


                ### Jira CHAIN-98   

            **CHAIN-98 - Refactor command interface and base Implementations to enumeration to represent states. Patch provided by Jonas Sprenger**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1499551 13f79535-47bb-0310-9956-ffa450edef68

            [dc845a7d5edbb43](https://github.com/ghacupha/commons-chain/commit/dc845a7d5edbb43) Benedikt Ritter *2013-07-03 20:45:37*


                ### Jira CODEC-67   

            **Fixing the headerFile location as per CODEC-67 and Benjamin's patch**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@651971 13f79535-47bb-0310-9956-ffa450edef68

            [407ce96bb0e5b3d](https://github.com/ghacupha/commons-chain/commit/407ce96bb0e5b3d) Henri Yandell *2008-04-27 16:00:39*


                ### Jira COMMONSSITE-57   

            **COMMONSSITE-57 Fix announce mod_mbox link**

                * (I used version 1.4-SNAPSHOT of the commons-build-plugin to do this - need to release it and update commons-parent at some point)
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1005115 13f79535-47bb-0310-9956-ffa450edef68

            [ed68efd408b55ef](https://github.com/ghacupha/commons-chain/commit/ed68efd408b55ef) Niall Pemberton *2010-10-06 16:38:08*


                ### Jira config-2   

            **Enhance the readability/writeability of configuration files for command**

                * chains, by supporting a new &lt;define&gt; element that dynamically adds new
                * Digester rules to the running instance, allowing use of elements without
                * having to specify the command or chain implementation class every time.
                * For example, assume you wanted to use two different instances of a
                * particular command in two different chains:
                * &lt;chains&gt;
                * ...
                * &lt;chain ...&gt;
                * ...
                * &lt;command className=&quot;com.mycompany.mycommands.FooCommand&quot;/&gt;
                * ...
                * &lt;/chain&gt;
                * &lt;chain ...&gt;
                * ...
                * &lt;command clasName=&quot;com.mycompany.mycommands.FooCommand&quot;/&gt;
                * ...
                * &lt;/chain&gt;
                * ...
                * &lt;/chains&gt;
                * Now, you can define an alias for this command and reuse it:
                * &lt;chains&gt;
                * ...
                * &lt;define name=&quot;foo&quot; className=&quot;com.mycompany.mycommands.FooCommand&quot;/&gt;
                * ...
                * &lt;chain ...&gt;
                * ...
                * &lt;foo&gt;
                * ...
                * &lt;/chain&gt;
                * &lt;chain ...&gt;
                * ...
                * &lt;foo&gt;
                * ...
                * &lt;/chain&gt;
                * ...
                * &lt;/chains&gt;
                * The dynamically generated rules include a Set Properties rule, so that you
                * can configure properties on aliased commands just like you can with the
                * &lt;chain&gt; or &lt;command&gt; elements directly.
                * See the unit test input file (test-config-2.xml) below for more examples.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142892 13f79535-47bb-0310-9956-ffa450edef68

            [79309690bc13bff](https://github.com/ghacupha/commons-chain/commit/79309690bc13bff) Craig R. McClanahan *2004-07-16 19:06:01*


                ### Jira java-1   

            **Get the java-1.3 profile working**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@931981 13f79535-47bb-0310-9956-ffa450edef68

            [b8e61e5ff3c4879](https://github.com/ghacupha/commons-chain/commit/b8e61e5ff3c4879) Niall Pemberton *2010-04-08 15:54:04*


                ### Jira jsf-1   

            **Update for current jsf-1.0-beta release.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142839 13f79535-47bb-0310-9956-ffa450edef68

            [64e591e5ab62230](https://github.com/ghacupha/commons-chain/commit/64e591e5ab62230) Ted Nathan Husted *2004-01-09 03:29:41*


                ### Jira parent-10   

            **Upgrade to commons-parent-10 pom**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@654484 13f79535-47bb-0310-9956-ffa450edef68

            [e95f4f2922093f2](https://github.com/ghacupha/commons-chain/commit/e95f4f2922093f2) Niall Pemberton *2008-05-08 11:43:09*


                ### Jira parent-12   

            **Update to commons-parent-12**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@827830 13f79535-47bb-0310-9956-ffa450edef68

            [cb8fa96e61e0b9e](https://github.com/ghacupha/commons-chain/commit/cb8fa96e61e0b9e) Niall Pemberton *2009-10-20 23:00:29*


                ### Jira parent-14   

            **Upgrade to commons-parent-14 (and maven-javadoc-plugin 2.5 when specified)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@923495 13f79535-47bb-0310-9956-ffa450edef68

            [d50860a94d8ce42](https://github.com/ghacupha/commons-chain/commit/d50860a94d8ce42) Niall Pemberton *2010-03-15 23:10:18*


                ### Jira parent-7   

            **upgrade to commons-parent-7**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@612219 13f79535-47bb-0310-9956-ffa450edef68

            [0470db8c6a439d2](https://github.com/ghacupha/commons-chain/commit/0470db8c6a439d2) Niall Pemberton *2008-01-15 21:04:51*


                ### Jira parent-8   

            **Upgrade to commons-parent-8 and add configuration properties for OSGi (maven-bundle-plugin) and commons-build-plugin**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@632815 13f79535-47bb-0310-9956-ffa450edef68

            [ef71ee6d2646d19](https://github.com/ghacupha/commons-chain/commit/ef71ee6d2646d19) Niall Pemberton *2008-03-02 19:37:56*


                ### Jira version-2   

            **fixed wrong version number, 3.0 not planned yet**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165755 13f79535-47bb-0310-9956-ffa450edef68

            [6f556306e42e1e6](https://github.com/ghacupha/commons-chain/commit/6f556306e42e1e6) Simone Tripodi *2011-09-06 16:27:41*

            **added missing @since tag in isFrozen() method javadoc**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165395 13f79535-47bb-0310-9956-ffa450edef68

            [e81bb399d3e36cd](https://github.com/ghacupha/commons-chain/commit/e81bb399d3e36cd) Simone Tripodi *2011-09-05 19:07:51*

            **added missing @since tag in getCommands() method javadoc**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165392 13f79535-47bb-0310-9956-ffa450edef68

            [2a53c9bb208f898](https://github.com/ghacupha/commons-chain/commit/2a53c9bb208f898) Simone Tripodi *2011-09-05 19:03:45*

            **added CHAIN-56 in the changelist**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165082 13f79535-47bb-0310-9956-ffa450edef68

            [4fcb1118173bb31](https://github.com/ghacupha/commons-chain/commit/4fcb1118173bb31) Simone Tripodi *2011-09-04 18:52:18*

            **[CHAIN-56] clever Context with generic type auto-cast feature**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165075 13f79535-47bb-0310-9956-ffa450edef68

            [575ca905ae623a2](https://github.com/ghacupha/commons-chain/commit/575ca905ae623a2) Simone Tripodi *2011-09-04 17:02:05*

            **added missing serialVersionUID**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165071 13f79535-47bb-0310-9956-ffa450edef68

            [77e809d179bcaab](https://github.com/ghacupha/commons-chain/commit/77e809d179bcaab) Simone Tripodi *2011-09-04 16:24:11*

            **infered MapEntry generic types**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165070 13f79535-47bb-0310-9956-ffa450edef68

            [dc13846a3082137](https://github.com/ghacupha/commons-chain/commit/dc13846a3082137) Simone Tripodi *2011-09-04 16:21:36*

            **muted HttpSession.getAttrbibuteNames() warnings, it is known that Session attribute names are String**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165069 13f79535-47bb-0310-9956-ffa450edef68

            [b882635f0f30f9c](https://github.com/ghacupha/commons-chain/commit/b882635f0f30f9c) Simone Tripodi *2011-09-04 16:20:44*

            **muted HttpServletReuqets.getAttrbibuteNames() warnings, it is known that Servlet request attribute names are String**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165067 13f79535-47bb-0310-9956-ffa450edef68

            [a459a81f1ba3e15](https://github.com/ghacupha/commons-chain/commit/a459a81f1ba3e15) Simone Tripodi *2011-09-04 16:19:18*

            **used the getCatalogKey() variant, as suggested in the javadoc**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165066 13f79535-47bb-0310-9956-ffa450edef68

            [fbb6d14e31deb2d](https://github.com/ghacupha/commons-chain/commit/fbb6d14e31deb2d) Simone Tripodi *2011-09-04 16:16:55*

            **extending LookupCommand, ServletPathMapper can be assigned to Command**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165065 13f79535-47bb-0310-9956-ffa450edef68

            [e9718c2a7298c27](https://github.com/ghacupha/commons-chain/commit/e9718c2a7298c27) Simone Tripodi *2011-09-04 16:16:11*

            **Command requires the <C extends Context> generic type**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165064 13f79535-47bb-0310-9956-ffa450edef68

            [2fec867cfc3429c](https://github.com/ghacupha/commons-chain/commit/2fec867cfc3429c) Simone Tripodi *2011-09-04 16:15:30*

            **muted HttpServletReuqets.getInitParameterNames() warnings, it is known that Servlet request parameter names are String**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165063 13f79535-47bb-0310-9956-ffa450edef68

            [c34d0dc8be97b18](https://github.com/ghacupha/commons-chain/commit/c34d0dc8be97b18) Simone Tripodi *2011-09-04 16:05:02*

            **muted HttpServletReuqets.getInitParameterNames() warnings, it is known that Servlet request parameter names are String**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165061 13f79535-47bb-0310-9956-ffa450edef68

            [050e73dbe510844](https://github.com/ghacupha/commons-chain/commit/050e73dbe510844) Simone Tripodi *2011-09-04 16:03:49*

            **muted ServletContext.getInitParamNames() warnings, it is known that init param names are String**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165055 13f79535-47bb-0310-9956-ffa450edef68

            [0388d77f82f8fc2](https://github.com/ghacupha/commons-chain/commit/0388d77f82f8fc2) Simone Tripodi *2011-09-04 15:54:10*

            **muted ServletContext.getHeaderNames() warnings, it is known that header names are String**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165054 13f79535-47bb-0310-9956-ffa450edef68

            [47cdb4ae6929d37](https://github.com/ghacupha/commons-chain/commit/47cdb4ae6929d37) Simone Tripodi *2011-09-04 15:53:06*

            **muted ServletContext.getHeaderNames() warnings, it is known that attribute names are String**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165053 13f79535-47bb-0310-9956-ffa450edef68

            [d332c1f65087524](https://github.com/ghacupha/commons-chain/commit/d332c1f65087524) Simone Tripodi *2011-09-04 15:50:47*

            **muted ServletContext.getAttributeNames() warnings, it is known that attribute names are String**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165051 13f79535-47bb-0310-9956-ffa450edef68

            [5cf08906fabcbb0](https://github.com/ghacupha/commons-chain/commit/5cf08906fabcbb0) Simone Tripodi *2011-09-04 15:49:15*

            **used the getParameter() variant, as suggested in the javadoc**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165050 13f79535-47bb-0310-9956-ffa450edef68

            [f23d8fbbfd84e94](https://github.com/ghacupha/commons-chain/commit/f23d8fbbfd84e94) Simone Tripodi *2011-09-04 15:43:03*

            **extending LookupCommand, RequestParameterMapper can be assigned to Command**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165049 13f79535-47bb-0310-9956-ffa450edef68

            [7cc0ef637857f41](https://github.com/ghacupha/commons-chain/commit/7cc0ef637857f41) Simone Tripodi *2011-09-04 15:39:26*

            **Command requires the <C extends Context> generic type**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165048 13f79535-47bb-0310-9956-ffa450edef68

            [b17cf0e62b24ea1](https://github.com/ghacupha/commons-chain/commit/b17cf0e62b24ea1) Simone Tripodi *2011-09-04 15:38:38*

            **used the non-deprecated getCatalogKey() variant, as suggested in the javadoc**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165045 13f79535-47bb-0310-9956-ffa450edef68

            [31c55baee44e386](https://github.com/ghacupha/commons-chain/commit/31c55baee44e386) Simone Tripodi *2011-09-04 15:06:06*

            **extending LookupCommand, PathInfoMapper can be assigned to Command**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165042 13f79535-47bb-0310-9956-ffa450edef68

            [3321a1041a59048](https://github.com/ghacupha/commons-chain/commit/3321a1041a59048) Simone Tripodi *2011-09-04 14:54:04*

            **Added missing Context generic type (PathInfoMapper is a Command)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165038 13f79535-47bb-0310-9956-ffa450edef68

            [d148ea5d516e927](https://github.com/ghacupha/commons-chain/commit/d148ea5d516e927) Simone Tripodi *2011-09-04 14:45:49*

            **Servlets will use ServletWebContext in Chains**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165032 13f79535-47bb-0310-9956-ffa450edef68

            [a5e277408845cf4](https://github.com/ghacupha/commons-chain/commit/a5e277408845cf4) Simone Tripodi *2011-09-04 14:36:31*

            **added missing generated serialVersionUID**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165030 13f79535-47bb-0310-9956-ffa450edef68

            [a4bdc858041f9e2](https://github.com/ghacupha/commons-chain/commit/a4bdc858041f9e2) Simone Tripodi *2011-09-04 14:18:15*

            **fixed Map generic types on empty maps**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165029 13f79535-47bb-0310-9956-ffa450edef68

            [c31bcfb7f2d08f6](https://github.com/ghacupha/commons-chain/commit/c31bcfb7f2d08f6) Simone Tripodi *2011-09-04 14:17:33*

            **added missing generated serialVersionUID**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165028 13f79535-47bb-0310-9956-ffa450edef68

            [db3c5d3fffe4c41](https://github.com/ghacupha/commons-chain/commit/db3c5d3fffe4c41) Simone Tripodi *2011-09-04 14:16:15*

            **added missing MapEntry generic types**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165027 13f79535-47bb-0310-9956-ffa450edef68

            [5e2007e075454a1](https://github.com/ghacupha/commons-chain/commit/5e2007e075454a1) Simone Tripodi *2011-09-04 14:15:38*

            **added missing MapEntry generic types**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165026 13f79535-47bb-0310-9956-ffa450edef68

            [a7a5a87f6e4bc9b](https://github.com/ghacupha/commons-chain/commit/a7a5a87f6e4bc9b) Simone Tripodi *2011-09-04 14:14:48*

            **added missing MapEntry generic types**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165024 13f79535-47bb-0310-9956-ffa450edef68

            [e472f1f8b124de7](https://github.com/ghacupha/commons-chain/commit/e472f1f8b124de7) Simone Tripodi *2011-09-04 14:13:59*

            **added missing generated serialVersionUID**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165022 13f79535-47bb-0310-9956-ffa450edef68

            [406868fb29c69b6](https://github.com/ghacupha/commons-chain/commit/406868fb29c69b6) Simone Tripodi *2011-09-04 14:12:13*

            **removed dead code, resourceURL cannot be null, at least it is not possible to estabilish a connection**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165021 13f79535-47bb-0310-9956-ffa450edef68

            [16cbe1a08c5eb94](https://github.com/ghacupha/commons-chain/commit/16cbe1a08c5eb94) Simone Tripodi *2011-09-04 14:10:56*

            **fixed generics on ServletContext paths**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165020 13f79535-47bb-0310-9956-ffa450edef68

            [0e0429c72d4a2ed](https://github.com/ghacupha/commons-chain/commit/0e0429c72d4a2ed) Simone Tripodi *2011-09-04 14:06:09*

            **used the non-deprecated parseJarResources() variant**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165019 13f79535-47bb-0310-9956-ffa450edef68

            [bc0b2284bffcc3a](https://github.com/ghacupha/commons-chain/commit/bc0b2284bffcc3a) Simone Tripodi *2011-09-04 14:02:53*

            **used non-deprecated ChainResources.parseClassResources method**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165017 13f79535-47bb-0310-9956-ffa450edef68

            [144c1fda68ae568](https://github.com/ghacupha/commons-chain/commit/144c1fda68ae568) Simone Tripodi *2011-09-04 13:58:20*

            **used non-deprecated ChainResources.parseWebResources method**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165016 13f79535-47bb-0310-9956-ffa450edef68

            [4d7ca38bfa3b3e2](https://github.com/ghacupha/commons-chain/commit/4d7ca38bfa3b3e2) Simone Tripodi *2011-09-04 13:57:18*

            **no reason to reinvent the parser, switched over java tokenizer implementation**

                * fixed path array length
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165015 13f79535-47bb-0310-9956-ffa450edef68

            [a7f526410758752](https://github.com/ghacupha/commons-chain/commit/a7f526410758752) Simone Tripodi *2011-09-04 13:55:01*

            **added missing serialVersionUID**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1165013 13f79535-47bb-0310-9956-ffa450edef68

            [10c899fe7dd1bea](https://github.com/ghacupha/commons-chain/commit/10c899fe7dd1bea) Simone Tripodi *2011-09-04 13:35:12*

            **muted Class generic type warnings**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164670 13f79535-47bb-0310-9956-ffa450edef68

            [b63d123bda4387f](https://github.com/ghacupha/commons-chain/commit/b63d123bda4387f) Simone Tripodi *2011-09-02 18:36:21*

            **muted Map.Entry generics warnings**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164669 13f79535-47bb-0310-9956-ffa450edef68

            [520ab80c5525d1a](https://github.com/ghacupha/commons-chain/commit/520ab80c5525d1a) Simone Tripodi *2011-09-02 18:35:25*

            **trailing spaces**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164534 13f79535-47bb-0310-9956-ffa450edef68

            [3a1b7d3b6607faf](https://github.com/ghacupha/commons-chain/commit/3a1b7d3b6607faf) Simone Tripodi *2011-09-02 13:53:56*

            **added the CHAIN-53 issue**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164531 13f79535-47bb-0310-9956-ffa450edef68

            [4496c72a81de95d](https://github.com/ghacupha/commons-chain/commit/4496c72a81de95d) Simone Tripodi *2011-09-02 13:40:44*

            **added missing serialVersionUID, Serializable classes require it**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164521 13f79535-47bb-0310-9956-ffa450edef68

            [3480e0d40e1638e](https://github.com/ghacupha/commons-chain/commit/3480e0d40e1638e) Simone Tripodi *2011-09-02 13:20:29*

            **just muted the map entry generic type warning**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164514 13f79535-47bb-0310-9956-ffa450edef68

            [4a911f42972d38d](https://github.com/ghacupha/commons-chain/commit/4a911f42972d38d) Simone Tripodi *2011-09-02 12:51:55*

            **fixed descriptors Map generic types**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164513 13f79535-47bb-0310-9956-ffa450edef68

            [34e2be8a3c5c12e](https://github.com/ghacupha/commons-chain/commit/34e2be8a3c5c12e) Simone Tripodi *2011-09-02 12:46:49*

            **Serializable requires serialVersionUID!**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164512 13f79535-47bb-0310-9956-ffa450edef68

            [8b72c7684ea76fa](https://github.com/ghacupha/commons-chain/commit/8b72c7684ea76fa) Simone Tripodi *2011-09-02 12:40:45*

            **added missing serialVersionUID, Serializable classes require it**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164511 13f79535-47bb-0310-9956-ffa450edef68

            [6e1d0f1428bbe69](https://github.com/ghacupha/commons-chain/commit/6e1d0f1428bbe69) Simone Tripodi *2011-09-02 12:39:46*

            **fixed Filter generic type, if command = Command<C> && command instance of Filter --> Filter<C>**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164510 13f79535-47bb-0310-9956-ffa450edef68

            [7b9a18e05eeb4f5](https://github.com/ghacupha/commons-chain/commit/7b9a18e05eeb4f5) Simone Tripodi *2011-09-02 12:38:34*

            **fixed generics on extractMethod() signature**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164509 13f79535-47bb-0310-9956-ffa450edef68

            [b7b5752e262e26f](https://github.com/ghacupha/commons-chain/commit/b7b5752e262e26f) Simone Tripodi *2011-09-02 12:36:15*

            **just muted the class array generic warning**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164508 13f79535-47bb-0310-9956-ffa450edef68

            [9b572380a985b07](https://github.com/ghacupha/commons-chain/commit/9b572380a985b07) Simone Tripodi *2011-09-02 12:35:18*

            **removed unneeded cast**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164506 13f79535-47bb-0310-9956-ffa450edef68

            [949d2a03732c2c9](https://github.com/ghacupha/commons-chain/commit/949d2a03732c2c9) Simone Tripodi *2011-09-02 12:32:49*

            **fixed generics warnings on Catalog<C> and FIlter<C> resolution**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164505 13f79535-47bb-0310-9956-ffa450edef68

            [4adb67136477064](https://github.com/ghacupha/commons-chain/commit/4adb67136477064) Simone Tripodi *2011-09-02 12:31:39*

            **just muted the class generic warning**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164503 13f79535-47bb-0310-9956-ffa450edef68

            [8ba7f0ee0387673](https://github.com/ghacupha/commons-chain/commit/8ba7f0ee0387673) Simone Tripodi *2011-09-02 12:27:54*

            **excluded myfaces dependencies that could collide with chain dependencies**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164501 13f79535-47bb-0310-9956-ffa450edef68

            [e1597863451f237](https://github.com/ghacupha/commons-chain/commit/e1597863451f237) Simone Tripodi *2011-09-02 12:21:00*

            **fixed checkstyle violation: Variable 'response' must be private and have accessor methods. (getter was already present)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164374 13f79535-47bb-0310-9956-ffa450edef68

            [1b39be3cf4d79be](https://github.com/ghacupha/commons-chain/commit/1b39be3cf4d79be) Simone Tripodi *2011-09-02 07:09:39*

            **fixed checkstyle violation: Variable 'request' must be private and have accessor methods. (getter was already present)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164373 13f79535-47bb-0310-9956-ffa450edef68

            [5a2ef9baf2b058e](https://github.com/ghacupha/commons-chain/commit/5a2ef9baf2b058e) Simone Tripodi *2011-09-02 07:09:17*

            **fixed checkstyle violation: Variable 'context' must be private and have accessor methods. (getter was already present)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164372 13f79535-47bb-0310-9956-ffa450edef68

            [504d1a2c958dea5](https://github.com/ghacupha/commons-chain/commit/504d1a2c958dea5) Simone Tripodi *2011-09-02 07:08:43*

            **fixed checkstyle violation: Variable 'response' must be private and have accessor methods. (getter was already present)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164369 13f79535-47bb-0310-9956-ffa450edef68

            [3d1e9daffc34e2e](https://github.com/ghacupha/commons-chain/commit/3d1e9daffc34e2e) Simone Tripodi *2011-09-02 06:59:03*

            **fixed checkstyle violation: Variable 'request' must be private and have accessor methods. (getter was already present)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164368 13f79535-47bb-0310-9956-ffa450edef68

            [7c40dbf183cd87f](https://github.com/ghacupha/commons-chain/commit/7c40dbf183cd87f) Simone Tripodi *2011-09-02 06:57:45*

            **fixed checkstyle violation: Variable 'context' must be private and have accessor methods. (getter was already present)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164367 13f79535-47bb-0310-9956-ffa450edef68

            [eb3a30eafe01307](https://github.com/ghacupha/commons-chain/commit/eb3a30eafe01307) Simone Tripodi *2011-09-02 06:56:56*

            **fixed checkstyle violation: ';' is preceded with whitespace.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164366 13f79535-47bb-0310-9956-ffa450edef68

            [4887d4b26042057](https://github.com/ghacupha/commons-chain/commit/4887d4b26042057) Simone Tripodi *2011-09-02 06:53:26*

            **fixed checkstyle violation: '{' should be on the previous line.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164365 13f79535-47bb-0310-9956-ffa450edef68

            [c5ec32c7bd9f074](https://github.com/ghacupha/commons-chain/commit/c5ec32c7bd9f074) Simone Tripodi *2011-09-02 06:51:27*

            **fixed checkstyle violations: Expected @param tag for '<C>'.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164364 13f79535-47bb-0310-9956-ffa450edef68

            [aed888261ae851f](https://github.com/ghacupha/commons-chain/commit/aed888261ae851f) Simone Tripodi *2011-09-02 06:50:52*

            **removed unused imports**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164264 13f79535-47bb-0310-9956-ffa450edef68

            [33266a2e2457359](https://github.com/ghacupha/commons-chain/commit/33266a2e2457359) Simone Tripodi *2011-09-01 20:29:46*

            **the command list can be final**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164261 13f79535-47bb-0310-9956-ffa450edef68

            [22efcf93e148a0e](https://github.com/ghacupha/commons-chain/commit/22efcf93e148a0e) Simone Tripodi *2011-09-01 20:28:11*

            **fixed checkstyle violation: Variable 'frozen' must be private and have accessor methods.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164260 13f79535-47bb-0310-9956-ffa450edef68

            [26c1bd07e86c51d](https://github.com/ghacupha/commons-chain/commit/26c1bd07e86c51d) Simone Tripodi *2011-09-01 20:27:20*

            **fixed checkstyle violation: Variable 'commands' must be private and have accessor methods.**

                * Variable &#39;commands&#39; set final
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164254 13f79535-47bb-0310-9956-ffa450edef68

            [963f7908229a04a](https://github.com/ghacupha/commons-chain/commit/963f7908229a04a) Simone Tripodi *2011-09-01 20:23:50*

            **fixed checkstyle violations: Expected @param tag for '<C>'.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164250 13f79535-47bb-0310-9956-ffa450edef68

            [9c2a965f2c73a46](https://github.com/ghacupha/commons-chain/commit/9c2a965f2c73a46) Simone Tripodi *2011-09-01 20:20:12*

            **fixed checkstyle violations: Expected @param tag for '<C>'.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164245 13f79535-47bb-0310-9956-ffa450edef68

            [c6159d161952357](https://github.com/ghacupha/commons-chain/commit/c6159d161952357) Simone Tripodi *2011-09-01 20:16:24*

            **fixed checkstyle violations: Expected @param tag for '<C>'.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164242 13f79535-47bb-0310-9956-ffa450edef68

            [c54b56533702e41](https://github.com/ghacupha/commons-chain/commit/c54b56533702e41) Simone Tripodi *2011-09-01 20:14:08*

            **added generics to Command<?> catalog**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1164178 13f79535-47bb-0310-9956-ffa450edef68

            [34266170f271315](https://github.com/ghacupha/commons-chain/commit/34266170f271315) Simone Tripodi *2011-09-01 17:17:47*

            **code simplifications; merge 'if (foo) return true; else return false;' type constructs; remove unnecessary parens; remove unnecessary elses**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163814 13f79535-47bb-0310-9956-ffa450edef68

            [059542869b245d1](https://github.com/ghacupha/commons-chain/commit/059542869b245d1) Matthew Jason Benson *2011-08-31 20:50:06*

            **fixed checkstyle violations: Conditional logic can be removed.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163800 13f79535-47bb-0310-9956-ffa450edef68

            [d1a160b7a903bac](https://github.com/ghacupha/commons-chain/commit/d1a160b7a903bac) Simone Tripodi *2011-08-31 20:27:48*

            **fixed checkstyle violations: Conditional logic can be removed.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163799 13f79535-47bb-0310-9956-ffa450edef68

            [8f391f1aabfaa0d](https://github.com/ghacupha/commons-chain/commit/8f391f1aabfaa0d) Simone Tripodi *2011-08-31 20:26:16*

            **empty line with trailing spaces**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163797 13f79535-47bb-0310-9956-ffa450edef68

            [0d0a2787885adc9](https://github.com/ghacupha/commons-chain/commit/0d0a2787885adc9) Simone Tripodi *2011-08-31 20:24:43*

            **fixed checkstyle violation: Unused import - java.util.Iterator**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163796 13f79535-47bb-0310-9956-ffa450edef68

            [26e42a6ac31bf37](https://github.com/ghacupha/commons-chain/commit/26e42a6ac31bf37) Simone Tripodi *2011-08-31 20:22:26*

            **package.html replaced by package-info.java files**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163793 13f79535-47bb-0310-9956-ffa450edef68

            [cc1a684a79b696d](https://github.com/ghacupha/commons-chain/commit/cc1a684a79b696d) Simone Tripodi *2011-08-31 20:20:25*

            **used collections method to add commands from an existing collection**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163745 13f79535-47bb-0310-9956-ffa450edef68

            [26084aaed286913](https://github.com/ghacupha/commons-chain/commit/26084aaed286913) Simone Tripodi *2011-08-31 19:04:48*

            **used smarter ArrayList instead of continuous replaced fixed arrays**

                * that modification introduces a Clirr error
                * &quot;Changed type of field commands from org.apache.commons.chain.Command[] to java.util.List&quot;
                * it was used anyway only as internal data structure to store Command instances &amp; for test purposes, not a meaningful change
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163743 13f79535-47bb-0310-9956-ffa450edef68

            [df06058d30706a2](https://github.com/ghacupha/commons-chain/commit/df06058d30706a2) Simone Tripodi *2011-08-31 19:01:10*

            **fixed generic array type warnings**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163735 13f79535-47bb-0310-9956-ffa450edef68

            [f17fcb7d97a1370](https://github.com/ghacupha/commons-chain/commit/f17fcb7d97a1370) Simone Tripodi *2011-08-31 18:25:10*

            **fixed generic types warnings**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163733 13f79535-47bb-0310-9956-ffa450edef68

            [616b1197237e788](https://github.com/ghacupha/commons-chain/commit/616b1197237e788) Simone Tripodi *2011-08-31 18:23:28*

            **fixed generic types warnings**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163732 13f79535-47bb-0310-9956-ffa450edef68

            [2ee1cacb9c0a758](https://github.com/ghacupha/commons-chain/commit/2ee1cacb9c0a758) Simone Tripodi *2011-08-31 18:21:48*

            **removed @Override annotation for interfaces methods implementation**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163728 13f79535-47bb-0310-9956-ffa450edef68

            [79129f8580b2335](https://github.com/ghacupha/commons-chain/commit/79129f8580b2335) Simone Tripodi *2011-08-31 18:11:36*

            **replaced <T> generic with <C> that stands for 'Context', it is more intuitive**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1163636 13f79535-47bb-0310-9956-ffa450edef68

            [5c1486fe47f10d8](https://github.com/ghacupha/commons-chain/commit/5c1486fe47f10d8) Simone Tripodi *2011-08-31 14:26:26*

            **fixed clirr report generation**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1162953 13f79535-47bb-0310-9956-ffa450edef68

            [57601f24ffa92ad](https://github.com/ghacupha/commons-chain/commit/57601f24ffa92ad) Simone Tripodi *2011-08-29 19:33:12*

            **added the distribution management**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1162936 13f79535-47bb-0310-9956-ffa450edef68

            [5e6876556b7c88d](https://github.com/ghacupha/commons-chain/commit/5e6876556b7c88d) Simone Tripodi *2011-08-29 18:33:06*

            **upgraded major version**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1162934 13f79535-47bb-0310-9956-ffa450edef68

            [2971ae980b371ee](https://github.com/ghacupha/commons-chain/commit/2971ae980b371ee) Simone Tripodi *2011-08-29 18:30:27*

            **added Elijah Zupancic in the contributors list**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1162929 13f79535-47bb-0310-9956-ffa450edef68

            [318cc94ab5a91a6](https://github.com/ghacupha/commons-chain/commit/318cc94ab5a91a6) Simone Tripodi *2011-08-29 18:24:22*

            **[CHAIN-53] Global Update of Chain - Generics, JDK 1.5, Update Dependency Versions - patch submitted by Elijah Zupancic**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1162332 13f79535-47bb-0310-9956-ffa450edef68

            [495e5f7ccfcad46](https://github.com/ghacupha/commons-chain/commit/495e5f7ccfcad46) Simone Tripodi *2011-08-27 12:34:14*

            **copied the current trunk on a branch to experiment the 2.0 version as discussed in the ML**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/branches/version-2.0-work@1160659 13f79535-47bb-0310-9956-ffa450edef68

            [ce5f735c7ec1c2b](https://github.com/ghacupha/commons-chain/commit/ce5f735c7ec1c2b) Simone Tripodi *2011-08-23 12:30:34*


            ### No issue

            **Added and configured changelog recording mechanism**


            [45064279be55bc1](https://github.com/ghacupha/commons-chain/commit/45064279be55bc1) Edwin Njeru *2018-04-04 14:07:34*

            **Added and configured changelog recording mechanism**


            [e04714e87e4cd34](https://github.com/ghacupha/commons-chain/commit/e04714e87e4cd34) Edwin Njeru *2018-04-04 14:00:05*

            **Added and configured changelog recording mechanism**


            [7e9591bc599f0f8](https://github.com/ghacupha/commons-chain/commit/7e9591bc599f0f8) Edwin Njeru *2018-04-04 13:59:42*

            **added java 8 semantics to ContextBase**


            [1c89108356b235d](https://github.com/ghacupha/commons-chain/commit/1c89108356b235d) Edwin Njeru *2018-04-04 12:52:53*

            **added java 8 semantics to ContextBase**


            [d69513f77429560](https://github.com/ghacupha/commons-chain/commit/d69513f77429560) Edwin Njeru *2018-04-04 12:15:38*

            **change assert cases to junit assertTrue tests in RemoveCommandTestCase**


            [2ab764a34d910dd](https://github.com/ghacupha/commons-chain/commit/2ab764a34d910dd) Edwin Njeru *2018-04-04 12:08:35*

            **change assert cases to junit assertTrue tests in RemoveCommandTestCase**


            [4d1e8d763e316c6](https://github.com/ghacupha/commons-chain/commit/4d1e8d763e316c6) Edwin Njeru *2018-04-04 12:03:56*

            **removed unnecessary testEquals test to equivalent object created through createContext method**


            [50bbb0a31adfc0c](https://github.com/ghacupha/commons-chain/commit/50bbb0a31adfc0c) Edwin Njeru *2018-04-04 11:11:03*

            **changed the return type for keySet in the ContextBase to KeySetView and changed language level to 1.8**


            [3a402779ccd195f](https://github.com/ghacupha/commons-chain/commit/3a402779ccd195f) Edwin Njeru *2018-04-04 10:44:49*

            **Update commons-parent from 40 to 43.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1820499 13f79535-47bb-0310-9956-ffa450edef68

            [5d194b2ab6adf26](https://github.com/ghacupha/commons-chain/commit/5d194b2ab6adf26) Gary D. Gregory *2018-01-07 21:03:15*

            **(chore) adding commons.module.name to pom**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1796412 13f79535-47bb-0310-9956-ffa450edef68

            [b812b68651ec8fe](https://github.com/ghacupha/commons-chain/commit/b812b68651ec8fe) Rob Tompkins *2017-05-27 15:11:38*

            **commons-parent 32 -> 40.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1749793 13f79535-47bb-0310-9956-ffa450edef68

            [5b3673e411269c6](https://github.com/ghacupha/commons-chain/commit/5b3673e411269c6) Gary D. Gregory *2016-06-22 22:24:49*

            **Update old school @exception with new school @throws.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1747104 13f79535-47bb-0310-9956-ffa450edef68

            [3c9f548f4a809a4](https://github.com/ghacupha/commons-chain/commit/3c9f548f4a809a4) Gary D. Gregory *2016-06-07 00:50:15*

            **Add Eclipse files to svn:ignore.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1747103 13f79535-47bb-0310-9956-ffa450edef68

            [def8de61b2ecee2](https://github.com/ghacupha/commons-chain/commit/def8de61b2ecee2) Gary D. Gregory *2016-06-07 00:49:31*

            **Update copyright for 2016 in NOTICE.txt**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1725415 13f79535-47bb-0310-9956-ffa450edef68

            [1fe5bccca22aaa5](https://github.com/ghacupha/commons-chain/commit/1fe5bccca22aaa5) Gary D. Gregory *2016-01-19 06:19:49*

            **Collect the DOAPs**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1718920 13f79535-47bb-0310-9956-ffa450edef68

            [87308216da7a6fc](https://github.com/ghacupha/commons-chain/commit/87308216da7a6fc) Sebastian Bazley *2015-12-09 17:32:04*

            **Each version must be in its own release section**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1678353 13f79535-47bb-0310-9956-ffa450edef68

            [e21bc29c8b5285c](https://github.com/ghacupha/commons-chain/commit/e21bc29c8b5285c) Sebastian Bazley *2015-05-08 13:54:49*

            **Typo**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1643393 13f79535-47bb-0310-9956-ffa450edef68

            [70baa08cc0d3cb9](https://github.com/ghacupha/commons-chain/commit/70baa08cc0d3cb9) Sebastian Bazley *2014-12-05 19:01:00*

            **developed at->developed by**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1534730 13f79535-47bb-0310-9956-ffa450edef68

            [4db28901ef897dd](https://github.com/ghacupha/commons-chain/commit/4db28901ef897dd) Henri Yandell *2013-10-22 19:04:12*

            **updated ignore list**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1500821 13f79535-47bb-0310-9956-ffa450edef68

            [8fb3d821b69fcbc](https://github.com/ghacupha/commons-chain/commit/8fb3d821b69fcbc) Simone Tripodi *2013-07-08 16:25:15*

            **Update to latest parent pom**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1499850 13f79535-47bb-0310-9956-ffa450edef68

            [e83dbf8f2402755](https://github.com/ghacupha/commons-chain/commit/e83dbf8f2402755) Benedikt Ritter *2013-07-04 19:58:27*

            **PMD - Remove unnecessary parentheses**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497553 13f79535-47bb-0310-9956-ffa450edef68

            [a7511a374b6195b](https://github.com/ghacupha/commons-chain/commit/a7511a374b6195b) Benedikt Ritter *2013-06-27 20:11:00*

            **Only document RuntimeExceptions in JavaDoc, not in method signature**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497550 13f79535-47bb-0310-9956-ffa450edef68

            [8d787e16cd2b03b](https://github.com/ghacupha/commons-chain/commit/8d787e16cd2b03b) Benedikt Ritter *2013-06-27 20:09:08*

            **Use Id keyword instead instead of author tag**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497547 13f79535-47bb-0310-9956-ffa450edef68

            [cda164cb72b4ecf](https://github.com/ghacupha/commons-chain/commit/cda164cb72b4ecf) Benedikt Ritter *2013-06-27 20:03:26*

            **Add missing AL header**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497544 13f79535-47bb-0310-9956-ffa450edef68

            [93739c3a76c74d6](https://github.com/ghacupha/commons-chain/commit/93739c3a76c74d6) Benedikt Ritter *2013-06-27 20:01:40*

            **Remove redundant import**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497542 13f79535-47bb-0310-9956-ffa450edef68

            [936dfb0ff5174c9](https://github.com/ghacupha/commons-chain/commit/936dfb0ff5174c9) Benedikt Ritter *2013-06-27 20:00:33*

            **Add missing license header**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497541 13f79535-47bb-0310-9956-ffa450edef68

            [b2c473a65377e47](https://github.com/ghacupha/commons-chain/commit/b2c473a65377e47) Benedikt Ritter *2013-06-27 19:59:27*

            **Remove unused import, remove unnecessary empty lines**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497540 13f79535-47bb-0310-9956-ffa450edef68

            [1ec804ff3d1a589](https://github.com/ghacupha/commons-chain/commit/1ec804ff3d1a589) Benedikt Ritter *2013-06-27 19:58:04*

            **Checkstyle: add missing white spaces**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497536 13f79535-47bb-0310-9956-ffa450edef68

            [9f17afd33c71f5f](https://github.com/ghacupha/commons-chain/commit/9f17afd33c71f5f) Benedikt Ritter *2013-06-27 19:56:05*

            **Add some more missing version keywords**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497535 13f79535-47bb-0310-9956-ffa450edef68

            [f4a1df033ccc985](https://github.com/ghacupha/commons-chain/commit/f4a1df033ccc985) Benedikt Ritter *2013-06-27 19:53:55*

            **Add version keyword**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497534 13f79535-47bb-0310-9956-ffa450edef68

            [fc83db76cdbb8a9](https://github.com/ghacupha/commons-chain/commit/fc83db76cdbb8a9) Benedikt Ritter *2013-06-27 19:52:36*

            **Remove unnecessary empty lines and comments**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497533 13f79535-47bb-0310-9956-ffa450edef68

            [53cd1abd3e736f0](https://github.com/ghacupha/commons-chain/commit/53cd1abd3e736f0) Benedikt Ritter *2013-06-27 19:51:53*

            **Update to latest commons logging version**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497513 13f79535-47bb-0310-9956-ffa450edef68

            [f704b9a99222e48](https://github.com/ghacupha/commons-chain/commit/f704b9a99222e48) Benedikt Ritter *2013-06-27 19:25:32*

            **Update to latest CP**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1497505 13f79535-47bb-0310-9956-ffa450edef68

            [acb4f72cb6d45a2](https://github.com/ghacupha/commons-chain/commit/acb4f72cb6d45a2) Benedikt Ritter *2013-06-27 19:11:12*

            **Use enhanced for loop**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1496627 13f79535-47bb-0310-9956-ffa450edef68

            [0247d48321cfdb0](https://github.com/ghacupha/commons-chain/commit/0247d48321cfdb0) Benedikt Ritter *2013-06-25 20:19:29*

            **PMD - Remove useless parentheses**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1496625 13f79535-47bb-0310-9956-ffa450edef68

            [28f80b32797f165](https://github.com/ghacupha/commons-chain/commit/28f80b32797f165) Benedikt Ritter *2013-06-25 20:13:52*

            **No need to import Context just for JavaDoc**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1496614 13f79535-47bb-0310-9956-ffa450edef68

            [709d21eccce7f8f](https://github.com/ghacupha/commons-chain/commit/709d21eccce7f8f) Benedikt Ritter *2013-06-25 19:48:55*

            **Set svn props**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1496604 13f79535-47bb-0310-9956-ffa450edef68

            [5dff38009b3e4c2](https://github.com/ghacupha/commons-chain/commit/5dff38009b3e4c2) Benedikt Ritter *2013-06-25 19:32:59*

            **Make sure NonDelegetingCommand always returns true**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1496603 13f79535-47bb-0310-9956-ffa450edef68

            [32ee53a05e65f08](https://github.com/ghacupha/commons-chain/commit/32ee53a05e65f08) Benedikt Ritter *2013-06-25 19:31:58*

            **Add test for NonDelegatingCommand**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1496599 13f79535-47bb-0310-9956-ffa450edef68

            [340ad1d60117da6](https://github.com/ghacupha/commons-chain/commit/340ad1d60117da6) Benedikt Ritter *2013-06-25 19:26:13*

            **Minimum required JRE according to maven.compiler.source is 1.6**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1496594 13f79535-47bb-0310-9956-ffa450edef68

            [8cffb392ef2c0b3](https://github.com/ghacupha/commons-chain/commit/8cffb392ef2c0b3) Benedikt Ritter *2013-06-25 19:11:54*

            **Update to latest FindBugs plugin version**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1496191 13f79535-47bb-0310-9956-ffa450edef68

            [4e183ab2bc83f00](https://github.com/ghacupha/commons-chain/commit/4e183ab2bc83f00) Benedikt Ritter *2013-06-24 20:08:11*

            **Organize imports, use classes from org.junit package**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1495719 13f79535-47bb-0310-9956-ffa450edef68

            [2cf379d395a38c2](https://github.com/ghacupha/commons-chain/commit/2cf379d395a38c2) Benedikt Ritter *2013-06-22 12:44:05*

            **Use Id svn keyword instead of revision only**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1494273 13f79535-47bb-0310-9956-ffa450edef68

            [d02be35415819ef](https://github.com/ghacupha/commons-chain/commit/d02be35415819ef) Benedikt Ritter *2013-06-18 19:58:51*

            **Use explicit imports instead of wildcards**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1494272 13f79535-47bb-0310-9956-ffa450edef68

            [72c479a5eb72d9e](https://github.com/ghacupha/commons-chain/commit/72c479a5eb72d9e) Benedikt Ritter *2013-06-18 19:58:13*

            **Suffix test case classes with "TestCase"**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1494262 13f79535-47bb-0310-9956-ffa450edef68

            [78c116feb465cbc](https://github.com/ghacupha/commons-chain/commit/78c116feb465cbc) Benedikt Ritter *2013-06-18 19:05:56*

            **Remove IDE config file**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1494260 13f79535-47bb-0310-9956-ffa450edef68

            [cd135de981e050e](https://github.com/ghacupha/commons-chain/commit/cd135de981e050e) Benedikt Ritter *2013-06-18 19:00:47*

            **Use Id svn keyword**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493558 13f79535-47bb-0310-9956-ffa450edef68

            [decbbfef771546a](https://github.com/ghacupha/commons-chain/commit/decbbfef771546a) Benedikt Ritter *2013-06-16 18:03:13*

            **Remove unneeded brackets**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493552 13f79535-47bb-0310-9956-ffa450edef68

            [c81dc4ecc1122d1](https://github.com/ghacupha/commons-chain/commit/c81dc4ecc1122d1) Benedikt Ritter *2013-06-16 17:55:49*

            **JavaDoc for new matcher**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493549 13f79535-47bb-0310-9956-ffa450edef68

            [de9b23643bf58f7](https://github.com/ghacupha/commons-chain/commit/de9b23643bf58f7) Benedikt Ritter *2013-06-16 17:52:12*

            **Set svn props**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493548 13f79535-47bb-0310-9956-ffa450edef68

            [89d230db84bb955](https://github.com/ghacupha/commons-chain/commit/89d230db84bb955) Benedikt Ritter *2013-06-16 17:51:19*

            **Update to latest JUnit release**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493501 13f79535-47bb-0310-9956-ffa450edef68

            [a4072ced7d305b3](https://github.com/ghacupha/commons-chain/commit/a4072ced7d305b3) Benedikt Ritter *2013-06-16 12:05:48*

            **No need to create an anonymous subclass here**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493362 13f79535-47bb-0310-9956-ffa450edef68

            [28e918bf86c78e4](https://github.com/ghacupha/commons-chain/commit/28e918bf86c78e4) Benedikt Ritter *2013-06-15 14:13:29*

            **Use Id svn keyword**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493361 13f79535-47bb-0310-9956-ffa450edef68

            [9bb434ebd027197](https://github.com/ghacupha/commons-chain/commit/9bb434ebd027197) Benedikt Ritter *2013-06-15 14:09:47*

            **Use actual email addresses**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493358 13f79535-47bb-0310-9956-ffa450edef68

            [ab88c7d28eabcf4](https://github.com/ghacupha/commons-chain/commit/ab88c7d28eabcf4) Benedikt Ritter *2013-06-15 14:06:59*

            **Apply compose method instead of using comments**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493213 13f79535-47bb-0310-9956-ffa450edef68

            [e97e720f845c219](https://github.com/ghacupha/commons-chain/commit/e97e720f845c219) Benedikt Ritter *2013-06-14 19:10:45*

            **Use Id svn keyword**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493202 13f79535-47bb-0310-9956-ffa450edef68

            [83d5fadf4f05f75](https://github.com/ghacupha/commons-chain/commit/83d5fadf4f05f75) Benedikt Ritter *2013-06-14 18:51:37*

            **Invert assertions**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493201 13f79535-47bb-0310-9956-ffa450edef68

            [b4408b8c84912f0](https://github.com/ghacupha/commons-chain/commit/b4408b8c84912f0) Benedikt Ritter *2013-06-14 18:49:45*

            **Remove unneeded hyphens in JavaDoc**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1493152 13f79535-47bb-0310-9956-ffa450edef68

            [dacb912b9f022d4](https://github.com/ghacupha/commons-chain/commit/dacb912b9f022d4) Benedikt Ritter *2013-06-14 16:51:37*

            **Remove unused imports**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492865 13f79535-47bb-0310-9956-ffa450edef68

            [9359e2214dea089](https://github.com/ghacupha/commons-chain/commit/9359e2214dea089) Benedikt Ritter *2013-06-13 21:00:08*

            **Correct SVN keywords declaration**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492864 13f79535-47bb-0310-9956-ffa450edef68

            [cdcebb2bcbc94f5](https://github.com/ghacupha/commons-chain/commit/cdcebb2bcbc94f5) Benedikt Ritter *2013-06-13 20:59:41*

            **Set svn props**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492863 13f79535-47bb-0310-9956-ffa450edef68

            [fae341ae0d1cbc0](https://github.com/ghacupha/commons-chain/commit/fae341ae0d1cbc0) Benedikt Ritter *2013-06-13 20:58:52*

            **Code formatting**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492862 13f79535-47bb-0310-9956-ffa450edef68

            [52494df4a8d378c](https://github.com/ghacupha/commons-chain/commit/52494df4a8d378c) Benedikt Ritter *2013-06-13 20:56:54*

            **Invert assert messages**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492840 13f79535-47bb-0310-9956-ffa450edef68

            [6abe23cb25b7346](https://github.com/ghacupha/commons-chain/commit/6abe23cb25b7346) Benedikt Ritter *2013-06-13 20:06:59*

            **Set svn keywords**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492838 13f79535-47bb-0310-9956-ffa450edef68

            [f2e7d90fa2882a2](https://github.com/ghacupha/commons-chain/commit/f2e7d90fa2882a2) Benedikt Ritter *2013-06-13 19:57:31*

            **Remove unused imports**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492835 13f79535-47bb-0310-9956-ffa450edef68

            [ecc41ce57f18937](https://github.com/ghacupha/commons-chain/commit/ecc41ce57f18937) Benedikt Ritter *2013-06-13 19:50:58*

            **Pull up common methods in abstract base class**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492833 13f79535-47bb-0310-9956-ffa450edef68

            [0de2787ff47059b](https://github.com/ghacupha/commons-chain/commit/0de2787ff47059b) Benedikt Ritter *2013-06-13 19:50:01*

            **Don't use wildcard imports**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492817 13f79535-47bb-0310-9956-ffa450edef68

            [2acbd2f5394b9b0](https://github.com/ghacupha/commons-chain/commit/2acbd2f5394b9b0) Benedikt Ritter *2013-06-13 18:51:35*

            **Rename tests according to the classes under test**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492805 13f79535-47bb-0310-9956-ffa450edef68

            [d1d92f785063460](https://github.com/ghacupha/commons-chain/commit/d1d92f785063460) Benedikt Ritter *2013-06-13 18:40:46*

            **Check that log is not null (instead of the assertion message)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492412 13f79535-47bb-0310-9956-ffa450edef68

            [f5f8b929e1f6158](https://github.com/ghacupha/commons-chain/commit/f5f8b929e1f6158) Benedikt Ritter *2013-06-12 20:30:33*

            **Remove unneeded this qualifier**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492411 13f79535-47bb-0310-9956-ffa450edef68

            [5a8044bc66d7f65](https://github.com/ghacupha/commons-chain/commit/5a8044bc66d7f65) Benedikt Ritter *2013-06-12 20:22:22*

            **Correct keyword declaration**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492409 13f79535-47bb-0310-9956-ffa450edef68

            [ca2b76e5e850e8e](https://github.com/ghacupha/commons-chain/commit/ca2b76e5e850e8e) Benedikt Ritter *2013-06-12 20:16:31*

            **Use Id keyword instead of revision**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492408 13f79535-47bb-0310-9956-ffa450edef68

            [cf2a20e7bc5b2ae](https://github.com/ghacupha/commons-chain/commit/cf2a20e7bc5b2ae) Benedikt Ritter *2013-06-12 20:15:42*

            **Invert even more assertions**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492394 13f79535-47bb-0310-9956-ffa450edef68

            [83a707f9422866f](https://github.com/ghacupha/commons-chain/commit/83a707f9422866f) Benedikt Ritter *2013-06-12 19:32:52*

            **Invert assertion**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492392 13f79535-47bb-0310-9956-ffa450edef68

            [5a8f9ca832323ba](https://github.com/ghacupha/commons-chain/commit/5a8f9ca832323ba) Benedikt Ritter *2013-06-12 19:28:38*

            **Use Id svn keyword instead of Date keyword**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1492385 13f79535-47bb-0310-9956-ffa450edef68

            [1c3ba81796896da](https://github.com/ghacupha/commons-chain/commit/1c3ba81796896da) Benedikt Ritter *2013-06-12 19:22:21*

            **Remove unused import**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1491949 13f79535-47bb-0310-9956-ffa450edef68

            [7d70359bad97d59](https://github.com/ghacupha/commons-chain/commit/7d70359bad97d59) Benedikt Ritter *2013-06-11 20:46:45*

            **Invert assert messages, they will be shown when an assertion fails**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1491947 13f79535-47bb-0310-9956-ffa450edef68

            [398e2b46c951052](https://github.com/ghacupha/commons-chain/commit/398e2b46c951052) Benedikt Ritter *2013-06-11 20:34:49*

            **Never use Date property, it depends on the client's locale. Use Id instead.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1491933 13f79535-47bb-0310-9956-ffa450edef68

            [e7200d8962018d3](https://github.com/ghacupha/commons-chain/commit/e7200d8962018d3) Benedikt Ritter *2013-06-11 20:07:43*

            **Tweak JavaDoc**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1491930 13f79535-47bb-0310-9956-ffa450edef68

            [8f1e3c297a49d46](https://github.com/ghacupha/commons-chain/commit/8f1e3c297a49d46) Benedikt Ritter *2013-06-11 20:01:21*

            **Use enhanced for loop instead of iteration with counter**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1491929 13f79535-47bb-0310-9956-ffa450edef68

            [9c4e04622385136](https://github.com/ghacupha/commons-chain/commit/9c4e04622385136) Benedikt Ritter *2013-06-11 19:59:39*

            **Fix failing test**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1491926 13f79535-47bb-0310-9956-ffa450edef68

            [e723fb56d73c09a](https://github.com/ghacupha/commons-chain/commit/e723fb56d73c09a) Benedikt Ritter *2013-06-11 19:55:11*

            **Add some tests to verify input parameter validation of constrcutors**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1491925 13f79535-47bb-0310-9956-ffa450edef68

            [63a57769eabd5e2](https://github.com/ghacupha/commons-chain/commit/63a57769eabd5e2) Benedikt Ritter *2013-06-11 19:51:22*

            **Use var args instead of array as parameter**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1491924 13f79535-47bb-0310-9956-ffa450edef68

            [e16d360eeb37d6b](https://github.com/ghacupha/commons-chain/commit/e16d360eeb37d6b) Benedikt Ritter *2013-06-11 19:47:16*

            **Update to latest commons parent pom**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1491200 13f79535-47bb-0310-9956-ffa450edef68

            [a4269c3481fdccc](https://github.com/ghacupha/commons-chain/commit/a4269c3481fdccc) Benedikt Ritter *2013-06-09 12:28:17*

            **Chain 2 requires Java 5**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1491189 13f79535-47bb-0310-9956-ffa450edef68

            [04aa49946a9663d](https://github.com/ghacupha/commons-chain/commit/04aa49946a9663d) Benedikt Ritter *2013-06-09 12:10:13*

            **Correct typo in exception message**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1491184 13f79535-47bb-0310-9956-ffa450edef68

            [b92ed0a5f32a8b5](https://github.com/ghacupha/commons-chain/commit/b92ed0a5f32a8b5) Benedikt Ritter *2013-06-09 11:38:12*

            **Replace StringBuffer with StringBuilder**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1488513 13f79535-47bb-0310-9956-ffa450edef68

            [722a5161d49a4b6](https://github.com/ghacupha/commons-chain/commit/722a5161d49a4b6) Benedikt Ritter *2013-06-01 12:39:42*

            **Correct indentation**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1488506 13f79535-47bb-0310-9956-ffa450edef68

            [d2bffad9c36a845](https://github.com/ghacupha/commons-chain/commit/d2bffad9c36a845) Benedikt Ritter *2013-06-01 12:02:39*

            **Missed those missing empty lines...**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1488505 13f79535-47bb-0310-9956-ffa450edef68

            [392eed433e82937](https://github.com/ghacupha/commons-chain/commit/392eed433e82937) Benedikt Ritter *2013-06-01 11:46:07*

            **Code formatting, no functional changes**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1488503 13f79535-47bb-0310-9956-ffa450edef68

            [a942453220b7219](https://github.com/ghacupha/commons-chain/commit/a942453220b7219) Benedikt Ritter *2013-06-01 11:33:55*

            **if the ConfigParser is not available in the classpath, then the application is in an illegal status**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1486528 13f79535-47bb-0310-9956-ffa450edef68

            [2a2d561171ca590](https://github.com/ghacupha/commons-chain/commit/2a2d561171ca590) Simone Tripodi *2013-05-27 07:38:38*

            **Trailing spaces**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1471761 13f79535-47bb-0310-9956-ffa450edef68

            [0087f30bcd7c0f5](https://github.com/ghacupha/commons-chain/commit/0087f30bcd7c0f5) Sebastian Bazley *2013-04-24 23:05:20*

            **Avoid potential NPE**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1471597 13f79535-47bb-0310-9956-ffa450edef68

            [eddf67d8f952c95](https://github.com/ghacupha/commons-chain/commit/eddf67d8f952c95) Sebastian Bazley *2013-04-24 18:42:21*

            **Javadoc typo**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1471594 13f79535-47bb-0310-9956-ffa450edef68

            [7e3f90120094d35](https://github.com/ghacupha/commons-chain/commit/7e3f90120094d35) Sebastian Bazley *2013-04-24 18:37:05*

            **Override hashCode when overridin equals**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1471593 13f79535-47bb-0310-9956-ffa450edef68

            [9115f3ea2c0ce1d](https://github.com/ghacupha/commons-chain/commit/9115f3ea2c0ce1d) Sebastian Bazley *2013-04-24 18:32:29*

            **Use new variable; don't overwrite the original.**

                * Fix generic warning
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1471591 13f79535-47bb-0310-9956-ffa450edef68

            [8673ce1244afce3](https://github.com/ghacupha/commons-chain/commit/8673ce1244afce3) Sebastian Bazley *2013-04-24 18:29:12*

            **Add some missing method @Override markers**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1471589 13f79535-47bb-0310-9956-ffa450edef68

            [c29a7e522c3ad3f](https://github.com/ghacupha/commons-chain/commit/c29a7e522c3ad3f) Sebastian Bazley *2013-04-24 18:24:58*

            **Make unboxing explicit.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1471586 13f79535-47bb-0310-9956-ffa450edef68

            [e9e47e65ac7854f](https://github.com/ghacupha/commons-chain/commit/e9e47e65ac7854f) Sebastian Bazley *2013-04-24 18:22:38*

            **Not possible to avoid raw type here because of poor Faces API**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1471583 13f79535-47bb-0310-9956-ffa450edef68

            [4fe8653e7af1b15](https://github.com/ghacupha/commons-chain/commit/4fe8653e7af1b15) Sebastian Bazley *2013-04-24 18:20:11*

            **Unnecessary casts**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1471575 13f79535-47bb-0310-9956-ffa450edef68

            [e27468e73aa6a31](https://github.com/ghacupha/commons-chain/commit/e27468e73aa6a31) Sebastian Bazley *2013-04-24 18:16:38*

            **Unnecessary ;**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1471572 13f79535-47bb-0310-9956-ffa450edef68

            [7c129b2715b5a84](https://github.com/ghacupha/commons-chain/commit/7c129b2715b5a84) Sebastian Bazley *2013-04-24 18:12:28*

            **Add some missing method @Override markers**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1471571 13f79535-47bb-0310-9956-ffa450edef68

            [017e76dbf80b933](https://github.com/ghacupha/commons-chain/commit/017e76dbf80b933) Sebastian Bazley *2013-04-24 18:10:34*

            **Private immutable fields might as well be final (helps with thread-safety)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1471558 13f79535-47bb-0310-9956-ffa450edef68

            [a0c275333167aef](https://github.com/ghacupha/commons-chain/commit/a0c275333167aef) Sebastian Bazley *2013-04-24 17:40:22*

            **Fix up URLs so they point to actual sites; this allows relative URLs to work properly**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1459912 13f79535-47bb-0310-9956-ffa450edef68

            [28f63a9ce77787f](https://github.com/ghacupha/commons-chain/commit/28f63a9ce77787f) Sebastian Bazley *2013-03-22 17:49:27*

            **trivial: updated ignore list**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1457298 13f79535-47bb-0310-9956-ffa450edef68

            [429e922068cdb42](https://github.com/ghacupha/commons-chain/commit/429e922068cdb42) Simone Tripodi *2013-03-16 19:59:59*

            **restore download cgi**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1450539 13f79535-47bb-0310-9956-ffa450edef68

            [d3ba0f394a988af](https://github.com/ghacupha/commons-chain/commit/d3ba0f394a988af) Olivier Lamy *2013-02-26 23:53:27*

            **developed by => developed at**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1440692 13f79535-47bb-0310-9956-ffa450edef68

            [39cb491fb4d7bb1](https://github.com/ghacupha/commons-chain/commit/39cb491fb4d7bb1) Sebastian Bazley *2013-01-30 21:43:00*

            **configure svnpubsub**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1434465 13f79535-47bb-0310-9956-ffa450edef68

            [f099c3fcac458c8](https://github.com/ghacupha/commons-chain/commit/f099c3fcac458c8) Olivier Lamy *2013-01-16 22:53:18*

            **both Filter/Chain extend Command interface - no need to overload the add() method - as shown in the Chain interface where Filter is not explicitly specified**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1376910 13f79535-47bb-0310-9956-ffa450edef68

            [d53a90edc58bd82](https://github.com/ghacupha/commons-chain/commit/d53a90edc58bd82) Simone Tripodi *2012-08-24 13:39:40*

            **just for a matter of completeness, Catalog explicitly allows adding Chain(s)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1372433 13f79535-47bb-0310-9956-ffa450edef68

            [013f4d0a5417e71](https://github.com/ghacupha/commons-chain/commit/013f4d0a5417e71) Simone Tripodi *2012-08-13 14:14:47*

            **Chains method to add commands made less verbose**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1372429 13f79535-47bb-0310-9956-ffa450edef68

            [92daea3937273e5](https://github.com/ghacupha/commons-chain/commit/92daea3937273e5) Simone Tripodi *2012-08-13 14:06:54*

            **typo**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1371261 13f79535-47bb-0310-9956-ffa450edef68

            [586c47ef2bee0f5](https://github.com/ghacupha/commons-chain/commit/586c47ef2bee0f5) Simone Tripodi *2012-08-09 15:43:29*

            **added fluent methods to setup Filter instances as well in both Chain/Catalog**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1371240 13f79535-47bb-0310-9956-ffa450edef68

            [256ca8e0fddf4cb](https://github.com/ghacupha/commons-chain/commit/256ca8e0fddf4cb) Simone Tripodi *2012-08-09 14:54:16*

            **just fixed raw types**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1370303 13f79535-47bb-0310-9956-ffa450edef68

            [145b7b92a8b0d32](https://github.com/ghacupha/commons-chain/commit/145b7b92a8b0d32) Simone Tripodi *2012-08-07 15:07:23*

            **just fixed raw types**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1370302 13f79535-47bb-0310-9956-ffa450edef68

            [536115a4fb8eaea](https://github.com/ghacupha/commons-chain/commit/536115a4fb8eaea) Simone Tripodi *2012-08-07 15:06:10*

            **community explicitly expressed the preference to upgrade supported JDK to 1.6**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1369902 13f79535-47bb-0310-9956-ffa450edef68

            [6f1232fa271320f](https://github.com/ghacupha/commons-chain/commit/6f1232fa271320f) Simone Tripodi *2012-08-06 18:10:22*

            **XML format**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1369826 13f79535-47bb-0310-9956-ffa450edef68

            [df65a6399dd3a80](https://github.com/ghacupha/commons-chain/commit/df65a6399dd3a80) Simone Tripodi *2012-08-06 13:03:35*

            **XML format, no functional modifications**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1366634 13f79535-47bb-0310-9956-ffa450edef68

            [fb2dce04ad40be9](https://github.com/ghacupha/commons-chain/commit/fb2dce04ad40be9) Simone Tripodi *2012-07-28 09:54:02*

            **updated ignore list**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1366633 13f79535-47bb-0310-9956-ffa450edef68

            [0ea73d2d8f9dd7a](https://github.com/ghacupha/commons-chain/commit/0ea73d2d8f9dd7a) Simone Tripodi *2012-07-28 09:52:44*

            **as dscusses to dev@, configuration stuff have been moved to a proper subdirectory**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1366630 13f79535-47bb-0310-9956-ffa450edef68

            [aaa20af3ac4c98a](https://github.com/ghacupha/commons-chain/commit/aaa20af3ac4c98a) Simone Tripodi *2012-07-28 09:49:45*

            **reordered actions based on @issue DESC**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1366629 13f79535-47bb-0310-9956-ffa450edef68

            [0fe1e6447572807](https://github.com/ghacupha/commons-chain/commit/0fe1e6447572807) Simone Tripodi *2012-07-28 09:37:33*

            **XML format, no functional modifications**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1366628 13f79535-47bb-0310-9956-ffa450edef68

            [39171261eee977d](https://github.com/ghacupha/commons-chain/commit/39171261eee977d) Simone Tripodi *2012-07-28 09:36:14*

            **@issue attribute first in each action to make easier keeping the actions sorted desc**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1366627 13f79535-47bb-0310-9956-ffa450edef68

            [68ce360f8a53423](https://github.com/ghacupha/commons-chain/commit/68ce360f8a53423) Simone Tripodi *2012-07-28 09:34:57*

            **Fixed build break caused by overriding jdk 1.7 constructor in RuntimeException.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1366598 13f79535-47bb-0310-9956-ffa450edef68

            [7f56c908f5ccbfd](https://github.com/ghacupha/commons-chain/commit/7f56c908f5ccbfd) Elijah Zupancic *2012-07-28 05:17:24*

            **suppressed "Plugin execution not covered by lifecycle configuration" in eclipse**

                * no side effects to the rest of the build
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363678 13f79535-47bb-0310-9956-ffa450edef68

            [aeda85edbc3768b](https://github.com/ghacupha/commons-chain/commit/aeda85edbc3768b) Simone Tripodi *2012-07-20 08:31:31*

            **just removed empty lines, no functional modifications**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363305 13f79535-47bb-0310-9956-ffa450edef68

            [a5bc2978c2e3c83](https://github.com/ghacupha/commons-chain/commit/a5bc2978c2e3c83) Simone Tripodi *2012-07-19 11:42:53*

            **dropped @author tags; committers and contributors moved to related sections in pom.xml**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363288 13f79535-47bb-0310-9956-ffa450edef68

            [4466d400e52538f](https://github.com/ghacupha/commons-chain/commit/4466d400e52538f) Simone Tripodi *2012-07-19 10:40:56*

            **unified @version javadoc tag to Id only - some used Id, some Revision and Date, some other did not set it at all**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363278 13f79535-47bb-0310-9956-ffa450edef68

            [ce80a379bfc00f4](https://github.com/ghacupha/commons-chain/commit/ce80a379bfc00f4) Simone Tripodi *2012-07-19 10:22:52*

            **updated release notes according to resolved issues on JIRA**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363267 13f79535-47bb-0310-9956-ffa450edef68

            [3e53010765de083](https://github.com/ghacupha/commons-chain/commit/3e53010765de083) Simone Tripodi *2012-07-19 09:03:23*

            **javadoc typo**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363256 13f79535-47bb-0310-9956-ffa450edef68

            [43ad1b5ca83cbf2](https://github.com/ghacupha/commons-chain/commit/43ad1b5ca83cbf2) Simone Tripodi *2012-07-19 08:12:16*

            **removed unneeded 'else' branches**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363116 13f79535-47bb-0310-9956-ffa450edef68

            [4a51874e95cc903](https://github.com/ghacupha/commons-chain/commit/4a51874e95cc903) Simone Tripodi *2012-07-18 21:05:45*

            **removed unneeded 'else' branch**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363114 13f79535-47bb-0310-9956-ffa450edef68

            [060d9e4d728f92e](https://github.com/ghacupha/commons-chain/commit/060d9e4d728f92e) Simone Tripodi *2012-07-18 21:02:01*

            **took advantage from StringBuilder chaining methods**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363113 13f79535-47bb-0310-9956-ffa450edef68

            [185ddc078485ab0](https://github.com/ghacupha/commons-chain/commit/185ddc078485ab0) Simone Tripodi *2012-07-18 21:00:39*

            **StringBuffer replaced by StringBuilder**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363112 13f79535-47bb-0310-9956-ffa450edef68

            [35bff675579a964](https://github.com/ghacupha/commons-chain/commit/35bff675579a964) Simone Tripodi *2012-07-18 20:59:36*

            **no reason to concatenate strings when using a StringBuffer**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363111 13f79535-47bb-0310-9956-ffa450edef68

            [940e7a4bd893746](https://github.com/ghacupha/commons-chain/commit/940e7a4bd893746) Simone Tripodi *2012-07-18 20:58:40*

            **code format, no functional modifications**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363109 13f79535-47bb-0310-9956-ffa450edef68

            [a8b33ffef0665a2](https://github.com/ghacupha/commons-chain/commit/a8b33ffef0665a2) Simone Tripodi *2012-07-18 20:56:01*

            **removed unneeded 'else' branches**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363104 13f79535-47bb-0310-9956-ffa450edef68

            [069c422f60c4941](https://github.com/ghacupha/commons-chain/commit/069c422f60c4941) Simone Tripodi *2012-07-18 20:48:01*

            **removed unneeded 'else' branch**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363103 13f79535-47bb-0310-9956-ffa450edef68

            [53db5fc0268246a](https://github.com/ghacupha/commons-chain/commit/53db5fc0268246a) Simone Tripodi *2012-07-18 20:44:39*

            **code format, no functional modifications**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363102 13f79535-47bb-0310-9956-ffa450edef68

            [12f8158c6d4e38e](https://github.com/ghacupha/commons-chain/commit/12f8158c6d4e38e) Simone Tripodi *2012-07-18 20:43:46*

            **just dropped empty lines, no functional modifications**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363100 13f79535-47bb-0310-9956-ffa450edef68

            [b7b12630fe4d9ff](https://github.com/ghacupha/commons-chain/commit/b7b12630fe4d9ff) Simone Tripodi *2012-07-18 20:31:57*

            **added aux modules links to APIs docs**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1363072 13f79535-47bb-0310-9956-ffa450edef68

            [9696590cafeb852](https://github.com/ghacupha/commons-chain/commit/9696590cafeb852) Simone Tripodi *2012-07-18 19:51:06*

            **XML format, no functional modifications**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362998 13f79535-47bb-0310-9956-ffa450edef68

            [da27a2f0b2cdd0f](https://github.com/ghacupha/commons-chain/commit/da27a2f0b2cdd0f) Simone Tripodi *2012-07-18 16:15:16*

            **added a page to describe chains2 modules**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362995 13f79535-47bb-0310-9956-ffa450edef68

            [c11b8125414ebae](https://github.com/ghacupha/commons-chain/commit/c11b8125414ebae) Simone Tripodi *2012-07-18 16:06:25*

            **skip samples deploy via mvn expression rather than plugin declaration**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362955 13f79535-47bb-0310-9956-ffa450edef68

            [b7f964824ab8f58](https://github.com/ghacupha/commons-chain/commit/b7f964824ab8f58) Simone Tripodi *2012-07-18 13:54:50*

            **added missing past releases in the DOAP descriptor**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362953 13f79535-47bb-0310-9956-ffa450edef68

            [f65c5e5f685ec6a](https://github.com/ghacupha/commons-chain/commit/f65c5e5f685ec6a) Simone Tripodi *2012-07-18 13:51:45*

            **upgraded parent pom reference**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362939 13f79535-47bb-0310-9956-ffa450edef68

            [9f36028e642db84](https://github.com/ghacupha/commons-chain/commit/9f36028e642db84) Simone Tripodi *2012-07-18 13:22:33*

            **include bin dependencies to -bin packages (mainly ASF commons components, with deps) and special L&N to cover digester transitive dependencies license**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362934 13f79535-47bb-0310-9956-ffa450edef68

            [35ec49815234e81](https://github.com/ghacupha/commons-chain/commit/35ec49815234e81) Simone Tripodi *2012-07-18 13:18:11*

            **don't tweak assembly names when deploying them - mvn will rename them!**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362926 13f79535-47bb-0310-9956-ffa450edef68

            [8fc182a4a78935b](https://github.com/ghacupha/commons-chain/commit/8fc182a4a78935b) Simone Tripodi *2012-07-18 13:03:05*

            **renamed core module artifactId adding the -core postfix**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362911 13f79535-47bb-0310-9956-ffa450edef68

            [0313bfe8c0f97f7](https://github.com/ghacupha/commons-chain/commit/0313bfe8c0f97f7) Simone Tripodi *2012-07-18 12:36:17*

            **XML format, no functional modifications**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362905 13f79535-47bb-0310-9956-ffa450edef68

            [b89254aff8dae40](https://github.com/ghacupha/commons-chain/commit/b89254aff8dae40) Simone Tripodi *2012-07-18 12:17:32*

            **Elijah moved to committers list**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362904 13f79535-47bb-0310-9956-ffa450edef68

            [9d1e1aa9b1824cc](https://github.com/ghacupha/commons-chain/commit/9d1e1aa9b1824cc) Simone Tripodi *2012-07-18 12:15:41*

            **trailing spaces on empty line**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362883 13f79535-47bb-0310-9956-ffa450edef68

            [0c212328310f947](https://github.com/ghacupha/commons-chain/commit/0c212328310f947) Simone Tripodi *2012-07-18 11:14:22*

            **skip site deploying for sample applications**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362882 13f79535-47bb-0310-9956-ffa450edef68

            [b45503aa0c6dda5](https://github.com/ghacupha/commons-chain/commit/b45503aa0c6dda5) Simone Tripodi *2012-07-18 11:13:04*

            **added RC profile for site deploying**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362881 13f79535-47bb-0310-9956-ffa450edef68

            [8634b5d97c9ed16](https://github.com/ghacupha/commons-chain/commit/8634b5d97c9ed16) Simone Tripodi *2012-07-18 11:11:28*

            **aggregate javadoc when generating the site**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362879 13f79535-47bb-0310-9956-ffa450edef68

            [eab865f64ea5f14](https://github.com/ghacupha/commons-chain/commit/eab865f64ea5f14) Simone Tripodi *2012-07-18 11:02:29*

            **added changes document xsd (it helps auto-complete in IDEs)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362878 13f79535-47bb-0310-9956-ffa450edef68

            [9814ba72da3e42e](https://github.com/ghacupha/commons-chain/commit/9814ba72da3e42e) Simone Tripodi *2012-07-18 11:00:27*

            **XML format, no functional modifications**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362872 13f79535-47bb-0310-9956-ffa450edef68

            [8b06e43eb2bef03](https://github.com/ghacupha/commons-chain/commit/8b06e43eb2bef03) Simone Tripodi *2012-07-18 10:55:54*

            **removed empty useless profile**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362868 13f79535-47bb-0310-9956-ffa450edef68

            [3fc077a4948de9e](https://github.com/ghacupha/commons-chain/commit/3fc077a4948de9e) Simone Tripodi *2012-07-18 10:53:59*

            **don't skip chain2 assemblies deploy**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362863 13f79535-47bb-0310-9956-ffa450edef68

            [438193114a83c99](https://github.com/ghacupha/commons-chain/commit/438193114a83c99) Simone Tripodi *2012-07-18 10:45:59*

            **XML format, no functional modifications**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362861 13f79535-47bb-0310-9956-ffa450edef68

            [bdfe1d2549011e6](https://github.com/ghacupha/commons-chain/commit/bdfe1d2549011e6) Simone Tripodi *2012-07-18 10:43:00*

            **XML format, no functional modifications**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362860 13f79535-47bb-0310-9956-ffa450edef68

            [6ad0f6faf6a0cce](https://github.com/ghacupha/commons-chain/commit/6ad0f6faf6a0cce) Simone Tripodi *2012-07-18 10:39:00*

            **XML format, no functional configuration**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362857 13f79535-47bb-0310-9956-ffa450edef68

            [c6ce814a74b53af](https://github.com/ghacupha/commons-chain/commit/c6ce814a74b53af) Simone Tripodi *2012-07-18 10:36:56*

            **fixed servlet elements order according to web-app XSD**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362856 13f79535-47bb-0310-9956-ffa450edef68

            [3a789b3ba912c7c](https://github.com/ghacupha/commons-chain/commit/3a789b3ba912c7c) Simone Tripodi *2012-07-18 10:35:15*

            **XML format, no functional configuration**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362854 13f79535-47bb-0310-9956-ffa450edef68

            [9573f8051545aa8](https://github.com/ghacupha/commons-chain/commit/9573f8051545aa8) Simone Tripodi *2012-07-18 10:31:52*

            **fixed resource location in classpath**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362849 13f79535-47bb-0310-9956-ffa450edef68

            [2b35fb4e8182d16](https://github.com/ghacupha/commons-chain/commit/2b35fb4e8182d16) Simone Tripodi *2012-07-18 10:26:36*

            **XML format, no functional configuration**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362848 13f79535-47bb-0310-9956-ffa450edef68

            [b08cb749cb26c53](https://github.com/ghacupha/commons-chain/commit/b08cb749cb26c53) Simone Tripodi *2012-07-18 10:26:02*

            **added missing license header**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362846 13f79535-47bb-0310-9956-ffa450edef68

            [dda3c98231d36a4](https://github.com/ghacupha/commons-chain/commit/dda3c98231d36a4) Simone Tripodi *2012-07-18 10:25:01*

            **dropped old empty directories**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362845 13f79535-47bb-0310-9956-ffa450edef68

            [1725cf5bb5daa45](https://github.com/ghacupha/commons-chain/commit/1725cf5bb5daa45) Simone Tripodi *2012-07-18 10:24:10*

            **updated ignore list**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1362843 13f79535-47bb-0310-9956-ffa450edef68

            [5ccafb52aaf6d9c](https://github.com/ghacupha/commons-chain/commit/5ccafb52aaf6d9c) Simone Tripodi *2012-07-18 10:18:44*

            **update ignore list**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1328099 13f79535-47bb-0310-9956-ffa450edef68

            [afec8cdcf02eb23](https://github.com/ghacupha/commons-chain/commit/afec8cdcf02eb23) Simone Tripodi *2012-04-19 20:07:28*

            **reorganized pom stuff as suggested on http://maven.apache.org/developers/conventions/code.html - NO FUNCTIONAL CHANGES**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1300058 13f79535-47bb-0310-9956-ffa450edef68

            [163ca974f0d6278](https://github.com/ghacupha/commons-chain/commit/163ca974f0d6278) Simone Tripodi *2012-03-13 10:22:59*

            **parent upgrated to version 24**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1300035 13f79535-47bb-0310-9956-ffa450edef68

            [b0a4c1dda5c4e39](https://github.com/ghacupha/commons-chain/commit/b0a4c1dda5c4e39) Simone Tripodi *2012-03-13 09:47:16*

            **reused surefire settings provided by the parent**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1297893 13f79535-47bb-0310-9956-ffa450edef68

            [8c4d0dd9ab3c5f5](https://github.com/ghacupha/commons-chain/commit/8c4d0dd9ab3c5f5) Simone Tripodi *2012-03-07 08:58:20*

            **explicit use of the surefire-report plugin to aggregate test results**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1297393 13f79535-47bb-0310-9956-ffa450edef68

            [184b9a3330da3ae](https://github.com/ghacupha/commons-chain/commit/184b9a3330da3ae) Simone Tripodi *2012-03-06 09:15:10*

            **updated dependencies description**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295960 13f79535-47bb-0310-9956-ffa450edef68

            [2eedb154df19439](https://github.com/ghacupha/commons-chain/commit/2eedb154df19439) Simone Tripodi *2012-03-01 22:50:59*

            **that lazy loading initialization is not thread safe**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295951 13f79535-47bb-0310-9956-ffa450edef68

            [06919691aca2b31](https://github.com/ghacupha/commons-chain/commit/06919691aca2b31) Simone Tripodi *2012-03-01 22:28:43*

            **reuse of the same Digester instance is discouraged, since it is not thread safe**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295947 13f79535-47bb-0310-9956-ffa450edef68

            [40f0ae2433637c6](https://github.com/ghacupha/commons-chain/commit/40f0ae2433637c6) Simone Tripodi *2012-03-01 22:25:42*

            **started migrating the configuration module to use Digester3**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295941 13f79535-47bb-0310-9956-ffa450edef68

            [59daf2d36c54a7a](https://github.com/ghacupha/commons-chain/commit/59daf2d36c54a7a) Simone Tripodi *2012-03-01 22:15:05*

            **managed commons-logging dependency, it prevents:**

                * be added as a dependency in the configuration module (not needed ad compile time, already managed by digester as transitive dependency)
                * be imported in the distribution package
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295922 13f79535-47bb-0310-9956-ffa450edef68

            [425192e485ec2eb](https://github.com/ghacupha/commons-chain/commit/425192e485ec2eb) Simone Tripodi *2012-03-01 21:48:10*

            **started updating next release notes**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295506 13f79535-47bb-0310-9956-ffa450edef68

            [a2a4b68a19c9773](https://github.com/ghacupha/commons-chain/commit/a2a4b68a19c9773) Simone Tripodi *2012-03-01 10:50:47*

            **dropped checkstyle resources, they were copied in the proper build-tools module**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295182 13f79535-47bb-0310-9956-ffa450edef68

            [01611ed60b790dd](https://github.com/ghacupha/commons-chain/commit/01611ed60b790dd) Simone Tripodi *2012-02-29 16:28:06*

            **removed old sources dir, now working only on modules**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295181 13f79535-47bb-0310-9956-ffa450edef68

            [44ef6d7eb952f74](https://github.com/ghacupha/commons-chain/commit/44ef6d7eb952f74) Simone Tripodi *2012-02-29 16:26:58*

            **added a module that contains configurations of quality metricts tools, such as checkstyle, pmd, etc...**

                * that will simplify sharing the same checkstyle config across multiple modules
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295137 13f79535-47bb-0310-9956-ffa450edef68

            [b58c7976fa655fb](https://github.com/ghacupha/commons-chain/commit/b58c7976fa655fb) Simone Tripodi *2012-02-29 14:45:10*

            **just format NO FUNCTIONAL CHANGES**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295046 13f79535-47bb-0310-9956-ffa450edef68

            [cffe6387f875cb6](https://github.com/ghacupha/commons-chain/commit/cffe6387f875cb6) Simone Tripodi *2012-02-29 09:53:26*

            **added assembly XSD references**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295043 13f79535-47bb-0310-9956-ffa450edef68

            [e442e0e86d9e9f3](https://github.com/ghacupha/commons-chain/commit/e442e0e86d9e9f3) Simone Tripodi *2012-02-29 09:52:22*

            **updated ignore list**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295041 13f79535-47bb-0310-9956-ffa450edef68

            [2b27b7c960f707d](https://github.com/ghacupha/commons-chain/commit/2b27b7c960f707d) Simone Tripodi *2012-02-29 09:49:40*

            **typo, side effect of the copy'n'paste**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1295031 13f79535-47bb-0310-9956-ffa450edef68

            [ee21e205f6a2ca4](https://github.com/ghacupha/commons-chain/commit/ee21e205f6a2ca4) Simone Tripodi *2012-02-29 09:27:52*

            **added site XSD descriptor**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1294543 13f79535-47bb-0310-9956-ffa450edef68

            [1a7e0eaf6b42001](https://github.com/ghacupha/commons-chain/commit/1a7e0eaf6b42001) Simone Tripodi *2012-02-28 10:09:37*

            **updated findbugs-maven-plugin to latest released version**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1294211 13f79535-47bb-0310-9956-ffa450edef68

            [2e3e28ba9aa9ae3](https://github.com/ghacupha/commons-chain/commit/2e3e28ba9aa9ae3) Simone Tripodi *2012-02-27 16:47:15*

            **updated maven-javadoc-plugin**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1294210 13f79535-47bb-0310-9956-ffa450edef68

            [91495a96bbd1294](https://github.com/ghacupha/commons-chain/commit/91495a96bbd1294) Simone Tripodi *2012-02-27 16:46:24*

            **updated checkstyle plugin**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1294208 13f79535-47bb-0310-9956-ffa450edef68

            [6ae938d4f9da7d7](https://github.com/ghacupha/commons-chain/commit/6ae938d4f9da7d7) Simone Tripodi *2012-02-27 16:44:57*

            **dropped build plugins inherited from parent**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1294206 13f79535-47bb-0310-9956-ffa450edef68

            [8040041db389073](https://github.com/ghacupha/commons-chain/commit/8040041db389073) Simone Tripodi *2012-02-27 16:43:13*

            **dropped unused beanutils compile dependency, the digester brings its own to process the XML config**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1294205 13f79535-47bb-0310-9956-ffa450edef68

            [84d233d4e924c8c](https://github.com/ghacupha/commons-chain/commit/84d233d4e924c8c) Simone Tripodi *2012-02-27 16:39:55*

            **junit updated to latest recent version**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1294204 13f79535-47bb-0310-9956-ffa450edef68

            [3a746d6c23f5400](https://github.com/ghacupha/commons-chain/commit/3a746d6c23f5400) Simone Tripodi *2012-02-27 16:34:19*

            **parent updated to latest release version**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1294202 13f79535-47bb-0310-9956-ffa450edef68

            [1826370b4f70cd3](https://github.com/ghacupha/commons-chain/commit/1826370b4f70cd3) Simone Tripodi *2012-02-27 16:32:32*

            **updated copyright year**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1293701 13f79535-47bb-0310-9956-ffa450edef68

            [4411b9eb595c835](https://github.com/ghacupha/commons-chain/commit/4411b9eb595c835) Simone Tripodi *2012-02-25 22:08:43*

            **added myself in the committers list**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1293699 13f79535-47bb-0310-9956-ffa450edef68

            [898f55312115a78](https://github.com/ghacupha/commons-chain/commit/898f55312115a78) Simone Tripodi *2012-02-25 22:04:16*

            **typo**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1243828 13f79535-47bb-0310-9956-ffa450edef68

            [87e9fa6c75dc13f](https://github.com/ghacupha/commons-chain/commit/87e9fa6c75dc13f) Simone Tripodi *2012-02-14 08:46:51*

            **moved 2.0 contributors to "due-to" attribute**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1242923 13f79535-47bb-0310-9956-ffa450edef68

            [26a36dc08a224ca](https://github.com/ghacupha/commons-chain/commit/26a36dc08a224ca) Simone Tripodi *2012-02-10 21:09:49*

            **4 spaces replaced with 2 spaces, as generally adopted in commons**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1173821 13f79535-47bb-0310-9956-ffa450edef68

            [93457f9952b3d43](https://github.com/ghacupha/commons-chain/commit/93457f9952b3d43) Simone Tripodi *2011-09-21 20:05:35*

            **added missing release metadata**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1173819 13f79535-47bb-0310-9956-ffa450edef68

            [d30e0f61aa60317](https://github.com/ghacupha/commons-chain/commit/d30e0f61aa60317) Simone Tripodi *2011-09-21 20:03:47*

            **parent reference updated to version 22**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1173818 13f79535-47bb-0310-9956-ffa450edef68

            [c0f47f6a689018f](https://github.com/ghacupha/commons-chain/commit/c0f47f6a689018f) Simone Tripodi *2011-09-21 20:02:11*

            **use compiler properties instead of fixed values**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1172660 13f79535-47bb-0310-9956-ffa450edef68

            [cc56d6f992658a1](https://github.com/ghacupha/commons-chain/commit/cc56d6f992658a1) Simone Tripodi *2011-09-19 15:29:58*

            **upgrated findbugs plugin**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1171791 13f79535-47bb-0310-9956-ffa450edef68

            [798f9c8b720f049](https://github.com/ghacupha/commons-chain/commit/798f9c8b720f049) Simone Tripodi *2011-09-16 21:21:34*

            **assertion methods imported from org.junit.Assert instead of junit.framework.Assert**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1170853 13f79535-47bb-0310-9956-ffa450edef68

            [4f099063ed9ffc2](https://github.com/ghacupha/commons-chain/commit/4f099063ed9ffc2) Simone Tripodi *2011-09-14 21:27:04*

            **simplified parametrized tests executions via JUnit's Parameterized feature**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1170851 13f79535-47bb-0310-9956-ffa450edef68

            [7dac6c054ddb579](https://github.com/ghacupha/commons-chain/commit/7dac6c054ddb579) Simone Tripodi *2011-09-14 21:23:34*

            **Remove Java 1.5 profile.**

                * It was originally a profile to support Java 1.3, but 1.3 was accidentally changed to 1.5 in r1162332, as part of the move to Java 1.5 (global edit error).
                * There&#39;s no need to revert profile to 1.3 as we don&#39;t support that Java version any more, so just rm.
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1170368 13f79535-47bb-0310-9956-ffa450edef68

            [8cd20e0feecf3a5](https://github.com/ghacupha/commons-chain/commit/8cd20e0feecf3a5) Sebastian Bazley *2011-09-13 22:23:06*

            **ConcurrentHashMap#put(K, V) method doesn't allow neither the key nor the value be null, managed null values for retro-compatibility (old users would be maybe used to set null values)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1170340 13f79535-47bb-0310-9956-ffa450edef68

            [f6136e6fd95db5b](https://github.com/ghacupha/commons-chain/commit/f6136e6fd95db5b) Simone Tripodi *2011-09-13 20:42:09*

            **moving the 2.0-work branch in trunk as voted on http://markmail.org/message/rw6ymp65bmr75fur**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1166862 13f79535-47bb-0310-9956-ffa450edef68

            [ffa77b106f670b6](https://github.com/ghacupha/commons-chain/commit/ffa77b106f670b6) Simone Tripodi *2011-09-08 19:06:19*

            **Fix Oracle Javadoc site references (was Sun.)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1095934 13f79535-47bb-0310-9956-ffa450edef68

            [eddcfe2d8475b27](https://github.com/ghacupha/commons-chain/commit/eddcfe2d8475b27) Gary D. Gregory *2011-04-22 13:46:56*

            **Remove my @author tags**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1088801 13f79535-47bb-0310-9956-ffa450edef68

            [a5d157b5da4ac48](https://github.com/ghacupha/commons-chain/commit/a5d157b5da4ac48) Niall Pemberton *2011-04-04 22:06:02*

            **Ignore Eclipse files.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1087166 13f79535-47bb-0310-9956-ffa450edef68

            [4d731e2bc0b5227](https://github.com/ghacupha/commons-chain/commit/4d731e2bc0b5227) Gary D. Gregory *2011-03-31 03:24:58*

            **Add cobertura-maven-plugin and upgrade findbugs-maven-plugin from 1.2 to 2.3.1**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1005280 13f79535-47bb-0310-9956-ffa450edef68

            [ed4286dbfc3e6da](https://github.com/ghacupha/commons-chain/commit/ed4286dbfc3e6da) Niall Pemberton *2010-10-06 22:31:23*

            **Upgrade maven-changes-plugin from version 2.0 to 2.3**

                * Version 2.3 doesn&#39;t like the &lt;dueto name=&quot;...&quot;/&gt; element for multiple attributions so move them to &lt;action due-to=&quot;...&quot;&gt; element as a comma separated list
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1005274 13f79535-47bb-0310-9956-ffa450edef68

            [d3819dbe8728991](https://github.com/ghacupha/commons-chain/commit/d3819dbe8728991) Niall Pemberton *2010-10-06 22:16:23*

            **Upgrade maven-checkstyle-plugin from version 2.1 to 2.6**

                * maven-checkstyle-plugin 2.4 onwards uses Checkstyle 5.0 (upgraded from Checkstyle 4.4).
                * Checkstyle 5.0 is not 100% backwardly compatible with release 4.4 and the following changes need to be made to make it work:
                * Replace &quot;PackageHtml&quot; with &quot;JavadocPackage&quot; and configure the &quot;allowLegacy&quot; parameter so that it checks for package.html files (rather than package-info.java)
                * Move &quot;Header&quot; out of &quot;TreeWalker&quot;(not allowed)
                * Move &quot;FileLength&quot; out of &quot;TreeWalker&quot;(not allowed)
                * Replace &quot;TabCharacter&quot; (java files) with &quot;FileTabCharacter&quot;, move it out of &quot;TreeWalker&quot; and configure the &quot;fileExtensions&quot; parameter
                * Replace &quot;GenericIllegalRegexp&quot; (for trailing spaces check) with &quot;RegexpSingleline&quot;, move it out of &quot;TreeWalker&quot;
                * See the Release Notes for incompatible changes and fixes here:
                * http://checkstyle.sourceforge.net/releasenotes.html
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@1005273 13f79535-47bb-0310-9956-ffa450edef68

            [a9a9e6423222e6e](https://github.com/ghacupha/commons-chain/commit/a9a9e6423222e6e) Niall Pemberton *2010-10-06 22:06:08*

            **Fix default target**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@997308 13f79535-47bb-0310-9956-ffa450edef68

            [f269ad0fb2b8caa](https://github.com/ghacupha/commons-chain/commit/f269ad0fb2b8caa) Niall Pemberton *2010-09-15 12:25:52*

            **Upgrade to commons-parent version 15**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@936207 13f79535-47bb-0310-9956-ffa450edef68

            [03fdd0e20965cf4](https://github.com/ghacupha/commons-chain/commit/03fdd0e20965cf4) Niall Pemberton *2010-04-21 09:02:56*

            **Replace m1 generated ant build with hand writtern one**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@932482 13f79535-47bb-0310-9956-ffa450edef68

            [9ace55383e00fff](https://github.com/ghacupha/commons-chain/commit/9ace55383e00fff) Niall Pemberton *2010-04-09 16:10:30*

            **consistency**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@932396 13f79535-47bb-0310-9956-ffa450edef68

            [5b590cd8109612f](https://github.com/ghacupha/commons-chain/commit/5b590cd8109612f) Niall Pemberton *2010-04-09 12:57:49*

            **Re-generate chanin mailing list page**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@932062 13f79535-47bb-0310-9956-ffa450edef68

            [5f0ddce5814617a](https://github.com/ghacupha/commons-chain/commit/5f0ddce5814617a) Niall Pemberton *2010-04-08 18:54:25*

            **Update building instructions**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@932045 13f79535-47bb-0310-9956-ffa450edef68

            [8eee5bef96151a8](https://github.com/ghacupha/commons-chain/commit/8eee5bef96151a8) Niall Pemberton *2010-04-08 18:15:58*

            **Move changes.xml to default m2 location**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@932044 13f79535-47bb-0310-9956-ffa450edef68

            [23a5ce097c3bdb0](https://github.com/ghacupha/commons-chain/commit/23a5ce097c3bdb0) Niall Pemberton *2010-04-08 18:15:28*

            **Oops, revert accidental change**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@932033 13f79535-47bb-0310-9956-ffa450edef68

            [5c4e99217acf028](https://github.com/ghacupha/commons-chain/commit/5c4e99217acf028) Niall Pemberton *2010-04-08 18:00:03*

            **Re-organize to standard m2 layout**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@932029 13f79535-47bb-0310-9956-ffa450edef68

            [36bf4488c03bfa8](https://github.com/ghacupha/commons-chain/commit/36bf4488c03bfa8) Niall Pemberton *2010-04-08 17:53:07*

            **Add custom mailing list page generated by commons-build-plugin**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@931912 13f79535-47bb-0310-9956-ffa450edef68

            [5ebc1ff604db74b](https://github.com/ghacupha/commons-chain/commit/5ebc1ff604db74b) Niall Pemberton *2010-04-08 12:36:19*

            **Fix up jakarta download references**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@929316 13f79535-47bb-0310-9956-ffa450edef68

            [62207928cda5ca8](https://github.com/ghacupha/commons-chain/commit/62207928cda5ca8) Sebastian Bazley *2010-03-30 21:50:28*

            **Remove m1 cvs-usage.xml & navigation.xml files**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@928537 13f79535-47bb-0310-9956-ffa450edef68

            [77ec2b8472535b0](https://github.com/ghacupha/commons-chain/commit/77ec2b8472535b0) Niall Pemberton *2010-03-28 23:58:39*

            **Removing M1 build, M2 build seems fine**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@928525 13f79535-47bb-0310-9956-ffa450edef68

            [3a013f017ac32ad](https://github.com/ghacupha/commons-chain/commit/3a013f017ac32ad) Henri Yandell *2010-03-28 23:40:21*

            **Update components to point to the new download pages**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@923339 13f79535-47bb-0310-9956-ffa450edef68

            [7bec2df91714679](https://github.com/ghacupha/commons-chain/commit/7bec2df91714679) Niall Pemberton *2010-03-15 17:04:53*

            **Re-generate the download pages using the new commons-build-plugin .12 (via commons-parent version 13)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@920156 13f79535-47bb-0310-9956-ffa450edef68

            [a61b2f354f2053b](https://github.com/ghacupha/commons-chain/commit/a61b2f354f2053b) Niall Pemberton *2010-03-08 00:11:50*

            **Upgrade to version 13 of commons-parent**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@920154 13f79535-47bb-0310-9956-ffa450edef68

            [0f27d036c3cf071](https://github.com/ghacupha/commons-chain/commit/0f27d036c3cf071) Niall Pemberton *2010-03-08 00:05:47*

            **Update to the latest BeanUtils 1.8.2 release**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@835643 13f79535-47bb-0310-9956-ffa450edef68

            [8a56e9f644c925e](https://github.com/ghacupha/commons-chain/commit/8a56e9f644c925e) Niall Pemberton *2009-11-12 23:41:18*

            **Fix remaining doap files in commons-proper**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@779652 13f79535-47bb-0310-9956-ffa450edef68

            [1009b575fe1a917](https://github.com/ghacupha/commons-chain/commit/1009b575fe1a917) Sebastian Bazley *2009-05-28 16:39:02*

            **Upgrade to latest clirr plugin version 2.2.2 (fixes problem downloading the old artifact from the repo)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@687301 13f79535-47bb-0310-9956-ffa450edef68

            [54a8cb90ee80c13](https://github.com/ghacupha/commons-chain/commit/54a8cb90ee80c13) Niall Pemberton *2008-08-20 12:56:25*

            **change commons-parent to version 11**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@678495 13f79535-47bb-0310-9956-ffa450edef68

            [2a8f46a7ddcb237](https://github.com/ghacupha/commons-chain/commit/2a8f46a7ddcb237) Niall Pemberton *2008-07-21 17:43:58*

            **Roll version to 1.3-SNAPSHOT following Chain 1.2 release**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@662266 13f79535-47bb-0310-9956-ffa450edef68

            [8b41b4ac8537c54](https://github.com/ghacupha/commons-chain/commit/8b41b4ac8537c54) Niall Pemberton *2008-06-01 18:51:57*

            **Set release date, if RC3 succeeds**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@661365 13f79535-47bb-0310-9956-ffa450edef68

            [9aa4f3efb53b257](https://github.com/ghacupha/commons-chain/commit/9aa4f3efb53b257) Niall Pemberton *2008-05-29 15:41:31*

            **Fix typos - thanks to Sebb**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@661364 13f79535-47bb-0310-9956-ffa450edef68

            [fb26cd0ad985629](https://github.com/ghacupha/commons-chain/commit/fb26cd0ad985629) Niall Pemberton *2008-05-29 15:39:44*

            **Reduce FindBugs noise - remove dead code (not even sure why this impl. exists since it does nothing)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@661362 13f79535-47bb-0310-9956-ffa450edef68

            [09445b3cd937e0b](https://github.com/ghacupha/commons-chain/commit/09445b3cd937e0b) Niall Pemberton *2008-05-29 15:36:10*

            **implement log() methods**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@661352 13f79535-47bb-0310-9956-ffa450edef68

            [1d30c1d800beca6](https://github.com/ghacupha/commons-chain/commit/1d30c1d800beca6) Niall Pemberton *2008-05-29 15:19:44*

            **Add mock ServletConfig implementation**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@661351 13f79535-47bb-0310-9956-ffa450edef68

            [6e12e065df7acac](https://github.com/ghacupha/commons-chain/commit/6e12e065df7acac) Niall Pemberton *2008-05-29 15:18:41*

            **Add description to readme**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@661120 13f79535-47bb-0310-9956-ffa450edef68

            [789e8168f7204f7](https://github.com/ghacupha/commons-chain/commit/789e8168f7204f7) Niall Pemberton *2008-05-28 22:11:22*

            **Upgrade to Logging 1.1.1 version**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@661118 13f79535-47bb-0310-9956-ffa450edef68

            [0283effd04dd986](https://github.com/ghacupha/commons-chain/commit/0283effd04dd986) Niall Pemberton *2008-05-28 22:10:53*

            **Add 2nd example webapp that uses ChainProcessor**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@661103 13f79535-47bb-0310-9956-ffa450edef68

            [69b9d5c396bbc0d](https://github.com/ghacupha/commons-chain/commit/69b9d5c396bbc0d) Niall Pemberton *2008-05-28 21:49:43*

            **Use more efficient iterator on the entrySet to avoid the Map.get() lookup - thanks to FindBugs**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@661007 13f79535-47bb-0310-9956-ffa450edef68

            [b49ab5df7db84c8](https://github.com/ghacupha/commons-chain/commit/b49ab5df7db84c8) Niall Pemberton *2008-05-28 16:28:49*

            **Add findbugs plugin**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@659363 13f79535-47bb-0310-9956-ffa450edef68

            [0acbb9701e598e2](https://github.com/ghacupha/commons-chain/commit/0acbb9701e598e2) Niall Pemberton *2008-05-23 02:08:50*

            **correct references io --> chain**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@659362 13f79535-47bb-0310-9956-ffa450edef68

            [93121a13ec9b8ad](https://github.com/ghacupha/commons-chain/commit/93121a13ec9b8ad) Niall Pemberton *2008-05-23 02:00:23*

            **Fix typo in the project description and checkstyle plugin config - thanks to Luc**

                * - typo in the project description in the pom.xml
                * - configuration of the license header file name in wrong case
                * - change license header file configuration to pom.xml(m2)/project.properties(m1)
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@659361 13f79535-47bb-0310-9956-ffa450edef68

            [8272f3b77a0c5e7](https://github.com/ghacupha/commons-chain/commit/8272f3b77a0c5e7) Niall Pemberton *2008-05-23 01:59:45*

            **Update logging version**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658982 13f79535-47bb-0310-9956-ffa450edef68

            [de3170b17688738](https://github.com/ghacupha/commons-chain/commit/de3170b17688738) Niall Pemberton *2008-05-22 02:21:57*

            **Add xerces dependency to get ant build working on JDK 1.3**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658978 13f79535-47bb-0310-9956-ffa450edef68

            [5e9f36356fe474f](https://github.com/ghacupha/commons-chain/commit/5e9f36356fe474f) Niall Pemberton *2008-05-22 02:13:12*

            **Upgrade to Logging 1.1.1**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658854 13f79535-47bb-0310-9956-ffa450edef68

            [baf7de49b34ee73](https://github.com/ghacupha/commons-chain/commit/baf7de49b34ee73) Niall Pemberton *2008-05-21 20:42:04*

            **Fix typo**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658657 13f79535-47bb-0310-9956-ffa450edef68

            [0176395c2abc5f4](https://github.com/ghacupha/commons-chain/commit/0176395c2abc5f4) Niall Pemberton *2008-05-21 12:39:19*

            **Fix svn properties - thanks to Sebb**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658574 13f79535-47bb-0310-9956-ffa450edef68

            [25a4b108b2cd079](https://github.com/ghacupha/commons-chain/commit/25a4b108b2cd079) Niall Pemberton *2008-05-21 07:23:24*

            **Correct link**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658506 13f79535-47bb-0310-9956-ffa450edef68

            [bec7e6df54e1738](https://github.com/ghacupha/commons-chain/commit/bec7e6df54e1738) Niall Pemberton *2008-05-21 00:19:17*

            **Update release date (hopefully!)**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658504 13f79535-47bb-0310-9956-ffa450edef68

            [1cf5dd92538c033](https://github.com/ghacupha/commons-chain/commit/1cf5dd92538c033) Niall Pemberton *2008-05-21 00:15:58*

            **Use m2 svn page**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658502 13f79535-47bb-0310-9956-ffa450edef68

            [f12f58767aa25f8](https://github.com/ghacupha/commons-chain/commit/f12f58767aa25f8) Niall Pemberton *2008-05-21 00:13:42*

            **minor change**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658501 13f79535-47bb-0310-9956-ffa450edef68

            [7afaeda5b83ef92](https://github.com/ghacupha/commons-chain/commit/7afaeda5b83ef92) Niall Pemberton *2008-05-21 00:12:15*

            **Add a note on how to build the example webapp**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658500 13f79535-47bb-0310-9956-ffa450edef68

            [c71533e0cf63af6](https://github.com/ghacupha/commons-chain/commit/c71533e0cf63af6) Niall Pemberton *2008-05-21 00:07:37*

            **add SNAPSHOT back**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658498 13f79535-47bb-0310-9956-ffa450edef68

            [2b35452a7e59967](https://github.com/ghacupha/commons-chain/commit/2b35452a7e59967) Niall Pemberton *2008-05-20 23:58:27*

            **Exclude dependencies MyFaces API is dragging in**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658496 13f79535-47bb-0310-9956-ffa450edef68

            [5b46b453880492f](https://github.com/ghacupha/commons-chain/commit/5b46b453880492f) Niall Pemberton *2008-05-20 23:56:48*

            **Add links to JDK javadocs, regenerate download page, correct Javadoc links**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658490 13f79535-47bb-0310-9956-ffa450edef68

            [874ab3ebdd1eec7](https://github.com/ghacupha/commons-chain/commit/874ab3ebdd1eec7) Niall Pemberton *2008-05-20 23:36:45*

            **Fix javadoc warnings**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658489 13f79535-47bb-0310-9956-ffa450edef68

            [81f8ebefbcac41e](https://github.com/ghacupha/commons-chain/commit/81f8ebefbcac41e) Niall Pemberton *2008-05-20 23:35:48*

            **Update copyright years**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658482 13f79535-47bb-0310-9956-ffa450edef68

            [49673db6a523786](https://github.com/ghacupha/commons-chain/commit/49673db6a523786) Niall Pemberton *2008-05-20 23:05:35*

            **Update building instructions**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658479 13f79535-47bb-0310-9956-ffa450edef68

            [367e6128f9c9b1c](https://github.com/ghacupha/commons-chain/commit/367e6128f9c9b1c) Niall Pemberton *2008-05-20 22:59:23*

            **Add example apps to source distro**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658477 13f79535-47bb-0310-9956-ffa450edef68

            [074ac3eada6bf3e](https://github.com/ghacupha/commons-chain/commit/074ac3eada6bf3e) Niall Pemberton *2008-05-20 22:59:02*

            **Add xml-apis to m1 build for JDK 1.3 and re-generate ant build**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658476 13f79535-47bb-0310-9956-ffa450edef68

            [8f1be8ae687944e](https://github.com/ghacupha/commons-chain/commit/8f1be8ae687944e) Niall Pemberton *2008-05-20 22:58:32*

            **Update m1 build and re-generate ant build**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658471 13f79535-47bb-0310-9956-ffa450edef68

            [c97b6e5b05209ce](https://github.com/ghacupha/commons-chain/commit/c97b6e5b05209ce) Niall Pemberton *2008-05-20 22:40:07*

            **Update site menus**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658469 13f79535-47bb-0310-9956-ffa450edef68

            [9415da25864034b](https://github.com/ghacupha/commons-chain/commit/9415da25864034b) Niall Pemberton *2008-05-20 22:39:18*

            **Update release notes and update and re-organize changes report to match**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658459 13f79535-47bb-0310-9956-ffa450edef68

            [62545b00024249d](https://github.com/ghacupha/commons-chain/commit/62545b00024249d) Niall Pemberton *2008-05-20 21:59:08*

            **Add a couple of missing license headers**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658456 13f79535-47bb-0310-9956-ffa450edef68

            [f52e33dab7bb3fb](https://github.com/ghacupha/commons-chain/commit/f52e33dab7bb3fb) Niall Pemberton *2008-05-20 21:52:02*

            **Add clirr report, remove PMD and specify reporting plugin versions**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658454 13f79535-47bb-0310-9956-ffa450edef68

            [2f0c373840d53d5](https://github.com/ghacupha/commons-chain/commit/2f0c373840d53d5) Niall Pemberton *2008-05-20 21:50:51*

            **Remove old example apps that don't work**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658452 13f79535-47bb-0310-9956-ffa450edef68

            [4d6306da7a6e3c8](https://github.com/ghacupha/commons-chain/commit/4d6306da7a6e3c8) Niall Pemberton *2008-05-20 21:47:57*

            **Upgrade to latest commons-parent and minor corrections**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658423 13f79535-47bb-0310-9956-ffa450edef68

            [c7031ebaa2f17d1](https://github.com/ghacupha/commons-chain/commit/c7031ebaa2f17d1) Niall Pemberton *2008-05-20 20:53:48*

            **Add some debugging to ChainListener**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658422 13f79535-47bb-0310-9956-ffa450edef68

            [a5d423519b3e0e8](https://github.com/ghacupha/commons-chain/commit/a5d423519b3e0e8) Niall Pemberton *2008-05-20 20:49:32*

            **Remove markup from changes.xml - m2 doesn't render it properly**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658354 13f79535-47bb-0310-9956-ffa450edef68

            [6a64f32684f757c](https://github.com/ghacupha/commons-chain/commit/6a64f32684f757c) Niall Pemberton *2008-05-20 17:21:57*

            **Remove £{basedir} for checkstyle config - doesn't work with maven 2.0.9**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@658353 13f79535-47bb-0310-9956-ffa450edef68

            [bb842ab98952408](https://github.com/ghacupha/commons-chain/commit/bb842ab98952408) Niall Pemberton *2008-05-20 17:21:15*

            **Fixing the assemblies to say project.version instead of version to stop '2.4.1' leaking through from the JVM properties. Also making it project.artifactId while I'm doing this.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@637007 13f79535-47bb-0310-9956-ffa450edef68

            [5e6eb13af366649](https://github.com/ghacupha/commons-chain/commit/5e6eb13af366649) Henri Yandell *2008-03-14 06:41:17*

            **Upgrade to version 9 of commons-parent**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@635244 13f79535-47bb-0310-9956-ffa450edef68

            [f2c7db73e9a458f](https://github.com/ghacupha/commons-chain/commit/f2c7db73e9a458f) Niall Pemberton *2008-03-09 14:21:48*

            **Add Issue Tracking and Download pages generated by commons-build-plugin**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@632817 13f79535-47bb-0310-9956-ffa450edef68

            [ae8314164df9a5c](https://github.com/ghacupha/commons-chain/commit/ae8314164df9a5c) Niall Pemberton *2008-03-02 19:46:00*

            **add m2 site.xml**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@632753 13f79535-47bb-0310-9956-ffa450edef68

            [fbabc27858b91b5](https://github.com/ghacupha/commons-chain/commit/fbabc27858b91b5) Niall Pemberton *2008-03-02 13:12:32*

            **remove local resources - this will (hopefully) be in the next parent pom**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@610600 13f79535-47bb-0310-9956-ffa450edef68

            [8051342b5c3da65](https://github.com/ghacupha/commons-chain/commit/8051342b5c3da65) Niall Pemberton *2008-01-09 22:37:48*

            **Upgrade to commons-parent version 6 release**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@609497 13f79535-47bb-0310-9956-ffa450edef68

            [835d1bd98d04e83](https://github.com/ghacupha/commons-chain/commit/835d1bd98d04e83) Niall Pemberton *2008-01-07 03:15:46*

            **Removing STATUS.html - there's no canonical data in this file**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@608768 13f79535-47bb-0310-9956-ffa450edef68

            [afd6d1a36e9973b](https://github.com/ghacupha/commons-chain/commit/afd6d1a36e9973b) Henri Yandell *2008-01-04 07:25:12*

            **Update m2 build - add assembly descriptors and get chain site generation working**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@595193 13f79535-47bb-0310-9956-ffa450edef68

            [31c3a204c8aab97](https://github.com/ghacupha/commons-chain/commit/31c3a204c8aab97) Niall Pemberton *2007-11-15 03:12:34*

            **Changing name to 'Commons Xxx'**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@568979 13f79535-47bb-0310-9956-ffa450edef68

            [0fc1c764ed043d9](https://github.com/ghacupha/commons-chain/commit/0fc1c764ed043d9) Henri Yandell *2007-08-23 13:38:00*

            **Removing the 'Commons ' from the names so all components are equivalent. This makes it look best in Continuum; no idea if it affects other places, but half of them don't have it so it hasn't been hurting them**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@568574 13f79535-47bb-0310-9956-ffa450edef68

            [0da0f77ecf6535d](https://github.com/ghacupha/commons-chain/commit/0da0f77ecf6535d) Henri Yandell *2007-08-22 11:50:58*

            **Updated commons parent version to 4.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@567499 13f79535-47bb-0310-9956-ffa450edef68

            [f899fa38bf0af61](https://github.com/ghacupha/commons-chain/commit/f899fa38bf0af61) Phil Steitz *2007-08-19 23:06:31*

            **TLP Move change wiki URLs from "wiki.apache.org/jakarta-commons" to "wiki.apache.org/commons"**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@562963 13f79535-47bb-0310-9956-ffa450edef68

            [aa011342a5cd47e](https://github.com/ghacupha/commons-chain/commit/aa011342a5cd47e) Niall Pemberton *2007-08-05 21:10:51*

            **Apache Apache**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@561500 13f79535-47bb-0310-9956-ffa450edef68

            [bc9507082e1c4fe](https://github.com/ghacupha/commons-chain/commit/bc9507082e1c4fe) Matthew Jason Benson *2007-07-31 20:36:11*

            **Move Commons TLP changes**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@561417 13f79535-47bb-0310-9956-ffa450edef68

            [f9c42aaf775b126](https://github.com/ghacupha/commons-chain/commit/f9c42aaf775b126) Niall Pemberton *2007-07-31 18:13:25*

            **Changes because of the TLP move.**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@561323 13f79535-47bb-0310-9956-ffa450edef68

            [a319089a0bcfc77](https://github.com/ghacupha/commons-chain/commit/a319089a0bcfc77) Dennis Lundberg *2007-07-31 13:24:16*

            **Fixing svn locations after TLP move**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@561233 13f79535-47bb-0310-9956-ffa450edef68

            [8218bfbc45ff364](https://github.com/ghacupha/commons-chain/commit/8218bfbc45ff364) Henri Yandell *2007-07-31 05:50:09*

            **TLP related blanket changes:**

                * s:jakarta.apache.org/commons:commons.apache.org:
                * s/commons-user@jakarta.apache.org/user@commons.apache.org/
                * s/commons-dev@jakarta.apache.org/dev@commons.apache.org/
                * s/Jakarta Commons/Apache Commons/
                * s:svn.apache.org/viewcvs/jakarta/commons:svn.apache.org/viewvc/commons:
                * s:svn.apache.org/viewcvs.cgi/jakarta/commons:svn.apache.org/viewvc/commons:
                * s:svn.apache.org/viewvc/jakarta/commons:svn.apache.org/viewvc/commons:
                * s:svn.apache.org/repos/asf/jakarta/commons:svn.apache.org/repos/asf/commons:
                * I&#39;d appreciate another pair of eyes on this. There are some categories we probably don&#39;t want to change ATM (hopefully, none of these snuck in):
                * Historicals (proposals etc.)
                * URLs that shouldn&#39;t change (DOCTYPE fragments etc.)
                * Test cases where namespace URLs matter etc. (I&#39;ll track any related nightly failures)
                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@561230 13f79535-47bb-0310-9956-ffa450edef68

            [aba6045bcc30e8b](https://github.com/ghacupha/commons-chain/commit/aba6045bcc30e8b) Rahul Akolkar *2007-07-31 04:17:09*

            **Moving to a css on the Commons site**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@560857 13f79535-47bb-0310-9956-ffa450edef68

            [23fefc9db408c52](https://github.com/ghacupha/commons-chain/commit/23fefc9db408c52) Henri Yandell *2007-07-30 03:57:33*

            **Fixing the mailing list addresses**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@560804 13f79535-47bb-0310-9956-ffa450edef68

            [ff806629bc69267](https://github.com/ghacupha/commons-chain/commit/ff806629bc69267) Henri Yandell *2007-07-29 20:14:22*

            **Moving to TLP**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/proper/chain/trunk@560660 13f79535-47bb-0310-9956-ffa450edef68

            [a1fc54abf4a9bdb](https://github.com/ghacupha/commons-chain/commit/a1fc54abf4a9bdb) Henri Yandell *2007-07-29 03:42:34*

            **Moving back :)**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@560658 13f79535-47bb-0310-9956-ffa450edef68

            [3aaf812ef9d642f](https://github.com/ghacupha/commons-chain/commit/3aaf812ef9d642f) Henri Yandell *2007-07-29 03:42:15*

            **Moving to TLP**

                * git-svn-id: https://svn.apache.org/repos/asf/commons/commons/proper/chain/trunk@560657 13f79535-47bb-0310-9956-ffa450edef68

            [f38e535ce065d02](https://github.com/ghacupha/commons-chain/commit/f38e535ce065d02) Henri Yandell *2007-07-29 03:40:41*

            **Updating to reflect website change**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@560518 13f79535-47bb-0310-9956-ffa450edef68

            [e63ecb4147de9a2](https://github.com/ghacupha/commons-chain/commit/e63ecb4147de9a2) Henri Yandell *2007-07-28 08:12:57*

            **Remove jakarta references from m1 and m2 builds**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@560337 13f79535-47bb-0310-9956-ffa450edef68

            [0c9fe51eab58232](https://github.com/ghacupha/commons-chain/commit/0c9fe51eab58232) Niall Pemberton *2007-07-27 17:52:04*

            **Update pom version, fix scm urls**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@560213 13f79535-47bb-0310-9956-ffa450edef68

            [21f72589e7afeb5](https://github.com/ghacupha/commons-chain/commit/21f72589e7afeb5) Niall Pemberton *2007-07-27 12:26:35*

            **Update NOTICE files in trunks-proper in light of TLP move (and add component names to NOTICEs where missing).**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@553294 13f79535-47bb-0310-9956-ffa450edef68

            [732a943295013fb](https://github.com/ghacupha/commons-chain/commit/732a943295013fb) Rahul Akolkar *2007-07-04 18:26:27*

            **Minor changes to example L&F**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@533029 13f79535-47bb-0310-9956-ffa450edef68

            [59e78987c56bb28](https://github.com/ghacupha/commons-chain/commit/59e78987c56bb28) Niall Pemberton *2007-04-27 09:18:19*

            **Add initial m2 pom and fix test case failing in m2**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@532948 13f79535-47bb-0310-9956-ffa450edef68

            [c9f990dff3b2cfc](https://github.com/ghacupha/commons-chain/commit/c9f990dff3b2cfc) Niall Pemberton *2007-04-27 03:53:59*

            **Setting the maven repo - apologies if this borks anything**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@486363 13f79535-47bb-0310-9956-ffa450edef68

            [196786cadcfff17](https://github.com/ghacupha/commons-chain/commit/196786cadcfff17) Henri Yandell *2006-12-12 22:11:41*

            **Add comments and urls to dependencies,. include maven reports under "development" section**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@484906 13f79535-47bb-0310-9956-ffa450edef68

            [094488cbb2d493b](https://github.com/ghacupha/commons-chain/commit/094488cbb2d493b) Niall Pemberton *2006-12-09 03:38:42*

            **Update release notes and site/doc tweaks**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@482968 13f79535-47bb-0310-9956-ffa450edef68

            [d66f26a73f6e4f2](https://github.com/ghacupha/commons-chain/commit/d66f26a73f6e4f2) Niall Pemberton *2006-12-06 08:44:48*

            **Add missing licenses, minor build/site improvements**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@480907 13f79535-47bb-0310-9956-ffa450edef68

            [4eedbf4b6faea76](https://github.com/ghacupha/commons-chain/commit/4eedbf4b6faea76) Niall Pemberton *2006-11-30 12:25:06*

            **Fixed copyright header**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@480477 13f79535-47bb-0310-9956-ffa450edef68

            [40489e5d64b94db](https://github.com/ghacupha/commons-chain/commit/40489e5d64b94db) Henri Yandell *2006-11-29 08:34:52*

            **Company change (somewhat belated).**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@479036 13f79535-47bb-0310-9956-ffa450edef68

            [56cacc66f47c39c](https://github.com/ghacupha/commons-chain/commit/56cacc66f47c39c) Martin Cooper *2006-11-24 23:01:04*

            **Point DOAP files to JIRA.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@472714 13f79535-47bb-0310-9956-ffa450edef68

            [297c62aa30b0dfc](https://github.com/ghacupha/commons-chain/commit/297c62aa30b0dfc) Rahul Akolkar *2006-11-09 00:26:31*

            **Missing SVN properties, possibly some large diffs, no functional change.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@472712 13f79535-47bb-0310-9956-ffa450edef68

            [26249d14744278f](https://github.com/ghacupha/commons-chain/commit/26249d14744278f) Rahul Akolkar *2006-11-09 00:14:44*

            **Peg Commons at JCL 1.0.4. Have only looked at proper for lack of cycles, can follow up with sandbox and dormant components as they graduate or get revived.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@472702 13f79535-47bb-0310-9956-ffa450edef68

            [a3b304552c1262e](https://github.com/ghacupha/commons-chain/commit/a3b304552c1262e) Rahul Akolkar *2006-11-08 23:39:13*

            **Switching viewcvs url to viewvc**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@430245 13f79535-47bb-0310-9956-ffa450edef68

            [73b64d73d74f8a7](https://github.com/ghacupha/commons-chain/commit/73b64d73d74f8a7) Henri Yandell *2006-08-10 05:09:05*

            **Fix mailing list archive links and Jira --> JIRA**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@422105 13f79535-47bb-0310-9956-ffa450edef68

            [176c2eb29a548b8](https://github.com/ghacupha/commons-chain/commit/176c2eb29a548b8) Niall Pemberton *2006-07-15 00:10:26*

            **Mark servlet, portlet and myfaces dependencies as "optional" (for the m2 pom) - currently this is causing Struts to include unwanted dependencies in its distro.**

                * See http://tinyurl.com/r7awd
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@421885 13f79535-47bb-0310-9956-ffa450edef68

            [677da46f9ff4516](https://github.com/ghacupha/commons-chain/commit/677da46f9ff4516) Niall Pemberton *2006-07-14 12:04:18*

            **Improve issue tracking page and reorganise site navigation**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@420689 13f79535-47bb-0310-9956-ffa450edef68

            [62d81605688323a](https://github.com/ghacupha/commons-chain/commit/62d81605688323a) Niall Pemberton *2006-07-11 03:30:38*

            **Use "maven.final.name" for checksum generation**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@420094 13f79535-47bb-0310-9956-ffa450edef68

            [a5f39c63f076312](https://github.com/ghacupha/commons-chain/commit/a5f39c63f076312) Niall Pemberton *2006-07-08 10:00:11*

            **Minor Javadoc corrections**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@416984 13f79535-47bb-0310-9956-ffa450edef68

            [ec10e1b0747f13c](https://github.com/ghacupha/commons-chain/commit/ec10e1b0747f13c) Niall Pemberton *2006-06-25 04:48:56*

            **Add the properties section to the JUnit and Servlet API dependencies in project.xml - as requested by Carlos Sanchez.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@416937 13f79535-47bb-0310-9956-ffa450edef68

            [ab7ff06272df4a4](https://github.com/ghacupha/commons-chain/commit/ab7ff06272df4a4) Niall Pemberton *2006-06-24 16:53:50*

            **Post Chain 1.1 release - roll the version number on to 1.2-SNAPSHOT**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@414699 13f79535-47bb-0310-9956-ffa450edef68

            [7081b3273aeb317](https://github.com/ghacupha/commons-chain/commit/7081b3273aeb317) Niall Pemberton *2006-06-15 22:54:44*

            **Revert groupId from org.apache.commons back to commons-chain for the Chain 1.1 release.**

                * The discussion regarding changing the groupId for Commons Components is currently ongoing with the one issue currently unresolved - see thread http://tinyurl.com/hfkuf
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@414409 13f79535-47bb-0310-9956-ffa450edef68

            [fedf13149eab9e0](https://github.com/ghacupha/commons-chain/commit/fedf13149eab9e0) Niall Pemberton *2006-06-14 23:18:50*

            **Update the version number for the 1.1 release**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@414358 13f79535-47bb-0310-9956-ffa450edef68

            [b44f8a99ebfd250](https://github.com/ghacupha/commons-chain/commit/b44f8a99ebfd250) Niall Pemberton *2006-06-14 19:11:14*

            **Remove out-of-date statement (isn't true for the maven build)**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@414242 13f79535-47bb-0310-9956-ffa450edef68

            [d59a65a7b306367](https://github.com/ghacupha/commons-chain/commit/d59a65a7b306367) Niall Pemberton *2006-06-14 13:33:04*

            **Add proper text release notes**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@413928 13f79535-47bb-0310-9956-ffa450edef68

            [72410c9294c3e6b](https://github.com/ghacupha/commons-chain/commit/72410c9294c3e6b) Niall Pemberton *2006-06-13 16:16:05*

            **Make the source distro unzip to a different directory**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@413876 13f79535-47bb-0310-9956-ffa450edef68

            [b8e99ed16036f47](https://github.com/ghacupha/commons-chain/commit/b8e99ed16036f47) Niall Pemberton *2006-06-13 11:47:36*

            **Update release notes**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@412796 13f79535-47bb-0310-9956-ffa450edef68

            [14842d4bd831c26](https://github.com/ghacupha/commons-chain/commit/14842d4bd831c26) Niall Pemberton *2006-06-08 16:47:40*

            **Add portlet mock objects and tests**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@412787 13f79535-47bb-0310-9956-ffa450edef68

            [0275987ab8b83e2](https://github.com/ghacupha/commons-chain/commit/0275987ab8b83e2) Niall Pemberton *2006-06-08 16:12:37*

            **Various minor changes for docs/build:**

                * - Add build instructions for JDK 1.3 and Changelog configuration
                * - Make default changelog configuration show changes in the last year (Chain doesn&#39;t change much)
                * - Update release notes to add missing revisions
                * - Add commented out dependency for JDK 1.3
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@412167 13f79535-47bb-0310-9956-ffa450edef68

            [2796d43214cee15](https://github.com/ghacupha/commons-chain/commit/2796d43214cee15) Niall Pemberton *2006-06-06 16:36:10*

            **Remove xdoc.copy.excludes and point RELEASE-NOTES.txt to changes-report.html**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@411973 13f79535-47bb-0310-9956-ffa450edef68

            [e7483c33c975a7d](https://github.com/ghacupha/commons-chain/commit/e7483c33c975a7d) Niall Pemberton *2006-06-06 02:34:58*

            **Fix Checkstyle and Javadoc warnings**

                * - LookupCommand&#39;s catalogFactory variable reverted to private (as it was in Chain 1.0)
                * - DisptachCommand&#39;s method, methods and methodKey variables changed to private (not yet released)
                * - add @since tags for Chain 1.1
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@411876 13f79535-47bb-0310-9956-ffa450edef68

            [0aab43e58f0d793](https://github.com/ghacupha/commons-chain/commit/0aab43e58f0d793) Niall Pemberton *2006-06-05 18:02:19*

            **Start Checkstyle clean up.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@410386 13f79535-47bb-0310-9956-ffa450edef68

            [0d293c8f41f134a](https://github.com/ghacupha/commons-chain/commit/0d293c8f41f134a) Niall Pemberton *2006-05-30 21:48:31*

            **Ignore target directory**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@409860 13f79535-47bb-0310-9956-ffa450edef68

            [32943c56ba2a380](https://github.com/ghacupha/commons-chain/commit/32943c56ba2a380) Dennis Lundberg *2006-05-27 19:08:26*

            **Change groupId to org.apache.commons**

                * Change artifactId by prefixing it with &quot;commons-chain-&quot;
                * Update the dependencies on struts and commons-chain to use versions that are available in the repository
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@409859 13f79535-47bb-0310-9956-ffa450edef68

            [368648f082dd940](https://github.com/ghacupha/commons-chain/commit/368648f082dd940) Dennis Lundberg *2006-05-27 19:06:18*

            **Change groupId to org.apache.commons**

                * Change artifactId by prefixing it with &quot;commons-chain-&quot;
                * Update the dependency on commons-chain to use a version that is available in the repository
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@409858 13f79535-47bb-0310-9956-ffa450edef68

            [3710275d83d2483](https://github.com/ghacupha/commons-chain/commit/3710275d83d2483) Dennis Lundberg *2006-05-27 19:05:08*

            **Change groupId to org.apache.commons**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@409857 13f79535-47bb-0310-9956-ffa450edef68

            [f990e420f9c9a55](https://github.com/ghacupha/commons-chain/commit/f990e420f9c9a55) Dennis Lundberg *2006-05-27 19:03:11*

            **add sane 'toString()' to MapEntryImpl**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@409177 13f79535-47bb-0310-9956-ffa450edef68

            [ed8eca0b7f2b153](https://github.com/ghacupha/commons-chain/commit/ed8eca0b7f2b153) Joseph Lad Germuska *2006-05-24 14:36:11*

            **Update maven build to include missing artifacts in distros.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@409144 13f79535-47bb-0310-9956-ffa450edef68

            [9a6985c684f519d](https://github.com/ghacupha/commons-chain/commit/9a6985c684f519d) Niall Pemberton *2006-05-24 11:42:31*

            **Remove dependency on commons-build and improve Chain site/documentation.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@409110 13f79535-47bb-0310-9956-ffa450edef68

            [d9abe78c4c7f988](https://github.com/ghacupha/commons-chain/commit/d9abe78c4c7f988) Niall Pemberton *2006-05-24 10:22:12*

            **Add myself to Commons Chain**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@409103 13f79535-47bb-0310-9956-ffa450edef68

            [4d09a800d9f97a1](https://github.com/ghacupha/commons-chain/commit/4d09a800d9f97a1) Niall Pemberton *2006-05-24 10:06:20*

            **Corrected site host name.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@408018 13f79535-47bb-0310-9956-ffa450edef68

            [cdbed5d92d16ad0](https://github.com/ghacupha/commons-chain/commit/cdbed5d92d16ad0) Robert Burrell Donkin *2006-05-20 16:14:12*

            **Added dependency to allow site build without maven tweaks.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@408017 13f79535-47bb-0310-9956-ffa450edef68

            [ccf69a15a9f8cfa](https://github.com/ghacupha/commons-chain/commit/ccf69a15a9f8cfa) Robert Burrell Donkin *2006-05-20 16:13:03*

            **Switched url from bugzilla to jira**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@406847 13f79535-47bb-0310-9956-ffa450edef68

            [05eeed02e4ab586](https://github.com/ghacupha/commons-chain/commit/05eeed02e4ab586) Henri Yandell *2006-05-16 05:48:03*

            **Remove useless var**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@387850 13f79535-47bb-0310-9956-ffa450edef68

            [bd67f8a8e05007c](https://github.com/ghacupha/commons-chain/commit/bd67f8a8e05007c) James Mitchell *2006-03-22 12:52:57*

            **Modify maven build to add two non-standard attributes to the jar's manifest file to indicate the values of "maven.compile.source" and "maven.compile.target". Also modify the build to include an "Implementation-Vendor-Id" of "org.apache" in the jar's manifest.**

                * The two non-standard entires created in the manifest file will look something like the following:
                * X-Compile-Source-JDK: 1.3
                * X-Compile-Target-JDK: 1.3
                * This change serves two purposes:
                * 1) To provide comfort to users regarding JVM compatibility.
                * 2) Enable releases to be checked more easily for JVM compatibility.
                * The manifest specification indicates that &quot;unknown&quot; entries in the manifest file are ignored. These entries have been prefixed with &quot;X-&quot; which is a sometimes used &quot;convention&quot; for indicating non-standard entries.
                * See thread: http://tinyurl.com/839zh
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@377558 13f79535-47bb-0310-9956-ffa450edef68

            [3b2546e410cb6c8](https://github.com/ghacupha/commons-chain/commit/3b2546e410cb6c8) Niall Pemberton *2006-02-14 01:15:14*

            **fixing pmc from name to url**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@371924 13f79535-47bb-0310-9956-ffa450edef68

            [348f7e64c85a377](https://github.com/ghacupha/commons-chain/commit/348f7e64c85a377) Henri Yandell *2006-01-24 14:29:48*

            **Adding doap files for each component for the projects.apache.org site**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@371566 13f79535-47bb-0310-9956-ffa450edef68

            [26a03c15c6406dc](https://github.com/ghacupha/commons-chain/commit/26a03c15c6406dc) Henri Yandell *2006-01-23 16:12:55*

            **fix bug in handling 'InvocationTargetException'**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@356422 13f79535-47bb-0310-9956-ffa450edef68

            [af8fac3ebda4e82](https://github.com/ghacupha/commons-chain/commit/af8fac3ebda4e82) Joseph Lad Germuska *2005-12-13 00:09:43*

            **Bug 37314 - Fixes to POMs**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@348035 13f79535-47bb-0310-9956-ffa450edef68

            [160a916ab6521bd](https://github.com/ghacupha/commons-chain/commit/160a916ab6521bd) Dion Gillard *2005-11-21 23:55:44*

            **since the tree has changed since 1.0, update the version to avoid confusion building from trunk**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@327839 13f79535-47bb-0310-9956-ffa450edef68

            [0e40043f37124b7](https://github.com/ghacupha/commons-chain/commit/0e40043f37124b7) Brett Porter *2005-10-23 19:30:11*

            **Bug 37107: Apply standard Maven naming for Sun JARs (servlet, portlet, JSF).  Thanks to Wendy Smoak for the patch.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@322530 13f79535-47bb-0310-9956-ffa450edef68

            [7e46a540aff3e18](https://github.com/ghacupha/commons-chain/commit/7e46a540aff3e18) Joseph Lad Germuska *2005-10-17 00:15:41*

            **add constructor which takes an already built map of commands, for easier use in dependency-injection environments**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@315059 13f79535-47bb-0310-9956-ffa450edef68

            [15749b9b769ae08](https://github.com/ghacupha/commons-chain/commit/15749b9b769ae08) Joseph Lad Germuska *2005-10-12 21:52:37*

            **add constants to help keep return intentions clear**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@314997 13f79535-47bb-0310-9956-ffa450edef68

            [e404bb65408a28d](https://github.com/ghacupha/commons-chain/commit/e404bb65408a28d) Joseph Lad Germuska *2005-10-12 18:56:48*

            **Catch InvocationTargetException and throw its cause instead, except when the cause is not an instance of Exception.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@178565 13f79535-47bb-0310-9956-ffa450edef68

            [29ce45ca43458ed](https://github.com/ghacupha/commons-chain/commit/29ce45ca43458ed) Joseph Lad Germuska *2005-05-26 01:48:57*

            **Expose catalogFactory so that subclasses can get at it.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@178563 13f79535-47bb-0310-9956-ffa450edef68

            [f754ed8aaaac5b5](https://github.com/ghacupha/commons-chain/commit/f754ed8aaaac5b5) Joseph Lad Germuska *2005-05-26 01:22:21*

            **Refactoring to make it easier for lookups to work against a CatalogFactory of any origin, instead of being bound to the static singleton instance returned by CatalogFactory.getInstance()**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@165087 13f79535-47bb-0310-9956-ffa450edef68

            [4a26ee463b8dd2d](https://github.com/ghacupha/commons-chain/commit/4a26ee463b8dd2d) Joseph Lad Germuska *2005-04-28 02:11:38*

            **Remove obsolete information about a default context attribute being set if none is specified in web.xml.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@159506 13f79535-47bb-0310-9956-ffa450edef68

            [4b6d9b340ff8005](https://github.com/ghacupha/commons-chain/commit/4b6d9b340ff8005) Martin Cooper *2005-03-30 18:49:03*

            **Fix references to <chains> to be <catalog> instead.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@159443 13f79535-47bb-0310-9956-ffa450edef68

            [5d64efb7f3eb6af](https://github.com/ghacupha/commons-chain/commit/5d64efb7f3eb6af) Martin Cooper *2005-03-29 22:59:38*

            **Add eclipse project files to svn:ignore.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@157635 13f79535-47bb-0310-9956-ffa450edef68

            [eac473276a648b8](https://github.com/ghacupha/commons-chain/commit/eac473276a648b8) Joseph Lad Germuska *2005-03-16 03:14:18*

            **Factor out the comma-delimited parsing into a separate method, fix the whitespace-skipping bugs in it, and add unit tests to verify that.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@156615 13f79535-47bb-0310-9956-ffa450edef68

            [c6ef4ca5cf7ebcf](https://github.com/ghacupha/commons-chain/commit/c6ef4ca5cf7ebcf) Martin Cooper *2005-03-09 04:38:51*

            **convert .cvsignore to svn:ignore**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@155482 13f79535-47bb-0310-9956-ffa450edef68

            [4c731f89cf28338](https://github.com/ghacupha/commons-chain/commit/4c731f89cf28338) Dirk Verbeeck *2005-02-26 13:43:33*

            **svn:keywords correction**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@155403 13f79535-47bb-0310-9956-ffa450edef68

            [a862d790231525c](https://github.com/ghacupha/commons-chain/commit/a862d790231525c) Dirk Verbeeck *2005-02-26 12:52:46*

            **Add support for using LookupCommand in a way which does not pass through the**

                * result from the looked up command.  This will allow chains used by Lookup to
                * &quot;abort&quot; (by having some command return &#39;false&#39;) without aborting the chain from
                * which the lookup was performed.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@154949 13f79535-47bb-0310-9956-ffa450edef68

            [8fe4dfccd6361ec](https://github.com/ghacupha/commons-chain/commit/8fe4dfccd6361ec) Joseph Lad Germuska *2005-02-23 04:19:49*

            **remove used import**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@151071 13f79535-47bb-0310-9956-ffa450edef68

            [224722ff3334db3](https://github.com/ghacupha/commons-chain/commit/224722ff3334db3) James Mitchell *2005-02-02 22:17:52*

            **Use SVN changelog**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@149179 13f79535-47bb-0310-9956-ffa450edef68

            [360ec10e2acc870](https://github.com/ghacupha/commons-chain/commit/360ec10e2acc870) Dirk Verbeeck *2005-01-30 23:01:01*

            **Fix simply typo**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142927 13f79535-47bb-0310-9956-ffa450edef68

            [ea2b68c117c0754](https://github.com/ghacupha/commons-chain/commit/ea2b68c117c0754) James Mitchell *2005-01-08 19:54:16*

            **Adding new DispatchLookupCommand and test case.**

                * Altered the visibility of LookupCommand.getCommand()
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142926 13f79535-47bb-0310-9956-ffa450edef68

            [660449a5d870686](https://github.com/ghacupha/commons-chain/commit/660449a5d870686) James Mitchell *2005-01-08 18:02:28*

            **fix keyword**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142925 13f79535-47bb-0310-9956-ffa450edef68

            [7b1bfe86f688949](https://github.com/ghacupha/commons-chain/commit/7b1bfe86f688949) James Mitchell *2005-01-08 04:22:49*

            **Add new test for LookupCommand.**

                * Thanks Sean!!
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142924 13f79535-47bb-0310-9956-ffa450edef68

            [186bc9b88c88b34](https://github.com/ghacupha/commons-chain/commit/186bc9b88c88b34) James Mitchell *2005-01-08 04:17:56*

            **Fix bad test.  Thanks Sean**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142923 13f79535-47bb-0310-9956-ffa450edef68

            [3e5a1dd0a26fe38](https://github.com/ghacupha/commons-chain/commit/3e5a1dd0a26fe38) James Mitchell *2005-01-08 04:15:23*

            **add DispatchCommand and test case**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142922 13f79535-47bb-0310-9956-ffa450edef68

            [114ce532cf17ddf](https://github.com/ghacupha/commons-chain/commit/114ce532cf17ddf) Joseph Lad Germuska *2005-01-07 21:10:29*

            **add myself**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142921 13f79535-47bb-0310-9956-ffa450edef68

            [ec79cd55ed3c293](https://github.com/ghacupha/commons-chain/commit/ec79cd55ed3c293) Joseph Lad Germuska *2005-01-07 21:06:40*

            **add myself**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142920 13f79535-47bb-0310-9956-ffa450edef68

            [a0271d5f46821ee](https://github.com/ghacupha/commons-chain/commit/a0271d5f46821ee) James Mitchell *2005-01-07 19:23:23*

            **Fix for bug 32894**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142919 13f79535-47bb-0310-9956-ffa450edef68

            [3c8da9411b454ff](https://github.com/ghacupha/commons-chain/commit/3c8da9411b454ff) James Mitchell *2005-01-07 19:18:03*

            **Tweaks to the web site in preparation for 1.0 release.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142915 13f79535-47bb-0310-9956-ffa450edef68

            [9e1365146548c9b](https://github.com/ghacupha/commons-chain/commit/9e1365146548c9b) Martin Cooper *2004-12-10 05:11:55*

            **Make sure that testPristine() comes first. Relying on the order of methods**

                * in the source being the order in which they are called is not exactly a
                * best practice, but on the eve of a 1.0 release, switching the order of a
                * couple of methods is the most expedient way to resolve the failing tests.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142914 13f79535-47bb-0310-9956-ffa450edef68

            [1b18c9aff130cbd](https://github.com/ghacupha/commons-chain/commit/1b18c9aff130cbd) Martin Cooper *2004-12-09 05:23:14*

            **Now that the MyFaces version of the JSF API is available at ibiblio, change**

                * the Maven and Ant builds to depend on that, rather than the JSF API RI,
                * which cannot be made available in the same way.
                * This change should allow the nightly builds of Chain to succeed - or at
                * least not fail so early because the dependencies were not available.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142913 13f79535-47bb-0310-9956-ffa450edef68

            [1687c504012d55c](https://github.com/ghacupha/commons-chain/commit/1687c504012d55c) Martin Cooper *2004-12-08 06:33:13*

            **Fix around 660 Checkstyle errors prior to the 1.0 release.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142912 13f79535-47bb-0310-9956-ffa450edef68

            [28e3cf9968460ce](https://github.com/ghacupha/commons-chain/commit/28e3cf9968460ce) Martin Cooper *2004-11-30 05:52:23*

            **Update version for 1.0 release.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142911 13f79535-47bb-0310-9956-ffa450edef68

            [b1470ba10d67597](https://github.com/ghacupha/commons-chain/commit/b1470ba10d67597) Martin Cooper *2004-11-30 05:50:08*

            **Regenerate Ant build file to pick up changes to project.xml.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142910 13f79535-47bb-0310-9956-ffa450edef68

            [802df4abf86f627](https://github.com/ghacupha/commons-chain/commit/802df4abf86f627) Martin Cooper *2004-11-22 01:59:50*

            **Update BeanUtils and Digester versions; remove Collections dependency;**

                * update version number to 1.0-dev in anticipation of a 1.0 release soon.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142909 13f79535-47bb-0310-9956-ffa450edef68

            [87fab1e123b859d](https://github.com/ghacupha/commons-chain/commit/87fab1e123b859d) Martin Cooper *2004-11-22 01:55:12*

            **Updating for 1.0 release, removed old cookbook file**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142908 13f79535-47bb-0310-9956-ffa450edef68

            [48d22896b7bf15b](https://github.com/ghacupha/commons-chain/commit/48d22896b7bf15b) Donald J. Brown *2004-11-17 08:05:39*

            **Made CatalogBase thread-safe by synchronizing the map of commands**

                * PR: 32015
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142907 13f79535-47bb-0310-9956-ffa450edef68

            [737c246ca49d4fa](https://github.com/ghacupha/commons-chain/commit/737c246ca49d4fa) Donald J. Brown *2004-11-17 07:59:18*

            **Convert the DocBook chapter into Maven format and add it to the web site**

                * as a Cookbook.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142906 13f79535-47bb-0310-9956-ffa450edef68

            [3cd4b041fc588e7](https://github.com/ghacupha/commons-chain/commit/3cd4b041fc588e7) Martin Cooper *2004-11-16 20:43:03*

            **Add forgotten new class.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142903 13f79535-47bb-0310-9956-ffa450edef68

            [a976ecaf8b8e021](https://github.com/ghacupha/commons-chain/commit/a976ecaf8b8e021) Craig R. McClanahan *2004-10-18 18:47:12*

            **Update ChainListener and ChainServlet (and the subordinate servlet related**

                * processing commands) to make the presence of the attribute init parameter
                * (org.apache.commons.chain.CONFIG_ATTR) select the previous behavior
                * where a Catalog is registered as an application scope parameter.  Absence
                * of this init parameter will trigger the new-style behavior where config
                * files are assumed to contain &lt;catalog&gt; elements, which will cause the catalogs
                * to be registered with the CatalogFactory for this application.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142902 13f79535-47bb-0310-9956-ffa450edef68

            [5eb461ba21ccd93](https://github.com/ghacupha/commons-chain/commit/5eb461ba21ccd93) Craig R. McClanahan *2004-10-18 01:48:52*

            **Update tests to reflect the modified APIs and logic.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142901 13f79535-47bb-0310-9956-ffa450edef68

            [4f7a77d7aa5daf3](https://github.com/ghacupha/commons-chain/commit/4f7a77d7aa5daf3) Craig R. McClanahan *2004-10-18 01:09:06*

            **Make CatalogFactory an abstract class instead of an interface, and make**

                * the getInstance() and clear() methods static on this class.  This is
                * necessary both to avoid applications having to reference CatalogFactoryBase,
                * but also to ensure that the clear() method actually releases all references
                * to the relevant class loader -- in the original scheme, we would still have
                * been leaving garbage lying around.
                * Refine ConfigRuleSet so that multiple &lt;factory&gt; elements with the same
                * catalog name will cause the nested chain and command definitions to be
                * merged, instead of replacing the entire catalog with only the contents
                * of the last &lt;factory&gt; element.
                * FIXME: Modify ConfigureListener and ConfigureServlet to use the new
                * mechanisms that expect a &lt;factory&gt; element -- but find a backwards
                * compatible way to continue supporting existing use cases.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142900 13f79535-47bb-0310-9956-ffa450edef68

            [dcf2216f2e91c3f](https://github.com/ghacupha/commons-chain/commit/dcf2216f2e91c3f) Craig R. McClanahan *2004-10-18 01:07:42*

            **Add a unit test for CatalogFactoryBase.**

                * Hmm ... having to explictly reference CatalogFactoryBase to call getInstance()
                * seems a little odd ... maybe we should make CatalogFactory itself a concrete
                * class instead of an interface (analogous to LogFactory in [logging]).
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142899 13f79535-47bb-0310-9956-ffa450edef68

            [52be40e3d5dafe9](https://github.com/ghacupha/commons-chain/commit/52be40e3d5dafe9) Craig R. McClanahan *2004-10-17 22:39:00*

            **Add a clear() method to CatalogFactory() so that, for example, a web**

                * application can clean up allocated catalogs when it shuts down.
                * Commit a new CatalogFactoryBase concrete implementation of CatalogFactory,
                * originally contribted by Sean Schofield, with the following tweaks:
                * Use Java2 collections classes (including necessary synchronization)
                * instead of Hashtable.
                * Make the private string constant used to name the default Catalog
                * instance less susceptible to being stepped on by applications.
                * Support the getNames() and clear() methods that were added to
                * the CatalogFactory interface.
                * Factor out the common logic used to look up the relevant class
                * loader (also making it more robust by using the class loader that
                * loaded this class if there is no thread context class loader)
                * and the logic to retrieve the appropriate Map of Catalogs related
                * to a particular ClassLoader.
                * Hint hint ... we still need unit tests for this class :-).
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142898 13f79535-47bb-0310-9956-ffa450edef68

            [cc1568a57ba8f29](https://github.com/ghacupha/commons-chain/commit/cc1568a57ba8f29) Craig R. McClanahan *2004-10-17 01:53:53*

            **Per discussion on the Commons Developer list, remove the getInstance() method**

                * that doesn&#39;t really belong here.  Also, add a getNames() method to iterate
                * over the names of all known catalogs, similar to how Catalog can iterate over
                * the names of all known commands.
                * Finally, change line endings from DOS to UNIX (which will probably make the
                * diff report unreadable, but only this time) since I&#39;m committing on a Unix
                * system.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142897 13f79535-47bb-0310-9956-ffa450edef68

            [90eccdb3d9bfd37](https://github.com/ghacupha/commons-chain/commit/90eccdb3d9bfd37) Craig R. McClanahan *2004-10-17 01:23:01*

            **Commit the proposed CatalogFactory interface, from Sean Schofield.  This is**

                * primarily for discussion at this point; I&#39;m not (quite) ready to consider it
                * to be part of the final API for [chain].
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142896 13f79535-47bb-0310-9956-ffa450edef68

            [9ea64701a7f6421](https://github.com/ghacupha/commons-chain/commit/9ea64701a7f6421) Craig R. McClanahan *2004-10-02 19:20:55*

            **Updating Pluto url**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142895 13f79535-47bb-0310-9956-ffa450edef68

            [16eef05eb5b856e](https://github.com/ghacupha/commons-chain/commit/16eef05eb5b856e) Donald J. Brown *2004-09-29 19:18:54*

            **Changed all servlet Map implementations to use the Map.Entry implementation**

                * MapEntry, rather than returning the values which caused Map.putAll() to
                * throw confusing ClassCastExceptions
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142894 13f79535-47bb-0310-9956-ffa450edef68

            [798ac6959f28756](https://github.com/ghacupha/commons-chain/commit/798ac6959f28756) Donald J. Brown *2004-09-10 22:43:20*

            **Adding postGoal to copy css stylesheets from commons-build when site is generated. Please maintain this modification for consistent look and feel across commons subprojects.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142893 13f79535-47bb-0310-9956-ffa450edef68

            [0c14f1078a122af](https://github.com/ghacupha/commons-chain/commit/0c14f1078a122af) Mark R. Diggory *2004-08-17 15:38:44*

            **Reformat to restore indentation.  No functional changes.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142891 13f79535-47bb-0310-9956-ffa450edef68

            [d4cfa2e2425fce8](https://github.com/ghacupha/commons-chain/commit/d4cfa2e2425fce8) Craig R. McClanahan *2004-07-16 17:53:39*

            **Allow a global default to be set for the o.a.c.c.Chain implementation class**

                * to be used when instantiating a new chain.
                * Submitted by:  Manfred Wolff &lt;wolff AT manfred-wolff.de&gt;
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142890 13f79535-47bb-0310-9956-ffa450edef68

            [65332de80658466](https://github.com/ghacupha/commons-chain/commit/65332de80658466) Craig R. McClanahan *2004-07-09 00:03:25*

            **Added deploy info based of jxpath's config**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142889 13f79535-47bb-0310-9956-ffa450edef68

            [30c628ff281c103](https://github.com/ghacupha/commons-chain/commit/30c628ff281c103) Donald J. Brown *2004-07-03 18:51:48*

            **Got the site to build completely**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142888 13f79535-47bb-0310-9956-ffa450edef68

            [18af2dfe8bfa07f](https://github.com/ghacupha/commons-chain/commit/18af2dfe8bfa07f) Donald J. Brown *2004-07-01 21:46:45*

            **Adding checkstyle config from jxpath, modified maven build to get**

                * unit tests to run and documents built
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142887 13f79535-47bb-0310-9956-ffa450edef68

            [9b7916275a8c0c2](https://github.com/ghacupha/commons-chain/commit/9b7916275a8c0c2) Donald J. Brown *2004-07-01 21:34:09*

            **Changed references from sandbox to commons proper, added self to dev**

                * list, modified maven config to get it to build
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142886 13f79535-47bb-0310-9956-ffa450edef68

            [6044d36d2c20080](https://github.com/ghacupha/commons-chain/commit/6044d36d2c20080) Donald J. Brown *2004-07-01 21:19:21*

            **Add properties for sdocbook plugin. Several JARs have to be downloaded manually, making the sdocbook plugin a pain to install.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142885 13f79535-47bb-0310-9956-ffa450edef68

            [9ce8775b9d967ff](https://github.com/ghacupha/commons-chain/commit/9ce8775b9d967ff) Ted Nathan Husted *2004-06-21 17:50:49*

            **Add generated HTML while we adjust the build. Edits should be made to sdocbook/chapter-chain.xml.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142884 13f79535-47bb-0310-9956-ffa450edef68

            [6fea865d389f988](https://github.com/ghacupha/commons-chain/commit/6fea865d389f988) Ted Nathan Husted *2004-06-21 17:49:43*

            **Move to default sdocbook directory**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142883 13f79535-47bb-0310-9956-ffa450edef68

            [c75dd406562c211](https://github.com/ghacupha/commons-chain/commit/c75dd406562c211) Ted Nathan Husted *2004-06-21 17:48:42*

            **Initial checkin of the Commons Chain Cookbook. This is in DocBook and needs to be integrated with the Maven build, but I wanted to get it under CVS. We may need to downsize it to Simplified DocBook.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142882 13f79535-47bb-0310-9956-ffa450edef68

            [246f7a09c9d294b](https://github.com/ghacupha/commons-chain/commit/246f7a09c9d294b) Ted Nathan Husted *2004-06-21 16:48:08*

            **Add controller application.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142881 13f79535-47bb-0310-9956-ffa450edef68

            [d4230c54debbf76](https://github.com/ghacupha/commons-chain/commit/d4230c54debbf76) Ted Nathan Husted *2004-06-01 00:56:48*

            **Add tests.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142880 13f79535-47bb-0310-9956-ffa450edef68

            [acc2dc0d5e795f7](https://github.com/ghacupha/commons-chain/commit/acc2dc0d5e795f7) Ted Nathan Husted *2004-06-01 00:52:47*

            **Javadoc and code formatting.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142879 13f79535-47bb-0310-9956-ffa450edef68

            [bc426c72fcd6150](https://github.com/ghacupha/commons-chain/commit/bc426c72fcd6150) Ted Nathan Husted *2004-06-01 00:51:18*

            **Add simple CommandAction class.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142878 13f79535-47bb-0310-9956-ffa450edef68

            [60ca4ba9fe94942](https://github.com/ghacupha/commons-chain/commit/60ca4ba9fe94942) Ted Nathan Husted *2004-06-01 00:49:17*

            **Javadoc updates.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142877 13f79535-47bb-0310-9956-ffa450edef68

            [357b29f955ca0df](https://github.com/ghacupha/commons-chain/commit/357b29f955ca0df) Ted Nathan Husted *2004-06-01 00:48:41*

            **Add ProfileCheck and Profile classes.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142876 13f79535-47bb-0310-9956-ffa450edef68

            [cfe671e410d8fab](https://github.com/ghacupha/commons-chain/commit/cfe671e410d8fab) Ted Nathan Husted *2004-06-01 00:48:05*

            **update to commons l&f, new navigation, license info**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142875 13f79535-47bb-0310-9956-ffa450edef68

            [b47fa4bcc2be40e](https://github.com/ghacupha/commons-chain/commit/b47fa4bcc2be40e) Dirk Verbeeck *2004-05-30 21:02:21*

            **Tweak build.xml to allow property substitution of the Maven executable**

                * to actually work on a Unix system.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142874 13f79535-47bb-0310-9956-ffa450edef68

            [3bb6fa7aeff5d5e](https://github.com/ghacupha/commons-chain/commit/3bb6fa7aeff5d5e) Craig R. McClanahan *2004-04-10 21:23:06*

            **Add entry for RegisterAdd mapping**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142873 13f79535-47bb-0310-9956-ffa450edef68

            [d4ef1edf8000afa](https://github.com/ghacupha/commons-chain/commit/d4ef1edf8000afa) Ted Nathan Husted *2004-04-09 00:39:04*

            **Add OpenOffice presentation**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142872 13f79535-47bb-0310-9956-ffa450edef68

            [ddc0254008c9af3](https://github.com/ghacupha/commons-chain/commit/ddc0254008c9af3) Ted Nathan Husted *2004-04-08 23:41:34*

            **Add LogonUser Command**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142871 13f79535-47bb-0310-9956-ffa450edef68

            [9dc76c946bcce6d](https://github.com/ghacupha/commons-chain/commit/9dc76c946bcce6d) Ted Nathan Husted *2004-04-08 23:33:33*

            **Move validation config under struts-config, convert to finely-grained**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142870 13f79535-47bb-0310-9956-ffa450edef68

            [5c8dca5a2d0aa75](https://github.com/ghacupha/commons-chain/commit/5c8dca5a2d0aa75) Ted Nathan Husted *2004-04-08 23:32:34*

            **Simplify checklogin tag**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142869 13f79535-47bb-0310-9956-ffa450edef68

            [4b33ad3583e0a9d](https://github.com/ghacupha/commons-chain/commit/4b33ad3583e0a9d) Ted Nathan Husted *2004-04-08 23:31:54*

            **Expand Logon action**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142868 13f79535-47bb-0310-9956-ffa450edef68

            [d94773cb680fd25](https://github.com/ghacupha/commons-chain/commit/d94773cb680fd25) Ted Nathan Husted *2004-04-08 23:29:32*

            **Add Menu mapping**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142867 13f79535-47bb-0310-9956-ffa450edef68

            [d88f2b2b62f70f7](https://github.com/ghacupha/commons-chain/commit/d88f2b2b62f70f7) Ted Nathan Husted *2004-04-08 23:28:32*

            **Optimize imports**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142866 13f79535-47bb-0310-9956-ffa450edef68

            [8b5b02d8225979b](https://github.com/ghacupha/commons-chain/commit/8b5b02d8225979b) Ted Nathan Husted *2004-04-08 23:26:07*

            **Refactor entry keys**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142865 13f79535-47bb-0310-9956-ffa450edef68

            [25234fe22244a2e](https://github.com/ghacupha/commons-chain/commit/25234fe22244a2e) Ted Nathan Husted *2004-04-08 23:24:48*

            **Javadoc, refactorings**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142864 13f79535-47bb-0310-9956-ffa450edef68

            [415b7da31e558ce](https://github.com/ghacupha/commons-chain/commit/415b7da31e558ce) Ted Nathan Husted *2004-04-08 23:23:47*

            **Add LogonAction to postcheck state**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142863 13f79535-47bb-0310-9956-ffa450edef68

            [16267900a3803a6](https://github.com/ghacupha/commons-chain/commit/16267900a3803a6) Ted Nathan Husted *2004-04-08 23:21:02*

            **Remove development cruft**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142862 13f79535-47bb-0310-9956-ffa450edef68

            [7d1e0d753390365](https://github.com/ghacupha/commons-chain/commit/7d1e0d753390365) Ted Nathan Husted *2004-04-08 23:19:59*

            **white component logo**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142861 13f79535-47bb-0310-9956-ffa450edef68

            [4c7125da4f7094b](https://github.com/ghacupha/commons-chain/commit/4c7125da4f7094b) Dirk Verbeeck *2004-04-05 20:11:50*

            **Correct scope reference**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142860 13f79535-47bb-0310-9956-ffa450edef68

            [94d84fe1699e289](https://github.com/ghacupha/commons-chain/commit/94d84fe1699e289) Ted Nathan Husted *2004-04-01 03:39:16*

            **Add LogonUser command**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142859 13f79535-47bb-0310-9956-ffa450edef68

            [c6dc3bf9d1917d0](https://github.com/ghacupha/commons-chain/commit/c6dc3bf9d1917d0) Ted Nathan Husted *2004-04-01 03:38:22*

            **"Simplified" version using conventional Struts signatures**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142858 13f79535-47bb-0310-9956-ffa450edef68

            [5e31081ba4fe468](https://github.com/ghacupha/commons-chain/commit/5e31081ba4fe468) Ted Nathan Husted *2004-04-01 03:37:20*

            **Implement code to pass LogonUser test. Test for failure.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142857 13f79535-47bb-0310-9956-ffa450edef68

            [e6faca6aba69a7e](https://github.com/ghacupha/commons-chain/commit/e6faca6aba69a7e) Ted Nathan Husted *2004-03-29 02:34:20*

            **Add LogonUser test.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142856 13f79535-47bb-0310-9956-ffa450edef68

            [72f87d4ddfa962a](https://github.com/ghacupha/commons-chain/commit/72f87d4ddfa962a) Ted Nathan Husted *2004-03-29 01:37:39*

            **Enable LocaleChange action**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142855 13f79535-47bb-0310-9956-ffa450edef68

            [83a7f0cc4a1e92e](https://github.com/ghacupha/commons-chain/commit/83a7f0cc4a1e92e) Ted Nathan Husted *2004-03-29 00:54:59*

            **Add LocaleChange test**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142854 13f79535-47bb-0310-9956-ffa450edef68

            [a24a3ae2c075613](https://github.com/ghacupha/commons-chain/commit/a24a3ae2c075613) Ted Nathan Husted *2004-03-29 00:54:23*

            **Come current**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142853 13f79535-47bb-0310-9956-ffa450edef68

            [591c0803b2abf54](https://github.com/ghacupha/commons-chain/commit/591c0803b2abf54) Ted Nathan Husted *2004-03-29 00:53:28*

            **Refactor class and packages naming.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142852 13f79535-47bb-0310-9956-ffa450edef68

            [edef7e3ee9c0376](https://github.com/ghacupha/commons-chain/commit/edef7e3ee9c0376) Ted Nathan Husted *2004-03-29 00:52:22*

            **Remove obsolete file (using version under Struts example)**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142851 13f79535-47bb-0310-9956-ffa450edef68

            [c315f1679f90008](https://github.com/ghacupha/commons-chain/commit/c315f1679f90008) Ted Nathan Husted *2004-03-29 00:49:38*

            **Refactor MailReader and related classes**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142850 13f79535-47bb-0310-9956-ffa450edef68

            [9d4fd3d3828b030](https://github.com/ghacupha/commons-chain/commit/9d4fd3d3828b030) Ted Nathan Husted *2004-03-28 03:20:56*

            **Extend design of CommandAction**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142849 13f79535-47bb-0310-9956-ffa450edef68

            [9edf948d4a00bdf](https://github.com/ghacupha/commons-chain/commit/9edf948d4a00bdf) Ted Nathan Husted *2004-03-27 18:21:30*

            **Add test and code for LocaleCommand**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142848 13f79535-47bb-0310-9956-ffa450edef68

            [46d5cb137408d48](https://github.com/ghacupha/commons-chain/commit/46d5cb137408d48) Ted Nathan Husted *2004-03-27 03:58:02*

            **Rename ActionContext as Helper objects.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142847 13f79535-47bb-0310-9956-ffa450edef68

            [a098acddd442386](https://github.com/ghacupha/commons-chain/commit/a098acddd442386) Ted Nathan Husted *2004-03-27 03:56:20*

            **Add Junit dependency for testing.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142846 13f79535-47bb-0310-9956-ffa450edef68

            [325991fad456d39](https://github.com/ghacupha/commons-chain/commit/325991fad456d39) Ted Nathan Husted *2004-03-26 18:22:41*

            **Interpose interface for ActionContext; clean up comments; add Locale method.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142845 13f79535-47bb-0310-9956-ffa450edef68

            [38be7cdbc9f825a](https://github.com/ghacupha/commons-chain/commit/38be7cdbc9f825a) Ted Nathan Husted *2004-03-26 18:21:48*

            **Initial import of MailReader Example application for Commons Chain**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142844 13f79535-47bb-0310-9956-ffa450edef68

            [fc16135b0041bfc](https://github.com/ghacupha/commons-chain/commit/fc16135b0041bfc) Ted Nathan Husted *2004-03-25 12:42:04*

            **Add status subsection around status**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142843 13f79535-47bb-0310-9956-ffa450edef68

            [79563d3e3a78a5c](https://github.com/ghacupha/commons-chain/commit/79563d3e3a78a5c) Stephen Colebourne *2004-02-28 17:21:11*

            **Change to Apache License 2.0**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142842 13f79535-47bb-0310-9956-ffa450edef68

            [28c5f9d422169a9](https://github.com/ghacupha/commons-chain/commit/28c5f9d422169a9) Stephen Colebourne *2004-02-25 00:01:07*

            **Tidy formatting**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142841 13f79535-47bb-0310-9956-ffa450edef68

            [5d8f4e02d06128b](https://github.com/ghacupha/commons-chain/commit/5d8f4e02d06128b) Ted Nathan Husted *2004-01-09 03:32:53*

            **Update portlet and jsf dependencies; migrate deprecated id element to groupId and artifactId**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142840 13f79535-47bb-0310-9956-ffa450edef68

            [b93fe41699cd19a](https://github.com/ghacupha/commons-chain/commit/b93fe41699cd19a) Ted Nathan Husted *2004-01-09 03:32:07*

            **Add imports for class names used in {@link ...} tags in the Javadocs, to**

                * avoid warning messages from the javadoc tool in 1.4.2.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142838 13f79535-47bb-0310-9956-ffa450edef68

            [5f82e2dfa54f49b](https://github.com/ghacupha/commons-chain/commit/5f82e2dfa54f49b) Craig R. McClanahan *2003-11-09 01:57:21*

            **Deal correctly with null passed in as the "resources" parameter value (which**

                * the Javadocs say is perfectly legal).
                * Submitted by:  Jeff Caddel &lt;jcaddel at cox.net&gt;
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142837 13f79535-47bb-0310-9956-ffa450edef68

            [1ee6e3a4645d9ef](https://github.com/ghacupha/commons-chain/commit/1ee6e3a4645d9ef) Craig R. McClanahan *2003-11-09 01:51:51*

            **Add minimal Mavenisation, so that we can create a web site. The main page**

                * is pretty much the same as the &#39;Rationale&#39; section of the initial proposal,
                * with minor changes. (Thanks, Craig!) The download page was borrowed from
                * Commons FileUpload.
                * IMPORTANT NOTE: I deliberately did NOT include incl_nav.xml in the nav menu
                * because that seems to push project-specific pages to the very bottom of the
                * menu, which, IMHO, is a *very bad thing*.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142836 13f79535-47bb-0310-9956-ffa450edef68

            [2c6a1b66857cc7a](https://github.com/ghacupha/commons-chain/commit/2c6a1b66857cc7a) Martin Cooper *2003-10-23 06:27:40*

            **Checkstyle cleanup.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142835 13f79535-47bb-0310-9956-ffa450edef68

            [c8977b12cd67bed](https://github.com/ghacupha/commons-chain/commit/c8977b12cd67bed) Martin Cooper *2003-10-22 06:21:24*

            **Remove unused imports & trailing whitespace.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142834 13f79535-47bb-0310-9956-ffa450edef68

            [161a8709ce208b8](https://github.com/ghacupha/commons-chain/commit/161a8709ce208b8) Martin Cooper *2003-10-21 15:55:10*

            **Fix log class name.**

                * PR: 23940
                * Submitted by: Otis Gospodnetic
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142833 13f79535-47bb-0310-9956-ffa450edef68

            [dc9c78badc93d69](https://github.com/ghacupha/commons-chain/commit/dc9c78badc93d69) Martin Cooper *2003-10-20 17:12:07*

            **Remove unused imports.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142832 13f79535-47bb-0310-9956-ffa450edef68

            [76e0151a08fac5f](https://github.com/ghacupha/commons-chain/commit/76e0151a08fac5f) Martin Cooper *2003-10-20 05:25:41*

            **Replace tabs with spaces.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142831 13f79535-47bb-0310-9956-ffa450edef68

            [0e10a804759567f](https://github.com/ghacupha/commons-chain/commit/0e10a804759567f) Martin Cooper *2003-10-18 05:30:19*

            **Add myself as a committer.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142830 13f79535-47bb-0310-9956-ffa450edef68

            [51ae8d9c1a4b40c](https://github.com/ghacupha/commons-chain/commit/51ae8d9c1a4b40c) Martin Cooper *2003-10-18 05:28:58*

            **Fixed types in apache licenses**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142829 13f79535-47bb-0310-9956-ffa450edef68

            [3c7dc02d24fe990](https://github.com/ghacupha/commons-chain/commit/3c7dc02d24fe990) Robert Burrell Donkin *2003-10-12 09:11:53*

            **Add a simple servlet that lets you dispatch incoming requests to an**

                * appropriate chain.  Three sample mapping commands (by path info,
                * extension matching, or a named request parameter) were checked in earlier.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142828 13f79535-47bb-0310-9956-ffa450edef68

            [d1735fedab823fb](https://github.com/ghacupha/commons-chain/commit/d1735fedab823fb) Craig R. McClanahan *2003-10-10 03:55:51*

            **Add a trio of useful Command implementations suitable for use as the**

                * &quot;default&quot; command to be executed by CommandProcessor.  They support
                * mapping of an incoming request to a particular command based on the
                * extra path information (PathInfoMapper), a specified request parameter
                * value (RequsetParameterMapper), or the servlet path information
                * (ServletPathMapper) from the incoming request.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142827 13f79535-47bb-0310-9956-ffa450edef68

            [72448fdcf563420](https://github.com/ghacupha/commons-chain/commit/72448fdcf563420) Craig R. McClanahan *2003-10-05 03:02:34*

            **ContextListener that loads resoruces from classpath on demand.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142825 13f79535-47bb-0310-9956-ffa450edef68

            [86b0846187b3bb2](https://github.com/ghacupha/commons-chain/commit/86b0846187b3bb2) Ted Nathan Husted *2003-10-01 17:04:02*

            **Conform license and Javadoc; no code changes.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142824 13f79535-47bb-0310-9956-ffa450edef68

            [a64f1d68f730697](https://github.com/ghacupha/commons-chain/commit/a64f1d68f730697) Ted Nathan Husted *2003-10-01 12:41:07*

            **Conform license.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142823 13f79535-47bb-0310-9956-ffa450edef68

            [68b3c046df3c8db](https://github.com/ghacupha/commons-chain/commit/68b3c046df3c8db) Ted Nathan Husted *2003-10-01 12:32:03*

            **Correct copyright date.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142822 13f79535-47bb-0310-9956-ffa450edef68

            [7c92038695d1b5b](https://github.com/ghacupha/commons-chain/commit/7c92038695d1b5b) Ted Nathan Husted *2003-10-01 12:31:50*

            **Tweak the build.xml "compile.tests" target to represent  that Digester depends on BeanUtils and Collections also being present.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142821 13f79535-47bb-0310-9956-ffa450edef68

            [5a984c7089e8706](https://github.com/ghacupha/commons-chain/commit/5a984c7089e8706) Ted Nathan Husted *2003-10-01 12:28:01*

            **Update sample properties file for beanutils and collections libraries.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142820 13f79535-47bb-0310-9956-ffa450edef68

            [45e3a33843cf133](https://github.com/ghacupha/commons-chain/commit/45e3a33843cf133) Craig R. McClanahan *2003-10-01 04:25:35*

            **Migrate ChainServlet to package org.apache.commons.chain.web, since it**

                * will be useful in portlet and JavaServer Faces environments as well.
                * Add ChainListener as an alternative configuration mechanism for
                * Servlet 2.3 or later systems (it takes advantage of the getResourcePaths()
                * method on ServletContext to scan all JAR files in &quot;/WEB-INF/lib&quot; for
                * &quot;META-INF/chain-config.xml&quot; resorces, and loads them automatically).
                * Tweak the build.xml conditionals to correctly represent the fact that
                * Digester depends on BeanUtils and Collections also being present.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142819 13f79535-47bb-0310-9956-ffa450edef68

            [63c398b1d21750e](https://github.com/ghacupha/commons-chain/commit/63c398b1d21750e) Craig R. McClanahan *2003-10-01 04:23:00*

            **Update license file.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142818 13f79535-47bb-0310-9956-ffa450edef68

            [c6e517269d1fe0e](https://github.com/ghacupha/commons-chain/commit/c6e517269d1fe0e) Ted Nathan Husted *2003-09-30 01:45:25*

            **Add commons-logging -- optional support.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142817 13f79535-47bb-0310-9956-ffa450edef68

            [631039ff166f25d](https://github.com/ghacupha/commons-chain/commit/631039ff166f25d) Ted Nathan Husted *2003-09-30 01:44:44*

            **License and Javadoc tweaks only. No code changes.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142816 13f79535-47bb-0310-9956-ffa450edef68

            [5e18dc347efca5e](https://github.com/ghacupha/commons-chain/commit/5e18dc347efca5e) Ted Nathan Husted *2003-09-29 20:02:08*

            **Replace rendundant Javadoc with reference to Interface.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142815 13f79535-47bb-0310-9956-ffa450edef68

            [9a449000f58ef9a](https://github.com/ghacupha/commons-chain/commit/9a449000f58ef9a) Ted Nathan Husted *2003-09-29 17:45:29*

            **Update regarding Commons Logging dependance.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142813 13f79535-47bb-0310-9956-ffa450edef68

            [1a5a44cf12b3f8c](https://github.com/ghacupha/commons-chain/commit/1a5a44cf12b3f8c) Ted Nathan Husted *2003-09-29 15:38:36*

            **Add convenience static for storing a default catalog attribute in some context.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142812 13f79535-47bb-0310-9956-ffa450edef68

            [ff83a03b8a7215f](https://github.com/ghacupha/commons-chain/commit/ff83a03b8a7215f) Ted Nathan Husted *2003-09-29 15:35:47*

            **Generic ChainSerlvet to allow loading a Catalog in any servlet environment. Contributed by Matthew J. Sgarlata,**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142811 13f79535-47bb-0310-9956-ffa450edef68

            [352e6e2e12864a9](https://github.com/ghacupha/commons-chain/commit/352e6e2e12864a9) Ted Nathan Husted *2003-09-29 15:34:45*

            **Forgot to delete a class that is now obsolete due to the "has-a" -> "is-a"**

                * transition for Context.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142810 13f79535-47bb-0310-9956-ffa450edef68

            [ff521d5b8a4c368](https://github.com/ghacupha/commons-chain/commit/ff521d5b8a4c368) Craig R. McClanahan *2003-09-29 06:03:57*

            **Initial phase of switching to Context "is-a" Map instead of**

                * Context &quot;has-a&quot; Map.  There are some pretty interesting intricacies
                * to implementing the entire Map contract.
                * FIXME:  Missing unit tests for the following methods on the Set returned
                * by ContextBase.keySet():  equals(), hashCode(), iterator(), remove(),
                * removeAll(), retain(), retainAll(), toArray(), toArray(Object[]).
                * FIXME:  Missing unit tests for the returned objects from
                * ContextBase.entrySet() and ContextBase.values().
                * FIXME:  ServletWebContext needs a better equals() method, given the fact
                * that it creates new subordinate Map implementations, even if you pass in
                * the same context/request/response parameters.
                * FIXME:  All of the subordinate maps in org.apache.commons.chain.web.servlet
                * (and the ones to be created in o.a.c.c.w.faces and o.a.c.c.w.portlet) need
                * complete tests for all of the Map contracts.  There are most certainly some
                * holes that need to be filled here.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142809 13f79535-47bb-0310-9956-ffa450edef68

            [2c51a25cf55f8ce](https://github.com/ghacupha/commons-chain/commit/2c51a25cf55f8ce) Craig R. McClanahan *2003-09-29 06:02:14*

            **Rearrange warning notes to avoid whines from Javadoc under JDK 1.4.2.**

                * Cosmetics only; no content or functional change.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142808 13f79535-47bb-0310-9956-ffa450edef68

            [3e477527b51ba9a](https://github.com/ghacupha/commons-chain/commit/3e477527b51ba9a) Craig R. McClanahan *2003-09-27 18:15:12*

            **Minor corrections.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142807 13f79535-47bb-0310-9956-ffa450edef68

            [234124805510ef7](https://github.com/ghacupha/commons-chain/commit/234124805510ef7) Ted Nathan Husted *2003-09-27 03:57:48*

            **Add experimental ContextMap2 class.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142806 13f79535-47bb-0310-9956-ffa450edef68

            [a8fe39326ce9f3c](https://github.com/ghacupha/commons-chain/commit/a8fe39326ce9f3c) Ted Nathan Husted *2003-09-27 03:57:28*

            **Add Husted to the Committers list.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142805 13f79535-47bb-0310-9956-ffa450edef68

            [18f6ec42966319d](https://github.com/ghacupha/commons-chain/commit/18f6ec42966319d) Ted Nathan Husted *2003-09-17 15:19:14*

            ***EXPERIMENTAL* change that allows JavaBean properties to use the internal Map for storage, rather than defining an external field. I like the concept, but I'm concerned about breaking encapsulation.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142804 13f79535-47bb-0310-9956-ffa450edef68

            [4ff16f5070ce276](https://github.com/ghacupha/commons-chain/commit/4ff16f5070ce276) Ted Nathan Husted *2003-09-17 15:17:58*

            **JavaDoc update.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142803 13f79535-47bb-0310-9956-ffa450edef68

            [925850a1a871b8a](https://github.com/ghacupha/commons-chain/commit/925850a1a871b8a) Ted Nathan Husted *2003-09-17 15:16:08*

            **Apply Tidy to markup. No content changes.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142802 13f79535-47bb-0310-9956-ffa450edef68

            [6dc438084976ea6](https://github.com/ghacupha/commons-chain/commit/6dc438084976ea6) Ted Nathan Husted *2003-09-17 15:06:04*

            **Closing parentheses**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142801 13f79535-47bb-0310-9956-ffa450edef68

            [06b198968ca916e](https://github.com/ghacupha/commons-chain/commit/06b198968ca916e) Ted Nathan Husted *2003-09-17 15:03:47*

            **Add whiteboard page with Agility entry.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142800 13f79535-47bb-0310-9956-ffa450edef68

            [5e34cbb77906028](https://github.com/ghacupha/commons-chain/commit/5e34cbb77906028) Ted Nathan Husted *2003-09-17 15:02:57*

            **Change signature of Filter.postprocess() to return a boolean that indicates**

                * an exception has been &quot;handled&quot; and therefore does not need to be rethrown
                * at the end of the Filter&#39;s processing.
                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142799 13f79535-47bb-0310-9956-ffa450edef68

            [a8b63d26c6c59f5](https://github.com/ghacupha/commons-chain/commit/a8b63d26c6c59f5) Craig R. McClanahan *2003-08-31 21:50:53*

            **Optimize imports only (no other changes)**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142798 13f79535-47bb-0310-9956-ffa450edef68

            [76c81819be676cd](https://github.com/ghacupha/commons-chain/commit/76c81819be676cd) Ted Nathan Husted *2003-08-12 20:33:25*

            **Fix typographical errors.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142797 13f79535-47bb-0310-9956-ffa450edef68

            [28f19fdc85f8b43](https://github.com/ghacupha/commons-chain/commit/28f19fdc85f8b43) Ted Nathan Husted *2003-08-12 19:33:56*

            **Add note regarding conditional compilation.**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142796 13f79535-47bb-0310-9956-ffa450edef68

            [9dda2609c544874](https://github.com/ghacupha/commons-chain/commit/9dda2609c544874) Ted Nathan Husted *2003-08-12 19:33:03*

            **Initial revision**

                * git-svn-id: https://svn.apache.org/repos/asf/jakarta/commons/proper/chain/trunk@142792 13f79535-47bb-0310-9956-ffa450edef68

            [d1dce747950bd3f](https://github.com/ghacupha/commons-chain/commit/d1dce747950bd3f) Craig R. McClanahan *2003-08-11 04:44:15*




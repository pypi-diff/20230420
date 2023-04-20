# Comparing `tmp/peak-mas-1.0.4.tar.gz` & `tmp/peak-mas-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peak-mas-1.0.4.tar", last modified: Mon Feb 20 18:44:05 2023, max compression
+gzip compressed data, was "peak-mas-1.0.5.tar", last modified: Thu Apr 20 14:28:00 2023, max compression
```

## Comparing `peak-mas-1.0.4.tar` & `peak-mas-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-02-20 18:44:05.030562 peak-mas-1.0.4/
--rw-rw-rw-   0        0        0    35821 2022-11-16 16:13:16.000000 peak-mas-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     6923 2023-02-20 18:44:05.029553 peak-mas-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5951 2022-11-16 16:13:16.000000 peak-mas-1.0.4/README.md
--rw-rw-rw-   0        0        0     1880 2023-02-20 18:43:31.000000 peak-mas-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-20 18:44:05.030562 peak-mas-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-20 18:44:04.987803 peak-mas-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-02-20 18:44:05.002802 peak-mas-1.0.4/src/peak/
--rw-rw-rw-   0        0        0     1085 2023-02-20 18:43:31.000000 peak-mas-1.0.4/src/peak/__init__.py
--rw-rw-rw-   0        0        0     3695 2022-11-25 22:47:20.000000 peak-mas-1.0.4/src/peak/__main__.py
--rw-rw-rw-   0        0        0    19682 2023-02-20 18:40:58.000000 peak-mas-1.0.4/src/peak/agents.py
--rw-rw-rw-   0        0        0    10640 2023-01-24 09:13:09.000000 peak-mas-1.0.4/src/peak/behaviours.py
--rw-rw-rw-   0        0        0     3449 2023-01-02 19:31:42.000000 peak-mas-1.0.4/src/peak/bootloader.py
-drwxrwxrwx   0        0        0        0 2023-02-20 18:44:05.005801 peak-mas-1.0.4/src/peak/cli/
--rw-rw-rw-   0        0        0        0 2022-11-16 16:13:16.000000 peak-mas-1.0.4/src/peak/cli/__init__.py
--rw-rw-rw-   0        0        0      977 2022-11-21 11:46:54.000000 peak-mas-1.0.4/src/peak/cli/df.py
--rw-rw-rw-   0        0        0     3984 2022-11-21 11:56:24.000000 peak-mas-1.0.4/src/peak/cli/mas.py
--rw-rw-rw-   0        0        0     6503 2023-02-20 18:40:58.000000 peak-mas-1.0.4/src/peak/core.py
--rw-rw-rw-   0        0        0     2275 2022-11-21 11:46:54.000000 peak-mas-1.0.4/src/peak/drivers.py
--rw-rw-rw-   0        0        0     6101 2022-11-21 11:46:54.000000 peak-mas-1.0.4/src/peak/properties.py
-drwxrwxrwx   0        0        0        0 2023-02-20 18:44:05.027808 peak-mas-1.0.4/src/peak_mas.egg-info/
--rw-rw-rw-   0        0        0     6923 2023-02-20 18:44:04.000000 peak-mas-1.0.4/src/peak_mas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-02-20 18:44:04.000000 peak-mas-1.0.4/src/peak_mas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-20 18:44:04.000000 peak-mas-1.0.4/src/peak_mas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-02-20 18:44:04.000000 peak-mas-1.0.4/src/peak_mas.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      121 2023-02-20 18:44:04.000000 peak-mas-1.0.4/src/peak_mas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-02-20 18:44:04.000000 peak-mas-1.0.4/src/peak_mas.egg-info/top_level.txt
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-04-20 14:28:00.929259 peak-mas-1.0.5/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    35148 2022-11-16 18:35:26.000000 peak-mas-1.0.5/LICENSE
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6792 2023-04-20 14:28:00.929259 peak-mas-1.0.5/PKG-INFO
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     5843 2022-11-16 18:35:26.000000 peak-mas-1.0.5/README.md
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     1664 2023-04-20 14:27:36.000000 peak-mas-1.0.5/pyproject.toml
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       38 2023-04-20 14:28:00.929259 peak-mas-1.0.5/setup.cfg
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-04-20 14:28:00.925259 peak-mas-1.0.5/src/
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-04-20 14:28:00.927260 peak-mas-1.0.5/src/peak/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      669 2023-04-20 14:27:36.000000 peak-mas-1.0.5/src/peak/__init__.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3299 2023-04-20 14:25:32.000000 peak-mas-1.0.5/src/peak/__main__.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    17766 2023-04-20 14:25:38.000000 peak-mas-1.0.5/src/peak/agents.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3519 2023-04-20 14:25:45.000000 peak-mas-1.0.5/src/peak/behaviours.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3657 2023-04-20 13:30:25.000000 peak-mas-1.0.5/src/peak/bootloader.py
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-04-20 14:28:00.927260 peak-mas-1.0.5/src/peak/cli/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2022-11-16 18:35:26.000000 peak-mas-1.0.5/src/peak/cli/__init__.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      845 2023-04-20 14:25:17.000000 peak-mas-1.0.5/src/peak/cli/df.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     2837 2023-04-20 14:25:25.000000 peak-mas-1.0.5/src/peak/cli/mas.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6776 2023-04-20 13:30:25.000000 peak-mas-1.0.5/src/peak/core.py
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-04-20 14:28:00.929259 peak-mas-1.0.5/src/peak_mas.egg-info/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6792 2023-04-20 14:28:00.000000 peak-mas-1.0.5/src/peak_mas.egg-info/PKG-INFO
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      438 2023-04-20 14:28:00.000000 peak-mas-1.0.5/src/peak_mas.egg-info/SOURCES.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        1 2023-04-20 14:28:00.000000 peak-mas-1.0.5/src/peak_mas.egg-info/dependency_links.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       44 2023-04-20 14:28:00.000000 peak-mas-1.0.5/src/peak_mas.egg-info/entry_points.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      119 2023-04-20 14:28:00.000000 peak-mas-1.0.5/src/peak_mas.egg-info/requires.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        5 2023-04-20 14:28:00.000000 peak-mas-1.0.5/src/peak_mas.egg-info/top_level.txt
```

### Comparing `peak-mas-1.0.4/LICENSE` & `peak-mas-1.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `peak-mas-1.0.4/PKG-INFO` & `peak-mas-1.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,433 +1,425 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2070 6561  : 2.1..Name: pea
-00000020: 6b2d 6d61 730d 0a56 6572 7369 6f6e 3a20  k-mas..Version: 
-00000030: 312e 302e 340d 0a53 756d 6d61 7279 3a20  1.0.4..Summary: 
-00000040: 5079 7468 6f6e 2d62 6173 6564 2066 7261  Python-based fra
-00000050: 6d65 776f 726b 2066 6f72 2068 6574 6572  mework for heter
-00000060: 6f67 656e 656f 7573 2061 6765 6e74 2063  ogeneous agent c
-00000070: 6f6d 6d75 6e69 7469 6573 0d0a 4175 7468  ommunities..Auth
-00000080: 6f72 2d65 6d61 696c 3a20 4272 756e 6f20  or-email: Bruno 
-00000090: 5269 6265 6972 6f20 3c62 7267 7269 4069  Ribeiro <brgri@i
-000000a0: 7365 702e 6970 702e 7074 3e0d 0a50 726f  sep.ipp.pt>..Pro
-000000b0: 6a65 6374 2d55 524c 3a20 486f 6d65 7061  ject-URL: Homepa
-000000c0: 6765 2c20 6874 7470 733a 2f2f 7777 772e  ge, https://www.
-000000d0: 6765 6361 642e 6973 6570 2e69 7070 2e70  gecad.isep.ipp.p
-000000e0: 742f 7065 616b 0d0a 5072 6f6a 6563 742d  t/peak..Project-
-000000f0: 5552 4c3a 2047 6974 6875 622c 2068 7474  URL: Github, htt
-00000100: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000110: 6765 6361 642d 6772 6f75 702f 7065 616b  gecad-group/peak
-00000120: 2d6d 6173 0d0a 4b65 7977 6f72 6473 3a20  -mas..Keywords: 
-00000130: 6672 616d 6577 6f72 6b2c 6d75 6c74 6961  framework,multia
-00000140: 6765 6e74 2c61 6765 6e74 2d62 6173 6564  gent,agent-based
-00000150: 2c65 636f 7379 7374 656d 2c73 7061 6465  ,ecosystem,spade
-00000160: 2c78 6d70 700d 0a43 6c61 7373 6966 6965  ,xmpp..Classifie
-00000170: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
-00000180: 4920 4170 7072 6f76 6564 203a 3a20 474e  I Approved :: GN
-00000190: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
-000001a0: 204c 6963 656e 7365 2076 3320 2847 504c   License v3 (GPL
-000001b0: 7633 290d 0a43 6c61 7373 6966 6965 723a  v3)..Classifier:
-000001c0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000001d0: 6775 6167 6520 3a3a 2050 7974 686f 6e0d  guage :: Python.
-000001e0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000001f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000200: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000210: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-00000220: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000230: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000240: 332e 390d 0a43 6c61 7373 6966 6965 723a  3.9..Classifier:
-00000250: 2045 6e76 6972 6f6e 6d65 6e74 203a 3a20   Environment :: 
-00000260: 436f 6e73 6f6c 650d 0a43 6c61 7373 6966  Console..Classif
-00000270: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00000280: 7973 7465 6d20 3a3a 204d 6963 726f 736f  ystem :: Microso
-00000290: 6674 203a 3a20 5769 6e64 6f77 730d 0a43  ft :: Windows..C
-000002a0: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
-000002b0: 7469 6e67 2053 7973 7465 6d20 3a3a 2050  ting System :: P
-000002c0: 4f53 4958 203a 3a20 4c69 6e75 780d 0a43  OSIX :: Linux..C
-000002d0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-000002e0: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
-000002f0: 6e67 696e 6565 7269 6e67 0d0a 436c 6173  ngineering..Clas
-00000300: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
-00000310: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
-00000320: 6e65 6572 696e 6720 3a3a 2041 7274 6966  neering :: Artif
-00000330: 6963 6961 6c20 496e 7465 6c6c 6967 656e  icial Intelligen
-00000340: 6365 0d0a 5265 7175 6972 6573 2d50 7974  ce..Requires-Pyt
-00000350: 686f 6e3a 203d 3d33 2e39 2e36 0d0a 4465  hon: ==3.9.6..De
-00000360: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-00000370: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-00000380: 6b64 6f77 6e0d 0a50 726f 7669 6465 732d  kdown..Provides-
-00000390: 4578 7472 613a 2062 7569 6c64 0d0a 5072  Extra: build..Pr
-000003a0: 6f76 6964 6573 2d45 7874 7261 3a20 6465  ovides-Extra: de
-000003b0: 760d 0a4c 6963 656e 7365 2d46 696c 653a  v..License-File:
-000003c0: 204c 4943 454e 5345 0d0a 0d0a 2320 5045   LICENSE....# PE
-000003d0: 414b 3a20 5079 7468 6f6e 2d62 6173 6564  AK: Python-based
-000003e0: 2066 7261 6d65 776f 726b 2066 6f72 2068   framework for h
-000003f0: 6574 6572 6f67 656e 6f75 7320 6167 656e  eterogenous agen
-00000400: 7420 636f 6d6d 756e 6974 6965 730d 0a0d  t communities...
-00000410: 0a21 5b44 4f49 5d28 6874 7470 733a 2f2f  .![DOI](https://
-00000420: 696d 672e 7368 6965 6c64 732e 696f 2f73  img.shields.io/s
-00000430: 7461 7469 632f 7631 3f6c 696e 6b3d 6874  tatic/v1?link=ht
-00000440: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
-00000450: 2e31 3030 372f 3937 382d 332d 3033 312d  .1007/978-3-031-
-00000460: 3138 3035 302d 375f 3726 6c69 6e6b 3d68  18050-7_7&link=h
-00000470: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00000480: 302e 3130 3037 2f39 3738 2d33 2d30 3331  0.1007/978-3-031
-00000490: 2d31 3830 3530 2d37 5f37 266c 6162 656c  -18050-7_7&label
-000004a0: 3d44 4f49 266d 6573 7361 6765 3d39 3738  =DOI&message=978
-000004b0: 2d33 2d30 3331 2d31 3830 3530 2d37 2663  -3-031-18050-7&c
-000004c0: 6f6c 6f72 3d62 6c75 6529 2021 5b50 7950  olor=blue) ![PyP
-000004d0: 4920 2d20 5079 7468 6f6e 2056 6572 7369  I - Python Versi
-000004e0: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
-000004f0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000500: 7079 7665 7273 696f 6e73 2f70 6561 6b2d  pyversions/peak-
-00000510: 6d61 7329 2021 5b50 7950 495d 2868 7474  mas) ![PyPI](htt
-00000520: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000530: 2e69 6f2f 7079 7069 2f76 2f70 6561 6b2d  .io/pypi/v/peak-
-00000540: 6d61 7329 2021 5b47 6974 4875 625d 2868  mas) ![GitHub](h
-00000550: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000560: 6473 2e69 6f2f 6769 7468 7562 2f6c 6963  ds.io/github/lic
-00000570: 656e 7365 2f67 6563 6164 2d67 726f 7570  ense/gecad-group
-00000580: 2f70 6561 6b2d 6d61 7329 2021 5b70 6f77  /peak-mas) ![pow
-00000590: 6572 6564 2062 795d 2868 7474 7073 3a2f  ered by](https:/
-000005a0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000005b0: 7374 6174 6963 2f76 313f 6c61 6265 6c3d  static/v1?label=
-000005c0: 706f 7765 7265 6425 3230 6279 266d 6573  powered%20by&mes
-000005d0: 7361 6765 3d47 4543 4144 2663 6f6c 6f72  sage=GECAD&color
-000005e0: 3d31 3737 3938 3526 6c61 6265 6c43 6f6c  =177985&labelCol
-000005f0: 6f72 3d64 6535 6434 6126 3f6c 696e 6b3d  or=de5d4a&?link=
-00000600: 6874 7470 3a2f 2f67 6563 6164 2e69 7365  http://gecad.ise
-00000610: 702e 6970 702e 7074 266c 696e 6b3d 6874  p.ipp.pt&link=ht
-00000620: 7470 3a2f 2f67 6563 6164 2e69 7365 702e  tp://gecad.isep.
-00000630: 6970 702e 7074 2f29 2021 5b63 6f64 6520  ipp.pt/) ![code 
-00000640: 7374 796c 655d 2868 7474 7073 3a2f 2f69  style](https://i
-00000650: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000660: 6467 652f 636f 6465 2532 3073 7479 6c65  dge/code%20style
-00000670: 2d62 6c61 636b 2d62 6c61 636b 2920 215b  -black-black) ![
-00000680: 696d 706f 7274 7320 6973 6f72 745d 2868  imports isort](h
-00000690: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000006a0: 6473 2e69 6f2f 7374 6174 6963 2f76 313f  ds.io/static/v1?
-000006b0: 6c61 6265 6c3d 696d 706f 7274 7326 6d65  label=imports&me
-000006c0: 7373 6167 653d 6973 6f72 7426 636f 6c6f  ssage=isort&colo
-000006d0: 723d 626c 7565 266c 6162 656c 436f 6c6f  r=blue&labelColo
-000006e0: 723d 6f72 616e 6765 290d 0a0d 0a50 4541  r=orange)....PEA
-000006f0: 4b20 6973 2061 206d 756c 7469 2d61 6765  K is a multi-age
-00000700: 6e74 2073 7973 7465 6d20 6672 616d 6577  nt system framew
-00000710: 6f72 6b20 7768 6963 6820 6865 6c70 7320  ork which helps 
-00000720: 7468 6520 7573 6572 7320 6465 7665 6c6f  the users develo
-00000730: 702c 206d 6f6e 6974 6f72 2c20 616e 616c  p, monitor, anal
-00000740: 797a 6520 616e 6420 6d61 696e 7461 696e  yze and maintain
-00000750: 2065 636f 7379 7374 656d 206f 6620 6865   ecosystem of he
-00000760: 7465 726f 6765 6e65 6f75 7320 6167 656e  terogeneous agen
-00000770: 7420 636f 6d6d 756e 6974 6965 732e 2054  t communities. T
-00000780: 6869 7320 6563 6f73 7973 7465 6d20 6973  his ecosystem is
-00000790: 2020 7768 6572 6520 7661 7269 6f75 7320    where various 
-000007a0: 6d75 6c74 692d 6167 656e 7420 7379 7374  multi-agent syst
-000007b0: 656d 7320 6361 6e20 636f 6578 6973 742c  ems can coexist,
-000007c0: 2069 6e74 6572 6163 7420 616e 6420 7368   interact and sh
-000007d0: 6172 6520 7265 736f 7572 6365 7320 6265  are resources be
-000007e0: 7477 6565 6e20 7468 656d 2e20 0d0a 5468  tween them. ..Th
-000007f0: 6973 2066 7261 6d65 776f 726b 2069 7320  is framework is 
-00000800: 6261 7365 6420 6f6e 203c 6120 6872 6566  based on <a href
-00000810: 3d22 6874 7470 733a 2f2f 7370 6164 652d  ="https://spade-
-00000820: 6d61 732e 7265 6164 7468 6564 6f63 732e  mas.readthedocs.
-00000830: 696f 2f65 6e2f 6c61 7465 7374 2f22 2074  io/en/latest/" t
-00000840: 6172 6765 743d 225f 626c 616e 6b22 3e53  arget="_blank">S
-00000850: 5041 4445 3c2f 613e 2e0d 0a0d 0a0d 0a23  PADE</a>.......#
-00000860: 2320 5072 6572 6571 7569 7369 7465 730d  # Prerequisites.
-00000870: 0a0d 0a2d 2050 7974 686f 6e20 3d3d 2033  ...- Python == 3
-00000880: 2e39 2e36 0d0a 2d20 584d 5050 2053 6572  .9.6..- XMPP Ser
-00000890: 7665 7220 285b 7365 6520 646f 6373 5d28  ver ([see docs](
-000008a0: 6874 7470 733a 2f2f 7777 772e 6765 6361  https://www.geca
-000008b0: 642e 6973 6570 2e69 7070 2e70 742f 7065  d.isep.ipp.pt/pe
-000008c0: 616b 2929 0d0a 0d0a 0d0a 2323 2049 6e73  ak))......## Ins
-000008d0: 7461 6c6c 696e 6720 5045 414b 0d0a 0d0a  talling PEAK....
-000008e0: 2323 2320 436f 6e64 610d 0a0d 0a54 6f20  ### Conda....To 
-000008f0: 696e 7374 616c 6c20 7573 696e 6720 636f  install using co
-00000900: 6e64 612c 2064 6f77 6e6c 6f61 6420 7468  nda, download th
-00000910: 6520 656e 7669 726f 6e6d 656e 742e 796d  e environment.ym
-00000920: 6c20 6669 6c65 2066 726f 6d20 7468 6520  l file from the 
-00000930: 7265 706f 7369 746f 7279 2061 6e64 2074  repository and t
-00000940: 6865 6e20 7573 6520 7468 6520 666f 6c6c  hen use the foll
-00000950: 6f77 696e 6720 636f 6d6d 616e 643a 0d0a  owing command:..
-00000960: 6060 6062 6173 680d 0a24 2063 6f6e 6461  ```bash..$ conda
-00000970: 2065 6e76 2063 7265 6174 6520 2d2d 6669   env create --fi
-00000980: 6c65 2065 6e76 6972 6f6e 6d65 6e74 2e79  le environment.y
-00000990: 6d6c 090d 0a60 6060 0d0a 5468 6973 2077  ml...```..This w
-000009a0: 696c 6c20 6372 6561 7465 2061 2063 6f6e  ill create a con
-000009b0: 6461 2065 6e76 6972 6f6e 6d65 6e74 2063  da environment c
-000009c0: 616c 6c65 6420 5f70 6561 6b5f 2e0d 0a0d  alled _peak_....
-000009d0: 0a23 2323 2050 6970 0d0a 0d0a 546f 2069  .### Pip....To i
-000009e0: 6e73 7461 6c6c 2075 7369 6e67 2070 6970  nstall using pip
-000009f0: 2c20 6a75 7374 2074 7970 6520 7468 6520  , just type the 
-00000a00: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
-00000a10: 643a 0d0a 6060 6062 6173 680d 0a24 2070  d:..```bash..$ p
-00000a20: 6970 2069 6e73 7461 6c6c 2070 6561 6b2d  ip install peak-
-00000a30: 6d61 730d 0a60 6060 0d0a 0d0a 0d0a 2323  mas..```......##
-00000a40: 2055 7369 6e67 2050 4541 4b0d 0a0d 0a23   Using PEAK....#
-00000a50: 2323 204e 6f74 6573 206f 6e20 5350 4144  ## Notes on SPAD
-00000a60: 450d 0a0d 0a41 7320 616c 7265 6164 7920  E....As already 
-00000a70: 7361 6964 2050 4541 4b20 6973 2062 6173  said PEAK is bas
-00000a80: 6564 206f 6e20 5350 4144 452e 2054 6869  ed on SPADE. Thi
-00000a90: 7320 6d65 616e 7320 7468 6174 2065 7665  s means that eve
-00000aa0: 7279 2066 756e 6374 696f 6e61 6c69 7479  ry functionality
-00000ab0: 206f 6620 5350 4144 4520 6973 2061 7661   of SPADE is ava
-00000ac0: 696c 6162 6c65 2074 6f20 7468 6520 7573  ilable to the us
-00000ad0: 6572 2e20 5765 2068 6967 686c 7920 7265  er. We highly re
-00000ae0: 636f 6d6d 656e 6420 796f 7520 746f 2073  commend you to s
-00000af0: 6565 203c 6120 6872 6566 3d22 6874 7470  ee <a href="http
-00000b00: 733a 2f2f 7370 6164 652d 6d61 732e 7265  s://spade-mas.re
-00000b10: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00000b20: 6c61 7465 7374 2f22 2074 6172 6765 743d  latest/" target=
-00000b30: 225f 626c 616e 6b22 3e53 5041 4445 3c2f  "_blank">SPADE</
-00000b40: 613e 2065 7861 6d70 6c65 7320 616e 6420  a> examples and 
-00000b50: 646f 6375 6d65 6e74 6174 696f 6e20 6265  documentation be
-00000b60: 666f 7265 2073 7461 7274 696e 6720 7573  fore starting us
-00000b70: 696e 6720 5045 414b 2e20 4f6e 6365 2079  ing PEAK. Once y
-00000b80: 6f75 2061 7265 2066 616d 696c 6961 7269  ou are familiari
-00000b90: 7a65 6420 7769 7468 2053 5041 4445 2773  zed with SPADE's
-00000ba0: 206d 6563 6861 6e69 6373 2079 6f75 2063   mechanics you c
-00000bb0: 616e 2073 7461 7274 2075 7369 6e67 2050  an start using P
-00000bc0: 4541 4b2e 0d0a 0d0a 2323 2320 4e6f 7465  EAK.....### Note
-00000bd0: 7320 6f6e 2058 4d50 500d 0a0d 0a54 6f20  s on XMPP....To 
-00000be0: 7275 6e20 616e 7920 5045 414b 2773 2061  run any PEAK's a
-00000bf0: 6765 6e74 2079 6f75 2077 696c 6c20 6e65  gent you will ne
-00000c00: 6564 2061 2058 4d50 5020 7365 7276 6572  ed a XMPP server
-00000c10: 2e20 596f 7520 6361 6e20 6569 7468 6572  . You can either
-00000c20: 2063 6f6e 6669 6775 7265 206f 6e65 206f   configure one o
-00000c30: 6e20 796f 7572 206d 6163 6869 6e65 2c20  n your machine, 
-00000c40: 7265 6d6f 7465 6c79 206f 7220 7573 6520  remotely or use 
-00000c50: 6120 7075 626c 6963 2073 6572 7665 722e  a public server.
-00000c60: 2054 6865 206f 6e6c 7920 6973 7375 6520   The only issue 
-00000c70: 7769 7468 2074 6865 2070 7562 6c69 6320  with the public 
-00000c80: 7365 7276 6572 7320 6973 2074 6861 7420  servers is that 
-00000c90: 7468 6579 2064 6f6e 2774 2075 7375 616c  they don't usual
-00000ca0: 6c79 2068 6176 6520 616c 6c20 7468 6520  ly have all the 
-00000cb0: 636f 6e66 6967 7572 6174 696f 6e73 2072  configurations r
-00000cc0: 6571 7569 7265 6420 746f 2072 756e 2073  equired to run s
-00000cd0: 6f6d 6520 5045 414b 2773 2066 756e 6374  ome PEAK's funct
-00000ce0: 696f 6e61 6c69 7469 6573 2e20 546f 2063  ionalities. To c
-00000cf0: 6f6e 6669 6775 7265 2074 6865 2073 6572  onfigure the ser
-00000d00: 7665 7220 796f 7520 6361 6e20 7265 6164  ver you can read
-00000d10: 2074 6865 2022 436f 6e66 6967 7572 6520   the "Configure 
-00000d20: 584d 5050 2073 6572 7665 7222 2073 6563  XMPP server" sec
-00000d30: 7469 6f6e 2069 6e20 7468 6520 3c61 2068  tion in the <a h
-00000d40: 7265 663d 2268 7474 703a 2f2f 7777 772e  ref="http://www.
-00000d50: 6765 6361 642e 6973 6570 2e69 7070 2e70  gecad.isep.ipp.p
-00000d60: 742f 7065 616b 2220 7461 7267 6574 3d22  t/peak" target="
-00000d70: 5f62 6c61 6e6b 223e 646f 6375 6d65 6e74  _blank">document
-00000d80: 6174 696f 6e3c 2f61 3e2e 0d0a 0d0a 2323  ation</a>.....##
-00000d90: 2320 4865 6c6c 6f20 576f 726c 6420 4167  # Hello World Ag
-00000da0: 656e 7420 4578 616d 706c 650d 0a0d 0a4f  ent Example....O
-00000db0: 6e65 2074 6869 6e67 2074 6861 7420 7761  ne thing that wa
-00000dc0: 7320 6164 6465 6420 696e 2050 4541 4b20  s added in PEAK 
-00000dd0: 7761 7320 7468 6520 7761 7920 7468 6520  was the way the 
-00000de0: 7573 6572 2065 7865 6375 7465 7320 7468  user executes th
-00000df0: 6520 6167 656e 7473 2e20 5045 414b 2061  e agents. PEAK a
-00000e00: 6464 6564 2061 2043 4c49 2c20 696e 7370  dded a CLI, insp
-00000e10: 6972 6564 2069 6e20 4a41 4445 2c20 746f  ired in JADE, to
-00000e20: 2068 656c 7020 7468 6520 7573 6572 2065   help the user e
-00000e30: 7865 6375 7465 2065 6e64 2063 6f6e 6669  xecute end confi
-00000e40: 6775 7265 2065 6163 6820 6167 656e 7420  gure each agent 
-00000e50: 696e 2061 2065 6173 7920 616e 6420 696e  in a easy and in
-00000e60: 7475 6974 6976 6520 6d61 6e6e 6572 2e0d  tuitive manner..
-00000e70: 0a49 6e20 7468 6973 2065 7861 6d70 6c65  .In this example
-00000e80: 2077 6520 7769 6c6c 2073 686f 7720 796f   we will show yo
-00000e90: 7520 686f 7720 746f 2065 7865 6375 7465  u how to execute
-00000ea0: 2061 2073 696e 676c 6520 6167 656e 742e   a single agent.
-00000eb0: 2053 6176 6520 7468 6520 666f 6c6c 6f77   Save the follow
-00000ec0: 696e 6720 636f 6465 2069 6e20 6120 6669  ing code in a fi
-00000ed0: 6c65 2063 616c 6c65 6420 6061 6765 6e74  le called `agent
-00000ee0: 2e70 7960 2e0d 0a0d 0a60 6060 7079 7468  .py`.....```pyth
-00000ef0: 6f6e 200d 0a66 726f 6d20 7065 616b 2069  on ..from peak i
-00000f00: 6d70 6f72 7420 4167 656e 740d 0a66 726f  mport Agent..fro
-00000f10: 6d20 7065 616b 2e62 6568 6176 696f 7572  m peak.behaviour
-00000f20: 7320 696d 706f 7274 204f 6e65 5368 6f74  s import OneShot
-00000f30: 4265 6861 7669 6f75 720d 0a0d 0a63 6c61  Behaviour....cla
-00000f40: 7373 2061 6765 6e74 2841 6765 6e74 293a  ss agent(Agent):
-00000f50: 0d0a c2a0 20c2 a020 636c 6173 7320 4865  .... .. class He
-00000f60: 6c6c 6f57 6f72 6c64 284f 6e65 5368 6f74  lloWorld(OneShot
-00000f70: 4265 6861 7669 6f75 7229 3a0d 0ac2 a020  Behaviour):.... 
-00000f80: c2a0 20c2 a020 c2a0 2061 7379 6e63 2064  .. .. .. async d
-00000f90: 6566 2072 756e 2873 656c 6629 202d 3e20  ef run(self) -> 
-00000fa0: 4e6f 6e65 3a0d 0ac2 a020 c2a0 20c2 a020  None:.... .. .. 
-00000fb0: c2a0 20c2 a020 c2a0 2070 7269 6e74 2822  .. .. .. print("
-00000fc0: 4865 6c6c 6f20 576f 726c 6422 290d 0ac2  Hello World")...
-00000fd0: a020 c2a0 20c2 a020 c2a0 20c2 a020 c2a0  . .. .. .. .. ..
-00000fe0: 2061 7761 6974 2073 656c 662e 6167 656e   await self.agen
-00000ff0: 742e 7374 6f70 2829 0d0a 0d0a c2a0 20c2  t.stop()...... .
-00001000: a020 6173 796e 6320 6465 6620 7365 7475  . async def setu
-00001010: 7028 7365 6c66 2920 2d3e 204e 6f6e 653a  p(self) -> None:
-00001020: 0d0a c2a0 20c2 a020 c2a0 20c2 a020 7365  .... .. .. .. se
-00001030: 6c66 2e61 6464 5f62 6568 6176 696f 7572  lf.add_behaviour
-00001040: 2873 656c 662e 4865 6c6c 6f57 6f72 6c64  (self.HelloWorld
-00001050: 2829 290d 0a60 6060 0d0a 4974 2069 7320  ())..```..It is 
-00001060: 6e65 6365 7373 6172 7920 7468 6174 2074  necessary that t
-00001070: 6865 206e 616d 6520 6f66 2074 6865 2066  he name of the f
-00001080: 696c 6520 6973 2074 6865 2073 616d 6520  ile is the same 
-00001090: 6173 2074 6865 206e 616d 6520 6f66 2074  as the name of t
-000010a0: 6865 2061 6765 6e74 2773 2063 6c61 7373  he agent's class
-000010b0: 2073 6f20 5045 414b 2063 616e 2064 6f20   so PEAK can do 
-000010c0: 7468 6520 7072 6f70 6572 2070 6172 7369  the proper parsi
-000010d0: 6e67 2e20 5468 6973 2061 6765 6e74 206f  ng. This agent o
-000010e0: 6e6c 7920 6861 7320 6120 6265 6861 7669  nly has a behavi
-000010f0: 6f72 2074 6861 7420 7072 696e 7473 2074  or that prints t
-00001100: 6f20 7468 6520 7465 726d 696e 616c 2074  o the terminal t
-00001110: 6865 2022 4865 6c6c 6f20 576f 726c 6422  he "Hello World"
-00001120: 206d 6573 7361 6765 2e20 546f 2065 7865   message. To exe
-00001130: 6375 7465 2074 6865 2061 6765 6e74 206a  cute the agent j
-00001140: 7573 7420 7479 7065 2074 6865 2066 6f6c  ust type the fol
-00001150: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0d  lowing command:.
-00001160: 0a60 6060 6261 7368 200d 0a24 2070 6561  .```bash ..$ pea
-00001170: 6b20 7275 6e20 7061 7468 2f74 6f2f 6167  k run path/to/ag
-00001180: 656e 742e 7079 202d 6a20 6167 656e 7440  ent.py -j agent@
-00001190: 6c6f 6361 6c68 6f73 740d 0a60 6060 0d0a  localhost..```..
-000011a0: 4368 616e 6765 2074 6865 2060 6c6f 6361  Change the `loca
-000011b0: 6c68 6f73 7460 2074 6f20 7468 6520 646f  lhost` to the do
-000011c0: 6d61 696e 206f 6620 7468 6520 584d 5050  main of the XMPP
-000011d0: 2073 6572 7665 7220 796f 7520 7761 6e74   server you want
-000011e0: 2074 6f20 636f 6e6e 6563 742e 0d0a 0d0a   to connect.....
-000011f0: 3c64 6574 6169 6c73 3e3c 7375 6d6d 6172  <details><summar
-00001200: 793e 4e6f 7465 3c2f 7375 6d6d 6172 793e  y>Note</summary>
-00001210: 0d0a 3c70 3e0d 0a0d 0a49 6620 796f 7520  ..<p>....If you 
-00001220: 7761 6e74 2074 6f20 6b6e 6f77 206d 6f72  want to know mor
-00001230: 6520 6162 6f75 7420 6561 6368 2063 6f6d  e about each com
-00001240: 6d61 6e64 2077 6520 7265 636f 6d6d 656e  mand we recommen
-00001250: 6420 7265 6164 696e 6720 7468 6520 5b64  d reading the [d
-00001260: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-00001270: 7470 3a2f 2f77 7777 2e67 6563 6164 2e69  tp://www.gecad.i
-00001280: 7365 702e 6970 702e 7074 2f70 6561 6b29  sep.ipp.pt/peak)
-00001290: 206f 7220 7573 696e 6720 7468 6520 602d   or using the `-
-000012a0: 6860 206f 7074 696f 6e20 746f 2073 6565  h` option to see
-000012b0: 2074 6865 2068 656c 7020 6d65 7373 6167   the help messag
-000012c0: 652e 0d0a 0d0a 3c2f 703e 0d0a 3c2f 6465  e.....</p>..</de
-000012d0: 7461 696c 733e 0d0a 0d0a 466f 7220 6d6f  tails>....For mo
-000012e0: 7265 2061 6476 616e 6365 6420 6675 6e63  re advanced func
-000012f0: 7469 6f6e 616c 6974 6965 7320 616e 6420  tionalities and 
-00001300: 6578 616d 706c 6573 2077 6520 7265 636f  examples we reco
-00001310: 6d6d 656e 6420 796f 7520 746f 2068 6561  mmend you to hea
-00001320: 6420 666f 7277 6172 6420 746f 2074 6865  d forward to the
-00001330: 203c 6120 6872 6566 3d22 6874 7470 3a2f   <a href="http:/
-00001340: 2f77 7777 2e67 6563 6164 2e69 7365 702e  /www.gecad.isep.
-00001350: 6970 702e 7074 2f70 6561 6b22 2074 6172  ipp.pt/peak" tar
-00001360: 6765 743d 225f 626c 616e 6b22 3e64 6f63  get="_blank">doc
-00001370: 756d 656e 7461 7469 6f6e 2077 6562 7369  umentation websi
-00001380: 7465 3c2f 613e 2e0d 0a0d 0a0d 0a23 2320  te</a>.......## 
-00001390: 5375 7070 6f72 740d 0a0d 0a55 7365 2074  Support....Use t
-000013a0: 6865 203c 6120 6872 6566 3d22 6874 7470  he <a href="http
-000013b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
-000013c0: 6563 6164 2d67 726f 7570 2f70 6561 6b2d  ecad-group/peak-
-000013d0: 6d61 732f 6469 7363 7573 7369 6f6e 7322  mas/discussions"
-000013e0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-000013f0: 3e44 6973 6375 7373 696f 6e3c 2f61 3e20  >Discussion</a> 
-00001400: 7061 6765 2069 6620 796f 7520 6861 7665  page if you have
-00001410: 2061 6e79 2071 7565 7374 696f 6e73 206f   any questions o
-00001420: 7220 6964 6561 7320 796f 7520 776f 756c  r ideas you woul
-00001430: 6420 6c69 6b65 2073 6f20 7365 6520 696d  d like so see im
-00001440: 706c 656d 656e 7465 642e 0d0a 546f 2061  plemented...To a
-00001450: 6c65 7274 2061 6e20 6973 7375 6520 6f72  lert an issue or
-00001460: 2061 2062 7567 2070 6c65 6173 6520 706f   a bug please po
-00001470: 7374 2069 6e20 7468 6520 3c61 2068 7265  st in the <a hre
-00001480: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00001490: 622e 636f 6d2f 6765 6361 642d 6772 6f75  b.com/gecad-grou
-000014a0: 702f 7065 616b 2d6d 6173 2f69 7373 7565  p/peak-mas/issue
-000014b0: 7322 2074 6172 6765 743d 225f 626c 616e  s" target="_blan
-000014c0: 6b22 3e49 7373 7565 733c 2f61 3e20 7061  k">Issues</a> pa
-000014d0: 6765 2e0d 0a0d 0a23 2320 526f 6164 6d61  ge.....## Roadma
-000014e0: 700d 0a0d 0a54 6869 7320 6172 6520 736f  p....This are so
-000014f0: 6d65 2066 756e 6374 696f 6e61 6c69 7469  me functionaliti
-00001500: 6573 2074 6861 7420 6172 6520 6265 696e  es that are bein
-00001510: 6720 6465 7665 6c6f 7065 6420 616e 6420  g developed and 
-00001520: 7769 6c6c 2062 6520 7265 6c65 6173 6564  will be released
-00001530: 2069 6e20 6120 6e65 6172 2066 7574 7572   in a near futur
-00001540: 653a 0d0a 2d20 5b20 5d20 4372 6561 7465  e:..- [ ] Create
-00001550: 2061 2044 6f63 6b65 7220 666f 7220 584d   a Docker for XM
-00001560: 5050 2073 6572 7665 7220 616e 6420 5045  PP server and PE
-00001570: 414b 2e0d 0a2d 205b 205d 2041 6464 2064  AK...- [ ] Add d
-00001580: 796e 616d 6963 2073 7065 6564 206f 7074  ynamic speed opt
-00001590: 696f 6e20 746f 2050 4541 4b27 7320 696e  ion to PEAK's in
-000015a0: 7465 726e 616c 2063 6c6f 636b 2e0d 0a2d  ternal clock...-
-000015b0: 205b 205d 2041 6464 206d 756c 7469 2d74   [ ] Add multi-t
-000015c0: 6872 6561 6469 6e67 206f 7074 696f 6e20  hreading option 
-000015d0: 746f 2074 6865 2065 7865 6375 7469 6f6e  to the execution
-000015e0: 2063 6f6e 6669 6775 7261 7469 6f6e 732e   configurations.
-000015f0: 0d0a 2d20 5b20 5d20 496d 706c 656d 656e  ..- [ ] Implemen
-00001600: 7420 5965 6c6c 6f77 2050 6167 6520 5365  t Yellow Page Se
-00001610: 7276 6963 6520 696e 2044 4620 6167 656e  rvice in DF agen
-00001620: 742e 0d0a 2d20 5b20 5d20 496d 706c 656d  t...- [ ] Implem
-00001630: 656e 7420 4461 7461 2041 6e61 6c79 7369  ent Data Analysi
-00001640: 7320 7365 6374 696f 6e20 696e 2074 6865  s section in the
-00001650: 2044 6173 6862 6f61 7264 2e0d 0a0d 0a23   Dashboard.....#
-00001660: 2320 5363 6965 6e74 6966 6963 2050 7562  # Scientific Pub
-00001670: 6c69 6361 7469 6f6e 730d 0a0d 0a2d 2052  lications....- R
-00001680: 6962 6569 726f 2c20 422e 2c20 5065 7265  ibeiro, B., Pere
-00001690: 6972 612c 2048 2e2c 2047 6f6d 6573 2c20  ira, H., Gomes, 
-000016a0: 4c2e 2c20 5661 6c65 2c20 5a2e 2028 3230  L., Vale, Z. (20
-000016b0: 3233 292e 2050 7974 686f 6e2d 4261 7365  23). Python-Base
-000016c0: 6420 4563 6f73 7973 7465 6d20 666f 7220  d Ecosystem for 
-000016d0: 4167 656e 7420 436f 6d6d 756e 6974 6965  Agent Communitie
-000016e0: 7320 5369 6d75 6c61 7469 6f6e 2e20 496e  s Simulation. In
-000016f0: 3a20 2cc2 a05f 6574 2061 6c2e 5fc2 a031  : ,.._et al._..1
-00001700: 3774 6820 496e 7465 726e 6174 696f 6e61  7th Internationa
-00001710: 6c20 436f 6e66 6572 656e 6365 206f 6e20  l Conference on 
-00001720: 536f 6674 2043 6f6d 7075 7469 6e67 204d  Soft Computing M
-00001730: 6f64 656c 7320 696e 2049 6e64 7573 7472  odels in Industr
-00001740: 6961 6c20 616e 6420 456e 7669 726f 6e6d  ial and Environm
-00001750: 656e 7461 6c20 4170 706c 6963 6174 696f  ental Applicatio
-00001760: 6e73 2028 534f 434f 2032 3032 3229 2e20  ns (SOCO 2022). 
-00001770: 534f 434f 2032 3032 322e 204c 6563 7475  SOCO 2022. Lectu
-00001780: 7265 204e 6f74 6573 2069 6e20 4e65 7477  re Notes in Netw
-00001790: 6f72 6b73 2061 6e64 2053 7973 7465 6d73  orks and Systems
-000017a0: 2c20 766f 6c20 3533 312e 2053 7072 696e  , vol 531. Sprin
-000017b0: 6765 722c 2043 6861 6d2e 2068 7474 7073  ger, Cham. https
-000017c0: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3130  ://doi.org/10.10
-000017d0: 3037 2f39 3738 2d33 2d30 3331 2d31 3830  07/978-3-031-180
-000017e0: 3530 2d37 5f37 0d0a 0d0a 2323 2043 6f6e  50-7_7....## Con
-000017f0: 7472 6962 7574 696e 6720 746f 2050 4541  tributing to PEA
-00001800: 4b0d 0a0d 0a50 756c 6c20 7265 7175 6573  K....Pull reques
-00001810: 7473 2061 7265 2077 656c 636f 6d65 2e20  ts are welcome. 
-00001820: 466f 7220 6d61 6a6f 7220 6368 616e 6765  For major change
-00001830: 732c 2070 6c65 6173 6520 6f70 656e 2061  s, please open a
-00001840: 2064 6973 6375 7373 696f 6e20 6669 7273   discussion firs
-00001850: 7420 746f 2064 6973 6375 7373 2077 6861  t to discuss wha
-00001860: 7420 796f 7520 776f 756c 6420 6c69 6b65  t you would like
-00001870: 2074 6f20 6368 616e 6765 2e0d 0a0d 0a54   to change.....T
-00001880: 6865 2065 7861 6d70 6c65 7320 6172 6520  he examples are 
-00001890: 7573 6564 2061 7320 6120 666f 726d 206f  used as a form o
-000018a0: 6620 7465 7374 696e 6720 7468 6520 6672  f testing the fr
-000018b0: 616d 6577 6f72 6b2e 2053 6f20 706c 6561  amework. So plea
-000018c0: 7365 206d 616b 6520 7375 7265 2074 6f20  se make sure to 
-000018d0: 7570 6461 7465 2074 6865 2065 7861 6d70  update the examp
-000018e0: 6c65 7320 6173 2061 7070 726f 7072 6961  les as appropria
-000018f0: 7465 206f 7220 6d61 6b65 206e 6577 206f  te or make new o
-00001900: 6e65 732e 200d 0a0d 0a54 6f20 666f 726d  nes. ....To form
-00001910: 6174 2074 6865 2063 6f64 6520 706c 6561  at the code plea
-00001920: 7365 2075 7365 2074 6865 203c 6120 6872  se use the <a hr
-00001930: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
-00001940: 2e6f 7267 2f70 726f 6a65 6374 2f62 6c61  .org/project/bla
-00001950: 636b 2f22 2074 6172 6765 743d 225f 626c  ck/" target="_bl
-00001960: 616e 6b22 3e62 6c61 636b 3c2f 613e 2061  ank">black</a> a
-00001970: 6e64 203c 6120 6872 6566 3d22 6874 7470  nd <a href="http
-00001980: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00001990: 6a65 6374 2f69 736f 7274 2f22 2074 6172  ject/isort/" tar
-000019a0: 6765 743d 225f 626c 616e 6b22 3e69 736f  get="_blank">iso
-000019b0: 7274 3c2f 613e 2070 6163 6b61 6765 732e  rt</a> packages.
-000019c0: 200d 0a0d 0a46 6f72 2074 6865 2063 6f6d   ....For the com
-000019d0: 6d69 7473 2070 6c65 6173 6520 666f 6c6c  mits please foll
-000019e0: 6f77 2074 6865 203c 6120 6872 6566 3d22  ow the <a href="
-000019f0: 7777 772e 636f 6e76 656e 7469 6f6e 616c  www.conventional
-00001a00: 636f 6d6d 6974 732e 6f72 6722 2074 6172  commits.org" tar
-00001a10: 6765 743d 225f 626c 616e 6b22 3e43 6f6e  get="_blank">Con
-00001a20: 7665 6e74 696f 6e61 6c20 436f 6d6d 6974  ventional Commit
-00001a30: 7320 4775 6964 656c 696e 653c 2f61 3e2e  s Guideline</a>.
-00001a40: 0d0a 0d0a 2323 204c 6963 656e 7365 0d0a  ....## License..
-00001a50: 0d0a 6050 4541 4b60 c2a0 6973 2066 7265  ..`PEAK`..is fre
-00001a60: 6520 616e 6420 6f70 656e 2d73 6f75 7263  e and open-sourc
-00001a70: 6520 736f 6674 7761 7265 206c 6963 656e  e software licen
-00001a80: 7365 6420 756e 6465 7220 7468 6520 3c61  sed under the <a
-00001a90: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00001aa0: 6974 6875 622e 636f 6d2f 6765 6361 642d  ithub.com/gecad-
-00001ab0: 6772 6f75 702f 7065 616b 2d6d 6173 2f62  group/peak-mas/b
-00001ac0: 6c6f 622f 6465 7665 6c6f 702f 4c49 4345  lob/develop/LICE
-00001ad0: 4e53 4522 2074 6172 6765 743d 225f 626c  NSE" target="_bl
-00001ae0: 616e 6b22 3e47 4e55 2047 656e 6572 616c  ank">GNU General
-00001af0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-00001b00: 7633 2e30 3c2f 613e 2e0d 0a              v3.0</a>...
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7065 616b  : 2.1.Name: peak
+00000020: 2d6d 6173 0a56 6572 7369 6f6e 3a20 312e  -mas.Version: 1.
+00000030: 302e 350a 5375 6d6d 6172 793a 2050 7974  0.5.Summary: Pyt
+00000040: 686f 6e2d 6261 7365 6420 6672 616d 6577  hon-based framew
+00000050: 6f72 6b20 666f 7220 6865 7465 726f 6765  ork for heteroge
+00000060: 6e65 6f75 7320 6167 656e 7420 636f 6d6d  neous agent comm
+00000070: 756e 6974 6965 730a 4175 7468 6f72 2d65  unities.Author-e
+00000080: 6d61 696c 3a20 4272 756e 6f20 5269 6265  mail: Bruno Ribe
+00000090: 6972 6f20 3c62 7267 7269 4069 7365 702e  iro <brgri@isep.
+000000a0: 6970 702e 7074 3e0a 5072 6f6a 6563 742d  ipp.pt>.Project-
+000000b0: 5552 4c3a 2048 6f6d 6570 6167 652c 2068  URL: Homepage, h
+000000c0: 7474 7073 3a2f 2f77 7777 2e67 6563 6164  ttps://www.gecad
+000000d0: 2e69 7365 702e 6970 702e 7074 2f70 6561  .isep.ipp.pt/pea
+000000e0: 6b0a 5072 6f6a 6563 742d 5552 4c3a 2047  k.Project-URL: G
+000000f0: 6974 6875 622c 2068 7474 7073 3a2f 2f67  ithub, https://g
+00000100: 6974 6875 622e 636f 6d2f 6765 6361 642d  ithub.com/gecad-
+00000110: 6772 6f75 702f 7065 616b 2d6d 6173 0a4b  group/peak-mas.K
+00000120: 6579 776f 7264 733a 2066 7261 6d65 776f  eywords: framewo
+00000130: 726b 2c6d 756c 7469 6167 656e 742c 6167  rk,multiagent,ag
+00000140: 656e 742d 6261 7365 642c 6563 6f73 7973  ent-based,ecosys
+00000150: 7465 6d2c 7370 6164 652c 786d 7070 0a43  tem,spade,xmpp.C
+00000160: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
+00000170: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000180: 6564 203a 3a20 474e 5520 4765 6e65 7261  ed :: GNU Genera
+00000190: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+000001a0: 2076 3320 2847 504c 7633 290a 436c 6173   v3 (GPLv3).Clas
+000001b0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000001c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001d0: 5079 7468 6f6e 0a43 6c61 7373 6966 6965  Python.Classifie
+000001e0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000001f0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000200: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
+00000210: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000220: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000230: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
+00000240: 6965 723a 2045 6e76 6972 6f6e 6d65 6e74  ier: Environment
+00000250: 203a 3a20 436f 6e73 6f6c 650a 436c 6173   :: Console.Clas
+00000260: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
+00000270: 6720 5379 7374 656d 203a 3a20 4d69 6372  g System :: Micr
+00000280: 6f73 6f66 7420 3a3a 2057 696e 646f 7773  osoft :: Windows
+00000290: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+000002a0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+000002b0: 2050 4f53 4958 203a 3a20 4c69 6e75 780a   POSIX :: Linux.
+000002c0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+000002d0: 6320 3a3a 2053 6369 656e 7469 6669 632f  c :: Scientific/
+000002e0: 456e 6769 6e65 6572 696e 670a 436c 6173  Engineering.Clas
+000002f0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00000300: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
+00000310: 6e65 6572 696e 6720 3a3a 2041 7274 6966  neering :: Artif
+00000320: 6963 6961 6c20 496e 7465 6c6c 6967 656e  icial Intelligen
+00000330: 6365 0a52 6571 7569 7265 732d 5079 7468  ce.Requires-Pyth
+00000340: 6f6e 3a20 3d3d 332e 392e 360a 4465 7363  on: ==3.9.6.Desc
+00000350: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+00000360: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00000370: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
+00000380: 7261 3a20 6275 696c 640a 5072 6f76 6964  ra: build.Provid
+00000390: 6573 2d45 7874 7261 3a20 6465 760a 4c69  es-Extra: dev.Li
+000003a0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
+000003b0: 4e53 450a 0a23 2050 4541 4b3a 2050 7974  NSE..# PEAK: Pyt
+000003c0: 686f 6e2d 6261 7365 6420 6672 616d 6577  hon-based framew
+000003d0: 6f72 6b20 666f 7220 6865 7465 726f 6765  ork for heteroge
+000003e0: 6e6f 7573 2061 6765 6e74 2063 6f6d 6d75  nous agent commu
+000003f0: 6e69 7469 6573 0a0a 215b 444f 495d 2868  nities..![DOI](h
+00000400: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000410: 6473 2e69 6f2f 7374 6174 6963 2f76 313f  ds.io/static/v1?
+00000420: 6c69 6e6b 3d68 7474 7073 3a2f 2f64 6f69  link=https://doi
+00000430: 2e6f 7267 2f31 302e 3130 3037 2f39 3738  .org/10.1007/978
+00000440: 2d33 2d30 3331 2d31 3830 3530 2d37 5f37  -3-031-18050-7_7
+00000450: 266c 696e 6b3d 6874 7470 733a 2f2f 646f  &link=https://do
+00000460: 692e 6f72 672f 3130 2e31 3030 372f 3937  i.org/10.1007/97
+00000470: 382d 332d 3033 312d 3138 3035 302d 375f  8-3-031-18050-7_
+00000480: 3726 6c61 6265 6c3d 444f 4926 6d65 7373  7&label=DOI&mess
+00000490: 6167 653d 3937 382d 332d 3033 312d 3138  age=978-3-031-18
+000004a0: 3035 302d 3726 636f 6c6f 723d 626c 7565  050-7&color=blue
+000004b0: 2920 215b 5079 5049 202d 2050 7974 686f  ) ![PyPI - Pytho
+000004c0: 6e20 5665 7273 696f 6e5d 2868 7474 7073  n Version](https
+000004d0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000004e0: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
+000004f0: 732f 7065 616b 2d6d 6173 2920 215b 5079  s/peak-mas) ![Py
+00000500: 5049 5d28 6874 7470 733a 2f2f 696d 672e  PI](https://img.
+00000510: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000520: 762f 7065 616b 2d6d 6173 2920 215b 4769  v/peak-mas) ![Gi
+00000530: 7448 7562 5d28 6874 7470 733a 2f2f 696d  tHub](https://im
+00000540: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000550: 6875 622f 6c69 6365 6e73 652f 6765 6361  hub/license/geca
+00000560: 642d 6772 6f75 702f 7065 616b 2d6d 6173  d-group/peak-mas
+00000570: 2920 215b 706f 7765 7265 6420 6279 5d28  ) ![powered by](
+00000580: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000590: 6c64 732e 696f 2f73 7461 7469 632f 7631  lds.io/static/v1
+000005a0: 3f6c 6162 656c 3d70 6f77 6572 6564 2532  ?label=powered%2
+000005b0: 3062 7926 6d65 7373 6167 653d 4745 4341  0by&message=GECA
+000005c0: 4426 636f 6c6f 723d 3137 3739 3835 266c  D&color=177985&l
+000005d0: 6162 656c 436f 6c6f 723d 6465 3564 3461  abelColor=de5d4a
+000005e0: 263f 6c69 6e6b 3d68 7474 703a 2f2f 6765  &?link=http://ge
+000005f0: 6361 642e 6973 6570 2e69 7070 2e70 7426  cad.isep.ipp.pt&
+00000600: 6c69 6e6b 3d68 7474 703a 2f2f 6765 6361  link=http://geca
+00000610: 642e 6973 6570 2e69 7070 2e70 742f 2920  d.isep.ipp.pt/) 
+00000620: 215b 636f 6465 2073 7479 6c65 5d28 6874  ![code style](ht
+00000630: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000640: 732e 696f 2f62 6164 6765 2f63 6f64 6525  s.io/badge/code%
+00000650: 3230 7374 796c 652d 626c 6163 6b2d 626c  20style-black-bl
+00000660: 6163 6b29 2021 5b69 6d70 6f72 7473 2069  ack) ![imports i
+00000670: 736f 7274 5d28 6874 7470 733a 2f2f 696d  sort](https://im
+00000680: 672e 7368 6965 6c64 732e 696f 2f73 7461  g.shields.io/sta
+00000690: 7469 632f 7631 3f6c 6162 656c 3d69 6d70  tic/v1?label=imp
+000006a0: 6f72 7473 266d 6573 7361 6765 3d69 736f  orts&message=iso
+000006b0: 7274 2663 6f6c 6f72 3d62 6c75 6526 6c61  rt&color=blue&la
+000006c0: 6265 6c43 6f6c 6f72 3d6f 7261 6e67 6529  belColor=orange)
+000006d0: 0a0a 5045 414b 2069 7320 6120 6d75 6c74  ..PEAK is a mult
+000006e0: 692d 6167 656e 7420 7379 7374 656d 2066  i-agent system f
+000006f0: 7261 6d65 776f 726b 2077 6869 6368 2068  ramework which h
+00000700: 656c 7073 2074 6865 2075 7365 7273 2064  elps the users d
+00000710: 6576 656c 6f70 2c20 6d6f 6e69 746f 722c  evelop, monitor,
+00000720: 2061 6e61 6c79 7a65 2061 6e64 206d 6169   analyze and mai
+00000730: 6e74 6169 6e20 6563 6f73 7973 7465 6d20  ntain ecosystem 
+00000740: 6f66 2068 6574 6572 6f67 656e 656f 7573  of heterogeneous
+00000750: 2061 6765 6e74 2063 6f6d 6d75 6e69 7469   agent communiti
+00000760: 6573 2e20 5468 6973 2065 636f 7379 7374  es. This ecosyst
+00000770: 656d 2069 7320 2077 6865 7265 2076 6172  em is  where var
+00000780: 696f 7573 206d 756c 7469 2d61 6765 6e74  ious multi-agent
+00000790: 2073 7973 7465 6d73 2063 616e 2063 6f65   systems can coe
+000007a0: 7869 7374 2c20 696e 7465 7261 6374 2061  xist, interact a
+000007b0: 6e64 2073 6861 7265 2072 6573 6f75 7263  nd share resourc
+000007c0: 6573 2062 6574 7765 656e 2074 6865 6d2e  es between them.
+000007d0: 200a 5468 6973 2066 7261 6d65 776f 726b   .This framework
+000007e0: 2069 7320 6261 7365 6420 6f6e 203c 6120   is based on <a 
+000007f0: 6872 6566 3d22 6874 7470 733a 2f2f 7370  href="https://sp
+00000800: 6164 652d 6d61 732e 7265 6164 7468 6564  ade-mas.readthed
+00000810: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000820: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
+00000830: 6b22 3e53 5041 4445 3c2f 613e 2e0a 0a0a  k">SPADE</a>....
+00000840: 2323 2050 7265 7265 7175 6973 6974 6573  ## Prerequisites
+00000850: 0a0a 2d20 5079 7468 6f6e 203d 3d20 332e  ..- Python == 3.
+00000860: 392e 360a 2d20 584d 5050 2053 6572 7665  9.6.- XMPP Serve
+00000870: 7220 285b 7365 6520 646f 6373 5d28 6874  r ([see docs](ht
+00000880: 7470 733a 2f2f 7777 772e 6765 6361 642e  tps://www.gecad.
+00000890: 6973 6570 2e69 7070 2e70 742f 7065 616b  isep.ipp.pt/peak
+000008a0: 2929 0a0a 0a23 2320 496e 7374 616c 6c69  ))...## Installi
+000008b0: 6e67 2050 4541 4b0a 0a23 2323 2043 6f6e  ng PEAK..### Con
+000008c0: 6461 0a0a 546f 2069 6e73 7461 6c6c 2075  da..To install u
+000008d0: 7369 6e67 2063 6f6e 6461 2c20 646f 776e  sing conda, down
+000008e0: 6c6f 6164 2074 6865 2065 6e76 6972 6f6e  load the environ
+000008f0: 6d65 6e74 2e79 6d6c 2066 696c 6520 6672  ment.yml file fr
+00000900: 6f6d 2074 6865 2072 6570 6f73 6974 6f72  om the repositor
+00000910: 7920 616e 6420 7468 656e 2075 7365 2074  y and then use t
+00000920: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00000930: 6d61 6e64 3a0a 6060 6062 6173 680a 2420  mand:.```bash.$ 
+00000940: 636f 6e64 6120 656e 7620 6372 6561 7465  conda env create
+00000950: 202d 2d66 696c 6520 656e 7669 726f 6e6d   --file environm
+00000960: 656e 742e 796d 6c09 0a60 6060 0a54 6869  ent.yml..```.Thi
+00000970: 7320 7769 6c6c 2063 7265 6174 6520 6120  s will create a 
+00000980: 636f 6e64 6120 656e 7669 726f 6e6d 656e  conda environmen
+00000990: 7420 6361 6c6c 6564 205f 7065 616b 5f2e  t called _peak_.
+000009a0: 0a0a 2323 2320 5069 700a 0a54 6f20 696e  ..### Pip..To in
+000009b0: 7374 616c 6c20 7573 696e 6720 7069 702c  stall using pip,
+000009c0: 206a 7573 7420 7479 7065 2074 6865 2066   just type the f
+000009d0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+000009e0: 3a0a 6060 6062 6173 680a 2420 7069 7020  :.```bash.$ pip 
+000009f0: 696e 7374 616c 6c20 7065 616b 2d6d 6173  install peak-mas
+00000a00: 0a60 6060 0a0a 0a23 2320 5573 696e 6720  .```...## Using 
+00000a10: 5045 414b 0a0a 2323 2320 4e6f 7465 7320  PEAK..### Notes 
+00000a20: 6f6e 2053 5041 4445 0a0a 4173 2061 6c72  on SPADE..As alr
+00000a30: 6561 6479 2073 6169 6420 5045 414b 2069  eady said PEAK i
+00000a40: 7320 6261 7365 6420 6f6e 2053 5041 4445  s based on SPADE
+00000a50: 2e20 5468 6973 206d 6561 6e73 2074 6861  . This means tha
+00000a60: 7420 6576 6572 7920 6675 6e63 7469 6f6e  t every function
+00000a70: 616c 6974 7920 6f66 2053 5041 4445 2069  ality of SPADE i
+00000a80: 7320 6176 6169 6c61 626c 6520 746f 2074  s available to t
+00000a90: 6865 2075 7365 722e 2057 6520 6869 6768  he user. We high
+00000aa0: 6c79 2072 6563 6f6d 6d65 6e64 2079 6f75  ly recommend you
+00000ab0: 2074 6f20 7365 6520 3c61 2068 7265 663d   to see <a href=
+00000ac0: 2268 7474 7073 3a2f 2f73 7061 6465 2d6d  "https://spade-m
+00000ad0: 6173 2e72 6561 6474 6865 646f 6373 2e69  as.readthedocs.i
+00000ae0: 6f2f 656e 2f6c 6174 6573 742f 2220 7461  o/en/latest/" ta
+00000af0: 7267 6574 3d22 5f62 6c61 6e6b 223e 5350  rget="_blank">SP
+00000b00: 4144 453c 2f61 3e20 6578 616d 706c 6573  ADE</a> examples
+00000b10: 2061 6e64 2064 6f63 756d 656e 7461 7469   and documentati
+00000b20: 6f6e 2062 6566 6f72 6520 7374 6172 7469  on before starti
+00000b30: 6e67 2075 7369 6e67 2050 4541 4b2e 204f  ng using PEAK. O
+00000b40: 6e63 6520 796f 7520 6172 6520 6661 6d69  nce you are fami
+00000b50: 6c69 6172 697a 6564 2077 6974 6820 5350  liarized with SP
+00000b60: 4144 4527 7320 6d65 6368 616e 6963 7320  ADE's mechanics 
+00000b70: 796f 7520 6361 6e20 7374 6172 7420 7573  you can start us
+00000b80: 696e 6720 5045 414b 2e0a 0a23 2323 204e  ing PEAK...### N
+00000b90: 6f74 6573 206f 6e20 584d 5050 0a0a 546f  otes on XMPP..To
+00000ba0: 2072 756e 2061 6e79 2050 4541 4b27 7320   run any PEAK's 
+00000bb0: 6167 656e 7420 796f 7520 7769 6c6c 206e  agent you will n
+00000bc0: 6565 6420 6120 584d 5050 2073 6572 7665  eed a XMPP serve
+00000bd0: 722e 2059 6f75 2063 616e 2065 6974 6865  r. You can eithe
+00000be0: 7220 636f 6e66 6967 7572 6520 6f6e 6520  r configure one 
+00000bf0: 6f6e 2079 6f75 7220 6d61 6368 696e 652c  on your machine,
+00000c00: 2072 656d 6f74 656c 7920 6f72 2075 7365   remotely or use
+00000c10: 2061 2070 7562 6c69 6320 7365 7276 6572   a public server
+00000c20: 2e20 5468 6520 6f6e 6c79 2069 7373 7565  . The only issue
+00000c30: 2077 6974 6820 7468 6520 7075 626c 6963   with the public
+00000c40: 2073 6572 7665 7273 2069 7320 7468 6174   servers is that
+00000c50: 2074 6865 7920 646f 6e27 7420 7573 7561   they don't usua
+00000c60: 6c6c 7920 6861 7665 2061 6c6c 2074 6865  lly have all the
+00000c70: 2063 6f6e 6669 6775 7261 7469 6f6e 7320   configurations 
+00000c80: 7265 7175 6972 6564 2074 6f20 7275 6e20  required to run 
+00000c90: 736f 6d65 2050 4541 4b27 7320 6675 6e63  some PEAK's func
+00000ca0: 7469 6f6e 616c 6974 6965 732e 2054 6f20  tionalities. To 
+00000cb0: 636f 6e66 6967 7572 6520 7468 6520 7365  configure the se
+00000cc0: 7276 6572 2079 6f75 2063 616e 2072 6561  rver you can rea
+00000cd0: 6420 7468 6520 2243 6f6e 6669 6775 7265  d the "Configure
+00000ce0: 2058 4d50 5020 7365 7276 6572 2220 7365   XMPP server" se
+00000cf0: 6374 696f 6e20 696e 2074 6865 203c 6120  ction in the <a 
+00000d00: 6872 6566 3d22 6874 7470 3a2f 2f77 7777  href="http://www
+00000d10: 2e67 6563 6164 2e69 7365 702e 6970 702e  .gecad.isep.ipp.
+00000d20: 7074 2f70 6561 6b22 2074 6172 6765 743d  pt/peak" target=
+00000d30: 225f 626c 616e 6b22 3e64 6f63 756d 656e  "_blank">documen
+00000d40: 7461 7469 6f6e 3c2f 613e 2e0a 0a23 2323  tation</a>...###
+00000d50: 2048 656c 6c6f 2057 6f72 6c64 2041 6765   Hello World Age
+00000d60: 6e74 2045 7861 6d70 6c65 0a0a 4f6e 6520  nt Example..One 
+00000d70: 7468 696e 6720 7468 6174 2077 6173 2061  thing that was a
+00000d80: 6464 6564 2069 6e20 5045 414b 2077 6173  dded in PEAK was
+00000d90: 2074 6865 2077 6179 2074 6865 2075 7365   the way the use
+00000da0: 7220 6578 6563 7574 6573 2074 6865 2061  r executes the a
+00000db0: 6765 6e74 732e 2050 4541 4b20 6164 6465  gents. PEAK adde
+00000dc0: 6420 6120 434c 492c 2069 6e73 7069 7265  d a CLI, inspire
+00000dd0: 6420 696e 204a 4144 452c 2074 6f20 6865  d in JADE, to he
+00000de0: 6c70 2074 6865 2075 7365 7220 6578 6563  lp the user exec
+00000df0: 7574 6520 656e 6420 636f 6e66 6967 7572  ute end configur
+00000e00: 6520 6561 6368 2061 6765 6e74 2069 6e20  e each agent in 
+00000e10: 6120 6561 7379 2061 6e64 2069 6e74 7569  a easy and intui
+00000e20: 7469 7665 206d 616e 6e65 722e 0a49 6e20  tive manner..In 
+00000e30: 7468 6973 2065 7861 6d70 6c65 2077 6520  this example we 
+00000e40: 7769 6c6c 2073 686f 7720 796f 7520 686f  will show you ho
+00000e50: 7720 746f 2065 7865 6375 7465 2061 2073  w to execute a s
+00000e60: 696e 676c 6520 6167 656e 742e 2053 6176  ingle agent. Sav
+00000e70: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00000e80: 636f 6465 2069 6e20 6120 6669 6c65 2063  code in a file c
+00000e90: 616c 6c65 6420 6061 6765 6e74 2e70 7960  alled `agent.py`
+00000ea0: 2e0a 0a60 6060 7079 7468 6f6e 200a 6672  ...```python .fr
+00000eb0: 6f6d 2070 6561 6b20 696d 706f 7274 2041  om peak import A
+00000ec0: 6765 6e74 0a66 726f 6d20 7065 616b 2e62  gent.from peak.b
+00000ed0: 6568 6176 696f 7572 7320 696d 706f 7274  ehaviours import
+00000ee0: 204f 6e65 5368 6f74 4265 6861 7669 6f75   OneShotBehaviou
+00000ef0: 720a 0a63 6c61 7373 2061 6765 6e74 2841  r..class agent(A
+00000f00: 6765 6e74 293a 0ac2 a020 c2a0 2063 6c61  gent):... .. cla
+00000f10: 7373 2048 656c 6c6f 576f 726c 6428 4f6e  ss HelloWorld(On
+00000f20: 6553 686f 7442 6568 6176 696f 7572 293a  eShotBehaviour):
+00000f30: 0ac2 a020 c2a0 20c2 a020 c2a0 2061 7379  ... .. .. .. asy
+00000f40: 6e63 2064 6566 2072 756e 2873 656c 6629  nc def run(self)
+00000f50: 202d 3e20 4e6f 6e65 3a0a c2a0 20c2 a020   -> None:... .. 
+00000f60: c2a0 20c2 a020 c2a0 20c2 a020 7072 696e  .. .. .. .. prin
+00000f70: 7428 2248 656c 6c6f 2057 6f72 6c64 2229  t("Hello World")
+00000f80: 0ac2 a020 c2a0 20c2 a020 c2a0 20c2 a020  ... .. .. .. .. 
+00000f90: c2a0 2061 7761 6974 2073 656c 662e 6167  .. await self.ag
+00000fa0: 656e 742e 7374 6f70 2829 0a0a c2a0 20c2  ent.stop().... .
+00000fb0: a020 6173 796e 6320 6465 6620 7365 7475  . async def setu
+00000fc0: 7028 7365 6c66 2920 2d3e 204e 6f6e 653a  p(self) -> None:
+00000fd0: 0ac2 a020 c2a0 20c2 a020 c2a0 2073 656c  ... .. .. .. sel
+00000fe0: 662e 6164 645f 6265 6861 7669 6f75 7228  f.add_behaviour(
+00000ff0: 7365 6c66 2e48 656c 6c6f 576f 726c 6428  self.HelloWorld(
+00001000: 2929 0a60 6060 0a49 7420 6973 206e 6563  )).```.It is nec
+00001010: 6573 7361 7279 2074 6861 7420 7468 6520  essary that the 
+00001020: 6e61 6d65 206f 6620 7468 6520 6669 6c65  name of the file
+00001030: 2069 7320 7468 6520 7361 6d65 2061 7320   is the same as 
+00001040: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
+00001050: 6167 656e 7427 7320 636c 6173 7320 736f  agent's class so
+00001060: 2050 4541 4b20 6361 6e20 646f 2074 6865   PEAK can do the
+00001070: 2070 726f 7065 7220 7061 7273 696e 672e   proper parsing.
+00001080: 2054 6869 7320 6167 656e 7420 6f6e 6c79   This agent only
+00001090: 2068 6173 2061 2062 6568 6176 696f 7220   has a behavior 
+000010a0: 7468 6174 2070 7269 6e74 7320 746f 2074  that prints to t
+000010b0: 6865 2074 6572 6d69 6e61 6c20 7468 6520  he terminal the 
+000010c0: 2248 656c 6c6f 2057 6f72 6c64 2220 6d65  "Hello World" me
+000010d0: 7373 6167 652e 2054 6f20 6578 6563 7574  ssage. To execut
+000010e0: 6520 7468 6520 6167 656e 7420 6a75 7374  e the agent just
+000010f0: 2074 7970 6520 7468 6520 666f 6c6c 6f77   type the follow
+00001100: 696e 6720 636f 6d6d 616e 643a 0a60 6060  ing command:.```
+00001110: 6261 7368 200a 2420 7065 616b 2072 756e  bash .$ peak run
+00001120: 2070 6174 682f 746f 2f61 6765 6e74 2e70   path/to/agent.p
+00001130: 7920 2d6a 2061 6765 6e74 406c 6f63 616c  y -j agent@local
+00001140: 686f 7374 0a60 6060 0a43 6861 6e67 6520  host.```.Change 
+00001150: 7468 6520 606c 6f63 616c 686f 7374 6020  the `localhost` 
+00001160: 746f 2074 6865 2064 6f6d 6169 6e20 6f66  to the domain of
+00001170: 2074 6865 2058 4d50 5020 7365 7276 6572   the XMPP server
+00001180: 2079 6f75 2077 616e 7420 746f 2063 6f6e   you want to con
+00001190: 6e65 6374 2e0a 0a3c 6465 7461 696c 733e  nect...<details>
+000011a0: 3c73 756d 6d61 7279 3e4e 6f74 653c 2f73  <summary>Note</s
+000011b0: 756d 6d61 7279 3e0a 3c70 3e0a 0a49 6620  ummary>.<p>..If 
+000011c0: 796f 7520 7761 6e74 2074 6f20 6b6e 6f77  you want to know
+000011d0: 206d 6f72 6520 6162 6f75 7420 6561 6368   more about each
+000011e0: 2063 6f6d 6d61 6e64 2077 6520 7265 636f   command we reco
+000011f0: 6d6d 656e 6420 7265 6164 696e 6720 7468  mmend reading th
+00001200: 6520 5b64 6f63 756d 656e 7461 7469 6f6e  e [documentation
+00001210: 5d28 6874 7470 3a2f 2f77 7777 2e67 6563  ](http://www.gec
+00001220: 6164 2e69 7365 702e 6970 702e 7074 2f70  ad.isep.ipp.pt/p
+00001230: 6561 6b29 206f 7220 7573 696e 6720 7468  eak) or using th
+00001240: 6520 602d 6860 206f 7074 696f 6e20 746f  e `-h` option to
+00001250: 2073 6565 2074 6865 2068 656c 7020 6d65   see the help me
+00001260: 7373 6167 652e 0a0a 3c2f 703e 0a3c 2f64  ssage...</p>.</d
+00001270: 6574 6169 6c73 3e0a 0a46 6f72 206d 6f72  etails>..For mor
+00001280: 6520 6164 7661 6e63 6564 2066 756e 6374  e advanced funct
+00001290: 696f 6e61 6c69 7469 6573 2061 6e64 2065  ionalities and e
+000012a0: 7861 6d70 6c65 7320 7765 2072 6563 6f6d  xamples we recom
+000012b0: 6d65 6e64 2079 6f75 2074 6f20 6865 6164  mend you to head
+000012c0: 2066 6f72 7761 7264 2074 6f20 7468 6520   forward to the 
+000012d0: 3c61 2068 7265 663d 2268 7474 703a 2f2f  <a href="http://
+000012e0: 7777 772e 6765 6361 642e 6973 6570 2e69  www.gecad.isep.i
+000012f0: 7070 2e70 742f 7065 616b 2220 7461 7267  pp.pt/peak" targ
+00001300: 6574 3d22 5f62 6c61 6e6b 223e 646f 6375  et="_blank">docu
+00001310: 6d65 6e74 6174 696f 6e20 7765 6273 6974  mentation websit
+00001320: 653c 2f61 3e2e 0a0a 0a23 2320 5375 7070  e</a>....## Supp
+00001330: 6f72 740a 0a55 7365 2074 6865 203c 6120  ort..Use the <a 
+00001340: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001350: 7468 7562 2e63 6f6d 2f67 6563 6164 2d67  thub.com/gecad-g
+00001360: 726f 7570 2f70 6561 6b2d 6d61 732f 6469  roup/peak-mas/di
+00001370: 7363 7573 7369 6f6e 7322 2074 6172 6765  scussions" targe
+00001380: 743d 225f 626c 616e 6b22 3e44 6973 6375  t="_blank">Discu
+00001390: 7373 696f 6e3c 2f61 3e20 7061 6765 2069  ssion</a> page i
+000013a0: 6620 796f 7520 6861 7665 2061 6e79 2071  f you have any q
+000013b0: 7565 7374 696f 6e73 206f 7220 6964 6561  uestions or idea
+000013c0: 7320 796f 7520 776f 756c 6420 6c69 6b65  s you would like
+000013d0: 2073 6f20 7365 6520 696d 706c 656d 656e   so see implemen
+000013e0: 7465 642e 0a54 6f20 616c 6572 7420 616e  ted..To alert an
+000013f0: 2069 7373 7565 206f 7220 6120 6275 6720   issue or a bug 
+00001400: 706c 6561 7365 2070 6f73 7420 696e 2074  please post in t
+00001410: 6865 203c 6120 6872 6566 3d22 6874 7470  he <a href="http
+00001420: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
+00001430: 6563 6164 2d67 726f 7570 2f70 6561 6b2d  ecad-group/peak-
+00001440: 6d61 732f 6973 7375 6573 2220 7461 7267  mas/issues" targ
+00001450: 6574 3d22 5f62 6c61 6e6b 223e 4973 7375  et="_blank">Issu
+00001460: 6573 3c2f 613e 2070 6167 652e 0a0a 2323  es</a> page...##
+00001470: 2052 6f61 646d 6170 0a0a 5468 6973 2061   Roadmap..This a
+00001480: 7265 2073 6f6d 6520 6675 6e63 7469 6f6e  re some function
+00001490: 616c 6974 6965 7320 7468 6174 2061 7265  alities that are
+000014a0: 2062 6569 6e67 2064 6576 656c 6f70 6564   being developed
+000014b0: 2061 6e64 2077 696c 6c20 6265 2072 656c   and will be rel
+000014c0: 6561 7365 6420 696e 2061 206e 6561 7220  eased in a near 
+000014d0: 6675 7475 7265 3a0a 2d20 5b20 5d20 4372  future:.- [ ] Cr
+000014e0: 6561 7465 2061 2044 6f63 6b65 7220 666f  eate a Docker fo
+000014f0: 7220 584d 5050 2073 6572 7665 7220 616e  r XMPP server an
+00001500: 6420 5045 414b 2e0a 2d20 5b20 5d20 4164  d PEAK..- [ ] Ad
+00001510: 6420 6479 6e61 6d69 6320 7370 6565 6420  d dynamic speed 
+00001520: 6f70 7469 6f6e 2074 6f20 5045 414b 2773  option to PEAK's
+00001530: 2069 6e74 6572 6e61 6c20 636c 6f63 6b2e   internal clock.
+00001540: 0a2d 205b 205d 2041 6464 206d 756c 7469  .- [ ] Add multi
+00001550: 2d74 6872 6561 6469 6e67 206f 7074 696f  -threading optio
+00001560: 6e20 746f 2074 6865 2065 7865 6375 7469  n to the executi
+00001570: 6f6e 2063 6f6e 6669 6775 7261 7469 6f6e  on configuration
+00001580: 732e 0a2d 205b 205d 2049 6d70 6c65 6d65  s..- [ ] Impleme
+00001590: 6e74 2059 656c 6c6f 7720 5061 6765 2053  nt Yellow Page S
+000015a0: 6572 7669 6365 2069 6e20 4446 2061 6765  ervice in DF age
+000015b0: 6e74 2e0a 2d20 5b20 5d20 496d 706c 656d  nt..- [ ] Implem
+000015c0: 656e 7420 4461 7461 2041 6e61 6c79 7369  ent Data Analysi
+000015d0: 7320 7365 6374 696f 6e20 696e 2074 6865  s section in the
+000015e0: 2044 6173 6862 6f61 7264 2e0a 0a23 2320   Dashboard...## 
+000015f0: 5363 6965 6e74 6966 6963 2050 7562 6c69  Scientific Publi
+00001600: 6361 7469 6f6e 730a 0a2d 2052 6962 6569  cations..- Ribei
+00001610: 726f 2c20 422e 2c20 5065 7265 6972 612c  ro, B., Pereira,
+00001620: 2048 2e2c 2047 6f6d 6573 2c20 4c2e 2c20   H., Gomes, L., 
+00001630: 5661 6c65 2c20 5a2e 2028 3230 3233 292e  Vale, Z. (2023).
+00001640: 2050 7974 686f 6e2d 4261 7365 6420 4563   Python-Based Ec
+00001650: 6f73 7973 7465 6d20 666f 7220 4167 656e  osystem for Agen
+00001660: 7420 436f 6d6d 756e 6974 6965 7320 5369  t Communities Si
+00001670: 6d75 6c61 7469 6f6e 2e20 496e 3a20 2cc2  mulation. In: ,.
+00001680: a05f 6574 2061 6c2e 5fc2 a031 3774 6820  ._et al._..17th 
+00001690: 496e 7465 726e 6174 696f 6e61 6c20 436f  International Co
+000016a0: 6e66 6572 656e 6365 206f 6e20 536f 6674  nference on Soft
+000016b0: 2043 6f6d 7075 7469 6e67 204d 6f64 656c   Computing Model
+000016c0: 7320 696e 2049 6e64 7573 7472 6961 6c20  s in Industrial 
+000016d0: 616e 6420 456e 7669 726f 6e6d 656e 7461  and Environmenta
+000016e0: 6c20 4170 706c 6963 6174 696f 6e73 2028  l Applications (
+000016f0: 534f 434f 2032 3032 3229 2e20 534f 434f  SOCO 2022). SOCO
+00001700: 2032 3032 322e 204c 6563 7475 7265 204e   2022. Lecture N
+00001710: 6f74 6573 2069 6e20 4e65 7477 6f72 6b73  otes in Networks
+00001720: 2061 6e64 2053 7973 7465 6d73 2c20 766f   and Systems, vo
+00001730: 6c20 3533 312e 2053 7072 696e 6765 722c  l 531. Springer,
+00001740: 2043 6861 6d2e 2068 7474 7073 3a2f 2f64   Cham. https://d
+00001750: 6f69 2e6f 7267 2f31 302e 3130 3037 2f39  oi.org/10.1007/9
+00001760: 3738 2d33 2d30 3331 2d31 3830 3530 2d37  78-3-031-18050-7
+00001770: 5f37 0a0a 2323 2043 6f6e 7472 6962 7574  _7..## Contribut
+00001780: 696e 6720 746f 2050 4541 4b0a 0a50 756c  ing to PEAK..Pul
+00001790: 6c20 7265 7175 6573 7473 2061 7265 2077  l requests are w
+000017a0: 656c 636f 6d65 2e20 466f 7220 6d61 6a6f  elcome. For majo
+000017b0: 7220 6368 616e 6765 732c 2070 6c65 6173  r changes, pleas
+000017c0: 6520 6f70 656e 2061 2064 6973 6375 7373  e open a discuss
+000017d0: 696f 6e20 6669 7273 7420 746f 2064 6973  ion first to dis
+000017e0: 6375 7373 2077 6861 7420 796f 7520 776f  cuss what you wo
+000017f0: 756c 6420 6c69 6b65 2074 6f20 6368 616e  uld like to chan
+00001800: 6765 2e0a 0a54 6865 2065 7861 6d70 6c65  ge...The example
+00001810: 7320 6172 6520 7573 6564 2061 7320 6120  s are used as a 
+00001820: 666f 726d 206f 6620 7465 7374 696e 6720  form of testing 
+00001830: 7468 6520 6672 616d 6577 6f72 6b2e 2053  the framework. S
+00001840: 6f20 706c 6561 7365 206d 616b 6520 7375  o please make su
+00001850: 7265 2074 6f20 7570 6461 7465 2074 6865  re to update the
+00001860: 2065 7861 6d70 6c65 7320 6173 2061 7070   examples as app
+00001870: 726f 7072 6961 7465 206f 7220 6d61 6b65  ropriate or make
+00001880: 206e 6577 206f 6e65 732e 200a 0a54 6f20   new ones. ..To 
+00001890: 666f 726d 6174 2074 6865 2063 6f64 6520  format the code 
+000018a0: 706c 6561 7365 2075 7365 2074 6865 203c  please use the <
+000018b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000018c0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000018d0: 2f62 6c61 636b 2f22 2074 6172 6765 743d  /black/" target=
+000018e0: 225f 626c 616e 6b22 3e62 6c61 636b 3c2f  "_blank">black</
+000018f0: 613e 2061 6e64 203c 6120 6872 6566 3d22  a> and <a href="
+00001900: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00001910: 2f70 726f 6a65 6374 2f69 736f 7274 2f22  /project/isort/"
+00001920: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00001930: 3e69 736f 7274 3c2f 613e 2070 6163 6b61  >isort</a> packa
+00001940: 6765 732e 200a 0a46 6f72 2074 6865 2063  ges. ..For the c
+00001950: 6f6d 6d69 7473 2070 6c65 6173 6520 666f  ommits please fo
+00001960: 6c6c 6f77 2074 6865 203c 6120 6872 6566  llow the <a href
+00001970: 3d22 7777 772e 636f 6e76 656e 7469 6f6e  ="www.convention
+00001980: 616c 636f 6d6d 6974 732e 6f72 6722 2074  alcommits.org" t
+00001990: 6172 6765 743d 225f 626c 616e 6b22 3e43  arget="_blank">C
+000019a0: 6f6e 7665 6e74 696f 6e61 6c20 436f 6d6d  onventional Comm
+000019b0: 6974 7320 4775 6964 656c 696e 653c 2f61  its Guideline</a
+000019c0: 3e2e 0a0a 2323 204c 6963 656e 7365 0a0a  >...## License..
+000019d0: 6050 4541 4b60 c2a0 6973 2066 7265 6520  `PEAK`..is free 
+000019e0: 616e 6420 6f70 656e 2d73 6f75 7263 6520  and open-source 
+000019f0: 736f 6674 7761 7265 206c 6963 656e 7365  software license
+00001a00: 6420 756e 6465 7220 7468 6520 3c61 2068  d under the <a h
+00001a10: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00001a20: 6875 622e 636f 6d2f 6765 6361 642d 6772  hub.com/gecad-gr
+00001a30: 6f75 702f 7065 616b 2d6d 6173 2f62 6c6f  oup/peak-mas/blo
+00001a40: 622f 6465 7665 6c6f 702f 4c49 4345 4e53  b/develop/LICENS
+00001a50: 4522 2074 6172 6765 743d 225f 626c 616e  E" target="_blan
+00001a60: 6b22 3e47 4e55 2047 656e 6572 616c 2050  k">GNU General P
+00001a70: 7562 6c69 6320 4c69 6365 6e73 6520 7633  ublic License v3
+00001a80: 2e30 3c2f 613e 2e0a                      .0</a>..
```

### Comparing `peak-mas-1.0.4/README.md` & `peak-mas-1.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,372 +1,366 @@
 00000000: 2320 5045 414b 3a20 5079 7468 6f6e 2d62  # PEAK: Python-b
 00000010: 6173 6564 2066 7261 6d65 776f 726b 2066  ased framework f
 00000020: 6f72 2068 6574 6572 6f67 656e 6f75 7320  or heterogenous 
 00000030: 6167 656e 7420 636f 6d6d 756e 6974 6965  agent communitie
-00000040: 730d 0a0d 0a21 5b44 4f49 5d28 6874 7470  s....![DOI](http
-00000050: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000060: 696f 2f73 7461 7469 632f 7631 3f6c 696e  io/static/v1?lin
-00000070: 6b3d 6874 7470 733a 2f2f 646f 692e 6f72  k=https://doi.or
-00000080: 672f 3130 2e31 3030 372f 3937 382d 332d  g/10.1007/978-3-
-00000090: 3033 312d 3138 3035 302d 375f 3726 6c69  031-18050-7_7&li
-000000a0: 6e6b 3d68 7474 7073 3a2f 2f64 6f69 2e6f  nk=https://doi.o
-000000b0: 7267 2f31 302e 3130 3037 2f39 3738 2d33  rg/10.1007/978-3
-000000c0: 2d30 3331 2d31 3830 3530 2d37 5f37 266c  -031-18050-7_7&l
-000000d0: 6162 656c 3d44 4f49 266d 6573 7361 6765  abel=DOI&message
-000000e0: 3d39 3738 2d33 2d30 3331 2d31 3830 3530  =978-3-031-18050
-000000f0: 2d37 2663 6f6c 6f72 3d62 6c75 6529 2021  -7&color=blue) !
-00000100: 5b50 7950 4920 2d20 5079 7468 6f6e 2056  [PyPI - Python V
-00000110: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
-00000120: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-00000130: 7970 692f 7079 7665 7273 696f 6e73 2f70  ypi/pyversions/p
-00000140: 6561 6b2d 6d61 7329 2021 5b50 7950 495d  eak-mas) ![PyPI]
-00000150: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000160: 656c 6473 2e69 6f2f 7079 7069 2f76 2f70  elds.io/pypi/v/p
-00000170: 6561 6b2d 6d61 7329 2021 5b47 6974 4875  eak-mas) ![GitHu
-00000180: 625d 2868 7474 7073 3a2f 2f69 6d67 2e73  b](https://img.s
-00000190: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-000001a0: 2f6c 6963 656e 7365 2f67 6563 6164 2d67  /license/gecad-g
-000001b0: 726f 7570 2f70 6561 6b2d 6d61 7329 2021  roup/peak-mas) !
-000001c0: 5b70 6f77 6572 6564 2062 795d 2868 7474  [powered by](htt
-000001d0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000001e0: 2e69 6f2f 7374 6174 6963 2f76 313f 6c61  .io/static/v1?la
-000001f0: 6265 6c3d 706f 7765 7265 6425 3230 6279  bel=powered%20by
-00000200: 266d 6573 7361 6765 3d47 4543 4144 2663  &message=GECAD&c
-00000210: 6f6c 6f72 3d31 3737 3938 3526 6c61 6265  olor=177985&labe
-00000220: 6c43 6f6c 6f72 3d64 6535 6434 6126 3f6c  lColor=de5d4a&?l
-00000230: 696e 6b3d 6874 7470 3a2f 2f67 6563 6164  ink=http://gecad
-00000240: 2e69 7365 702e 6970 702e 7074 266c 696e  .isep.ipp.pt&lin
-00000250: 6b3d 6874 7470 3a2f 2f67 6563 6164 2e69  k=http://gecad.i
-00000260: 7365 702e 6970 702e 7074 2f29 2021 5b63  sep.ipp.pt/) ![c
-00000270: 6f64 6520 7374 796c 655d 2868 7474 7073  ode style](https
-00000280: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000290: 6f2f 6261 6467 652f 636f 6465 2532 3073  o/badge/code%20s
-000002a0: 7479 6c65 2d62 6c61 636b 2d62 6c61 636b  tyle-black-black
-000002b0: 2920 215b 696d 706f 7274 7320 6973 6f72  ) ![imports isor
-000002c0: 745d 2868 7474 7073 3a2f 2f69 6d67 2e73  t](https://img.s
-000002d0: 6869 656c 6473 2e69 6f2f 7374 6174 6963  hields.io/static
-000002e0: 2f76 313f 6c61 6265 6c3d 696d 706f 7274  /v1?label=import
-000002f0: 7326 6d65 7373 6167 653d 6973 6f72 7426  s&message=isort&
-00000300: 636f 6c6f 723d 626c 7565 266c 6162 656c  color=blue&label
-00000310: 436f 6c6f 723d 6f72 616e 6765 290d 0a0d  Color=orange)...
-00000320: 0a50 4541 4b20 6973 2061 206d 756c 7469  .PEAK is a multi
-00000330: 2d61 6765 6e74 2073 7973 7465 6d20 6672  -agent system fr
-00000340: 616d 6577 6f72 6b20 7768 6963 6820 6865  amework which he
-00000350: 6c70 7320 7468 6520 7573 6572 7320 6465  lps the users de
-00000360: 7665 6c6f 702c 206d 6f6e 6974 6f72 2c20  velop, monitor, 
-00000370: 616e 616c 797a 6520 616e 6420 6d61 696e  analyze and main
-00000380: 7461 696e 2065 636f 7379 7374 656d 206f  tain ecosystem o
-00000390: 6620 6865 7465 726f 6765 6e65 6f75 7320  f heterogeneous 
-000003a0: 6167 656e 7420 636f 6d6d 756e 6974 6965  agent communitie
-000003b0: 732e 2054 6869 7320 6563 6f73 7973 7465  s. This ecosyste
-000003c0: 6d20 6973 2020 7768 6572 6520 7661 7269  m is  where vari
-000003d0: 6f75 7320 6d75 6c74 692d 6167 656e 7420  ous multi-agent 
-000003e0: 7379 7374 656d 7320 6361 6e20 636f 6578  systems can coex
-000003f0: 6973 742c 2069 6e74 6572 6163 7420 616e  ist, interact an
-00000400: 6420 7368 6172 6520 7265 736f 7572 6365  d share resource
-00000410: 7320 6265 7477 6565 6e20 7468 656d 2e20  s between them. 
-00000420: 0d0a 5468 6973 2066 7261 6d65 776f 726b  ..This framework
-00000430: 2069 7320 6261 7365 6420 6f6e 203c 6120   is based on <a 
-00000440: 6872 6566 3d22 6874 7470 733a 2f2f 7370  href="https://sp
-00000450: 6164 652d 6d61 732e 7265 6164 7468 6564  ade-mas.readthed
-00000460: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00000470: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
-00000480: 6b22 3e53 5041 4445 3c2f 613e 2e0d 0a0d  k">SPADE</a>....
-00000490: 0a0d 0a23 2320 5072 6572 6571 7569 7369  ...## Prerequisi
-000004a0: 7465 730d 0a0d 0a2d 2050 7974 686f 6e20  tes....- Python 
-000004b0: 3d3d 2033 2e39 2e36 0d0a 2d20 584d 5050  == 3.9.6..- XMPP
-000004c0: 2053 6572 7665 7220 285b 7365 6520 646f   Server ([see do
-000004d0: 6373 5d28 6874 7470 733a 2f2f 7777 772e  cs](https://www.
-000004e0: 6765 6361 642e 6973 6570 2e69 7070 2e70  gecad.isep.ipp.p
-000004f0: 742f 7065 616b 2929 0d0a 0d0a 0d0a 2323  t/peak))......##
-00000500: 2049 6e73 7461 6c6c 696e 6720 5045 414b   Installing PEAK
-00000510: 0d0a 0d0a 2323 2320 436f 6e64 610d 0a0d  ....### Conda...
-00000520: 0a54 6f20 696e 7374 616c 6c20 7573 696e  .To install usin
-00000530: 6720 636f 6e64 612c 2064 6f77 6e6c 6f61  g conda, downloa
-00000540: 6420 7468 6520 656e 7669 726f 6e6d 656e  d the environmen
-00000550: 742e 796d 6c20 6669 6c65 2066 726f 6d20  t.yml file from 
-00000560: 7468 6520 7265 706f 7369 746f 7279 2061  the repository a
-00000570: 6e64 2074 6865 6e20 7573 6520 7468 6520  nd then use the 
-00000580: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
-00000590: 643a 0d0a 6060 6062 6173 680d 0a24 2063  d:..```bash..$ c
-000005a0: 6f6e 6461 2065 6e76 2063 7265 6174 6520  onda env create 
-000005b0: 2d2d 6669 6c65 2065 6e76 6972 6f6e 6d65  --file environme
-000005c0: 6e74 2e79 6d6c 090d 0a60 6060 0d0a 5468  nt.yml...```..Th
-000005d0: 6973 2077 696c 6c20 6372 6561 7465 2061  is will create a
-000005e0: 2063 6f6e 6461 2065 6e76 6972 6f6e 6d65   conda environme
-000005f0: 6e74 2063 616c 6c65 6420 5f70 6561 6b5f  nt called _peak_
-00000600: 2e0d 0a0d 0a23 2323 2050 6970 0d0a 0d0a  .....### Pip....
-00000610: 546f 2069 6e73 7461 6c6c 2075 7369 6e67  To install using
-00000620: 2070 6970 2c20 6a75 7374 2074 7970 6520   pip, just type 
-00000630: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00000640: 6d6d 616e 643a 0d0a 6060 6062 6173 680d  mmand:..```bash.
-00000650: 0a24 2070 6970 2069 6e73 7461 6c6c 2070  .$ pip install p
-00000660: 6561 6b2d 6d61 730d 0a60 6060 0d0a 0d0a  eak-mas..```....
-00000670: 0d0a 2323 2055 7369 6e67 2050 4541 4b0d  ..## Using PEAK.
-00000680: 0a0d 0a23 2323 204e 6f74 6573 206f 6e20  ...### Notes on 
-00000690: 5350 4144 450d 0a0d 0a41 7320 616c 7265  SPADE....As alre
-000006a0: 6164 7920 7361 6964 2050 4541 4b20 6973  ady said PEAK is
-000006b0: 2062 6173 6564 206f 6e20 5350 4144 452e   based on SPADE.
-000006c0: 2054 6869 7320 6d65 616e 7320 7468 6174   This means that
-000006d0: 2065 7665 7279 2066 756e 6374 696f 6e61   every functiona
-000006e0: 6c69 7479 206f 6620 5350 4144 4520 6973  lity of SPADE is
-000006f0: 2061 7661 696c 6162 6c65 2074 6f20 7468   available to th
-00000700: 6520 7573 6572 2e20 5765 2068 6967 686c  e user. We highl
-00000710: 7920 7265 636f 6d6d 656e 6420 796f 7520  y recommend you 
-00000720: 746f 2073 6565 203c 6120 6872 6566 3d22  to see <a href="
-00000730: 6874 7470 733a 2f2f 7370 6164 652d 6d61  https://spade-ma
-00000740: 732e 7265 6164 7468 6564 6f63 732e 696f  s.readthedocs.io
-00000750: 2f65 6e2f 6c61 7465 7374 2f22 2074 6172  /en/latest/" tar
-00000760: 6765 743d 225f 626c 616e 6b22 3e53 5041  get="_blank">SPA
-00000770: 4445 3c2f 613e 2065 7861 6d70 6c65 7320  DE</a> examples 
-00000780: 616e 6420 646f 6375 6d65 6e74 6174 696f  and documentatio
-00000790: 6e20 6265 666f 7265 2073 7461 7274 696e  n before startin
-000007a0: 6720 7573 696e 6720 5045 414b 2e20 4f6e  g using PEAK. On
-000007b0: 6365 2079 6f75 2061 7265 2066 616d 696c  ce you are famil
-000007c0: 6961 7269 7a65 6420 7769 7468 2053 5041  iarized with SPA
-000007d0: 4445 2773 206d 6563 6861 6e69 6373 2079  DE's mechanics y
-000007e0: 6f75 2063 616e 2073 7461 7274 2075 7369  ou can start usi
-000007f0: 6e67 2050 4541 4b2e 0d0a 0d0a 2323 2320  ng PEAK.....### 
-00000800: 4e6f 7465 7320 6f6e 2058 4d50 500d 0a0d  Notes on XMPP...
-00000810: 0a54 6f20 7275 6e20 616e 7920 5045 414b  .To run any PEAK
-00000820: 2773 2061 6765 6e74 2079 6f75 2077 696c  's agent you wil
-00000830: 6c20 6e65 6564 2061 2058 4d50 5020 7365  l need a XMPP se
-00000840: 7276 6572 2e20 596f 7520 6361 6e20 6569  rver. You can ei
-00000850: 7468 6572 2063 6f6e 6669 6775 7265 206f  ther configure o
-00000860: 6e65 206f 6e20 796f 7572 206d 6163 6869  ne on your machi
-00000870: 6e65 2c20 7265 6d6f 7465 6c79 206f 7220  ne, remotely or 
-00000880: 7573 6520 6120 7075 626c 6963 2073 6572  use a public ser
-00000890: 7665 722e 2054 6865 206f 6e6c 7920 6973  ver. The only is
-000008a0: 7375 6520 7769 7468 2074 6865 2070 7562  sue with the pub
-000008b0: 6c69 6320 7365 7276 6572 7320 6973 2074  lic servers is t
-000008c0: 6861 7420 7468 6579 2064 6f6e 2774 2075  hat they don't u
-000008d0: 7375 616c 6c79 2068 6176 6520 616c 6c20  sually have all 
-000008e0: 7468 6520 636f 6e66 6967 7572 6174 696f  the configuratio
-000008f0: 6e73 2072 6571 7569 7265 6420 746f 2072  ns required to r
-00000900: 756e 2073 6f6d 6520 5045 414b 2773 2066  un some PEAK's f
-00000910: 756e 6374 696f 6e61 6c69 7469 6573 2e20  unctionalities. 
-00000920: 546f 2063 6f6e 6669 6775 7265 2074 6865  To configure the
-00000930: 2073 6572 7665 7220 796f 7520 6361 6e20   server you can 
-00000940: 7265 6164 2074 6865 2022 436f 6e66 6967  read the "Config
-00000950: 7572 6520 584d 5050 2073 6572 7665 7222  ure XMPP server"
-00000960: 2073 6563 7469 6f6e 2069 6e20 7468 6520   section in the 
-00000970: 3c61 2068 7265 663d 2268 7474 703a 2f2f  <a href="http://
-00000980: 7777 772e 6765 6361 642e 6973 6570 2e69  www.gecad.isep.i
-00000990: 7070 2e70 742f 7065 616b 2220 7461 7267  pp.pt/peak" targ
-000009a0: 6574 3d22 5f62 6c61 6e6b 223e 646f 6375  et="_blank">docu
-000009b0: 6d65 6e74 6174 696f 6e3c 2f61 3e2e 0d0a  mentation</a>...
-000009c0: 0d0a 2323 2320 4865 6c6c 6f20 576f 726c  ..### Hello Worl
-000009d0: 6420 4167 656e 7420 4578 616d 706c 650d  d Agent Example.
-000009e0: 0a0d 0a4f 6e65 2074 6869 6e67 2074 6861  ...One thing tha
-000009f0: 7420 7761 7320 6164 6465 6420 696e 2050  t was added in P
-00000a00: 4541 4b20 7761 7320 7468 6520 7761 7920  EAK was the way 
-00000a10: 7468 6520 7573 6572 2065 7865 6375 7465  the user execute
-00000a20: 7320 7468 6520 6167 656e 7473 2e20 5045  s the agents. PE
-00000a30: 414b 2061 6464 6564 2061 2043 4c49 2c20  AK added a CLI, 
-00000a40: 696e 7370 6972 6564 2069 6e20 4a41 4445  inspired in JADE
-00000a50: 2c20 746f 2068 656c 7020 7468 6520 7573  , to help the us
-00000a60: 6572 2065 7865 6375 7465 2065 6e64 2063  er execute end c
-00000a70: 6f6e 6669 6775 7265 2065 6163 6820 6167  onfigure each ag
-00000a80: 656e 7420 696e 2061 2065 6173 7920 616e  ent in a easy an
-00000a90: 6420 696e 7475 6974 6976 6520 6d61 6e6e  d intuitive mann
-00000aa0: 6572 2e0d 0a49 6e20 7468 6973 2065 7861  er...In this exa
-00000ab0: 6d70 6c65 2077 6520 7769 6c6c 2073 686f  mple we will sho
-00000ac0: 7720 796f 7520 686f 7720 746f 2065 7865  w you how to exe
-00000ad0: 6375 7465 2061 2073 696e 676c 6520 6167  cute a single ag
-00000ae0: 656e 742e 2053 6176 6520 7468 6520 666f  ent. Save the fo
-00000af0: 6c6c 6f77 696e 6720 636f 6465 2069 6e20  llowing code in 
-00000b00: 6120 6669 6c65 2063 616c 6c65 6420 6061  a file called `a
-00000b10: 6765 6e74 2e70 7960 2e0d 0a0d 0a60 6060  gent.py`.....```
-00000b20: 7079 7468 6f6e 200d 0a66 726f 6d20 7065  python ..from pe
-00000b30: 616b 2069 6d70 6f72 7420 4167 656e 740d  ak import Agent.
-00000b40: 0a66 726f 6d20 7065 616b 2e62 6568 6176  .from peak.behav
-00000b50: 696f 7572 7320 696d 706f 7274 204f 6e65  iours import One
-00000b60: 5368 6f74 4265 6861 7669 6f75 720d 0a0d  ShotBehaviour...
-00000b70: 0a63 6c61 7373 2061 6765 6e74 2841 6765  .class agent(Age
-00000b80: 6e74 293a 0d0a c2a0 20c2 a020 636c 6173  nt):.... .. clas
-00000b90: 7320 4865 6c6c 6f57 6f72 6c64 284f 6e65  s HelloWorld(One
-00000ba0: 5368 6f74 4265 6861 7669 6f75 7229 3a0d  ShotBehaviour):.
-00000bb0: 0ac2 a020 c2a0 20c2 a020 c2a0 2061 7379  ... .. .. .. asy
-00000bc0: 6e63 2064 6566 2072 756e 2873 656c 6629  nc def run(self)
-00000bd0: 202d 3e20 4e6f 6e65 3a0d 0ac2 a020 c2a0   -> None:.... ..
-00000be0: 20c2 a020 c2a0 20c2 a020 c2a0 2070 7269   .. .. .. .. pri
-00000bf0: 6e74 2822 4865 6c6c 6f20 576f 726c 6422  nt("Hello World"
-00000c00: 290d 0ac2 a020 c2a0 20c2 a020 c2a0 20c2  ).... .. .. .. .
-00000c10: a020 c2a0 2061 7761 6974 2073 656c 662e  . .. await self.
-00000c20: 6167 656e 742e 7374 6f70 2829 0d0a 0d0a  agent.stop()....
-00000c30: c2a0 20c2 a020 6173 796e 6320 6465 6620  .. .. async def 
-00000c40: 7365 7475 7028 7365 6c66 2920 2d3e 204e  setup(self) -> N
-00000c50: 6f6e 653a 0d0a c2a0 20c2 a020 c2a0 20c2  one:.... .. .. .
-00000c60: a020 7365 6c66 2e61 6464 5f62 6568 6176  . self.add_behav
-00000c70: 696f 7572 2873 656c 662e 4865 6c6c 6f57  iour(self.HelloW
-00000c80: 6f72 6c64 2829 290d 0a60 6060 0d0a 4974  orld())..```..It
-00000c90: 2069 7320 6e65 6365 7373 6172 7920 7468   is necessary th
-00000ca0: 6174 2074 6865 206e 616d 6520 6f66 2074  at the name of t
-00000cb0: 6865 2066 696c 6520 6973 2074 6865 2073  he file is the s
-00000cc0: 616d 6520 6173 2074 6865 206e 616d 6520  ame as the name 
-00000cd0: 6f66 2074 6865 2061 6765 6e74 2773 2063  of the agent's c
-00000ce0: 6c61 7373 2073 6f20 5045 414b 2063 616e  lass so PEAK can
-00000cf0: 2064 6f20 7468 6520 7072 6f70 6572 2070   do the proper p
-00000d00: 6172 7369 6e67 2e20 5468 6973 2061 6765  arsing. This age
-00000d10: 6e74 206f 6e6c 7920 6861 7320 6120 6265  nt only has a be
-00000d20: 6861 7669 6f72 2074 6861 7420 7072 696e  havior that prin
-00000d30: 7473 2074 6f20 7468 6520 7465 726d 696e  ts to the termin
-00000d40: 616c 2074 6865 2022 4865 6c6c 6f20 576f  al the "Hello Wo
-00000d50: 726c 6422 206d 6573 7361 6765 2e20 546f  rld" message. To
-00000d60: 2065 7865 6375 7465 2074 6865 2061 6765   execute the age
-00000d70: 6e74 206a 7573 7420 7479 7065 2074 6865  nt just type the
-00000d80: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00000d90: 6e64 3a0d 0a60 6060 6261 7368 200d 0a24  nd:..```bash ..$
-00000da0: 2070 6561 6b20 7275 6e20 7061 7468 2f74   peak run path/t
-00000db0: 6f2f 6167 656e 742e 7079 202d 6a20 6167  o/agent.py -j ag
-00000dc0: 656e 7440 6c6f 6361 6c68 6f73 740d 0a60  ent@localhost..`
-00000dd0: 6060 0d0a 4368 616e 6765 2074 6865 2060  ``..Change the `
-00000de0: 6c6f 6361 6c68 6f73 7460 2074 6f20 7468  localhost` to th
-00000df0: 6520 646f 6d61 696e 206f 6620 7468 6520  e domain of the 
-00000e00: 584d 5050 2073 6572 7665 7220 796f 7520  XMPP server you 
-00000e10: 7761 6e74 2074 6f20 636f 6e6e 6563 742e  want to connect.
-00000e20: 0d0a 0d0a 3c64 6574 6169 6c73 3e3c 7375  ....<details><su
-00000e30: 6d6d 6172 793e 4e6f 7465 3c2f 7375 6d6d  mmary>Note</summ
-00000e40: 6172 793e 0d0a 3c70 3e0d 0a0d 0a49 6620  ary>..<p>....If 
-00000e50: 796f 7520 7761 6e74 2074 6f20 6b6e 6f77  you want to know
-00000e60: 206d 6f72 6520 6162 6f75 7420 6561 6368   more about each
-00000e70: 2063 6f6d 6d61 6e64 2077 6520 7265 636f   command we reco
-00000e80: 6d6d 656e 6420 7265 6164 696e 6720 7468  mmend reading th
-00000e90: 6520 5b64 6f63 756d 656e 7461 7469 6f6e  e [documentation
-00000ea0: 5d28 6874 7470 3a2f 2f77 7777 2e67 6563  ](http://www.gec
-00000eb0: 6164 2e69 7365 702e 6970 702e 7074 2f70  ad.isep.ipp.pt/p
-00000ec0: 6561 6b29 206f 7220 7573 696e 6720 7468  eak) or using th
-00000ed0: 6520 602d 6860 206f 7074 696f 6e20 746f  e `-h` option to
-00000ee0: 2073 6565 2074 6865 2068 656c 7020 6d65   see the help me
-00000ef0: 7373 6167 652e 0d0a 0d0a 3c2f 703e 0d0a  ssage.....</p>..
-00000f00: 3c2f 6465 7461 696c 733e 0d0a 0d0a 466f  </details>....Fo
-00000f10: 7220 6d6f 7265 2061 6476 616e 6365 6420  r more advanced 
-00000f20: 6675 6e63 7469 6f6e 616c 6974 6965 7320  functionalities 
-00000f30: 616e 6420 6578 616d 706c 6573 2077 6520  and examples we 
-00000f40: 7265 636f 6d6d 656e 6420 796f 7520 746f  recommend you to
-00000f50: 2068 6561 6420 666f 7277 6172 6420 746f   head forward to
-00000f60: 2074 6865 203c 6120 6872 6566 3d22 6874   the <a href="ht
-00000f70: 7470 3a2f 2f77 7777 2e67 6563 6164 2e69  tp://www.gecad.i
-00000f80: 7365 702e 6970 702e 7074 2f70 6561 6b22  sep.ipp.pt/peak"
-00000f90: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00000fa0: 3e64 6f63 756d 656e 7461 7469 6f6e 2077  >documentation w
-00000fb0: 6562 7369 7465 3c2f 613e 2e0d 0a0d 0a0d  ebsite</a>......
-00000fc0: 0a23 2320 5375 7070 6f72 740d 0a0d 0a55  .## Support....U
-00000fd0: 7365 2074 6865 203c 6120 6872 6566 3d22  se the <a href="
-00000fe0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000ff0: 6f6d 2f67 6563 6164 2d67 726f 7570 2f70  om/gecad-group/p
-00001000: 6561 6b2d 6d61 732f 6469 7363 7573 7369  eak-mas/discussi
-00001010: 6f6e 7322 2074 6172 6765 743d 225f 626c  ons" target="_bl
-00001020: 616e 6b22 3e44 6973 6375 7373 696f 6e3c  ank">Discussion<
-00001030: 2f61 3e20 7061 6765 2069 6620 796f 7520  /a> page if you 
-00001040: 6861 7665 2061 6e79 2071 7565 7374 696f  have any questio
-00001050: 6e73 206f 7220 6964 6561 7320 796f 7520  ns or ideas you 
-00001060: 776f 756c 6420 6c69 6b65 2073 6f20 7365  would like so se
-00001070: 6520 696d 706c 656d 656e 7465 642e 0d0a  e implemented...
-00001080: 546f 2061 6c65 7274 2061 6e20 6973 7375  To alert an issu
-00001090: 6520 6f72 2061 2062 7567 2070 6c65 6173  e or a bug pleas
-000010a0: 6520 706f 7374 2069 6e20 7468 6520 3c61  e post in the <a
-000010b0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-000010c0: 6974 6875 622e 636f 6d2f 6765 6361 642d  ithub.com/gecad-
-000010d0: 6772 6f75 702f 7065 616b 2d6d 6173 2f69  group/peak-mas/i
-000010e0: 7373 7565 7322 2074 6172 6765 743d 225f  ssues" target="_
-000010f0: 626c 616e 6b22 3e49 7373 7565 733c 2f61  blank">Issues</a
-00001100: 3e20 7061 6765 2e0d 0a0d 0a23 2320 526f  > page.....## Ro
-00001110: 6164 6d61 700d 0a0d 0a54 6869 7320 6172  admap....This ar
-00001120: 6520 736f 6d65 2066 756e 6374 696f 6e61  e some functiona
-00001130: 6c69 7469 6573 2074 6861 7420 6172 6520  lities that are 
-00001140: 6265 696e 6720 6465 7665 6c6f 7065 6420  being developed 
-00001150: 616e 6420 7769 6c6c 2062 6520 7265 6c65  and will be rele
-00001160: 6173 6564 2069 6e20 6120 6e65 6172 2066  ased in a near f
-00001170: 7574 7572 653a 0d0a 2d20 5b20 5d20 4372  uture:..- [ ] Cr
-00001180: 6561 7465 2061 2044 6f63 6b65 7220 666f  eate a Docker fo
-00001190: 7220 584d 5050 2073 6572 7665 7220 616e  r XMPP server an
-000011a0: 6420 5045 414b 2e0d 0a2d 205b 205d 2041  d PEAK...- [ ] A
-000011b0: 6464 2064 796e 616d 6963 2073 7065 6564  dd dynamic speed
-000011c0: 206f 7074 696f 6e20 746f 2050 4541 4b27   option to PEAK'
-000011d0: 7320 696e 7465 726e 616c 2063 6c6f 636b  s internal clock
-000011e0: 2e0d 0a2d 205b 205d 2041 6464 206d 756c  ...- [ ] Add mul
-000011f0: 7469 2d74 6872 6561 6469 6e67 206f 7074  ti-threading opt
-00001200: 696f 6e20 746f 2074 6865 2065 7865 6375  ion to the execu
-00001210: 7469 6f6e 2063 6f6e 6669 6775 7261 7469  tion configurati
-00001220: 6f6e 732e 0d0a 2d20 5b20 5d20 496d 706c  ons...- [ ] Impl
-00001230: 656d 656e 7420 5965 6c6c 6f77 2050 6167  ement Yellow Pag
-00001240: 6520 5365 7276 6963 6520 696e 2044 4620  e Service in DF 
-00001250: 6167 656e 742e 0d0a 2d20 5b20 5d20 496d  agent...- [ ] Im
-00001260: 706c 656d 656e 7420 4461 7461 2041 6e61  plement Data Ana
-00001270: 6c79 7369 7320 7365 6374 696f 6e20 696e  lysis section in
-00001280: 2074 6865 2044 6173 6862 6f61 7264 2e0d   the Dashboard..
-00001290: 0a0d 0a23 2320 5363 6965 6e74 6966 6963  ...## Scientific
-000012a0: 2050 7562 6c69 6361 7469 6f6e 730d 0a0d   Publications...
-000012b0: 0a2d 2052 6962 6569 726f 2c20 422e 2c20  .- Ribeiro, B., 
-000012c0: 5065 7265 6972 612c 2048 2e2c 2047 6f6d  Pereira, H., Gom
-000012d0: 6573 2c20 4c2e 2c20 5661 6c65 2c20 5a2e  es, L., Vale, Z.
-000012e0: 2028 3230 3233 292e 2050 7974 686f 6e2d   (2023). Python-
-000012f0: 4261 7365 6420 4563 6f73 7973 7465 6d20  Based Ecosystem 
-00001300: 666f 7220 4167 656e 7420 436f 6d6d 756e  for Agent Commun
-00001310: 6974 6965 7320 5369 6d75 6c61 7469 6f6e  ities Simulation
-00001320: 2e20 496e 3a20 2cc2 a05f 6574 2061 6c2e  . In: ,.._et al.
-00001330: 5fc2 a031 3774 6820 496e 7465 726e 6174  _..17th Internat
-00001340: 696f 6e61 6c20 436f 6e66 6572 656e 6365  ional Conference
-00001350: 206f 6e20 536f 6674 2043 6f6d 7075 7469   on Soft Computi
-00001360: 6e67 204d 6f64 656c 7320 696e 2049 6e64  ng Models in Ind
-00001370: 7573 7472 6961 6c20 616e 6420 456e 7669  ustrial and Envi
-00001380: 726f 6e6d 656e 7461 6c20 4170 706c 6963  ronmental Applic
-00001390: 6174 696f 6e73 2028 534f 434f 2032 3032  ations (SOCO 202
-000013a0: 3229 2e20 534f 434f 2032 3032 322e 204c  2). SOCO 2022. L
-000013b0: 6563 7475 7265 204e 6f74 6573 2069 6e20  ecture Notes in 
-000013c0: 4e65 7477 6f72 6b73 2061 6e64 2053 7973  Networks and Sys
-000013d0: 7465 6d73 2c20 766f 6c20 3533 312e 2053  tems, vol 531. S
-000013e0: 7072 696e 6765 722c 2043 6861 6d2e 2068  pringer, Cham. h
-000013f0: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00001400: 302e 3130 3037 2f39 3738 2d33 2d30 3331  0.1007/978-3-031
-00001410: 2d31 3830 3530 2d37 5f37 0d0a 0d0a 2323  -18050-7_7....##
-00001420: 2043 6f6e 7472 6962 7574 696e 6720 746f   Contributing to
-00001430: 2050 4541 4b0d 0a0d 0a50 756c 6c20 7265   PEAK....Pull re
-00001440: 7175 6573 7473 2061 7265 2077 656c 636f  quests are welco
-00001450: 6d65 2e20 466f 7220 6d61 6a6f 7220 6368  me. For major ch
-00001460: 616e 6765 732c 2070 6c65 6173 6520 6f70  anges, please op
-00001470: 656e 2061 2064 6973 6375 7373 696f 6e20  en a discussion 
-00001480: 6669 7273 7420 746f 2064 6973 6375 7373  first to discuss
-00001490: 2077 6861 7420 796f 7520 776f 756c 6420   what you would 
-000014a0: 6c69 6b65 2074 6f20 6368 616e 6765 2e0d  like to change..
-000014b0: 0a0d 0a54 6865 2065 7861 6d70 6c65 7320  ...The examples 
-000014c0: 6172 6520 7573 6564 2061 7320 6120 666f  are used as a fo
-000014d0: 726d 206f 6620 7465 7374 696e 6720 7468  rm of testing th
-000014e0: 6520 6672 616d 6577 6f72 6b2e 2053 6f20  e framework. So 
-000014f0: 706c 6561 7365 206d 616b 6520 7375 7265  please make sure
-00001500: 2074 6f20 7570 6461 7465 2074 6865 2065   to update the e
-00001510: 7861 6d70 6c65 7320 6173 2061 7070 726f  xamples as appro
-00001520: 7072 6961 7465 206f 7220 6d61 6b65 206e  priate or make n
-00001530: 6577 206f 6e65 732e 200d 0a0d 0a54 6f20  ew ones. ....To 
-00001540: 666f 726d 6174 2074 6865 2063 6f64 6520  format the code 
-00001550: 706c 6561 7365 2075 7365 2074 6865 203c  please use the <
-00001560: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001570: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00001580: 2f62 6c61 636b 2f22 2074 6172 6765 743d  /black/" target=
-00001590: 225f 626c 616e 6b22 3e62 6c61 636b 3c2f  "_blank">black</
-000015a0: 613e 2061 6e64 203c 6120 6872 6566 3d22  a> and <a href="
-000015b0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-000015c0: 2f70 726f 6a65 6374 2f69 736f 7274 2f22  /project/isort/"
-000015d0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-000015e0: 3e69 736f 7274 3c2f 613e 2070 6163 6b61  >isort</a> packa
-000015f0: 6765 732e 200d 0a0d 0a46 6f72 2074 6865  ges. ....For the
-00001600: 2063 6f6d 6d69 7473 2070 6c65 6173 6520   commits please 
-00001610: 666f 6c6c 6f77 2074 6865 203c 6120 6872  follow the <a hr
-00001620: 6566 3d22 7777 772e 636f 6e76 656e 7469  ef="www.conventi
-00001630: 6f6e 616c 636f 6d6d 6974 732e 6f72 6722  onalcommits.org"
-00001640: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00001650: 3e43 6f6e 7665 6e74 696f 6e61 6c20 436f  >Conventional Co
-00001660: 6d6d 6974 7320 4775 6964 656c 696e 653c  mmits Guideline<
-00001670: 2f61 3e2e 0d0a 0d0a 2323 204c 6963 656e  /a>.....## Licen
-00001680: 7365 0d0a 0d0a 6050 4541 4b60 c2a0 6973  se....`PEAK`..is
-00001690: 2066 7265 6520 616e 6420 6f70 656e 2d73   free and open-s
-000016a0: 6f75 7263 6520 736f 6674 7761 7265 206c  ource software l
-000016b0: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
-000016c0: 6520 3c61 2068 7265 663d 2268 7474 7073  e <a href="https
-000016d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6765  ://github.com/ge
-000016e0: 6361 642d 6772 6f75 702f 7065 616b 2d6d  cad-group/peak-m
-000016f0: 6173 2f62 6c6f 622f 6465 7665 6c6f 702f  as/blob/develop/
-00001700: 4c49 4345 4e53 4522 2074 6172 6765 743d  LICENSE" target=
-00001710: 225f 626c 616e 6b22 3e47 4e55 2047 656e  "_blank">GNU Gen
-00001720: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-00001730: 6e73 6520 7633 2e30 3c2f 613e 2e0d 0a    nse v3.0</a>...
+00000040: 730a 0a21 5b44 4f49 5d28 6874 7470 733a  s..![DOI](https:
+00000050: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000060: 2f73 7461 7469 632f 7631 3f6c 696e 6b3d  /static/v1?link=
+00000070: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
+00000080: 3130 2e31 3030 372f 3937 382d 332d 3033  10.1007/978-3-03
+00000090: 312d 3138 3035 302d 375f 3726 6c69 6e6b  1-18050-7_7&link
+000000a0: 3d68 7474 7073 3a2f 2f64 6f69 2e6f 7267  =https://doi.org
+000000b0: 2f31 302e 3130 3037 2f39 3738 2d33 2d30  /10.1007/978-3-0
+000000c0: 3331 2d31 3830 3530 2d37 5f37 266c 6162  31-18050-7_7&lab
+000000d0: 656c 3d44 4f49 266d 6573 7361 6765 3d39  el=DOI&message=9
+000000e0: 3738 2d33 2d30 3331 2d31 3830 3530 2d37  78-3-031-18050-7
+000000f0: 2663 6f6c 6f72 3d62 6c75 6529 2021 5b50  &color=blue) ![P
+00000100: 7950 4920 2d20 5079 7468 6f6e 2056 6572  yPI - Python Ver
+00000110: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
+00000120: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000130: 692f 7079 7665 7273 696f 6e73 2f70 6561  i/pyversions/pea
+00000140: 6b2d 6d61 7329 2021 5b50 7950 495d 2868  k-mas) ![PyPI](h
+00000150: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000160: 6473 2e69 6f2f 7079 7069 2f76 2f70 6561  ds.io/pypi/v/pea
+00000170: 6b2d 6d61 7329 2021 5b47 6974 4875 625d  k-mas) ![GitHub]
+00000180: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000190: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+000001a0: 6963 656e 7365 2f67 6563 6164 2d67 726f  icense/gecad-gro
+000001b0: 7570 2f70 6561 6b2d 6d61 7329 2021 5b70  up/peak-mas) ![p
+000001c0: 6f77 6572 6564 2062 795d 2868 7474 7073  owered by](https
+000001d0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000001e0: 6f2f 7374 6174 6963 2f76 313f 6c61 6265  o/static/v1?labe
+000001f0: 6c3d 706f 7765 7265 6425 3230 6279 266d  l=powered%20by&m
+00000200: 6573 7361 6765 3d47 4543 4144 2663 6f6c  essage=GECAD&col
+00000210: 6f72 3d31 3737 3938 3526 6c61 6265 6c43  or=177985&labelC
+00000220: 6f6c 6f72 3d64 6535 6434 6126 3f6c 696e  olor=de5d4a&?lin
+00000230: 6b3d 6874 7470 3a2f 2f67 6563 6164 2e69  k=http://gecad.i
+00000240: 7365 702e 6970 702e 7074 266c 696e 6b3d  sep.ipp.pt&link=
+00000250: 6874 7470 3a2f 2f67 6563 6164 2e69 7365  http://gecad.ise
+00000260: 702e 6970 702e 7074 2f29 2021 5b63 6f64  p.ipp.pt/) ![cod
+00000270: 6520 7374 796c 655d 2868 7474 7073 3a2f  e style](https:/
+00000280: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000290: 6261 6467 652f 636f 6465 2532 3073 7479  badge/code%20sty
+000002a0: 6c65 2d62 6c61 636b 2d62 6c61 636b 2920  le-black-black) 
+000002b0: 215b 696d 706f 7274 7320 6973 6f72 745d  ![imports isort]
+000002c0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000002d0: 656c 6473 2e69 6f2f 7374 6174 6963 2f76  elds.io/static/v
+000002e0: 313f 6c61 6265 6c3d 696d 706f 7274 7326  1?label=imports&
+000002f0: 6d65 7373 6167 653d 6973 6f72 7426 636f  message=isort&co
+00000300: 6c6f 723d 626c 7565 266c 6162 656c 436f  lor=blue&labelCo
+00000310: 6c6f 723d 6f72 616e 6765 290a 0a50 4541  lor=orange)..PEA
+00000320: 4b20 6973 2061 206d 756c 7469 2d61 6765  K is a multi-age
+00000330: 6e74 2073 7973 7465 6d20 6672 616d 6577  nt system framew
+00000340: 6f72 6b20 7768 6963 6820 6865 6c70 7320  ork which helps 
+00000350: 7468 6520 7573 6572 7320 6465 7665 6c6f  the users develo
+00000360: 702c 206d 6f6e 6974 6f72 2c20 616e 616c  p, monitor, anal
+00000370: 797a 6520 616e 6420 6d61 696e 7461 696e  yze and maintain
+00000380: 2065 636f 7379 7374 656d 206f 6620 6865   ecosystem of he
+00000390: 7465 726f 6765 6e65 6f75 7320 6167 656e  terogeneous agen
+000003a0: 7420 636f 6d6d 756e 6974 6965 732e 2054  t communities. T
+000003b0: 6869 7320 6563 6f73 7973 7465 6d20 6973  his ecosystem is
+000003c0: 2020 7768 6572 6520 7661 7269 6f75 7320    where various 
+000003d0: 6d75 6c74 692d 6167 656e 7420 7379 7374  multi-agent syst
+000003e0: 656d 7320 6361 6e20 636f 6578 6973 742c  ems can coexist,
+000003f0: 2069 6e74 6572 6163 7420 616e 6420 7368   interact and sh
+00000400: 6172 6520 7265 736f 7572 6365 7320 6265  are resources be
+00000410: 7477 6565 6e20 7468 656d 2e20 0a54 6869  tween them. .Thi
+00000420: 7320 6672 616d 6577 6f72 6b20 6973 2062  s framework is b
+00000430: 6173 6564 206f 6e20 3c61 2068 7265 663d  ased on <a href=
+00000440: 2268 7474 7073 3a2f 2f73 7061 6465 2d6d  "https://spade-m
+00000450: 6173 2e72 6561 6474 6865 646f 6373 2e69  as.readthedocs.i
+00000460: 6f2f 656e 2f6c 6174 6573 742f 2220 7461  o/en/latest/" ta
+00000470: 7267 6574 3d22 5f62 6c61 6e6b 223e 5350  rget="_blank">SP
+00000480: 4144 453c 2f61 3e2e 0a0a 0a23 2320 5072  ADE</a>....## Pr
+00000490: 6572 6571 7569 7369 7465 730a 0a2d 2050  erequisites..- P
+000004a0: 7974 686f 6e20 3d3d 2033 2e39 2e36 0a2d  ython == 3.9.6.-
+000004b0: 2058 4d50 5020 5365 7276 6572 2028 5b73   XMPP Server ([s
+000004c0: 6565 2064 6f63 735d 2868 7474 7073 3a2f  ee docs](https:/
+000004d0: 2f77 7777 2e67 6563 6164 2e69 7365 702e  /www.gecad.isep.
+000004e0: 6970 702e 7074 2f70 6561 6b29 290a 0a0a  ipp.pt/peak))...
+000004f0: 2323 2049 6e73 7461 6c6c 696e 6720 5045  ## Installing PE
+00000500: 414b 0a0a 2323 2320 436f 6e64 610a 0a54  AK..### Conda..T
+00000510: 6f20 696e 7374 616c 6c20 7573 696e 6720  o install using 
+00000520: 636f 6e64 612c 2064 6f77 6e6c 6f61 6420  conda, download 
+00000530: 7468 6520 656e 7669 726f 6e6d 656e 742e  the environment.
+00000540: 796d 6c20 6669 6c65 2066 726f 6d20 7468  yml file from th
+00000550: 6520 7265 706f 7369 746f 7279 2061 6e64  e repository and
+00000560: 2074 6865 6e20 7573 6520 7468 6520 666f   then use the fo
+00000570: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
+00000580: 0a60 6060 6261 7368 0a24 2063 6f6e 6461  .```bash.$ conda
+00000590: 2065 6e76 2063 7265 6174 6520 2d2d 6669   env create --fi
+000005a0: 6c65 2065 6e76 6972 6f6e 6d65 6e74 2e79  le environment.y
+000005b0: 6d6c 090a 6060 600a 5468 6973 2077 696c  ml..```.This wil
+000005c0: 6c20 6372 6561 7465 2061 2063 6f6e 6461  l create a conda
+000005d0: 2065 6e76 6972 6f6e 6d65 6e74 2063 616c   environment cal
+000005e0: 6c65 6420 5f70 6561 6b5f 2e0a 0a23 2323  led _peak_...###
+000005f0: 2050 6970 0a0a 546f 2069 6e73 7461 6c6c   Pip..To install
+00000600: 2075 7369 6e67 2070 6970 2c20 6a75 7374   using pip, just
+00000610: 2074 7970 6520 7468 6520 666f 6c6c 6f77   type the follow
+00000620: 696e 6720 636f 6d6d 616e 643a 0a60 6060  ing command:.```
+00000630: 6261 7368 0a24 2070 6970 2069 6e73 7461  bash.$ pip insta
+00000640: 6c6c 2070 6561 6b2d 6d61 730a 6060 600a  ll peak-mas.```.
+00000650: 0a0a 2323 2055 7369 6e67 2050 4541 4b0a  ..## Using PEAK.
+00000660: 0a23 2323 204e 6f74 6573 206f 6e20 5350  .### Notes on SP
+00000670: 4144 450a 0a41 7320 616c 7265 6164 7920  ADE..As already 
+00000680: 7361 6964 2050 4541 4b20 6973 2062 6173  said PEAK is bas
+00000690: 6564 206f 6e20 5350 4144 452e 2054 6869  ed on SPADE. Thi
+000006a0: 7320 6d65 616e 7320 7468 6174 2065 7665  s means that eve
+000006b0: 7279 2066 756e 6374 696f 6e61 6c69 7479  ry functionality
+000006c0: 206f 6620 5350 4144 4520 6973 2061 7661   of SPADE is ava
+000006d0: 696c 6162 6c65 2074 6f20 7468 6520 7573  ilable to the us
+000006e0: 6572 2e20 5765 2068 6967 686c 7920 7265  er. We highly re
+000006f0: 636f 6d6d 656e 6420 796f 7520 746f 2073  commend you to s
+00000700: 6565 203c 6120 6872 6566 3d22 6874 7470  ee <a href="http
+00000710: 733a 2f2f 7370 6164 652d 6d61 732e 7265  s://spade-mas.re
+00000720: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00000730: 6c61 7465 7374 2f22 2074 6172 6765 743d  latest/" target=
+00000740: 225f 626c 616e 6b22 3e53 5041 4445 3c2f  "_blank">SPADE</
+00000750: 613e 2065 7861 6d70 6c65 7320 616e 6420  a> examples and 
+00000760: 646f 6375 6d65 6e74 6174 696f 6e20 6265  documentation be
+00000770: 666f 7265 2073 7461 7274 696e 6720 7573  fore starting us
+00000780: 696e 6720 5045 414b 2e20 4f6e 6365 2079  ing PEAK. Once y
+00000790: 6f75 2061 7265 2066 616d 696c 6961 7269  ou are familiari
+000007a0: 7a65 6420 7769 7468 2053 5041 4445 2773  zed with SPADE's
+000007b0: 206d 6563 6861 6e69 6373 2079 6f75 2063   mechanics you c
+000007c0: 616e 2073 7461 7274 2075 7369 6e67 2050  an start using P
+000007d0: 4541 4b2e 0a0a 2323 2320 4e6f 7465 7320  EAK...### Notes 
+000007e0: 6f6e 2058 4d50 500a 0a54 6f20 7275 6e20  on XMPP..To run 
+000007f0: 616e 7920 5045 414b 2773 2061 6765 6e74  any PEAK's agent
+00000800: 2079 6f75 2077 696c 6c20 6e65 6564 2061   you will need a
+00000810: 2058 4d50 5020 7365 7276 6572 2e20 596f   XMPP server. Yo
+00000820: 7520 6361 6e20 6569 7468 6572 2063 6f6e  u can either con
+00000830: 6669 6775 7265 206f 6e65 206f 6e20 796f  figure one on yo
+00000840: 7572 206d 6163 6869 6e65 2c20 7265 6d6f  ur machine, remo
+00000850: 7465 6c79 206f 7220 7573 6520 6120 7075  tely or use a pu
+00000860: 626c 6963 2073 6572 7665 722e 2054 6865  blic server. The
+00000870: 206f 6e6c 7920 6973 7375 6520 7769 7468   only issue with
+00000880: 2074 6865 2070 7562 6c69 6320 7365 7276   the public serv
+00000890: 6572 7320 6973 2074 6861 7420 7468 6579  ers is that they
+000008a0: 2064 6f6e 2774 2075 7375 616c 6c79 2068   don't usually h
+000008b0: 6176 6520 616c 6c20 7468 6520 636f 6e66  ave all the conf
+000008c0: 6967 7572 6174 696f 6e73 2072 6571 7569  igurations requi
+000008d0: 7265 6420 746f 2072 756e 2073 6f6d 6520  red to run some 
+000008e0: 5045 414b 2773 2066 756e 6374 696f 6e61  PEAK's functiona
+000008f0: 6c69 7469 6573 2e20 546f 2063 6f6e 6669  lities. To confi
+00000900: 6775 7265 2074 6865 2073 6572 7665 7220  gure the server 
+00000910: 796f 7520 6361 6e20 7265 6164 2074 6865  you can read the
+00000920: 2022 436f 6e66 6967 7572 6520 584d 5050   "Configure XMPP
+00000930: 2073 6572 7665 7222 2073 6563 7469 6f6e   server" section
+00000940: 2069 6e20 7468 6520 3c61 2068 7265 663d   in the <a href=
+00000950: 2268 7474 703a 2f2f 7777 772e 6765 6361  "http://www.geca
+00000960: 642e 6973 6570 2e69 7070 2e70 742f 7065  d.isep.ipp.pt/pe
+00000970: 616b 2220 7461 7267 6574 3d22 5f62 6c61  ak" target="_bla
+00000980: 6e6b 223e 646f 6375 6d65 6e74 6174 696f  nk">documentatio
+00000990: 6e3c 2f61 3e2e 0a0a 2323 2320 4865 6c6c  n</a>...### Hell
+000009a0: 6f20 576f 726c 6420 4167 656e 7420 4578  o World Agent Ex
+000009b0: 616d 706c 650a 0a4f 6e65 2074 6869 6e67  ample..One thing
+000009c0: 2074 6861 7420 7761 7320 6164 6465 6420   that was added 
+000009d0: 696e 2050 4541 4b20 7761 7320 7468 6520  in PEAK was the 
+000009e0: 7761 7920 7468 6520 7573 6572 2065 7865  way the user exe
+000009f0: 6375 7465 7320 7468 6520 6167 656e 7473  cutes the agents
+00000a00: 2e20 5045 414b 2061 6464 6564 2061 2043  . PEAK added a C
+00000a10: 4c49 2c20 696e 7370 6972 6564 2069 6e20  LI, inspired in 
+00000a20: 4a41 4445 2c20 746f 2068 656c 7020 7468  JADE, to help th
+00000a30: 6520 7573 6572 2065 7865 6375 7465 2065  e user execute e
+00000a40: 6e64 2063 6f6e 6669 6775 7265 2065 6163  nd configure eac
+00000a50: 6820 6167 656e 7420 696e 2061 2065 6173  h agent in a eas
+00000a60: 7920 616e 6420 696e 7475 6974 6976 6520  y and intuitive 
+00000a70: 6d61 6e6e 6572 2e0a 496e 2074 6869 7320  manner..In this 
+00000a80: 6578 616d 706c 6520 7765 2077 696c 6c20  example we will 
+00000a90: 7368 6f77 2079 6f75 2068 6f77 2074 6f20  show you how to 
+00000aa0: 6578 6563 7574 6520 6120 7369 6e67 6c65  execute a single
+00000ab0: 2061 6765 6e74 2e20 5361 7665 2074 6865   agent. Save the
+00000ac0: 2066 6f6c 6c6f 7769 6e67 2063 6f64 6520   following code 
+00000ad0: 696e 2061 2066 696c 6520 6361 6c6c 6564  in a file called
+00000ae0: 2060 6167 656e 742e 7079 602e 0a0a 6060   `agent.py`...``
+00000af0: 6070 7974 686f 6e20 0a66 726f 6d20 7065  `python .from pe
+00000b00: 616b 2069 6d70 6f72 7420 4167 656e 740a  ak import Agent.
+00000b10: 6672 6f6d 2070 6561 6b2e 6265 6861 7669  from peak.behavi
+00000b20: 6f75 7273 2069 6d70 6f72 7420 4f6e 6553  ours import OneS
+00000b30: 686f 7442 6568 6176 696f 7572 0a0a 636c  hotBehaviour..cl
+00000b40: 6173 7320 6167 656e 7428 4167 656e 7429  ass agent(Agent)
+00000b50: 3a0a c2a0 20c2 a020 636c 6173 7320 4865  :... .. class He
+00000b60: 6c6c 6f57 6f72 6c64 284f 6e65 5368 6f74  lloWorld(OneShot
+00000b70: 4265 6861 7669 6f75 7229 3a0a c2a0 20c2  Behaviour):... .
+00000b80: a020 c2a0 20c2 a020 6173 796e 6320 6465  . .. .. async de
+00000b90: 6620 7275 6e28 7365 6c66 2920 2d3e 204e  f run(self) -> N
+00000ba0: 6f6e 653a 0ac2 a020 c2a0 20c2 a020 c2a0  one:... .. .. ..
+00000bb0: 20c2 a020 c2a0 2070 7269 6e74 2822 4865   .. .. print("He
+00000bc0: 6c6c 6f20 576f 726c 6422 290a c2a0 20c2  llo World")... .
+00000bd0: a020 c2a0 20c2 a020 c2a0 20c2 a020 6177  . .. .. .. .. aw
+00000be0: 6169 7420 7365 6c66 2e61 6765 6e74 2e73  ait self.agent.s
+00000bf0: 746f 7028 290a 0ac2 a020 c2a0 2061 7379  top().... .. asy
+00000c00: 6e63 2064 6566 2073 6574 7570 2873 656c  nc def setup(sel
+00000c10: 6629 202d 3e20 4e6f 6e65 3a0a c2a0 20c2  f) -> None:... .
+00000c20: a020 c2a0 20c2 a020 7365 6c66 2e61 6464  . .. .. self.add
+00000c30: 5f62 6568 6176 696f 7572 2873 656c 662e  _behaviour(self.
+00000c40: 4865 6c6c 6f57 6f72 6c64 2829 290a 6060  HelloWorld()).``
+00000c50: 600a 4974 2069 7320 6e65 6365 7373 6172  `.It is necessar
+00000c60: 7920 7468 6174 2074 6865 206e 616d 6520  y that the name 
+00000c70: 6f66 2074 6865 2066 696c 6520 6973 2074  of the file is t
+00000c80: 6865 2073 616d 6520 6173 2074 6865 206e  he same as the n
+00000c90: 616d 6520 6f66 2074 6865 2061 6765 6e74  ame of the agent
+00000ca0: 2773 2063 6c61 7373 2073 6f20 5045 414b  's class so PEAK
+00000cb0: 2063 616e 2064 6f20 7468 6520 7072 6f70   can do the prop
+00000cc0: 6572 2070 6172 7369 6e67 2e20 5468 6973  er parsing. This
+00000cd0: 2061 6765 6e74 206f 6e6c 7920 6861 7320   agent only has 
+00000ce0: 6120 6265 6861 7669 6f72 2074 6861 7420  a behavior that 
+00000cf0: 7072 696e 7473 2074 6f20 7468 6520 7465  prints to the te
+00000d00: 726d 696e 616c 2074 6865 2022 4865 6c6c  rminal the "Hell
+00000d10: 6f20 576f 726c 6422 206d 6573 7361 6765  o World" message
+00000d20: 2e20 546f 2065 7865 6375 7465 2074 6865  . To execute the
+00000d30: 2061 6765 6e74 206a 7573 7420 7479 7065   agent just type
+00000d40: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00000d50: 6f6d 6d61 6e64 3a0a 6060 6062 6173 6820  ommand:.```bash 
+00000d60: 0a24 2070 6561 6b20 7275 6e20 7061 7468  .$ peak run path
+00000d70: 2f74 6f2f 6167 656e 742e 7079 202d 6a20  /to/agent.py -j 
+00000d80: 6167 656e 7440 6c6f 6361 6c68 6f73 740a  agent@localhost.
+00000d90: 6060 600a 4368 616e 6765 2074 6865 2060  ```.Change the `
+00000da0: 6c6f 6361 6c68 6f73 7460 2074 6f20 7468  localhost` to th
+00000db0: 6520 646f 6d61 696e 206f 6620 7468 6520  e domain of the 
+00000dc0: 584d 5050 2073 6572 7665 7220 796f 7520  XMPP server you 
+00000dd0: 7761 6e74 2074 6f20 636f 6e6e 6563 742e  want to connect.
+00000de0: 0a0a 3c64 6574 6169 6c73 3e3c 7375 6d6d  ..<details><summ
+00000df0: 6172 793e 4e6f 7465 3c2f 7375 6d6d 6172  ary>Note</summar
+00000e00: 793e 0a3c 703e 0a0a 4966 2079 6f75 2077  y>.<p>..If you w
+00000e10: 616e 7420 746f 206b 6e6f 7720 6d6f 7265  ant to know more
+00000e20: 2061 626f 7574 2065 6163 6820 636f 6d6d   about each comm
+00000e30: 616e 6420 7765 2072 6563 6f6d 6d65 6e64  and we recommend
+00000e40: 2072 6561 6469 6e67 2074 6865 205b 646f   reading the [do
+00000e50: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00000e60: 703a 2f2f 7777 772e 6765 6361 642e 6973  p://www.gecad.is
+00000e70: 6570 2e69 7070 2e70 742f 7065 616b 2920  ep.ipp.pt/peak) 
+00000e80: 6f72 2075 7369 6e67 2074 6865 2060 2d68  or using the `-h
+00000e90: 6020 6f70 7469 6f6e 2074 6f20 7365 6520  ` option to see 
+00000ea0: 7468 6520 6865 6c70 206d 6573 7361 6765  the help message
+00000eb0: 2e0a 0a3c 2f70 3e0a 3c2f 6465 7461 696c  ...</p>.</detail
+00000ec0: 733e 0a0a 466f 7220 6d6f 7265 2061 6476  s>..For more adv
+00000ed0: 616e 6365 6420 6675 6e63 7469 6f6e 616c  anced functional
+00000ee0: 6974 6965 7320 616e 6420 6578 616d 706c  ities and exampl
+00000ef0: 6573 2077 6520 7265 636f 6d6d 656e 6420  es we recommend 
+00000f00: 796f 7520 746f 2068 6561 6420 666f 7277  you to head forw
+00000f10: 6172 6420 746f 2074 6865 203c 6120 6872  ard to the <a hr
+00000f20: 6566 3d22 6874 7470 3a2f 2f77 7777 2e67  ef="http://www.g
+00000f30: 6563 6164 2e69 7365 702e 6970 702e 7074  ecad.isep.ipp.pt
+00000f40: 2f70 6561 6b22 2074 6172 6765 743d 225f  /peak" target="_
+00000f50: 626c 616e 6b22 3e64 6f63 756d 656e 7461  blank">documenta
+00000f60: 7469 6f6e 2077 6562 7369 7465 3c2f 613e  tion website</a>
+00000f70: 2e0a 0a0a 2323 2053 7570 706f 7274 0a0a  ....## Support..
+00000f80: 5573 6520 7468 6520 3c61 2068 7265 663d  Use the <a href=
+00000f90: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000fa0: 636f 6d2f 6765 6361 642d 6772 6f75 702f  com/gecad-group/
+00000fb0: 7065 616b 2d6d 6173 2f64 6973 6375 7373  peak-mas/discuss
+00000fc0: 696f 6e73 2220 7461 7267 6574 3d22 5f62  ions" target="_b
+00000fd0: 6c61 6e6b 223e 4469 7363 7573 7369 6f6e  lank">Discussion
+00000fe0: 3c2f 613e 2070 6167 6520 6966 2079 6f75  </a> page if you
+00000ff0: 2068 6176 6520 616e 7920 7175 6573 7469   have any questi
+00001000: 6f6e 7320 6f72 2069 6465 6173 2079 6f75  ons or ideas you
+00001010: 2077 6f75 6c64 206c 696b 6520 736f 2073   would like so s
+00001020: 6565 2069 6d70 6c65 6d65 6e74 6564 2e0a  ee implemented..
+00001030: 546f 2061 6c65 7274 2061 6e20 6973 7375  To alert an issu
+00001040: 6520 6f72 2061 2062 7567 2070 6c65 6173  e or a bug pleas
+00001050: 6520 706f 7374 2069 6e20 7468 6520 3c61  e post in the <a
+00001060: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00001070: 6974 6875 622e 636f 6d2f 6765 6361 642d  ithub.com/gecad-
+00001080: 6772 6f75 702f 7065 616b 2d6d 6173 2f69  group/peak-mas/i
+00001090: 7373 7565 7322 2074 6172 6765 743d 225f  ssues" target="_
+000010a0: 626c 616e 6b22 3e49 7373 7565 733c 2f61  blank">Issues</a
+000010b0: 3e20 7061 6765 2e0a 0a23 2320 526f 6164  > page...## Road
+000010c0: 6d61 700a 0a54 6869 7320 6172 6520 736f  map..This are so
+000010d0: 6d65 2066 756e 6374 696f 6e61 6c69 7469  me functionaliti
+000010e0: 6573 2074 6861 7420 6172 6520 6265 696e  es that are bein
+000010f0: 6720 6465 7665 6c6f 7065 6420 616e 6420  g developed and 
+00001100: 7769 6c6c 2062 6520 7265 6c65 6173 6564  will be released
+00001110: 2069 6e20 6120 6e65 6172 2066 7574 7572   in a near futur
+00001120: 653a 0a2d 205b 205d 2043 7265 6174 6520  e:.- [ ] Create 
+00001130: 6120 446f 636b 6572 2066 6f72 2058 4d50  a Docker for XMP
+00001140: 5020 7365 7276 6572 2061 6e64 2050 4541  P server and PEA
+00001150: 4b2e 0a2d 205b 205d 2041 6464 2064 796e  K..- [ ] Add dyn
+00001160: 616d 6963 2073 7065 6564 206f 7074 696f  amic speed optio
+00001170: 6e20 746f 2050 4541 4b27 7320 696e 7465  n to PEAK's inte
+00001180: 726e 616c 2063 6c6f 636b 2e0a 2d20 5b20  rnal clock..- [ 
+00001190: 5d20 4164 6420 6d75 6c74 692d 7468 7265  ] Add multi-thre
+000011a0: 6164 696e 6720 6f70 7469 6f6e 2074 6f20  ading option to 
+000011b0: 7468 6520 6578 6563 7574 696f 6e20 636f  the execution co
+000011c0: 6e66 6967 7572 6174 696f 6e73 2e0a 2d20  nfigurations..- 
+000011d0: 5b20 5d20 496d 706c 656d 656e 7420 5965  [ ] Implement Ye
+000011e0: 6c6c 6f77 2050 6167 6520 5365 7276 6963  llow Page Servic
+000011f0: 6520 696e 2044 4620 6167 656e 742e 0a2d  e in DF agent..-
+00001200: 205b 205d 2049 6d70 6c65 6d65 6e74 2044   [ ] Implement D
+00001210: 6174 6120 416e 616c 7973 6973 2073 6563  ata Analysis sec
+00001220: 7469 6f6e 2069 6e20 7468 6520 4461 7368  tion in the Dash
+00001230: 626f 6172 642e 0a0a 2323 2053 6369 656e  board...## Scien
+00001240: 7469 6669 6320 5075 626c 6963 6174 696f  tific Publicatio
+00001250: 6e73 0a0a 2d20 5269 6265 6972 6f2c 2042  ns..- Ribeiro, B
+00001260: 2e2c 2050 6572 6569 7261 2c20 482e 2c20  ., Pereira, H., 
+00001270: 476f 6d65 732c 204c 2e2c 2056 616c 652c  Gomes, L., Vale,
+00001280: 205a 2e20 2832 3032 3329 2e20 5079 7468   Z. (2023). Pyth
+00001290: 6f6e 2d42 6173 6564 2045 636f 7379 7374  on-Based Ecosyst
+000012a0: 656d 2066 6f72 2041 6765 6e74 2043 6f6d  em for Agent Com
+000012b0: 6d75 6e69 7469 6573 2053 696d 756c 6174  munities Simulat
+000012c0: 696f 6e2e 2049 6e3a 202c c2a0 5f65 7420  ion. In: ,.._et 
+000012d0: 616c 2e5f c2a0 3137 7468 2049 6e74 6572  al._..17th Inter
+000012e0: 6e61 7469 6f6e 616c 2043 6f6e 6665 7265  national Confere
+000012f0: 6e63 6520 6f6e 2053 6f66 7420 436f 6d70  nce on Soft Comp
+00001300: 7574 696e 6720 4d6f 6465 6c73 2069 6e20  uting Models in 
+00001310: 496e 6475 7374 7269 616c 2061 6e64 2045  Industrial and E
+00001320: 6e76 6972 6f6e 6d65 6e74 616c 2041 7070  nvironmental App
+00001330: 6c69 6361 7469 6f6e 7320 2853 4f43 4f20  lications (SOCO 
+00001340: 3230 3232 292e 2053 4f43 4f20 3230 3232  2022). SOCO 2022
+00001350: 2e20 4c65 6374 7572 6520 4e6f 7465 7320  . Lecture Notes 
+00001360: 696e 204e 6574 776f 726b 7320 616e 6420  in Networks and 
+00001370: 5379 7374 656d 732c 2076 6f6c 2035 3331  Systems, vol 531
+00001380: 2e20 5370 7269 6e67 6572 2c20 4368 616d  . Springer, Cham
+00001390: 2e20 6874 7470 733a 2f2f 646f 692e 6f72  . https://doi.or
+000013a0: 672f 3130 2e31 3030 372f 3937 382d 332d  g/10.1007/978-3-
+000013b0: 3033 312d 3138 3035 302d 375f 370a 0a23  031-18050-7_7..#
+000013c0: 2320 436f 6e74 7269 6275 7469 6e67 2074  # Contributing t
+000013d0: 6f20 5045 414b 0a0a 5075 6c6c 2072 6571  o PEAK..Pull req
+000013e0: 7565 7374 7320 6172 6520 7765 6c63 6f6d  uests are welcom
+000013f0: 652e 2046 6f72 206d 616a 6f72 2063 6861  e. For major cha
+00001400: 6e67 6573 2c20 706c 6561 7365 206f 7065  nges, please ope
+00001410: 6e20 6120 6469 7363 7573 7369 6f6e 2066  n a discussion f
+00001420: 6972 7374 2074 6f20 6469 7363 7573 7320  irst to discuss 
+00001430: 7768 6174 2079 6f75 2077 6f75 6c64 206c  what you would l
+00001440: 696b 6520 746f 2063 6861 6e67 652e 0a0a  ike to change...
+00001450: 5468 6520 6578 616d 706c 6573 2061 7265  The examples are
+00001460: 2075 7365 6420 6173 2061 2066 6f72 6d20   used as a form 
+00001470: 6f66 2074 6573 7469 6e67 2074 6865 2066  of testing the f
+00001480: 7261 6d65 776f 726b 2e20 536f 2070 6c65  ramework. So ple
+00001490: 6173 6520 6d61 6b65 2073 7572 6520 746f  ase make sure to
+000014a0: 2075 7064 6174 6520 7468 6520 6578 616d   update the exam
+000014b0: 706c 6573 2061 7320 6170 7072 6f70 7269  ples as appropri
+000014c0: 6174 6520 6f72 206d 616b 6520 6e65 7720  ate or make new 
+000014d0: 6f6e 6573 2e20 0a0a 546f 2066 6f72 6d61  ones. ..To forma
+000014e0: 7420 7468 6520 636f 6465 2070 6c65 6173  t the code pleas
+000014f0: 6520 7573 6520 7468 6520 3c61 2068 7265  e use the <a hre
+00001500: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
+00001510: 6f72 672f 7072 6f6a 6563 742f 626c 6163  org/project/blac
+00001520: 6b2f 2220 7461 7267 6574 3d22 5f62 6c61  k/" target="_bla
+00001530: 6e6b 223e 626c 6163 6b3c 2f61 3e20 616e  nk">black</a> an
+00001540: 6420 3c61 2068 7265 663d 2268 7474 7073  d <a href="https
+00001550: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00001560: 6563 742f 6973 6f72 742f 2220 7461 7267  ect/isort/" targ
+00001570: 6574 3d22 5f62 6c61 6e6b 223e 6973 6f72  et="_blank">isor
+00001580: 743c 2f61 3e20 7061 636b 6167 6573 2e20  t</a> packages. 
+00001590: 0a0a 466f 7220 7468 6520 636f 6d6d 6974  ..For the commit
+000015a0: 7320 706c 6561 7365 2066 6f6c 6c6f 7720  s please follow 
+000015b0: 7468 6520 3c61 2068 7265 663d 2277 7777  the <a href="www
+000015c0: 2e63 6f6e 7665 6e74 696f 6e61 6c63 6f6d  .conventionalcom
+000015d0: 6d69 7473 2e6f 7267 2220 7461 7267 6574  mits.org" target
+000015e0: 3d22 5f62 6c61 6e6b 223e 436f 6e76 656e  ="_blank">Conven
+000015f0: 7469 6f6e 616c 2043 6f6d 6d69 7473 2047  tional Commits G
+00001600: 7569 6465 6c69 6e65 3c2f 613e 2e0a 0a23  uideline</a>...#
+00001610: 2320 4c69 6365 6e73 650a 0a60 5045 414b  # License..`PEAK
+00001620: 60c2 a069 7320 6672 6565 2061 6e64 206f  `..is free and o
+00001630: 7065 6e2d 736f 7572 6365 2073 6f66 7477  pen-source softw
+00001640: 6172 6520 6c69 6365 6e73 6564 2075 6e64  are licensed und
+00001650: 6572 2074 6865 203c 6120 6872 6566 3d22  er the <a href="
+00001660: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001670: 6f6d 2f67 6563 6164 2d67 726f 7570 2f70  om/gecad-group/p
+00001680: 6561 6b2d 6d61 732f 626c 6f62 2f64 6576  eak-mas/blob/dev
+00001690: 656c 6f70 2f4c 4943 454e 5345 2220 7461  elop/LICENSE" ta
+000016a0: 7267 6574 3d22 5f62 6c61 6e6b 223e 474e  rget="_blank">GN
+000016b0: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
+000016c0: 204c 6963 656e 7365 2076 332e 303c 2f61   License v3.0</a
+000016d0: 3e2e 0a                                  >..
```

### Comparing `peak-mas-1.0.4/pyproject.toml` & `peak-mas-1.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,57 @@
-[build-system]
-
-requires = ["setuptools", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "peak-mas"
-version = "1.0.4"
-description = "Python-based framework for heterogeneous agent communities"
-readme = "README.md"
-authors = [{ name = "Bruno Ribeiro", email = "brgri@isep.ipp.pt" }]
-classifiers = [
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
-    "Environment :: Console",
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: POSIX :: Linux",
-    "Topic :: Scientific/Engineering",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence"
-]
-keywords = ["framework", "multiagent", "agent-based", "ecosystem", "spade", "xmpp"]
-dependencies = [
-    "aiohttp_cors",
-    "aioxmpp",
-    "pandas",
-    "pyModbusTCP",
-    "spade >= 3.2.2",
-    "PyYAML"
-]
-requires-python = "==3.9.6"
-
-[project.optional-dependencies]
-build = ["build", "twine"]
-dev = ["black", "isort", "mypy", "bumpver", "pipreqs"]
-
-[project.urls]
-Homepage = "https://www.gecad.isep.ipp.pt/peak"
-Github = "https://github.com/gecad-group/peak-mas"
-
-[project.scripts]
-peak = "peak.__main__:main"
-
-[tool.bumpver]
-current_version = "1.0.4"
-version_pattern = "MAJOR.MINOR.PATCH"
-commit_message  = "chore: bump version {old_version} -> {new_version}"
-commit          = true
-tag             = true
-push            = false
-
-[tool.bumpver.file_patterns]
-"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"src/peak/__init__.py" = ["{version}"]
-
-[tool.isort]
-profile                   = "black"
-import_heading_stdlib     = "Standard library imports"
-import_heading_thirdparty = "Third party imports"
-import_heading_firstparty = "Reader imports"
+[build-system]
+
+requires = ["setuptools", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "peak-mas"
+version = "1.0.5"
+description = "Python-based framework for heterogeneous agent communities"
+readme = "README.md"
+authors = [{ name = "Bruno Ribeiro", email = "brgri@isep.ipp.pt" }]
+classifiers = [
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Environment :: Console",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX :: Linux",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence"
+]
+keywords = ["framework", "multiagent", "agent-based", "ecosystem", "spade", "xmpp"]
+dependencies = [
+    "aiohttp_cors",
+    "aioxmpp",
+    "pandas",
+    "spade >= 3.2.2",
+    "PyYAML"
+]
+requires-python = "==3.9.6"
+
+[project.optional-dependencies]
+build = ["build", "twine"]
+dev = ["black", "isort", "mypy", "bumpver", "pipreqs", "autoflake"]
+
+[project.urls]
+Homepage = "https://www.gecad.isep.ipp.pt/peak"
+Github = "https://github.com/gecad-group/peak-mas"
+
+[project.scripts]
+peak = "peak.__main__:main"
+
+[tool.bumpver]
+current_version = "1.0.5"
+version_pattern = "MAJOR.MINOR.PATCH"
+commit_message  = "chore: bump version {old_version} -> {new_version}"
+commit          = true
+tag             = true
+push            = false
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
+"src/peak/__init__.py" = ["{version}"]
+
+[tool.isort]
+profile                   = "black"
```

### Comparing `peak-mas-1.0.4/src/peak/agents.py` & `peak-mas-1.0.5/src/peak/agents.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,506 +1,464 @@
-# Standard library imports
-import asyncio as _asyncio
-import logging as _logging
-from abc import ABCMeta as _ABCMeta
-from abc import abstractmethod
-from datetime import datetime, timedelta
-from json import dumps as json_dumps
-from json import loads as json_loads
-
-# Third party imports
-import aiohttp_cors
-from aioxmpp import JID
-
-# Reader imports
-from peak import Agent, CyclicBehaviour, Message, PeriodicBehaviour, Template
-from peak.properties import Properties
-
-_logger = _logging.getLogger(__name__)
-
-
-class SyncAgent(Agent, metaclass=_ABCMeta):
-    """Agent that is synchronized by the Synchronizer.
-
-    Every agent that needs to be synchronized needs
-    to extend this class.
-
-    Attributes:
-        period: An integer representing the number of the period inside the simulation.
-        time: A datetime of the current moment in the simmulation.
-    """
-
-    class _StepBehaviour(CyclicBehaviour):
-        """Listens for the Synchronizer's clock's ticks."""
-
-        async def on_start(self):
-            _logger.info("Waiting for simulation to start...")
-
-        async def run(self):
-            msg = await self.receive(10)
-            if msg:
-                if msg.get_metadata("sync") == "step":
-                    self.agent.period = int(msg.get_metadata("period"))
-                    if msg.get_metadata("time"):
-                        self.agent.time = datetime.strptime(
-                            msg.get_metadata("time"), "%Y-%m-%d %H:%M:%S"
-                        )
-                    if self.agent.period != 0:
-                        self.agent.iterate_properties()
-                    await self.agent.step()
-                    _logger.info(
-                        "Period "
-                        + str(self.agent.period)
-                        + " ("
-                        + str(self.agent.time)
-                        + ")"
-                    )
-                if msg.get_metadata("sync") == "stop":
-                    _logger.info("Simulation ended")
-                    self.kill()
-
-        async def on_end(self):
-            await self.agent.stop()
-
-    def __init__(
-        self, jid: JID, properties: Properties = None, verify_security: bool = False
-    ):
-        """Agent that listens to the Synchronizer.
-
-        Args:
-            jid: XMPP identifier of the agent.
-            properties: Atributes of the agent to be injected.
-            verify_security: If True verifies SSL certificates.
-        """
-        super().__init__(jid, properties, verify_security)
-        self.period = 0
-        self.time = 0
-        template_step = Template()
-        template_step.set_metadata("sync", "step")
-        template_stop = Template()
-        template_stop.set_metadata("sync", "stop")
-        template = template_step | template_stop
-        self.add_behaviour(self._StepBehaviour(), template)
-
-    @abstractmethod
-    async def step(self):
-        """Executed at each tick of the Synchronizer clock.
-
-        To be implemented by the user."""
-        raise NotImplementedError()
-
-
-class Synchronizer(Agent):
-    """Agent that synchronizes the other agents.
-
-    The Synchronizer creates a group of agents, awaits for
-    the agents to join the group and starts the clock of the
-    simulation.
-    """
-
-    class _PeriodicClock(PeriodicBehaviour):
-        """Handles the clock of the simulation.
-
-        This clock tracks the number of the current period
-        throughout the simulation.
-        """
-
-        def __init__(
-            self,
-            group_jid: str,
-            n_agents: int,
-            periods: int,
-            time_per_period: float,
-            start_at=None,
-        ):
-            super().__init__(time_per_period, start_at=start_at)
-            self.group_jid = group_jid
-            self.n_agents = n_agents
-            self.periods = periods
-
-        async def on_start(self):
-            while (
-                not len(await self.agent.group_members(self.group_jid)) >= self.n_agents
-            ):
-                await _asyncio.sleep(1)
-            self.current_period = 0
-            _logger.info("Starting simulation...")
-
-        async def run(self):
-            msg = Message()
-            msg.to = self.group_jid
-            if self.current_period >= self.periods:
-                msg.set_metadata("sync", "stop")
-                self.kill()
-            else:
-                _logger.info("Period " + str(self.current_period))
-                msg.body = "Period " + str(self.current_period)
-                msg.set_metadata("sync", "step")
-                msg.set_metadata("period", str(self.current_period))
-            await self.send_to_group(msg)
-            self.current_period += 1
-
-        async def on_end(self):
-            _logger.info("Ending simulation...")
-            await self.agent.stop()
-
-    class _DateTimeClock(PeriodicBehaviour):
-        """Handles the clock of the simulation.
-
-        This clock tracks the current date and time of the
-        simulation throughout its execution.
-        """
-
-        def __init__(
-            self,
-            jid,
-            n_agents: int,
-            initial_time: datetime,
-            end_time: datetime,
-            period_time_simulated: timedelta,
-            period_time_real: float,
-            start_at: datetime = None,
-        ):
-            super().__init__(period_time_real, start_at=start_at)
-            self.group_jid = jid
-            self.n_agents = n_agents
-            self.time = initial_time
-            self.end_time = end_time
-            self.period_time = period_time_simulated
-
-        async def on_start(self):
-            _logger.info("Waiting for all agents to enter the group...")
-            while (
-                not len(await self.agent.group_members(self.group_jid)) >= self.n_agents
-            ):
-                await _asyncio.sleep(1)
-            self.current_period = 0
-            _logger.info("Starting simulation...")
-
-        async def run(self):
-            msg = Message()
-            msg.to = self.group_jid
-            if self.time >= self.end_time:
-                msg.set_metadata("sync", "stop")
-                self.kill()
-            else:
-                _logger.info(
-                    "Period " + str(self.current_period) + " (" + str(self.time) + ")"
-                )
-                msg.body = (
-                    "Period " + str(self.current_period) + " (" + str(self.time) + ")"
-                )
-                msg.set_metadata("sync", "step")
-                msg.set_metadata("period", str(self.current_period))
-                msg.set_metadata(
-                    "time", datetime.strftime(self.time, "%Y-%m-%d %H:%M:%S")
-                )
-            await self.send_to_group(msg)
-            self.current_period += 1
-            self.time += self.period_time
-
-        async def on_end(self):
-            _logger.info("Ending simulation...")
-            await self.agent.stop()
-
-    async def sync_group_period(
-        self, group_jid: str, n_agents: int, time_per_period: float, periods: int
-    ):
-        """Synchronizes a group of agents.
-
-        The clock is based on the number of the current period.
-
-        Args:
-            group_jid: Identifier of the XMPP group to be synchronized.
-            n_agents: Number of agents to be synchronized. Synchronizer
-                awaits for this number of agents to join the group before
-                it starts the simulation.
-            time_per_period: time in seconds between each period.
-            periods: number of periods to simulate.
-        """
-        await self.join_group(group_jid)
-        self.add_behaviour(
-            self._PeriodicClock(group_jid, n_agents, periods, time_per_period)
-        )
-
-    async def sync_group_time(
-        self,
-        group_jid: str,
-        n_agents: int,
-        initial_time: datetime,
-        end_time: datetime,
-        internal_period_time: timedelta,
-        external_period_time: float,
-        start_at: datetime = None,
-    ):
-        """Synchronizes a group of agents.
-
-        The clock is based on the date and time inside of the simulation.
-
-        Args:
-            group_jid: Identifier of the XMPP group to be synchronized.
-            n_agents: Number of agents to be synchronized. Synchronizer
-                awaits for this number of agents to join the group before
-                it starts the simulation.
-            initial_time: defines the internal date and time at the start of the
-                simulation.
-            end_time: defines the internal date and time at which the simulation ends.
-            internal_period_time: time between each period inside the simulation.
-            period_time_real: time between each tick of the clock.
-            start_at: schedules the simulation start at a given time. If None the
-                simulation starts right away.
-        """
-        await self.join_group(group_jid)
-        self.add_behaviour(
-            self._DateTimeClock(
-                group_jid,
-                n_agents,
-                initial_time,
-                end_time,
-                internal_period_time,
-                external_period_time,
-                start_at,
-            )
-        )
-
-
-class DF(Agent):
-    """Directory Facilitator.
-
-    This agent makes available the data that it gathers from multi-agent systems
-    publicly through a REST API. It also provides a Yellow Page Service to the
-    agents.
-    """
-
-    class _GroupHierarchy(CyclicBehaviour):
-        """Manages the group structure of all the multi-agent systems."""
-
-        async def on_start(self):
-            self.logger = _logging.getLogger(self.__class__.__name__)
-            self.logger.debug("starting behaviour")
-            template = Template()
-            template.set_metadata("resource", "treehierarchy")
-            self.set_template(template)
-            self.agent.grouphierarchy_data = {
-                "nodes": set(),
-                "links": set(),
-                "categories": set(),
-                "node_members": {},
-                "tags": {},
-            }
-
-        async def run(self):
-            msg = await self.receive(60)
-            if msg:
-                self.logger.debug("message received")
-                path = msg.get_metadata("path")
-                domain = msg.get_metadata("domain")
-                if meta_tags := msg.get_metadata("tags"):
-                    tags = json_loads(meta_tags)
-                nodes = path.split("/")
-                self.logger.debug("nodes: " + str(nodes))
-                level = "level"
-
-                if (
-                    msg.get_metadata("leave")
-                    and msg.sender
-                    in self.agent.grouphierarchy_data["node_members"][nodes[-1]]
-                ):
-                    self.logger.debug(str(msg.sender) + " leaving " + path)
-                    self.agent.grouphierarchy_data["node_members"][nodes[-1]].remove(
-                        msg.sender
-                    )
-                    nodes = nodes[::-1]
-                    # remove empty nodes and links
-                    for i, node in enumerate(nodes):
-                        if len(
-                            self.agent.grouphierarchy_data["node_members"][node]
-                        ) == 0 and not any(
-                            node == source
-                            for source, _ in self.agent.grouphierarchy_data["links"]
-                        ):
-                            self.agent.grouphierarchy_data["node_members"].pop(
-                                node
-                            )  # this line can be removed, there is no need in removing the node from the dict
-                            self.agent.grouphierarchy_data["nodes"].remove(
-                                (node, level + str(len(nodes) - 1 - i), domain)
-                            )
-                            if i + 1 < len(nodes):
-                                self.agent.grouphierarchy_data["links"].remove(
-                                    (nodes[i + 1], node)
-                                )
-                    existing_categories = set()
-
-                    # remove categories if empty
-                    for _, level, _ in self.agent.grouphierarchy_data["nodes"]:
-                        existing_categories.add(level)
-                    difference = self.agent.grouphierarchy_data[
-                        "categories"
-                    ].difference(existing_categories)
-                    if any(difference):
-                        self.agent.grouphierarchy_data["categories"] -= difference
-
-                else:
-                    self.logger.debug(str(msg.sender) + " entering " + path)
-                    last = None
-                    for i, node in enumerate(nodes):
-                        self.agent.grouphierarchy_data["nodes"].add(
-                            (node, level + str(i), domain)
-                        )
-                        if node not in self.agent.grouphierarchy_data["node_members"]:
-                            self.agent.grouphierarchy_data["node_members"][node] = []
-                        self.agent.grouphierarchy_data["categories"].add(level + str(i))
-                        if last != None:
-                            self.agent.grouphierarchy_data["links"].add(
-                                (
-                                    last,
-                                    node,
-                                )
-                            )
-                        last = node
-                    self.agent.grouphierarchy_data["node_members"][last].append(
-                        msg.sender
-                    )
-                    for tag in tags:
-                        if tag not in self.agent.grouphierarchy_data["tags"]:
-                            self.agent.grouphierarchy_data["tags"][tag] = set()
-                        self.agent.grouphierarchy_data["tags"][tag].add(last)
-
-    class _SearchGroup(CyclicBehaviour):
-        """Handles all the requests to search for groups."""
-
-        async def on_start(self) -> None:
-            self.logger = _logging.getLogger(self.__class__.__name__)
-            self.logger.debug("starting behaviour")
-            template = Template()
-            template.set_metadata("resource", "searchgroup")
-            self.set_template(template)
-
-        async def run(self) -> None:
-            msg = await self.receive(60)
-            if msg and (meta_tags := msg.get_metadata("tags")):
-                tags = json_loads(meta_tags)
-                groups: set = self.agent.grouphierarchy_data["tags"][tags[0]]
-                for tag in tags[1:]:
-                    groups = groups.intersection(
-                        self.agent.grouphierarchy_data["tags"][tag]
-                    )
-                res = msg.make_reply()
-                res.set_metadata("groups", json_dumps(list(groups)))
-                await self.send(res)
-
-    class _CreateGraph(CyclicBehaviour):
-        """Handles the requests to create graphs"""
-
-        async def on_start(self):
-            self.logger = _logging.getLogger(self.__class__.__name__)
-            self.logger.debug("starting behaviour")
-            template = Template()
-            template.set_metadata("resource", "graph")
-            template.set_metadata("action", "create")
-            self.set_template(template)
-
-        async def run(self) -> None:
-            msg = await self.receive(60)
-            if msg:
-                self.logger.debug(msg.body)
-                graph_name = msg.get_metadata("graph_name")
-                graph_options = msg.get_metadata("graph_options")
-                properties = json_loads(msg.get_metadata("properties"))
-                self.agent.dataanalysis_data[graph_name] = {
-                    "graph_options": graph_options,
-                    "data": {},
-                }
-                for property in properties:
-                    self.agent.dataanalysis_data[graph_name]["data"][property] = []
-
-    class _UpdateGraph(CyclicBehaviour):
-        """Handles the requests to update the data of a given graph."""
-
-        async def on_start(self) -> None:
-            self.logger = _logging.getLogger(self.__class__.__name__)
-            self.logger.debug("starting behaviour")
-            template = Template()
-            template.set_metadata("resource", "graph")
-            template.set_metadata("action", "update")
-            self.set_template(template)
-
-        async def run(self) -> None:
-            msg = await self.receive(60)
-            if msg:
-                self.logger.debug(msg.body)
-                graph_name = msg.get_metadata("graph_name")
-                data = json_loads(msg.get_metadata("data"))
-                for property in data:
-                    self.agent.dataanalysis_data[graph_name]["data"][property].append(
-                        data[property]
-                    )
-                    self.logger.debug(
-                        'updating property "' + property + '" : ' + str(data[property])
-                    )
-
-    def __init__(self, domain, verify_security, port):
-        super().__init__(
-            JID.fromstr("df@" + domain + "/admin"), verify_security=verify_security
-        )
-        self.port = port
-
-    @classmethod
-    def name(cls, domain: str) -> str:
-        """Retrieves the JID of the DF based on the agent domain.
-
-        Args:
-            domain: server's name
-
-        Returns:
-            The string of the complete JID of the DF.
-        """
-        return "df@" + domain + "/admin"
-
-    async def setup(self):
-        self.grouphierarchy_data = dict()
-        self.dataanalysis_data = dict()
-        self.group_tags = dict()
-
-        self.add_behaviour(self._GroupHierarchy())
-        self.add_behaviour(self._SearchGroup())
-        self.add_behaviour(self._CreateGraph())
-        self.add_behaviour(self._UpdateGraph())
-
-        # Create routes.
-        self.web.add_get("/groups", self.get_groups, template=None)
-        self.web.add_get("/groups/refresh", self.refresh_groups, template=None)
-        self.web.add_get("/plots", self.get_plots, template=None)
-
-        # Configure default CORS settings.
-        cors = aiohttp_cors.setup(
-            self.web.app,
-            defaults={
-                "*": aiohttp_cors.ResourceOptions(
-                    allow_credentials=True,
-                    expose_headers="*",
-                    allow_headers="*",
-                )
-            },
-        )
-
-        # Configure CORS on all routes.
-        for route in list(self.web.app.router.routes()):
-            cors.add(route)
-
-        # Start web API
-        self.web.start(port=self.port)
-        _logger.info("REST API running on port " + self.port)
-
-    async def get_groups(self, request):
-        return {
-            "nodes": list(self.grouphierarchy_data["nodes"]),
-            "links": list(self.grouphierarchy_data["links"]),
-            "categories": list(self.grouphierarchy_data["categories"]),
-            "node_members": self.grouphierarchy_data["node_members"],
-        }
-
-    async def refresh_groups(self, request):
-        pass
-
-    async def get_plots(self, request):
-        return self.dataanalysis_data
+import asyncio as _asyncio
+import json
+import logging as _logging
+from abc import ABCMeta as _ABCMeta
+from abc import abstractmethod
+from datetime import datetime, timedelta
+
+import aiohttp_cors
+from aioxmpp import JID
+
+from peak import Agent, CyclicBehaviour, Message, PeriodicBehaviour, Template
+
+_logger = _logging.getLogger(__name__)
+
+
+class SyncAgent(Agent, metaclass=_ABCMeta):
+    """Is synchronized by the Synchronizer.
+
+    Every agent that needs to be synchronized needs
+    to extend this class.
+    """
+
+    class _StepBehaviour(CyclicBehaviour):
+        async def on_start(self):
+            self.logger.info("Waiting for simulation to start...")
+
+        async def run(self):
+            msg = await self.receive(10)
+            if msg:
+                if msg.get_metadata("sync") == "step":
+                    period = int(msg.get_metadata("period"))
+                    time = None
+                    if msg.get_metadata("time"):
+                        time = datetime.strptime(
+                            msg.get_metadata("time"), "%Y-%m-%d %H:%M:%S"
+                        )
+                    await self.agent.step(period, time)
+                    self.logger.info(msg.body)
+                if msg.get_metadata("sync") == "stop":
+                    self.logger.info("Simulation ended.")
+                    self.kill()
+
+        async def on_end(self):
+            await self.agent.stop()
+
+    def __init__(self, jid: JID, verify_security: bool = False):
+        """Inits the SyncAgent with the JID provided.
+
+        Args:
+            jid (:obj:`JID`): Agent's XMPP identifier.
+            verify_security (bool, optional): If True, verifies the SSL certificates.
+                Defaults to False.
+        """
+        super().__init__(jid, verify_security)
+        template_step = Template()
+        template_step.set_metadata("sync", "step")
+        template_stop = Template()
+        template_stop.set_metadata("sync", "stop")
+        template = template_step | template_stop
+        self.add_behaviour(self._StepBehaviour(), template)
+
+    @abstractmethod
+    async def step(self, period: int, time: datetime = None):
+        """Executed at each tick of the Synchronizer clock.
+
+        To be implemented by the user.
+
+        Args:
+            period (int): Number of the current period.
+            time (datetime, optional): Current datetime inside the simulation. It must be
+                configured in the Synchronizer."""
+        raise NotImplementedError()
+
+
+class Synchronizer(Agent):
+    """Synchronizes the syncagents.
+
+    The Synchronizer creates a group of agents, awaits for
+    the agents to join the group and starts the clock of the
+    simulation.
+    """
+
+    class _PeriodicClock(PeriodicBehaviour):
+        """Handles the clock of the simulation.
+
+        This clock tracks the number of the current period
+        throughout the simulation.
+        """
+
+        def __init__(
+            self,
+            group_jid: str,
+            n_agents: int,
+            periods: int,
+            time_per_period: float,
+            start_at=None,
+        ):
+            super().__init__(time_per_period, start_at=start_at)
+            self.group_jid = group_jid
+            self.n_agents = n_agents
+            self.periods = periods
+
+        async def on_start(self):
+            self.logger.info("Waiting for all agents to enter the group...")
+            while (
+                not len(await self.agent.group_members(self.group_jid)) >= self.n_agents
+            ):
+                await _asyncio.sleep(1)
+            self.current_period = 0
+            self.logger.info("Starting simulation...")
+
+        async def run(self):
+            msg = Message()
+            msg.to = self.group_jid
+            if self.current_period >= self.periods:
+                msg.set_metadata("sync", "stop")
+                self.kill()
+            else:
+                self.logger.info(f"Period {self.current_period}")
+                msg.body = f"Period {self.current_period}"
+                msg.set_metadata("sync", "step")
+                msg.set_metadata("period", str(self.current_period))
+            await self.send_to_group(msg)
+            self.current_period += 1
+
+        async def on_end(self):
+            self.logger.info("Ending simulation...")
+            await self.agent.stop()
+
+    class _DateTimeClock(PeriodicBehaviour):
+        """Handles the clock of the simulation.
+
+        This clock tracks the current date and time of the
+        simulation throughout its execution.
+        """
+
+        def __init__(
+            self,
+            jid,
+            n_agents: int,
+            initial_time: datetime,
+            end_time: datetime,
+            period_time_simulated: timedelta,
+            period_time_real: float,
+            start_at: datetime = None,
+        ):
+            super().__init__(period_time_real, start_at=start_at)
+            self.group_jid = jid
+            self.n_agents = n_agents
+            self.time = initial_time
+            self.end_time = end_time
+            self.period_time = period_time_simulated
+
+        async def on_start(self):
+            self.logger.info("Waiting for all agents to enter the group...")
+            while (
+                not len(await self.agent.group_members(self.group_jid)) >= self.n_agents
+            ):
+                await _asyncio.sleep(1)
+            self.current_period = 0
+            self.logger.info("Starting simulation...")
+
+        async def run(self):
+            msg = Message()
+            msg.to = self.group_jid
+            if self.time >= self.end_time:
+                msg.set_metadata("sync", "stop")
+                self.kill()
+            else:
+                self.logger.info(f"Period {self.current_period} ({self.time})")
+                msg.body = f"Period {self.current_period} ({self.time})"
+                msg.set_metadata("sync", "step")
+                msg.set_metadata("period", str(self.current_period))
+                msg.set_metadata(
+                    "time", datetime.strftime(self.time, "%Y-%m-%d %H:%M:%S")
+                )
+            await self.send_to_group(msg)
+            self.current_period += 1
+            self.time += self.period_time
+
+        async def on_end(self):
+            self.logger.info("Ending simulation...")
+            await self.agent.stop()
+
+    async def sync_group_period(
+        self, group_jid: str, n_agents: int, interval: float, periods: int
+    ):
+        """Synchronizes a group of agents.
+
+        The clock is based on the number of the current period.
+
+        Args:
+            group_jid: Identifier of the XMPP group to be synchronized.
+            n_agents: Number of agents to be synchronized. Synchronizer
+                awaits for this number of agents to join the group before
+                it starts the simulation.
+            interval: Time in seconds between each period.
+            periods: Number of periods to simulate.
+        """
+        await self.join_group(group_jid)
+        self.add_behaviour(self._PeriodicClock(group_jid, n_agents, periods, interval))
+
+    async def sync_group_time(
+        self,
+        group_jid: str,
+        n_agents: int,
+        initial_datetime: datetime,
+        end_datetime: datetime,
+        internal_interval: timedelta,
+        external_period_time: float,
+        start_at: datetime = None,
+    ):
+        """Synchronizes a group of agents.
+
+        Here two time dimensions are created. One is the real-time at which
+        the clock of the Synchronizer will run. The other is the fictional
+        datetime created inside the simulation. For example, one second
+        can correspond to one day inside the simulation.
+
+        Args:
+            group_jid: Identifier of the XMPP group to be synchronized.
+            n_agents: Number of agents to be synchronized. Synchronizer
+                awaits for this number of agents to join the group before
+                it starts the simulation.
+            initial_datetime: Defines the initial date and time inside the
+                simulation.
+            end_datetime: Defines the date and time at which the simulation ends.
+            internal_interval: Time between each period relative to the initial and
+                end datetimes.
+            interval: Time in seconds between each period relative to the Synchronizers
+                clock.
+            start_at: Schedules the simulation to start at a given time. If None the
+                simulation starts right away.
+        """
+        await self.join_group(group_jid)
+        self.add_behaviour(
+            self._DateTimeClock(
+                group_jid,
+                n_agents,
+                initial_datetime,
+                end_datetime,
+                internal_interval,
+                external_period_time,
+                start_at,
+            )
+        )
+
+
+class DF(Agent):
+    """Directory Facilitator.
+
+    This agent makes available the data that it gathers from multi-agent systems
+    publicly through a REST API. It also provides a Yellow Page Service to the
+    agents.
+    """
+
+    class _EcosystemHierarchy(CyclicBehaviour):
+        """Manages the group structure of all the multi-agent systems."""
+
+        async def on_start(self):
+            self.logger = self.agent.logger.getChild(self.__class__.__name__)
+            self.logger.debug("starting behaviour")
+            template = Template()
+            template.set_metadata("resource", "treehierarchy")
+            self.set_template(template)
+
+        async def run(self):
+            msg = await self.receive(60)
+            if msg:
+                self.logger.debug("message received")
+                path = msg.get_metadata("path")
+                domain = msg.get_metadata("domain")
+                if meta_tags := msg.get_metadata("tags"):
+                    tags = json.loads(meta_tags)
+                nodes = path.split("/")
+                self.logger.debug("nodes: " + str(nodes))
+                level = "level"
+
+                if (
+                    msg.get_metadata("leave")
+                    and msg.sender
+                    in self.agent.ecosystemhierarchy_data["node_members"][nodes[-1]]
+                ):
+                    self.logger.debug(str(msg.sender) + " leaving " + path)
+                    self.agent.ecosystemhierarchy_data["node_members"][
+                        nodes[-1]
+                    ].remove(msg.sender)
+                    nodes = nodes[::-1]
+                    # remove empty nodes and links
+                    for i, node in enumerate(nodes):
+                        if len(
+                            self.agent.ecosystemhierarchy_data["node_members"][node]
+                        ) == 0 and not any(
+                            node == source
+                            for source, _ in self.agent.ecosystemhierarchy_data["links"]
+                        ):
+                            self.agent.ecosystemhierarchy_data["node_members"].pop(
+                                node
+                            )  # this line can be removed, there is no need in removing the node from the dict
+                            self.agent.ecosystemhierarchy_data["nodes"].remove(
+                                (node, level + str(len(nodes) - 1 - i), domain)
+                            )
+                            if i + 1 < len(nodes):
+                                self.agent.ecosystemhierarchy_data["links"].remove(
+                                    (nodes[i + 1], node)
+                                )
+                    existing_categories = set()
+
+                    # remove categories if empty
+                    for _, level, _ in self.agent.ecosystemhierarchy_data["nodes"]:
+                        existing_categories.add(level)
+                    difference = self.agent.ecosystemhierarchy_data[
+                        "categories"
+                    ].difference(existing_categories)
+                    if any(difference):
+                        self.agent.ecosystemhierarchy_data["categories"] -= difference
+
+                else:
+                    self.logger.debug(str(msg.sender) + " entering " + path)
+                    last = None
+                    for i, node in enumerate(nodes):
+                        self.agent.ecosystemhierarchy_data["nodes"].add(
+                            (node, level + str(i), domain)
+                        )
+                        if (
+                            node
+                            not in self.agent.ecosystemhierarchy_data["node_members"]
+                        ):
+                            self.agent.ecosystemhierarchy_data["node_members"][
+                                node
+                            ] = []
+                        self.agent.ecosystemhierarchy_data["categories"].add(
+                            level + str(i)
+                        )
+                        if last != None:
+                            self.agent.ecosystemhierarchy_data["links"].add(
+                                (
+                                    last,
+                                    node,
+                                )
+                            )
+                        last = node
+                    self.agent.ecosystemhierarchy_data["node_members"][last].append(
+                        msg.sender
+                    )
+                    for tag in tags:
+                        if tag not in self.agent.ecosystemhierarchy_data["tags"]:
+                            self.agent.ecosystemhierarchy_data["tags"][tag] = set()
+                        self.agent.ecosystemhierarchy_data["tags"][tag].add(last)
+
+    class _SearchCommunity(CyclicBehaviour):
+        """Handles all the requests to search for groups."""
+
+        async def on_start(self) -> None:
+            self.logger = self.agent.logger.getChild(self.__class__.__name__)
+            self.logger.debug("starting behaviour")
+            template = Template()
+            template.set_metadata("resource", "searchgroup")
+            self.set_template(template)
+
+        async def run(self) -> None:
+            msg = await self.receive(60)
+            if msg and (meta_tags := msg.get_metadata("tags")):
+                tags = json.loads(meta_tags)
+                communities: set = self.agent.ecosystemhierarchy_data["tags"][tags[0]]
+                for tag in tags[1:]:
+                    communities = communities.intersection(
+                        self.agent.ecosystemhierarchy_data["tags"][tag]
+                    )
+                res = msg.make_reply()
+                res.set_metadata("communities", json.dumps(list(communities)))
+                await self.send(res)
+
+    class _CreateGraph(CyclicBehaviour):
+        """Handles the requests to create graphs"""
+
+        async def on_start(self):
+            self.logger = self.agent.logger.getChild(self.__class__.__name__)
+            self.logger.debug("starting behaviour")
+            template = Template()
+            template.set_metadata("resource", "graph")
+            template.set_metadata("action", "create")
+            self.set_template(template)
+
+        async def run(self) -> None:
+            msg = await self.receive(60)
+            if msg:
+                self.logger.debug(msg)
+                id = msg.get_metadata("id")
+                graph = json.loads(msg.get_metadata("graph"))
+                self.agent.dataanalysis_data[id] = graph
+
+    def __init__(self, domain, verify_security, port):
+        super().__init__(
+            JID.fromstr("df@" + domain + "/admin"), verify_security=verify_security
+        )
+        self.port = port
+        self.logger = _logger.getChild(self.__class__.__name__)
+
+    @classmethod
+    def name(cls, domain: str) -> str:
+        """Retrieves the JID of the DF based on the agent domain.
+
+        Args:
+            domain: server's name
+
+        Returns:
+            The string of the complete JID of the DF.
+        """
+        return "df@" + domain + "/admin"
+
+    async def setup(self):
+        self.ecosystemhierarchy_data = {
+            "nodes": set(),
+            "links": set(),
+            "categories": set(),
+            "node_members": {},
+            "tags": {},
+        }
+        self.dataanalysis_data = dict()
+        self.group_tags = dict()
+
+        self.add_behaviour(self._EcosystemHierarchy())
+        self.add_behaviour(self._SearchCommunity())
+        self.add_behaviour(self._CreateGraph())
+
+        # Create routes.
+        self.web.add_get("/groups", self.get_groups, template=None)
+        self.web.add_get("/groups/refresh", self.refresh_groups, template=None)
+        self.web.add_get("/plots", self.get_plots, template=None)
+
+        # Configure default CORS settings.
+        cors = aiohttp_cors.setup(
+            self.web.app,
+            defaults={
+                "*": aiohttp_cors.ResourceOptions(
+                    allow_credentials=True,
+                    expose_headers="*",
+                    allow_headers="*",
+                )
+            },
+        )
+
+        # Configure CORS on all routes.
+        for route in list(self.web.app.router.routes()):
+            cors.add(route)
+
+        # Start web API
+        self.web.start(port=self.port)
+        self.logger.info("REST API running on port " + self.port)
+
+    async def get_groups(self, request):
+        return {
+            "nodes": list(self.ecosystemhierarchy_data["nodes"]),
+            "links": list(self.ecosystemhierarchy_data["links"]),
+            "categories": list(self.ecosystemhierarchy_data["categories"]),
+            "node_members": self.ecosystemhierarchy_data["node_members"],
+        }
+
+    async def refresh_groups(self, request):
+        pass
+
+    async def get_plots(self, request):
+        return self.dataanalysis_data
```

### Comparing `peak-mas-1.0.4/src/peak/cli/df.py` & `peak-mas-1.0.5/src/peak/cli/df.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-# Standard library imports
-import logging
-from time import sleep
-
-# Reader imports
-from peak import DF
-
-
-def exec(log_level: int, domain: str, verify_security: bool, port: int, *args, **kargs):
-    """Executes the Directory Facilitator agent.
-
-    Args:
-        log_level: Logging level to be used in the DF's logs.
-        domain: Domain to which connect the DF.
-        verify_security: Verifies the SSL certificates.
-        port: Port to be used by the DF REST API.
-    """
-    logging.basicConfig(
-        level=log_level,
-        format="%(asctime)s [%(levelname)s] %(message)s",
-        handlers=[logging.StreamHandler()],
-    )
-    logger = logging.getLogger(__name__)
-    logger.info("Starting DF")
-    df = DF(domain, verify_security, port)
-    df.start().result()
-    logger.info("DF running")
-
-    try:
-        while df.is_alive():
-            sleep(10)
-    except KeyboardInterrupt:
-        df.stop()
-    logger.info("Stoped DF")
+import logging
+from time import sleep
+
+from peak import DF
+
+
+def exec(domain: str, verify_security: bool, port: int, *args, **kargs):
+    """Executes the Directory Facilitator agent.
+
+    Args:
+        log_level: Logging level to be used in the DF's logs.
+        domain: Domain to which connect the DF.
+        verify_security: Verifies the SSL certificates.
+        port: Port to be used by the DF REST API.
+    """
+    logger = logging.getLogger(__name__).parent
+    logger.handlers[1].setFormatter(
+        logging.Formatter("%(asctime)s [%(levelname)s] %(message)s")
+    )
+
+    logger.info("Starting DF")
+    df = DF(domain, verify_security, port)
+    df.start().result()
+    logger.info("DF running")
+
+    try:
+        while df.is_alive():
+            sleep(10)
+    except KeyboardInterrupt:
+        df.stop()
+    logger.info("Stoped DF")
```

### Comparing `peak-mas-1.0.4/src/peak_mas.egg-info/PKG-INFO` & `peak-mas-1.0.5/src/peak_mas.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,433 +1,425 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2070 6561  : 2.1..Name: pea
-00000020: 6b2d 6d61 730d 0a56 6572 7369 6f6e 3a20  k-mas..Version: 
-00000030: 312e 302e 340d 0a53 756d 6d61 7279 3a20  1.0.4..Summary: 
-00000040: 5079 7468 6f6e 2d62 6173 6564 2066 7261  Python-based fra
-00000050: 6d65 776f 726b 2066 6f72 2068 6574 6572  mework for heter
-00000060: 6f67 656e 656f 7573 2061 6765 6e74 2063  ogeneous agent c
-00000070: 6f6d 6d75 6e69 7469 6573 0d0a 4175 7468  ommunities..Auth
-00000080: 6f72 2d65 6d61 696c 3a20 4272 756e 6f20  or-email: Bruno 
-00000090: 5269 6265 6972 6f20 3c62 7267 7269 4069  Ribeiro <brgri@i
-000000a0: 7365 702e 6970 702e 7074 3e0d 0a50 726f  sep.ipp.pt>..Pro
-000000b0: 6a65 6374 2d55 524c 3a20 486f 6d65 7061  ject-URL: Homepa
-000000c0: 6765 2c20 6874 7470 733a 2f2f 7777 772e  ge, https://www.
-000000d0: 6765 6361 642e 6973 6570 2e69 7070 2e70  gecad.isep.ipp.p
-000000e0: 742f 7065 616b 0d0a 5072 6f6a 6563 742d  t/peak..Project-
-000000f0: 5552 4c3a 2047 6974 6875 622c 2068 7474  URL: Github, htt
-00000100: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000110: 6765 6361 642d 6772 6f75 702f 7065 616b  gecad-group/peak
-00000120: 2d6d 6173 0d0a 4b65 7977 6f72 6473 3a20  -mas..Keywords: 
-00000130: 6672 616d 6577 6f72 6b2c 6d75 6c74 6961  framework,multia
-00000140: 6765 6e74 2c61 6765 6e74 2d62 6173 6564  gent,agent-based
-00000150: 2c65 636f 7379 7374 656d 2c73 7061 6465  ,ecosystem,spade
-00000160: 2c78 6d70 700d 0a43 6c61 7373 6966 6965  ,xmpp..Classifie
-00000170: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
-00000180: 4920 4170 7072 6f76 6564 203a 3a20 474e  I Approved :: GN
-00000190: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
-000001a0: 204c 6963 656e 7365 2076 3320 2847 504c   License v3 (GPL
-000001b0: 7633 290d 0a43 6c61 7373 6966 6965 723a  v3)..Classifier:
-000001c0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000001d0: 6775 6167 6520 3a3a 2050 7974 686f 6e0d  guage :: Python.
-000001e0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000001f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000200: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000210: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-00000220: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000230: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000240: 332e 390d 0a43 6c61 7373 6966 6965 723a  3.9..Classifier:
-00000250: 2045 6e76 6972 6f6e 6d65 6e74 203a 3a20   Environment :: 
-00000260: 436f 6e73 6f6c 650d 0a43 6c61 7373 6966  Console..Classif
-00000270: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00000280: 7973 7465 6d20 3a3a 204d 6963 726f 736f  ystem :: Microso
-00000290: 6674 203a 3a20 5769 6e64 6f77 730d 0a43  ft :: Windows..C
-000002a0: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
-000002b0: 7469 6e67 2053 7973 7465 6d20 3a3a 2050  ting System :: P
-000002c0: 4f53 4958 203a 3a20 4c69 6e75 780d 0a43  OSIX :: Linux..C
-000002d0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-000002e0: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
-000002f0: 6e67 696e 6565 7269 6e67 0d0a 436c 6173  ngineering..Clas
-00000300: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
-00000310: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
-00000320: 6e65 6572 696e 6720 3a3a 2041 7274 6966  neering :: Artif
-00000330: 6963 6961 6c20 496e 7465 6c6c 6967 656e  icial Intelligen
-00000340: 6365 0d0a 5265 7175 6972 6573 2d50 7974  ce..Requires-Pyt
-00000350: 686f 6e3a 203d 3d33 2e39 2e36 0d0a 4465  hon: ==3.9.6..De
-00000360: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-00000370: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-00000380: 6b64 6f77 6e0d 0a50 726f 7669 6465 732d  kdown..Provides-
-00000390: 4578 7472 613a 2062 7569 6c64 0d0a 5072  Extra: build..Pr
-000003a0: 6f76 6964 6573 2d45 7874 7261 3a20 6465  ovides-Extra: de
-000003b0: 760d 0a4c 6963 656e 7365 2d46 696c 653a  v..License-File:
-000003c0: 204c 4943 454e 5345 0d0a 0d0a 2320 5045   LICENSE....# PE
-000003d0: 414b 3a20 5079 7468 6f6e 2d62 6173 6564  AK: Python-based
-000003e0: 2066 7261 6d65 776f 726b 2066 6f72 2068   framework for h
-000003f0: 6574 6572 6f67 656e 6f75 7320 6167 656e  eterogenous agen
-00000400: 7420 636f 6d6d 756e 6974 6965 730d 0a0d  t communities...
-00000410: 0a21 5b44 4f49 5d28 6874 7470 733a 2f2f  .![DOI](https://
-00000420: 696d 672e 7368 6965 6c64 732e 696f 2f73  img.shields.io/s
-00000430: 7461 7469 632f 7631 3f6c 696e 6b3d 6874  tatic/v1?link=ht
-00000440: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
-00000450: 2e31 3030 372f 3937 382d 332d 3033 312d  .1007/978-3-031-
-00000460: 3138 3035 302d 375f 3726 6c69 6e6b 3d68  18050-7_7&link=h
-00000470: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00000480: 302e 3130 3037 2f39 3738 2d33 2d30 3331  0.1007/978-3-031
-00000490: 2d31 3830 3530 2d37 5f37 266c 6162 656c  -18050-7_7&label
-000004a0: 3d44 4f49 266d 6573 7361 6765 3d39 3738  =DOI&message=978
-000004b0: 2d33 2d30 3331 2d31 3830 3530 2d37 2663  -3-031-18050-7&c
-000004c0: 6f6c 6f72 3d62 6c75 6529 2021 5b50 7950  olor=blue) ![PyP
-000004d0: 4920 2d20 5079 7468 6f6e 2056 6572 7369  I - Python Versi
-000004e0: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
-000004f0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000500: 7079 7665 7273 696f 6e73 2f70 6561 6b2d  pyversions/peak-
-00000510: 6d61 7329 2021 5b50 7950 495d 2868 7474  mas) ![PyPI](htt
-00000520: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000530: 2e69 6f2f 7079 7069 2f76 2f70 6561 6b2d  .io/pypi/v/peak-
-00000540: 6d61 7329 2021 5b47 6974 4875 625d 2868  mas) ![GitHub](h
-00000550: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000560: 6473 2e69 6f2f 6769 7468 7562 2f6c 6963  ds.io/github/lic
-00000570: 656e 7365 2f67 6563 6164 2d67 726f 7570  ense/gecad-group
-00000580: 2f70 6561 6b2d 6d61 7329 2021 5b70 6f77  /peak-mas) ![pow
-00000590: 6572 6564 2062 795d 2868 7474 7073 3a2f  ered by](https:/
-000005a0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000005b0: 7374 6174 6963 2f76 313f 6c61 6265 6c3d  static/v1?label=
-000005c0: 706f 7765 7265 6425 3230 6279 266d 6573  powered%20by&mes
-000005d0: 7361 6765 3d47 4543 4144 2663 6f6c 6f72  sage=GECAD&color
-000005e0: 3d31 3737 3938 3526 6c61 6265 6c43 6f6c  =177985&labelCol
-000005f0: 6f72 3d64 6535 6434 6126 3f6c 696e 6b3d  or=de5d4a&?link=
-00000600: 6874 7470 3a2f 2f67 6563 6164 2e69 7365  http://gecad.ise
-00000610: 702e 6970 702e 7074 266c 696e 6b3d 6874  p.ipp.pt&link=ht
-00000620: 7470 3a2f 2f67 6563 6164 2e69 7365 702e  tp://gecad.isep.
-00000630: 6970 702e 7074 2f29 2021 5b63 6f64 6520  ipp.pt/) ![code 
-00000640: 7374 796c 655d 2868 7474 7073 3a2f 2f69  style](https://i
-00000650: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000660: 6467 652f 636f 6465 2532 3073 7479 6c65  dge/code%20style
-00000670: 2d62 6c61 636b 2d62 6c61 636b 2920 215b  -black-black) ![
-00000680: 696d 706f 7274 7320 6973 6f72 745d 2868  imports isort](h
-00000690: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000006a0: 6473 2e69 6f2f 7374 6174 6963 2f76 313f  ds.io/static/v1?
-000006b0: 6c61 6265 6c3d 696d 706f 7274 7326 6d65  label=imports&me
-000006c0: 7373 6167 653d 6973 6f72 7426 636f 6c6f  ssage=isort&colo
-000006d0: 723d 626c 7565 266c 6162 656c 436f 6c6f  r=blue&labelColo
-000006e0: 723d 6f72 616e 6765 290d 0a0d 0a50 4541  r=orange)....PEA
-000006f0: 4b20 6973 2061 206d 756c 7469 2d61 6765  K is a multi-age
-00000700: 6e74 2073 7973 7465 6d20 6672 616d 6577  nt system framew
-00000710: 6f72 6b20 7768 6963 6820 6865 6c70 7320  ork which helps 
-00000720: 7468 6520 7573 6572 7320 6465 7665 6c6f  the users develo
-00000730: 702c 206d 6f6e 6974 6f72 2c20 616e 616c  p, monitor, anal
-00000740: 797a 6520 616e 6420 6d61 696e 7461 696e  yze and maintain
-00000750: 2065 636f 7379 7374 656d 206f 6620 6865   ecosystem of he
-00000760: 7465 726f 6765 6e65 6f75 7320 6167 656e  terogeneous agen
-00000770: 7420 636f 6d6d 756e 6974 6965 732e 2054  t communities. T
-00000780: 6869 7320 6563 6f73 7973 7465 6d20 6973  his ecosystem is
-00000790: 2020 7768 6572 6520 7661 7269 6f75 7320    where various 
-000007a0: 6d75 6c74 692d 6167 656e 7420 7379 7374  multi-agent syst
-000007b0: 656d 7320 6361 6e20 636f 6578 6973 742c  ems can coexist,
-000007c0: 2069 6e74 6572 6163 7420 616e 6420 7368   interact and sh
-000007d0: 6172 6520 7265 736f 7572 6365 7320 6265  are resources be
-000007e0: 7477 6565 6e20 7468 656d 2e20 0d0a 5468  tween them. ..Th
-000007f0: 6973 2066 7261 6d65 776f 726b 2069 7320  is framework is 
-00000800: 6261 7365 6420 6f6e 203c 6120 6872 6566  based on <a href
-00000810: 3d22 6874 7470 733a 2f2f 7370 6164 652d  ="https://spade-
-00000820: 6d61 732e 7265 6164 7468 6564 6f63 732e  mas.readthedocs.
-00000830: 696f 2f65 6e2f 6c61 7465 7374 2f22 2074  io/en/latest/" t
-00000840: 6172 6765 743d 225f 626c 616e 6b22 3e53  arget="_blank">S
-00000850: 5041 4445 3c2f 613e 2e0d 0a0d 0a0d 0a23  PADE</a>.......#
-00000860: 2320 5072 6572 6571 7569 7369 7465 730d  # Prerequisites.
-00000870: 0a0d 0a2d 2050 7974 686f 6e20 3d3d 2033  ...- Python == 3
-00000880: 2e39 2e36 0d0a 2d20 584d 5050 2053 6572  .9.6..- XMPP Ser
-00000890: 7665 7220 285b 7365 6520 646f 6373 5d28  ver ([see docs](
-000008a0: 6874 7470 733a 2f2f 7777 772e 6765 6361  https://www.geca
-000008b0: 642e 6973 6570 2e69 7070 2e70 742f 7065  d.isep.ipp.pt/pe
-000008c0: 616b 2929 0d0a 0d0a 0d0a 2323 2049 6e73  ak))......## Ins
-000008d0: 7461 6c6c 696e 6720 5045 414b 0d0a 0d0a  talling PEAK....
-000008e0: 2323 2320 436f 6e64 610d 0a0d 0a54 6f20  ### Conda....To 
-000008f0: 696e 7374 616c 6c20 7573 696e 6720 636f  install using co
-00000900: 6e64 612c 2064 6f77 6e6c 6f61 6420 7468  nda, download th
-00000910: 6520 656e 7669 726f 6e6d 656e 742e 796d  e environment.ym
-00000920: 6c20 6669 6c65 2066 726f 6d20 7468 6520  l file from the 
-00000930: 7265 706f 7369 746f 7279 2061 6e64 2074  repository and t
-00000940: 6865 6e20 7573 6520 7468 6520 666f 6c6c  hen use the foll
-00000950: 6f77 696e 6720 636f 6d6d 616e 643a 0d0a  owing command:..
-00000960: 6060 6062 6173 680d 0a24 2063 6f6e 6461  ```bash..$ conda
-00000970: 2065 6e76 2063 7265 6174 6520 2d2d 6669   env create --fi
-00000980: 6c65 2065 6e76 6972 6f6e 6d65 6e74 2e79  le environment.y
-00000990: 6d6c 090d 0a60 6060 0d0a 5468 6973 2077  ml...```..This w
-000009a0: 696c 6c20 6372 6561 7465 2061 2063 6f6e  ill create a con
-000009b0: 6461 2065 6e76 6972 6f6e 6d65 6e74 2063  da environment c
-000009c0: 616c 6c65 6420 5f70 6561 6b5f 2e0d 0a0d  alled _peak_....
-000009d0: 0a23 2323 2050 6970 0d0a 0d0a 546f 2069  .### Pip....To i
-000009e0: 6e73 7461 6c6c 2075 7369 6e67 2070 6970  nstall using pip
-000009f0: 2c20 6a75 7374 2074 7970 6520 7468 6520  , just type the 
-00000a00: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
-00000a10: 643a 0d0a 6060 6062 6173 680d 0a24 2070  d:..```bash..$ p
-00000a20: 6970 2069 6e73 7461 6c6c 2070 6561 6b2d  ip install peak-
-00000a30: 6d61 730d 0a60 6060 0d0a 0d0a 0d0a 2323  mas..```......##
-00000a40: 2055 7369 6e67 2050 4541 4b0d 0a0d 0a23   Using PEAK....#
-00000a50: 2323 204e 6f74 6573 206f 6e20 5350 4144  ## Notes on SPAD
-00000a60: 450d 0a0d 0a41 7320 616c 7265 6164 7920  E....As already 
-00000a70: 7361 6964 2050 4541 4b20 6973 2062 6173  said PEAK is bas
-00000a80: 6564 206f 6e20 5350 4144 452e 2054 6869  ed on SPADE. Thi
-00000a90: 7320 6d65 616e 7320 7468 6174 2065 7665  s means that eve
-00000aa0: 7279 2066 756e 6374 696f 6e61 6c69 7479  ry functionality
-00000ab0: 206f 6620 5350 4144 4520 6973 2061 7661   of SPADE is ava
-00000ac0: 696c 6162 6c65 2074 6f20 7468 6520 7573  ilable to the us
-00000ad0: 6572 2e20 5765 2068 6967 686c 7920 7265  er. We highly re
-00000ae0: 636f 6d6d 656e 6420 796f 7520 746f 2073  commend you to s
-00000af0: 6565 203c 6120 6872 6566 3d22 6874 7470  ee <a href="http
-00000b00: 733a 2f2f 7370 6164 652d 6d61 732e 7265  s://spade-mas.re
-00000b10: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00000b20: 6c61 7465 7374 2f22 2074 6172 6765 743d  latest/" target=
-00000b30: 225f 626c 616e 6b22 3e53 5041 4445 3c2f  "_blank">SPADE</
-00000b40: 613e 2065 7861 6d70 6c65 7320 616e 6420  a> examples and 
-00000b50: 646f 6375 6d65 6e74 6174 696f 6e20 6265  documentation be
-00000b60: 666f 7265 2073 7461 7274 696e 6720 7573  fore starting us
-00000b70: 696e 6720 5045 414b 2e20 4f6e 6365 2079  ing PEAK. Once y
-00000b80: 6f75 2061 7265 2066 616d 696c 6961 7269  ou are familiari
-00000b90: 7a65 6420 7769 7468 2053 5041 4445 2773  zed with SPADE's
-00000ba0: 206d 6563 6861 6e69 6373 2079 6f75 2063   mechanics you c
-00000bb0: 616e 2073 7461 7274 2075 7369 6e67 2050  an start using P
-00000bc0: 4541 4b2e 0d0a 0d0a 2323 2320 4e6f 7465  EAK.....### Note
-00000bd0: 7320 6f6e 2058 4d50 500d 0a0d 0a54 6f20  s on XMPP....To 
-00000be0: 7275 6e20 616e 7920 5045 414b 2773 2061  run any PEAK's a
-00000bf0: 6765 6e74 2079 6f75 2077 696c 6c20 6e65  gent you will ne
-00000c00: 6564 2061 2058 4d50 5020 7365 7276 6572  ed a XMPP server
-00000c10: 2e20 596f 7520 6361 6e20 6569 7468 6572  . You can either
-00000c20: 2063 6f6e 6669 6775 7265 206f 6e65 206f   configure one o
-00000c30: 6e20 796f 7572 206d 6163 6869 6e65 2c20  n your machine, 
-00000c40: 7265 6d6f 7465 6c79 206f 7220 7573 6520  remotely or use 
-00000c50: 6120 7075 626c 6963 2073 6572 7665 722e  a public server.
-00000c60: 2054 6865 206f 6e6c 7920 6973 7375 6520   The only issue 
-00000c70: 7769 7468 2074 6865 2070 7562 6c69 6320  with the public 
-00000c80: 7365 7276 6572 7320 6973 2074 6861 7420  servers is that 
-00000c90: 7468 6579 2064 6f6e 2774 2075 7375 616c  they don't usual
-00000ca0: 6c79 2068 6176 6520 616c 6c20 7468 6520  ly have all the 
-00000cb0: 636f 6e66 6967 7572 6174 696f 6e73 2072  configurations r
-00000cc0: 6571 7569 7265 6420 746f 2072 756e 2073  equired to run s
-00000cd0: 6f6d 6520 5045 414b 2773 2066 756e 6374  ome PEAK's funct
-00000ce0: 696f 6e61 6c69 7469 6573 2e20 546f 2063  ionalities. To c
-00000cf0: 6f6e 6669 6775 7265 2074 6865 2073 6572  onfigure the ser
-00000d00: 7665 7220 796f 7520 6361 6e20 7265 6164  ver you can read
-00000d10: 2074 6865 2022 436f 6e66 6967 7572 6520   the "Configure 
-00000d20: 584d 5050 2073 6572 7665 7222 2073 6563  XMPP server" sec
-00000d30: 7469 6f6e 2069 6e20 7468 6520 3c61 2068  tion in the <a h
-00000d40: 7265 663d 2268 7474 703a 2f2f 7777 772e  ref="http://www.
-00000d50: 6765 6361 642e 6973 6570 2e69 7070 2e70  gecad.isep.ipp.p
-00000d60: 742f 7065 616b 2220 7461 7267 6574 3d22  t/peak" target="
-00000d70: 5f62 6c61 6e6b 223e 646f 6375 6d65 6e74  _blank">document
-00000d80: 6174 696f 6e3c 2f61 3e2e 0d0a 0d0a 2323  ation</a>.....##
-00000d90: 2320 4865 6c6c 6f20 576f 726c 6420 4167  # Hello World Ag
-00000da0: 656e 7420 4578 616d 706c 650d 0a0d 0a4f  ent Example....O
-00000db0: 6e65 2074 6869 6e67 2074 6861 7420 7761  ne thing that wa
-00000dc0: 7320 6164 6465 6420 696e 2050 4541 4b20  s added in PEAK 
-00000dd0: 7761 7320 7468 6520 7761 7920 7468 6520  was the way the 
-00000de0: 7573 6572 2065 7865 6375 7465 7320 7468  user executes th
-00000df0: 6520 6167 656e 7473 2e20 5045 414b 2061  e agents. PEAK a
-00000e00: 6464 6564 2061 2043 4c49 2c20 696e 7370  dded a CLI, insp
-00000e10: 6972 6564 2069 6e20 4a41 4445 2c20 746f  ired in JADE, to
-00000e20: 2068 656c 7020 7468 6520 7573 6572 2065   help the user e
-00000e30: 7865 6375 7465 2065 6e64 2063 6f6e 6669  xecute end confi
-00000e40: 6775 7265 2065 6163 6820 6167 656e 7420  gure each agent 
-00000e50: 696e 2061 2065 6173 7920 616e 6420 696e  in a easy and in
-00000e60: 7475 6974 6976 6520 6d61 6e6e 6572 2e0d  tuitive manner..
-00000e70: 0a49 6e20 7468 6973 2065 7861 6d70 6c65  .In this example
-00000e80: 2077 6520 7769 6c6c 2073 686f 7720 796f   we will show yo
-00000e90: 7520 686f 7720 746f 2065 7865 6375 7465  u how to execute
-00000ea0: 2061 2073 696e 676c 6520 6167 656e 742e   a single agent.
-00000eb0: 2053 6176 6520 7468 6520 666f 6c6c 6f77   Save the follow
-00000ec0: 696e 6720 636f 6465 2069 6e20 6120 6669  ing code in a fi
-00000ed0: 6c65 2063 616c 6c65 6420 6061 6765 6e74  le called `agent
-00000ee0: 2e70 7960 2e0d 0a0d 0a60 6060 7079 7468  .py`.....```pyth
-00000ef0: 6f6e 200d 0a66 726f 6d20 7065 616b 2069  on ..from peak i
-00000f00: 6d70 6f72 7420 4167 656e 740d 0a66 726f  mport Agent..fro
-00000f10: 6d20 7065 616b 2e62 6568 6176 696f 7572  m peak.behaviour
-00000f20: 7320 696d 706f 7274 204f 6e65 5368 6f74  s import OneShot
-00000f30: 4265 6861 7669 6f75 720d 0a0d 0a63 6c61  Behaviour....cla
-00000f40: 7373 2061 6765 6e74 2841 6765 6e74 293a  ss agent(Agent):
-00000f50: 0d0a c2a0 20c2 a020 636c 6173 7320 4865  .... .. class He
-00000f60: 6c6c 6f57 6f72 6c64 284f 6e65 5368 6f74  lloWorld(OneShot
-00000f70: 4265 6861 7669 6f75 7229 3a0d 0ac2 a020  Behaviour):.... 
-00000f80: c2a0 20c2 a020 c2a0 2061 7379 6e63 2064  .. .. .. async d
-00000f90: 6566 2072 756e 2873 656c 6629 202d 3e20  ef run(self) -> 
-00000fa0: 4e6f 6e65 3a0d 0ac2 a020 c2a0 20c2 a020  None:.... .. .. 
-00000fb0: c2a0 20c2 a020 c2a0 2070 7269 6e74 2822  .. .. .. print("
-00000fc0: 4865 6c6c 6f20 576f 726c 6422 290d 0ac2  Hello World")...
-00000fd0: a020 c2a0 20c2 a020 c2a0 20c2 a020 c2a0  . .. .. .. .. ..
-00000fe0: 2061 7761 6974 2073 656c 662e 6167 656e   await self.agen
-00000ff0: 742e 7374 6f70 2829 0d0a 0d0a c2a0 20c2  t.stop()...... .
-00001000: a020 6173 796e 6320 6465 6620 7365 7475  . async def setu
-00001010: 7028 7365 6c66 2920 2d3e 204e 6f6e 653a  p(self) -> None:
-00001020: 0d0a c2a0 20c2 a020 c2a0 20c2 a020 7365  .... .. .. .. se
-00001030: 6c66 2e61 6464 5f62 6568 6176 696f 7572  lf.add_behaviour
-00001040: 2873 656c 662e 4865 6c6c 6f57 6f72 6c64  (self.HelloWorld
-00001050: 2829 290d 0a60 6060 0d0a 4974 2069 7320  ())..```..It is 
-00001060: 6e65 6365 7373 6172 7920 7468 6174 2074  necessary that t
-00001070: 6865 206e 616d 6520 6f66 2074 6865 2066  he name of the f
-00001080: 696c 6520 6973 2074 6865 2073 616d 6520  ile is the same 
-00001090: 6173 2074 6865 206e 616d 6520 6f66 2074  as the name of t
-000010a0: 6865 2061 6765 6e74 2773 2063 6c61 7373  he agent's class
-000010b0: 2073 6f20 5045 414b 2063 616e 2064 6f20   so PEAK can do 
-000010c0: 7468 6520 7072 6f70 6572 2070 6172 7369  the proper parsi
-000010d0: 6e67 2e20 5468 6973 2061 6765 6e74 206f  ng. This agent o
-000010e0: 6e6c 7920 6861 7320 6120 6265 6861 7669  nly has a behavi
-000010f0: 6f72 2074 6861 7420 7072 696e 7473 2074  or that prints t
-00001100: 6f20 7468 6520 7465 726d 696e 616c 2074  o the terminal t
-00001110: 6865 2022 4865 6c6c 6f20 576f 726c 6422  he "Hello World"
-00001120: 206d 6573 7361 6765 2e20 546f 2065 7865   message. To exe
-00001130: 6375 7465 2074 6865 2061 6765 6e74 206a  cute the agent j
-00001140: 7573 7420 7479 7065 2074 6865 2066 6f6c  ust type the fol
-00001150: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0d  lowing command:.
-00001160: 0a60 6060 6261 7368 200d 0a24 2070 6561  .```bash ..$ pea
-00001170: 6b20 7275 6e20 7061 7468 2f74 6f2f 6167  k run path/to/ag
-00001180: 656e 742e 7079 202d 6a20 6167 656e 7440  ent.py -j agent@
-00001190: 6c6f 6361 6c68 6f73 740d 0a60 6060 0d0a  localhost..```..
-000011a0: 4368 616e 6765 2074 6865 2060 6c6f 6361  Change the `loca
-000011b0: 6c68 6f73 7460 2074 6f20 7468 6520 646f  lhost` to the do
-000011c0: 6d61 696e 206f 6620 7468 6520 584d 5050  main of the XMPP
-000011d0: 2073 6572 7665 7220 796f 7520 7761 6e74   server you want
-000011e0: 2074 6f20 636f 6e6e 6563 742e 0d0a 0d0a   to connect.....
-000011f0: 3c64 6574 6169 6c73 3e3c 7375 6d6d 6172  <details><summar
-00001200: 793e 4e6f 7465 3c2f 7375 6d6d 6172 793e  y>Note</summary>
-00001210: 0d0a 3c70 3e0d 0a0d 0a49 6620 796f 7520  ..<p>....If you 
-00001220: 7761 6e74 2074 6f20 6b6e 6f77 206d 6f72  want to know mor
-00001230: 6520 6162 6f75 7420 6561 6368 2063 6f6d  e about each com
-00001240: 6d61 6e64 2077 6520 7265 636f 6d6d 656e  mand we recommen
-00001250: 6420 7265 6164 696e 6720 7468 6520 5b64  d reading the [d
-00001260: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-00001270: 7470 3a2f 2f77 7777 2e67 6563 6164 2e69  tp://www.gecad.i
-00001280: 7365 702e 6970 702e 7074 2f70 6561 6b29  sep.ipp.pt/peak)
-00001290: 206f 7220 7573 696e 6720 7468 6520 602d   or using the `-
-000012a0: 6860 206f 7074 696f 6e20 746f 2073 6565  h` option to see
-000012b0: 2074 6865 2068 656c 7020 6d65 7373 6167   the help messag
-000012c0: 652e 0d0a 0d0a 3c2f 703e 0d0a 3c2f 6465  e.....</p>..</de
-000012d0: 7461 696c 733e 0d0a 0d0a 466f 7220 6d6f  tails>....For mo
-000012e0: 7265 2061 6476 616e 6365 6420 6675 6e63  re advanced func
-000012f0: 7469 6f6e 616c 6974 6965 7320 616e 6420  tionalities and 
-00001300: 6578 616d 706c 6573 2077 6520 7265 636f  examples we reco
-00001310: 6d6d 656e 6420 796f 7520 746f 2068 6561  mmend you to hea
-00001320: 6420 666f 7277 6172 6420 746f 2074 6865  d forward to the
-00001330: 203c 6120 6872 6566 3d22 6874 7470 3a2f   <a href="http:/
-00001340: 2f77 7777 2e67 6563 6164 2e69 7365 702e  /www.gecad.isep.
-00001350: 6970 702e 7074 2f70 6561 6b22 2074 6172  ipp.pt/peak" tar
-00001360: 6765 743d 225f 626c 616e 6b22 3e64 6f63  get="_blank">doc
-00001370: 756d 656e 7461 7469 6f6e 2077 6562 7369  umentation websi
-00001380: 7465 3c2f 613e 2e0d 0a0d 0a0d 0a23 2320  te</a>.......## 
-00001390: 5375 7070 6f72 740d 0a0d 0a55 7365 2074  Support....Use t
-000013a0: 6865 203c 6120 6872 6566 3d22 6874 7470  he <a href="http
-000013b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
-000013c0: 6563 6164 2d67 726f 7570 2f70 6561 6b2d  ecad-group/peak-
-000013d0: 6d61 732f 6469 7363 7573 7369 6f6e 7322  mas/discussions"
-000013e0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-000013f0: 3e44 6973 6375 7373 696f 6e3c 2f61 3e20  >Discussion</a> 
-00001400: 7061 6765 2069 6620 796f 7520 6861 7665  page if you have
-00001410: 2061 6e79 2071 7565 7374 696f 6e73 206f   any questions o
-00001420: 7220 6964 6561 7320 796f 7520 776f 756c  r ideas you woul
-00001430: 6420 6c69 6b65 2073 6f20 7365 6520 696d  d like so see im
-00001440: 706c 656d 656e 7465 642e 0d0a 546f 2061  plemented...To a
-00001450: 6c65 7274 2061 6e20 6973 7375 6520 6f72  lert an issue or
-00001460: 2061 2062 7567 2070 6c65 6173 6520 706f   a bug please po
-00001470: 7374 2069 6e20 7468 6520 3c61 2068 7265  st in the <a hre
-00001480: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00001490: 622e 636f 6d2f 6765 6361 642d 6772 6f75  b.com/gecad-grou
-000014a0: 702f 7065 616b 2d6d 6173 2f69 7373 7565  p/peak-mas/issue
-000014b0: 7322 2074 6172 6765 743d 225f 626c 616e  s" target="_blan
-000014c0: 6b22 3e49 7373 7565 733c 2f61 3e20 7061  k">Issues</a> pa
-000014d0: 6765 2e0d 0a0d 0a23 2320 526f 6164 6d61  ge.....## Roadma
-000014e0: 700d 0a0d 0a54 6869 7320 6172 6520 736f  p....This are so
-000014f0: 6d65 2066 756e 6374 696f 6e61 6c69 7469  me functionaliti
-00001500: 6573 2074 6861 7420 6172 6520 6265 696e  es that are bein
-00001510: 6720 6465 7665 6c6f 7065 6420 616e 6420  g developed and 
-00001520: 7769 6c6c 2062 6520 7265 6c65 6173 6564  will be released
-00001530: 2069 6e20 6120 6e65 6172 2066 7574 7572   in a near futur
-00001540: 653a 0d0a 2d20 5b20 5d20 4372 6561 7465  e:..- [ ] Create
-00001550: 2061 2044 6f63 6b65 7220 666f 7220 584d   a Docker for XM
-00001560: 5050 2073 6572 7665 7220 616e 6420 5045  PP server and PE
-00001570: 414b 2e0d 0a2d 205b 205d 2041 6464 2064  AK...- [ ] Add d
-00001580: 796e 616d 6963 2073 7065 6564 206f 7074  ynamic speed opt
-00001590: 696f 6e20 746f 2050 4541 4b27 7320 696e  ion to PEAK's in
-000015a0: 7465 726e 616c 2063 6c6f 636b 2e0d 0a2d  ternal clock...-
-000015b0: 205b 205d 2041 6464 206d 756c 7469 2d74   [ ] Add multi-t
-000015c0: 6872 6561 6469 6e67 206f 7074 696f 6e20  hreading option 
-000015d0: 746f 2074 6865 2065 7865 6375 7469 6f6e  to the execution
-000015e0: 2063 6f6e 6669 6775 7261 7469 6f6e 732e   configurations.
-000015f0: 0d0a 2d20 5b20 5d20 496d 706c 656d 656e  ..- [ ] Implemen
-00001600: 7420 5965 6c6c 6f77 2050 6167 6520 5365  t Yellow Page Se
-00001610: 7276 6963 6520 696e 2044 4620 6167 656e  rvice in DF agen
-00001620: 742e 0d0a 2d20 5b20 5d20 496d 706c 656d  t...- [ ] Implem
-00001630: 656e 7420 4461 7461 2041 6e61 6c79 7369  ent Data Analysi
-00001640: 7320 7365 6374 696f 6e20 696e 2074 6865  s section in the
-00001650: 2044 6173 6862 6f61 7264 2e0d 0a0d 0a23   Dashboard.....#
-00001660: 2320 5363 6965 6e74 6966 6963 2050 7562  # Scientific Pub
-00001670: 6c69 6361 7469 6f6e 730d 0a0d 0a2d 2052  lications....- R
-00001680: 6962 6569 726f 2c20 422e 2c20 5065 7265  ibeiro, B., Pere
-00001690: 6972 612c 2048 2e2c 2047 6f6d 6573 2c20  ira, H., Gomes, 
-000016a0: 4c2e 2c20 5661 6c65 2c20 5a2e 2028 3230  L., Vale, Z. (20
-000016b0: 3233 292e 2050 7974 686f 6e2d 4261 7365  23). Python-Base
-000016c0: 6420 4563 6f73 7973 7465 6d20 666f 7220  d Ecosystem for 
-000016d0: 4167 656e 7420 436f 6d6d 756e 6974 6965  Agent Communitie
-000016e0: 7320 5369 6d75 6c61 7469 6f6e 2e20 496e  s Simulation. In
-000016f0: 3a20 2cc2 a05f 6574 2061 6c2e 5fc2 a031  : ,.._et al._..1
-00001700: 3774 6820 496e 7465 726e 6174 696f 6e61  7th Internationa
-00001710: 6c20 436f 6e66 6572 656e 6365 206f 6e20  l Conference on 
-00001720: 536f 6674 2043 6f6d 7075 7469 6e67 204d  Soft Computing M
-00001730: 6f64 656c 7320 696e 2049 6e64 7573 7472  odels in Industr
-00001740: 6961 6c20 616e 6420 456e 7669 726f 6e6d  ial and Environm
-00001750: 656e 7461 6c20 4170 706c 6963 6174 696f  ental Applicatio
-00001760: 6e73 2028 534f 434f 2032 3032 3229 2e20  ns (SOCO 2022). 
-00001770: 534f 434f 2032 3032 322e 204c 6563 7475  SOCO 2022. Lectu
-00001780: 7265 204e 6f74 6573 2069 6e20 4e65 7477  re Notes in Netw
-00001790: 6f72 6b73 2061 6e64 2053 7973 7465 6d73  orks and Systems
-000017a0: 2c20 766f 6c20 3533 312e 2053 7072 696e  , vol 531. Sprin
-000017b0: 6765 722c 2043 6861 6d2e 2068 7474 7073  ger, Cham. https
-000017c0: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3130  ://doi.org/10.10
-000017d0: 3037 2f39 3738 2d33 2d30 3331 2d31 3830  07/978-3-031-180
-000017e0: 3530 2d37 5f37 0d0a 0d0a 2323 2043 6f6e  50-7_7....## Con
-000017f0: 7472 6962 7574 696e 6720 746f 2050 4541  tributing to PEA
-00001800: 4b0d 0a0d 0a50 756c 6c20 7265 7175 6573  K....Pull reques
-00001810: 7473 2061 7265 2077 656c 636f 6d65 2e20  ts are welcome. 
-00001820: 466f 7220 6d61 6a6f 7220 6368 616e 6765  For major change
-00001830: 732c 2070 6c65 6173 6520 6f70 656e 2061  s, please open a
-00001840: 2064 6973 6375 7373 696f 6e20 6669 7273   discussion firs
-00001850: 7420 746f 2064 6973 6375 7373 2077 6861  t to discuss wha
-00001860: 7420 796f 7520 776f 756c 6420 6c69 6b65  t you would like
-00001870: 2074 6f20 6368 616e 6765 2e0d 0a0d 0a54   to change.....T
-00001880: 6865 2065 7861 6d70 6c65 7320 6172 6520  he examples are 
-00001890: 7573 6564 2061 7320 6120 666f 726d 206f  used as a form o
-000018a0: 6620 7465 7374 696e 6720 7468 6520 6672  f testing the fr
-000018b0: 616d 6577 6f72 6b2e 2053 6f20 706c 6561  amework. So plea
-000018c0: 7365 206d 616b 6520 7375 7265 2074 6f20  se make sure to 
-000018d0: 7570 6461 7465 2074 6865 2065 7861 6d70  update the examp
-000018e0: 6c65 7320 6173 2061 7070 726f 7072 6961  les as appropria
-000018f0: 7465 206f 7220 6d61 6b65 206e 6577 206f  te or make new o
-00001900: 6e65 732e 200d 0a0d 0a54 6f20 666f 726d  nes. ....To form
-00001910: 6174 2074 6865 2063 6f64 6520 706c 6561  at the code plea
-00001920: 7365 2075 7365 2074 6865 203c 6120 6872  se use the <a hr
-00001930: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
-00001940: 2e6f 7267 2f70 726f 6a65 6374 2f62 6c61  .org/project/bla
-00001950: 636b 2f22 2074 6172 6765 743d 225f 626c  ck/" target="_bl
-00001960: 616e 6b22 3e62 6c61 636b 3c2f 613e 2061  ank">black</a> a
-00001970: 6e64 203c 6120 6872 6566 3d22 6874 7470  nd <a href="http
-00001980: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00001990: 6a65 6374 2f69 736f 7274 2f22 2074 6172  ject/isort/" tar
-000019a0: 6765 743d 225f 626c 616e 6b22 3e69 736f  get="_blank">iso
-000019b0: 7274 3c2f 613e 2070 6163 6b61 6765 732e  rt</a> packages.
-000019c0: 200d 0a0d 0a46 6f72 2074 6865 2063 6f6d   ....For the com
-000019d0: 6d69 7473 2070 6c65 6173 6520 666f 6c6c  mits please foll
-000019e0: 6f77 2074 6865 203c 6120 6872 6566 3d22  ow the <a href="
-000019f0: 7777 772e 636f 6e76 656e 7469 6f6e 616c  www.conventional
-00001a00: 636f 6d6d 6974 732e 6f72 6722 2074 6172  commits.org" tar
-00001a10: 6765 743d 225f 626c 616e 6b22 3e43 6f6e  get="_blank">Con
-00001a20: 7665 6e74 696f 6e61 6c20 436f 6d6d 6974  ventional Commit
-00001a30: 7320 4775 6964 656c 696e 653c 2f61 3e2e  s Guideline</a>.
-00001a40: 0d0a 0d0a 2323 204c 6963 656e 7365 0d0a  ....## License..
-00001a50: 0d0a 6050 4541 4b60 c2a0 6973 2066 7265  ..`PEAK`..is fre
-00001a60: 6520 616e 6420 6f70 656e 2d73 6f75 7263  e and open-sourc
-00001a70: 6520 736f 6674 7761 7265 206c 6963 656e  e software licen
-00001a80: 7365 6420 756e 6465 7220 7468 6520 3c61  sed under the <a
-00001a90: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00001aa0: 6974 6875 622e 636f 6d2f 6765 6361 642d  ithub.com/gecad-
-00001ab0: 6772 6f75 702f 7065 616b 2d6d 6173 2f62  group/peak-mas/b
-00001ac0: 6c6f 622f 6465 7665 6c6f 702f 4c49 4345  lob/develop/LICE
-00001ad0: 4e53 4522 2074 6172 6765 743d 225f 626c  NSE" target="_bl
-00001ae0: 616e 6b22 3e47 4e55 2047 656e 6572 616c  ank">GNU General
-00001af0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-00001b00: 7633 2e30 3c2f 613e 2e0d 0a              v3.0</a>...
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7065 616b  : 2.1.Name: peak
+00000020: 2d6d 6173 0a56 6572 7369 6f6e 3a20 312e  -mas.Version: 1.
+00000030: 302e 350a 5375 6d6d 6172 793a 2050 7974  0.5.Summary: Pyt
+00000040: 686f 6e2d 6261 7365 6420 6672 616d 6577  hon-based framew
+00000050: 6f72 6b20 666f 7220 6865 7465 726f 6765  ork for heteroge
+00000060: 6e65 6f75 7320 6167 656e 7420 636f 6d6d  neous agent comm
+00000070: 756e 6974 6965 730a 4175 7468 6f72 2d65  unities.Author-e
+00000080: 6d61 696c 3a20 4272 756e 6f20 5269 6265  mail: Bruno Ribe
+00000090: 6972 6f20 3c62 7267 7269 4069 7365 702e  iro <brgri@isep.
+000000a0: 6970 702e 7074 3e0a 5072 6f6a 6563 742d  ipp.pt>.Project-
+000000b0: 5552 4c3a 2048 6f6d 6570 6167 652c 2068  URL: Homepage, h
+000000c0: 7474 7073 3a2f 2f77 7777 2e67 6563 6164  ttps://www.gecad
+000000d0: 2e69 7365 702e 6970 702e 7074 2f70 6561  .isep.ipp.pt/pea
+000000e0: 6b0a 5072 6f6a 6563 742d 5552 4c3a 2047  k.Project-URL: G
+000000f0: 6974 6875 622c 2068 7474 7073 3a2f 2f67  ithub, https://g
+00000100: 6974 6875 622e 636f 6d2f 6765 6361 642d  ithub.com/gecad-
+00000110: 6772 6f75 702f 7065 616b 2d6d 6173 0a4b  group/peak-mas.K
+00000120: 6579 776f 7264 733a 2066 7261 6d65 776f  eywords: framewo
+00000130: 726b 2c6d 756c 7469 6167 656e 742c 6167  rk,multiagent,ag
+00000140: 656e 742d 6261 7365 642c 6563 6f73 7973  ent-based,ecosys
+00000150: 7465 6d2c 7370 6164 652c 786d 7070 0a43  tem,spade,xmpp.C
+00000160: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
+00000170: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000180: 6564 203a 3a20 474e 5520 4765 6e65 7261  ed :: GNU Genera
+00000190: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+000001a0: 2076 3320 2847 504c 7633 290a 436c 6173   v3 (GPLv3).Clas
+000001b0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000001c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001d0: 5079 7468 6f6e 0a43 6c61 7373 6966 6965  Python.Classifie
+000001e0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000001f0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000200: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
+00000210: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000220: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000230: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
+00000240: 6965 723a 2045 6e76 6972 6f6e 6d65 6e74  ier: Environment
+00000250: 203a 3a20 436f 6e73 6f6c 650a 436c 6173   :: Console.Clas
+00000260: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
+00000270: 6720 5379 7374 656d 203a 3a20 4d69 6372  g System :: Micr
+00000280: 6f73 6f66 7420 3a3a 2057 696e 646f 7773  osoft :: Windows
+00000290: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+000002a0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+000002b0: 2050 4f53 4958 203a 3a20 4c69 6e75 780a   POSIX :: Linux.
+000002c0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+000002d0: 6320 3a3a 2053 6369 656e 7469 6669 632f  c :: Scientific/
+000002e0: 456e 6769 6e65 6572 696e 670a 436c 6173  Engineering.Clas
+000002f0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00000300: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
+00000310: 6e65 6572 696e 6720 3a3a 2041 7274 6966  neering :: Artif
+00000320: 6963 6961 6c20 496e 7465 6c6c 6967 656e  icial Intelligen
+00000330: 6365 0a52 6571 7569 7265 732d 5079 7468  ce.Requires-Pyth
+00000340: 6f6e 3a20 3d3d 332e 392e 360a 4465 7363  on: ==3.9.6.Desc
+00000350: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+00000360: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00000370: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
+00000380: 7261 3a20 6275 696c 640a 5072 6f76 6964  ra: build.Provid
+00000390: 6573 2d45 7874 7261 3a20 6465 760a 4c69  es-Extra: dev.Li
+000003a0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
+000003b0: 4e53 450a 0a23 2050 4541 4b3a 2050 7974  NSE..# PEAK: Pyt
+000003c0: 686f 6e2d 6261 7365 6420 6672 616d 6577  hon-based framew
+000003d0: 6f72 6b20 666f 7220 6865 7465 726f 6765  ork for heteroge
+000003e0: 6e6f 7573 2061 6765 6e74 2063 6f6d 6d75  nous agent commu
+000003f0: 6e69 7469 6573 0a0a 215b 444f 495d 2868  nities..![DOI](h
+00000400: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000410: 6473 2e69 6f2f 7374 6174 6963 2f76 313f  ds.io/static/v1?
+00000420: 6c69 6e6b 3d68 7474 7073 3a2f 2f64 6f69  link=https://doi
+00000430: 2e6f 7267 2f31 302e 3130 3037 2f39 3738  .org/10.1007/978
+00000440: 2d33 2d30 3331 2d31 3830 3530 2d37 5f37  -3-031-18050-7_7
+00000450: 266c 696e 6b3d 6874 7470 733a 2f2f 646f  &link=https://do
+00000460: 692e 6f72 672f 3130 2e31 3030 372f 3937  i.org/10.1007/97
+00000470: 382d 332d 3033 312d 3138 3035 302d 375f  8-3-031-18050-7_
+00000480: 3726 6c61 6265 6c3d 444f 4926 6d65 7373  7&label=DOI&mess
+00000490: 6167 653d 3937 382d 332d 3033 312d 3138  age=978-3-031-18
+000004a0: 3035 302d 3726 636f 6c6f 723d 626c 7565  050-7&color=blue
+000004b0: 2920 215b 5079 5049 202d 2050 7974 686f  ) ![PyPI - Pytho
+000004c0: 6e20 5665 7273 696f 6e5d 2868 7474 7073  n Version](https
+000004d0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000004e0: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
+000004f0: 732f 7065 616b 2d6d 6173 2920 215b 5079  s/peak-mas) ![Py
+00000500: 5049 5d28 6874 7470 733a 2f2f 696d 672e  PI](https://img.
+00000510: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000520: 762f 7065 616b 2d6d 6173 2920 215b 4769  v/peak-mas) ![Gi
+00000530: 7448 7562 5d28 6874 7470 733a 2f2f 696d  tHub](https://im
+00000540: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000550: 6875 622f 6c69 6365 6e73 652f 6765 6361  hub/license/geca
+00000560: 642d 6772 6f75 702f 7065 616b 2d6d 6173  d-group/peak-mas
+00000570: 2920 215b 706f 7765 7265 6420 6279 5d28  ) ![powered by](
+00000580: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000590: 6c64 732e 696f 2f73 7461 7469 632f 7631  lds.io/static/v1
+000005a0: 3f6c 6162 656c 3d70 6f77 6572 6564 2532  ?label=powered%2
+000005b0: 3062 7926 6d65 7373 6167 653d 4745 4341  0by&message=GECA
+000005c0: 4426 636f 6c6f 723d 3137 3739 3835 266c  D&color=177985&l
+000005d0: 6162 656c 436f 6c6f 723d 6465 3564 3461  abelColor=de5d4a
+000005e0: 263f 6c69 6e6b 3d68 7474 703a 2f2f 6765  &?link=http://ge
+000005f0: 6361 642e 6973 6570 2e69 7070 2e70 7426  cad.isep.ipp.pt&
+00000600: 6c69 6e6b 3d68 7474 703a 2f2f 6765 6361  link=http://geca
+00000610: 642e 6973 6570 2e69 7070 2e70 742f 2920  d.isep.ipp.pt/) 
+00000620: 215b 636f 6465 2073 7479 6c65 5d28 6874  ![code style](ht
+00000630: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000640: 732e 696f 2f62 6164 6765 2f63 6f64 6525  s.io/badge/code%
+00000650: 3230 7374 796c 652d 626c 6163 6b2d 626c  20style-black-bl
+00000660: 6163 6b29 2021 5b69 6d70 6f72 7473 2069  ack) ![imports i
+00000670: 736f 7274 5d28 6874 7470 733a 2f2f 696d  sort](https://im
+00000680: 672e 7368 6965 6c64 732e 696f 2f73 7461  g.shields.io/sta
+00000690: 7469 632f 7631 3f6c 6162 656c 3d69 6d70  tic/v1?label=imp
+000006a0: 6f72 7473 266d 6573 7361 6765 3d69 736f  orts&message=iso
+000006b0: 7274 2663 6f6c 6f72 3d62 6c75 6526 6c61  rt&color=blue&la
+000006c0: 6265 6c43 6f6c 6f72 3d6f 7261 6e67 6529  belColor=orange)
+000006d0: 0a0a 5045 414b 2069 7320 6120 6d75 6c74  ..PEAK is a mult
+000006e0: 692d 6167 656e 7420 7379 7374 656d 2066  i-agent system f
+000006f0: 7261 6d65 776f 726b 2077 6869 6368 2068  ramework which h
+00000700: 656c 7073 2074 6865 2075 7365 7273 2064  elps the users d
+00000710: 6576 656c 6f70 2c20 6d6f 6e69 746f 722c  evelop, monitor,
+00000720: 2061 6e61 6c79 7a65 2061 6e64 206d 6169   analyze and mai
+00000730: 6e74 6169 6e20 6563 6f73 7973 7465 6d20  ntain ecosystem 
+00000740: 6f66 2068 6574 6572 6f67 656e 656f 7573  of heterogeneous
+00000750: 2061 6765 6e74 2063 6f6d 6d75 6e69 7469   agent communiti
+00000760: 6573 2e20 5468 6973 2065 636f 7379 7374  es. This ecosyst
+00000770: 656d 2069 7320 2077 6865 7265 2076 6172  em is  where var
+00000780: 696f 7573 206d 756c 7469 2d61 6765 6e74  ious multi-agent
+00000790: 2073 7973 7465 6d73 2063 616e 2063 6f65   systems can coe
+000007a0: 7869 7374 2c20 696e 7465 7261 6374 2061  xist, interact a
+000007b0: 6e64 2073 6861 7265 2072 6573 6f75 7263  nd share resourc
+000007c0: 6573 2062 6574 7765 656e 2074 6865 6d2e  es between them.
+000007d0: 200a 5468 6973 2066 7261 6d65 776f 726b   .This framework
+000007e0: 2069 7320 6261 7365 6420 6f6e 203c 6120   is based on <a 
+000007f0: 6872 6566 3d22 6874 7470 733a 2f2f 7370  href="https://sp
+00000800: 6164 652d 6d61 732e 7265 6164 7468 6564  ade-mas.readthed
+00000810: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000820: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
+00000830: 6b22 3e53 5041 4445 3c2f 613e 2e0a 0a0a  k">SPADE</a>....
+00000840: 2323 2050 7265 7265 7175 6973 6974 6573  ## Prerequisites
+00000850: 0a0a 2d20 5079 7468 6f6e 203d 3d20 332e  ..- Python == 3.
+00000860: 392e 360a 2d20 584d 5050 2053 6572 7665  9.6.- XMPP Serve
+00000870: 7220 285b 7365 6520 646f 6373 5d28 6874  r ([see docs](ht
+00000880: 7470 733a 2f2f 7777 772e 6765 6361 642e  tps://www.gecad.
+00000890: 6973 6570 2e69 7070 2e70 742f 7065 616b  isep.ipp.pt/peak
+000008a0: 2929 0a0a 0a23 2320 496e 7374 616c 6c69  ))...## Installi
+000008b0: 6e67 2050 4541 4b0a 0a23 2323 2043 6f6e  ng PEAK..### Con
+000008c0: 6461 0a0a 546f 2069 6e73 7461 6c6c 2075  da..To install u
+000008d0: 7369 6e67 2063 6f6e 6461 2c20 646f 776e  sing conda, down
+000008e0: 6c6f 6164 2074 6865 2065 6e76 6972 6f6e  load the environ
+000008f0: 6d65 6e74 2e79 6d6c 2066 696c 6520 6672  ment.yml file fr
+00000900: 6f6d 2074 6865 2072 6570 6f73 6974 6f72  om the repositor
+00000910: 7920 616e 6420 7468 656e 2075 7365 2074  y and then use t
+00000920: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00000930: 6d61 6e64 3a0a 6060 6062 6173 680a 2420  mand:.```bash.$ 
+00000940: 636f 6e64 6120 656e 7620 6372 6561 7465  conda env create
+00000950: 202d 2d66 696c 6520 656e 7669 726f 6e6d   --file environm
+00000960: 656e 742e 796d 6c09 0a60 6060 0a54 6869  ent.yml..```.Thi
+00000970: 7320 7769 6c6c 2063 7265 6174 6520 6120  s will create a 
+00000980: 636f 6e64 6120 656e 7669 726f 6e6d 656e  conda environmen
+00000990: 7420 6361 6c6c 6564 205f 7065 616b 5f2e  t called _peak_.
+000009a0: 0a0a 2323 2320 5069 700a 0a54 6f20 696e  ..### Pip..To in
+000009b0: 7374 616c 6c20 7573 696e 6720 7069 702c  stall using pip,
+000009c0: 206a 7573 7420 7479 7065 2074 6865 2066   just type the f
+000009d0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+000009e0: 3a0a 6060 6062 6173 680a 2420 7069 7020  :.```bash.$ pip 
+000009f0: 696e 7374 616c 6c20 7065 616b 2d6d 6173  install peak-mas
+00000a00: 0a60 6060 0a0a 0a23 2320 5573 696e 6720  .```...## Using 
+00000a10: 5045 414b 0a0a 2323 2320 4e6f 7465 7320  PEAK..### Notes 
+00000a20: 6f6e 2053 5041 4445 0a0a 4173 2061 6c72  on SPADE..As alr
+00000a30: 6561 6479 2073 6169 6420 5045 414b 2069  eady said PEAK i
+00000a40: 7320 6261 7365 6420 6f6e 2053 5041 4445  s based on SPADE
+00000a50: 2e20 5468 6973 206d 6561 6e73 2074 6861  . This means tha
+00000a60: 7420 6576 6572 7920 6675 6e63 7469 6f6e  t every function
+00000a70: 616c 6974 7920 6f66 2053 5041 4445 2069  ality of SPADE i
+00000a80: 7320 6176 6169 6c61 626c 6520 746f 2074  s available to t
+00000a90: 6865 2075 7365 722e 2057 6520 6869 6768  he user. We high
+00000aa0: 6c79 2072 6563 6f6d 6d65 6e64 2079 6f75  ly recommend you
+00000ab0: 2074 6f20 7365 6520 3c61 2068 7265 663d   to see <a href=
+00000ac0: 2268 7474 7073 3a2f 2f73 7061 6465 2d6d  "https://spade-m
+00000ad0: 6173 2e72 6561 6474 6865 646f 6373 2e69  as.readthedocs.i
+00000ae0: 6f2f 656e 2f6c 6174 6573 742f 2220 7461  o/en/latest/" ta
+00000af0: 7267 6574 3d22 5f62 6c61 6e6b 223e 5350  rget="_blank">SP
+00000b00: 4144 453c 2f61 3e20 6578 616d 706c 6573  ADE</a> examples
+00000b10: 2061 6e64 2064 6f63 756d 656e 7461 7469   and documentati
+00000b20: 6f6e 2062 6566 6f72 6520 7374 6172 7469  on before starti
+00000b30: 6e67 2075 7369 6e67 2050 4541 4b2e 204f  ng using PEAK. O
+00000b40: 6e63 6520 796f 7520 6172 6520 6661 6d69  nce you are fami
+00000b50: 6c69 6172 697a 6564 2077 6974 6820 5350  liarized with SP
+00000b60: 4144 4527 7320 6d65 6368 616e 6963 7320  ADE's mechanics 
+00000b70: 796f 7520 6361 6e20 7374 6172 7420 7573  you can start us
+00000b80: 696e 6720 5045 414b 2e0a 0a23 2323 204e  ing PEAK...### N
+00000b90: 6f74 6573 206f 6e20 584d 5050 0a0a 546f  otes on XMPP..To
+00000ba0: 2072 756e 2061 6e79 2050 4541 4b27 7320   run any PEAK's 
+00000bb0: 6167 656e 7420 796f 7520 7769 6c6c 206e  agent you will n
+00000bc0: 6565 6420 6120 584d 5050 2073 6572 7665  eed a XMPP serve
+00000bd0: 722e 2059 6f75 2063 616e 2065 6974 6865  r. You can eithe
+00000be0: 7220 636f 6e66 6967 7572 6520 6f6e 6520  r configure one 
+00000bf0: 6f6e 2079 6f75 7220 6d61 6368 696e 652c  on your machine,
+00000c00: 2072 656d 6f74 656c 7920 6f72 2075 7365   remotely or use
+00000c10: 2061 2070 7562 6c69 6320 7365 7276 6572   a public server
+00000c20: 2e20 5468 6520 6f6e 6c79 2069 7373 7565  . The only issue
+00000c30: 2077 6974 6820 7468 6520 7075 626c 6963   with the public
+00000c40: 2073 6572 7665 7273 2069 7320 7468 6174   servers is that
+00000c50: 2074 6865 7920 646f 6e27 7420 7573 7561   they don't usua
+00000c60: 6c6c 7920 6861 7665 2061 6c6c 2074 6865  lly have all the
+00000c70: 2063 6f6e 6669 6775 7261 7469 6f6e 7320   configurations 
+00000c80: 7265 7175 6972 6564 2074 6f20 7275 6e20  required to run 
+00000c90: 736f 6d65 2050 4541 4b27 7320 6675 6e63  some PEAK's func
+00000ca0: 7469 6f6e 616c 6974 6965 732e 2054 6f20  tionalities. To 
+00000cb0: 636f 6e66 6967 7572 6520 7468 6520 7365  configure the se
+00000cc0: 7276 6572 2079 6f75 2063 616e 2072 6561  rver you can rea
+00000cd0: 6420 7468 6520 2243 6f6e 6669 6775 7265  d the "Configure
+00000ce0: 2058 4d50 5020 7365 7276 6572 2220 7365   XMPP server" se
+00000cf0: 6374 696f 6e20 696e 2074 6865 203c 6120  ction in the <a 
+00000d00: 6872 6566 3d22 6874 7470 3a2f 2f77 7777  href="http://www
+00000d10: 2e67 6563 6164 2e69 7365 702e 6970 702e  .gecad.isep.ipp.
+00000d20: 7074 2f70 6561 6b22 2074 6172 6765 743d  pt/peak" target=
+00000d30: 225f 626c 616e 6b22 3e64 6f63 756d 656e  "_blank">documen
+00000d40: 7461 7469 6f6e 3c2f 613e 2e0a 0a23 2323  tation</a>...###
+00000d50: 2048 656c 6c6f 2057 6f72 6c64 2041 6765   Hello World Age
+00000d60: 6e74 2045 7861 6d70 6c65 0a0a 4f6e 6520  nt Example..One 
+00000d70: 7468 696e 6720 7468 6174 2077 6173 2061  thing that was a
+00000d80: 6464 6564 2069 6e20 5045 414b 2077 6173  dded in PEAK was
+00000d90: 2074 6865 2077 6179 2074 6865 2075 7365   the way the use
+00000da0: 7220 6578 6563 7574 6573 2074 6865 2061  r executes the a
+00000db0: 6765 6e74 732e 2050 4541 4b20 6164 6465  gents. PEAK adde
+00000dc0: 6420 6120 434c 492c 2069 6e73 7069 7265  d a CLI, inspire
+00000dd0: 6420 696e 204a 4144 452c 2074 6f20 6865  d in JADE, to he
+00000de0: 6c70 2074 6865 2075 7365 7220 6578 6563  lp the user exec
+00000df0: 7574 6520 656e 6420 636f 6e66 6967 7572  ute end configur
+00000e00: 6520 6561 6368 2061 6765 6e74 2069 6e20  e each agent in 
+00000e10: 6120 6561 7379 2061 6e64 2069 6e74 7569  a easy and intui
+00000e20: 7469 7665 206d 616e 6e65 722e 0a49 6e20  tive manner..In 
+00000e30: 7468 6973 2065 7861 6d70 6c65 2077 6520  this example we 
+00000e40: 7769 6c6c 2073 686f 7720 796f 7520 686f  will show you ho
+00000e50: 7720 746f 2065 7865 6375 7465 2061 2073  w to execute a s
+00000e60: 696e 676c 6520 6167 656e 742e 2053 6176  ingle agent. Sav
+00000e70: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00000e80: 636f 6465 2069 6e20 6120 6669 6c65 2063  code in a file c
+00000e90: 616c 6c65 6420 6061 6765 6e74 2e70 7960  alled `agent.py`
+00000ea0: 2e0a 0a60 6060 7079 7468 6f6e 200a 6672  ...```python .fr
+00000eb0: 6f6d 2070 6561 6b20 696d 706f 7274 2041  om peak import A
+00000ec0: 6765 6e74 0a66 726f 6d20 7065 616b 2e62  gent.from peak.b
+00000ed0: 6568 6176 696f 7572 7320 696d 706f 7274  ehaviours import
+00000ee0: 204f 6e65 5368 6f74 4265 6861 7669 6f75   OneShotBehaviou
+00000ef0: 720a 0a63 6c61 7373 2061 6765 6e74 2841  r..class agent(A
+00000f00: 6765 6e74 293a 0ac2 a020 c2a0 2063 6c61  gent):... .. cla
+00000f10: 7373 2048 656c 6c6f 576f 726c 6428 4f6e  ss HelloWorld(On
+00000f20: 6553 686f 7442 6568 6176 696f 7572 293a  eShotBehaviour):
+00000f30: 0ac2 a020 c2a0 20c2 a020 c2a0 2061 7379  ... .. .. .. asy
+00000f40: 6e63 2064 6566 2072 756e 2873 656c 6629  nc def run(self)
+00000f50: 202d 3e20 4e6f 6e65 3a0a c2a0 20c2 a020   -> None:... .. 
+00000f60: c2a0 20c2 a020 c2a0 20c2 a020 7072 696e  .. .. .. .. prin
+00000f70: 7428 2248 656c 6c6f 2057 6f72 6c64 2229  t("Hello World")
+00000f80: 0ac2 a020 c2a0 20c2 a020 c2a0 20c2 a020  ... .. .. .. .. 
+00000f90: c2a0 2061 7761 6974 2073 656c 662e 6167  .. await self.ag
+00000fa0: 656e 742e 7374 6f70 2829 0a0a c2a0 20c2  ent.stop().... .
+00000fb0: a020 6173 796e 6320 6465 6620 7365 7475  . async def setu
+00000fc0: 7028 7365 6c66 2920 2d3e 204e 6f6e 653a  p(self) -> None:
+00000fd0: 0ac2 a020 c2a0 20c2 a020 c2a0 2073 656c  ... .. .. .. sel
+00000fe0: 662e 6164 645f 6265 6861 7669 6f75 7228  f.add_behaviour(
+00000ff0: 7365 6c66 2e48 656c 6c6f 576f 726c 6428  self.HelloWorld(
+00001000: 2929 0a60 6060 0a49 7420 6973 206e 6563  )).```.It is nec
+00001010: 6573 7361 7279 2074 6861 7420 7468 6520  essary that the 
+00001020: 6e61 6d65 206f 6620 7468 6520 6669 6c65  name of the file
+00001030: 2069 7320 7468 6520 7361 6d65 2061 7320   is the same as 
+00001040: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
+00001050: 6167 656e 7427 7320 636c 6173 7320 736f  agent's class so
+00001060: 2050 4541 4b20 6361 6e20 646f 2074 6865   PEAK can do the
+00001070: 2070 726f 7065 7220 7061 7273 696e 672e   proper parsing.
+00001080: 2054 6869 7320 6167 656e 7420 6f6e 6c79   This agent only
+00001090: 2068 6173 2061 2062 6568 6176 696f 7220   has a behavior 
+000010a0: 7468 6174 2070 7269 6e74 7320 746f 2074  that prints to t
+000010b0: 6865 2074 6572 6d69 6e61 6c20 7468 6520  he terminal the 
+000010c0: 2248 656c 6c6f 2057 6f72 6c64 2220 6d65  "Hello World" me
+000010d0: 7373 6167 652e 2054 6f20 6578 6563 7574  ssage. To execut
+000010e0: 6520 7468 6520 6167 656e 7420 6a75 7374  e the agent just
+000010f0: 2074 7970 6520 7468 6520 666f 6c6c 6f77   type the follow
+00001100: 696e 6720 636f 6d6d 616e 643a 0a60 6060  ing command:.```
+00001110: 6261 7368 200a 2420 7065 616b 2072 756e  bash .$ peak run
+00001120: 2070 6174 682f 746f 2f61 6765 6e74 2e70   path/to/agent.p
+00001130: 7920 2d6a 2061 6765 6e74 406c 6f63 616c  y -j agent@local
+00001140: 686f 7374 0a60 6060 0a43 6861 6e67 6520  host.```.Change 
+00001150: 7468 6520 606c 6f63 616c 686f 7374 6020  the `localhost` 
+00001160: 746f 2074 6865 2064 6f6d 6169 6e20 6f66  to the domain of
+00001170: 2074 6865 2058 4d50 5020 7365 7276 6572   the XMPP server
+00001180: 2079 6f75 2077 616e 7420 746f 2063 6f6e   you want to con
+00001190: 6e65 6374 2e0a 0a3c 6465 7461 696c 733e  nect...<details>
+000011a0: 3c73 756d 6d61 7279 3e4e 6f74 653c 2f73  <summary>Note</s
+000011b0: 756d 6d61 7279 3e0a 3c70 3e0a 0a49 6620  ummary>.<p>..If 
+000011c0: 796f 7520 7761 6e74 2074 6f20 6b6e 6f77  you want to know
+000011d0: 206d 6f72 6520 6162 6f75 7420 6561 6368   more about each
+000011e0: 2063 6f6d 6d61 6e64 2077 6520 7265 636f   command we reco
+000011f0: 6d6d 656e 6420 7265 6164 696e 6720 7468  mmend reading th
+00001200: 6520 5b64 6f63 756d 656e 7461 7469 6f6e  e [documentation
+00001210: 5d28 6874 7470 3a2f 2f77 7777 2e67 6563  ](http://www.gec
+00001220: 6164 2e69 7365 702e 6970 702e 7074 2f70  ad.isep.ipp.pt/p
+00001230: 6561 6b29 206f 7220 7573 696e 6720 7468  eak) or using th
+00001240: 6520 602d 6860 206f 7074 696f 6e20 746f  e `-h` option to
+00001250: 2073 6565 2074 6865 2068 656c 7020 6d65   see the help me
+00001260: 7373 6167 652e 0a0a 3c2f 703e 0a3c 2f64  ssage...</p>.</d
+00001270: 6574 6169 6c73 3e0a 0a46 6f72 206d 6f72  etails>..For mor
+00001280: 6520 6164 7661 6e63 6564 2066 756e 6374  e advanced funct
+00001290: 696f 6e61 6c69 7469 6573 2061 6e64 2065  ionalities and e
+000012a0: 7861 6d70 6c65 7320 7765 2072 6563 6f6d  xamples we recom
+000012b0: 6d65 6e64 2079 6f75 2074 6f20 6865 6164  mend you to head
+000012c0: 2066 6f72 7761 7264 2074 6f20 7468 6520   forward to the 
+000012d0: 3c61 2068 7265 663d 2268 7474 703a 2f2f  <a href="http://
+000012e0: 7777 772e 6765 6361 642e 6973 6570 2e69  www.gecad.isep.i
+000012f0: 7070 2e70 742f 7065 616b 2220 7461 7267  pp.pt/peak" targ
+00001300: 6574 3d22 5f62 6c61 6e6b 223e 646f 6375  et="_blank">docu
+00001310: 6d65 6e74 6174 696f 6e20 7765 6273 6974  mentation websit
+00001320: 653c 2f61 3e2e 0a0a 0a23 2320 5375 7070  e</a>....## Supp
+00001330: 6f72 740a 0a55 7365 2074 6865 203c 6120  ort..Use the <a 
+00001340: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001350: 7468 7562 2e63 6f6d 2f67 6563 6164 2d67  thub.com/gecad-g
+00001360: 726f 7570 2f70 6561 6b2d 6d61 732f 6469  roup/peak-mas/di
+00001370: 7363 7573 7369 6f6e 7322 2074 6172 6765  scussions" targe
+00001380: 743d 225f 626c 616e 6b22 3e44 6973 6375  t="_blank">Discu
+00001390: 7373 696f 6e3c 2f61 3e20 7061 6765 2069  ssion</a> page i
+000013a0: 6620 796f 7520 6861 7665 2061 6e79 2071  f you have any q
+000013b0: 7565 7374 696f 6e73 206f 7220 6964 6561  uestions or idea
+000013c0: 7320 796f 7520 776f 756c 6420 6c69 6b65  s you would like
+000013d0: 2073 6f20 7365 6520 696d 706c 656d 656e   so see implemen
+000013e0: 7465 642e 0a54 6f20 616c 6572 7420 616e  ted..To alert an
+000013f0: 2069 7373 7565 206f 7220 6120 6275 6720   issue or a bug 
+00001400: 706c 6561 7365 2070 6f73 7420 696e 2074  please post in t
+00001410: 6865 203c 6120 6872 6566 3d22 6874 7470  he <a href="http
+00001420: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
+00001430: 6563 6164 2d67 726f 7570 2f70 6561 6b2d  ecad-group/peak-
+00001440: 6d61 732f 6973 7375 6573 2220 7461 7267  mas/issues" targ
+00001450: 6574 3d22 5f62 6c61 6e6b 223e 4973 7375  et="_blank">Issu
+00001460: 6573 3c2f 613e 2070 6167 652e 0a0a 2323  es</a> page...##
+00001470: 2052 6f61 646d 6170 0a0a 5468 6973 2061   Roadmap..This a
+00001480: 7265 2073 6f6d 6520 6675 6e63 7469 6f6e  re some function
+00001490: 616c 6974 6965 7320 7468 6174 2061 7265  alities that are
+000014a0: 2062 6569 6e67 2064 6576 656c 6f70 6564   being developed
+000014b0: 2061 6e64 2077 696c 6c20 6265 2072 656c   and will be rel
+000014c0: 6561 7365 6420 696e 2061 206e 6561 7220  eased in a near 
+000014d0: 6675 7475 7265 3a0a 2d20 5b20 5d20 4372  future:.- [ ] Cr
+000014e0: 6561 7465 2061 2044 6f63 6b65 7220 666f  eate a Docker fo
+000014f0: 7220 584d 5050 2073 6572 7665 7220 616e  r XMPP server an
+00001500: 6420 5045 414b 2e0a 2d20 5b20 5d20 4164  d PEAK..- [ ] Ad
+00001510: 6420 6479 6e61 6d69 6320 7370 6565 6420  d dynamic speed 
+00001520: 6f70 7469 6f6e 2074 6f20 5045 414b 2773  option to PEAK's
+00001530: 2069 6e74 6572 6e61 6c20 636c 6f63 6b2e   internal clock.
+00001540: 0a2d 205b 205d 2041 6464 206d 756c 7469  .- [ ] Add multi
+00001550: 2d74 6872 6561 6469 6e67 206f 7074 696f  -threading optio
+00001560: 6e20 746f 2074 6865 2065 7865 6375 7469  n to the executi
+00001570: 6f6e 2063 6f6e 6669 6775 7261 7469 6f6e  on configuration
+00001580: 732e 0a2d 205b 205d 2049 6d70 6c65 6d65  s..- [ ] Impleme
+00001590: 6e74 2059 656c 6c6f 7720 5061 6765 2053  nt Yellow Page S
+000015a0: 6572 7669 6365 2069 6e20 4446 2061 6765  ervice in DF age
+000015b0: 6e74 2e0a 2d20 5b20 5d20 496d 706c 656d  nt..- [ ] Implem
+000015c0: 656e 7420 4461 7461 2041 6e61 6c79 7369  ent Data Analysi
+000015d0: 7320 7365 6374 696f 6e20 696e 2074 6865  s section in the
+000015e0: 2044 6173 6862 6f61 7264 2e0a 0a23 2320   Dashboard...## 
+000015f0: 5363 6965 6e74 6966 6963 2050 7562 6c69  Scientific Publi
+00001600: 6361 7469 6f6e 730a 0a2d 2052 6962 6569  cations..- Ribei
+00001610: 726f 2c20 422e 2c20 5065 7265 6972 612c  ro, B., Pereira,
+00001620: 2048 2e2c 2047 6f6d 6573 2c20 4c2e 2c20   H., Gomes, L., 
+00001630: 5661 6c65 2c20 5a2e 2028 3230 3233 292e  Vale, Z. (2023).
+00001640: 2050 7974 686f 6e2d 4261 7365 6420 4563   Python-Based Ec
+00001650: 6f73 7973 7465 6d20 666f 7220 4167 656e  osystem for Agen
+00001660: 7420 436f 6d6d 756e 6974 6965 7320 5369  t Communities Si
+00001670: 6d75 6c61 7469 6f6e 2e20 496e 3a20 2cc2  mulation. In: ,.
+00001680: a05f 6574 2061 6c2e 5fc2 a031 3774 6820  ._et al._..17th 
+00001690: 496e 7465 726e 6174 696f 6e61 6c20 436f  International Co
+000016a0: 6e66 6572 656e 6365 206f 6e20 536f 6674  nference on Soft
+000016b0: 2043 6f6d 7075 7469 6e67 204d 6f64 656c   Computing Model
+000016c0: 7320 696e 2049 6e64 7573 7472 6961 6c20  s in Industrial 
+000016d0: 616e 6420 456e 7669 726f 6e6d 656e 7461  and Environmenta
+000016e0: 6c20 4170 706c 6963 6174 696f 6e73 2028  l Applications (
+000016f0: 534f 434f 2032 3032 3229 2e20 534f 434f  SOCO 2022). SOCO
+00001700: 2032 3032 322e 204c 6563 7475 7265 204e   2022. Lecture N
+00001710: 6f74 6573 2069 6e20 4e65 7477 6f72 6b73  otes in Networks
+00001720: 2061 6e64 2053 7973 7465 6d73 2c20 766f   and Systems, vo
+00001730: 6c20 3533 312e 2053 7072 696e 6765 722c  l 531. Springer,
+00001740: 2043 6861 6d2e 2068 7474 7073 3a2f 2f64   Cham. https://d
+00001750: 6f69 2e6f 7267 2f31 302e 3130 3037 2f39  oi.org/10.1007/9
+00001760: 3738 2d33 2d30 3331 2d31 3830 3530 2d37  78-3-031-18050-7
+00001770: 5f37 0a0a 2323 2043 6f6e 7472 6962 7574  _7..## Contribut
+00001780: 696e 6720 746f 2050 4541 4b0a 0a50 756c  ing to PEAK..Pul
+00001790: 6c20 7265 7175 6573 7473 2061 7265 2077  l requests are w
+000017a0: 656c 636f 6d65 2e20 466f 7220 6d61 6a6f  elcome. For majo
+000017b0: 7220 6368 616e 6765 732c 2070 6c65 6173  r changes, pleas
+000017c0: 6520 6f70 656e 2061 2064 6973 6375 7373  e open a discuss
+000017d0: 696f 6e20 6669 7273 7420 746f 2064 6973  ion first to dis
+000017e0: 6375 7373 2077 6861 7420 796f 7520 776f  cuss what you wo
+000017f0: 756c 6420 6c69 6b65 2074 6f20 6368 616e  uld like to chan
+00001800: 6765 2e0a 0a54 6865 2065 7861 6d70 6c65  ge...The example
+00001810: 7320 6172 6520 7573 6564 2061 7320 6120  s are used as a 
+00001820: 666f 726d 206f 6620 7465 7374 696e 6720  form of testing 
+00001830: 7468 6520 6672 616d 6577 6f72 6b2e 2053  the framework. S
+00001840: 6f20 706c 6561 7365 206d 616b 6520 7375  o please make su
+00001850: 7265 2074 6f20 7570 6461 7465 2074 6865  re to update the
+00001860: 2065 7861 6d70 6c65 7320 6173 2061 7070   examples as app
+00001870: 726f 7072 6961 7465 206f 7220 6d61 6b65  ropriate or make
+00001880: 206e 6577 206f 6e65 732e 200a 0a54 6f20   new ones. ..To 
+00001890: 666f 726d 6174 2074 6865 2063 6f64 6520  format the code 
+000018a0: 706c 6561 7365 2075 7365 2074 6865 203c  please use the <
+000018b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000018c0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000018d0: 2f62 6c61 636b 2f22 2074 6172 6765 743d  /black/" target=
+000018e0: 225f 626c 616e 6b22 3e62 6c61 636b 3c2f  "_blank">black</
+000018f0: 613e 2061 6e64 203c 6120 6872 6566 3d22  a> and <a href="
+00001900: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00001910: 2f70 726f 6a65 6374 2f69 736f 7274 2f22  /project/isort/"
+00001920: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00001930: 3e69 736f 7274 3c2f 613e 2070 6163 6b61  >isort</a> packa
+00001940: 6765 732e 200a 0a46 6f72 2074 6865 2063  ges. ..For the c
+00001950: 6f6d 6d69 7473 2070 6c65 6173 6520 666f  ommits please fo
+00001960: 6c6c 6f77 2074 6865 203c 6120 6872 6566  llow the <a href
+00001970: 3d22 7777 772e 636f 6e76 656e 7469 6f6e  ="www.convention
+00001980: 616c 636f 6d6d 6974 732e 6f72 6722 2074  alcommits.org" t
+00001990: 6172 6765 743d 225f 626c 616e 6b22 3e43  arget="_blank">C
+000019a0: 6f6e 7665 6e74 696f 6e61 6c20 436f 6d6d  onventional Comm
+000019b0: 6974 7320 4775 6964 656c 696e 653c 2f61  its Guideline</a
+000019c0: 3e2e 0a0a 2323 204c 6963 656e 7365 0a0a  >...## License..
+000019d0: 6050 4541 4b60 c2a0 6973 2066 7265 6520  `PEAK`..is free 
+000019e0: 616e 6420 6f70 656e 2d73 6f75 7263 6520  and open-source 
+000019f0: 736f 6674 7761 7265 206c 6963 656e 7365  software license
+00001a00: 6420 756e 6465 7220 7468 6520 3c61 2068  d under the <a h
+00001a10: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00001a20: 6875 622e 636f 6d2f 6765 6361 642d 6772  hub.com/gecad-gr
+00001a30: 6f75 702f 7065 616b 2d6d 6173 2f62 6c6f  oup/peak-mas/blo
+00001a40: 622f 6465 7665 6c6f 702f 4c49 4345 4e53  b/develop/LICENS
+00001a50: 4522 2074 6172 6765 743d 225f 626c 616e  E" target="_blan
+00001a60: 6b22 3e47 4e55 2047 656e 6572 616c 2050  k">GNU General P
+00001a70: 7562 6c69 6320 4c69 6365 6e73 6520 7633  ublic License v3
+00001a80: 2e30 3c2f 613e 2e0a                      .0</a>..
```


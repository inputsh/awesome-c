# awesome-c [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)][387]

A curated list of C good stuff. This list contains *only* [free software][13] for code, and sellers who aren't evil for physical resources.

**LOOKING FOR MAINTAINERS:** This list is currently pretty much inactive. I'm looking for maintainers that can make it great again. See [#26](https://github.com/aleksandar-todorovic/awesome-c/issues/26) for more info, but the process is simple: add or fix a couple of things in this list and you'll become a contributor to a 850+ stars list.

This list was previously maintained by [@kozross](https://github.com/kozross). He decided to switch the list to a [new platform](https://notabug.org/koz.ross/awesome-c), so I've decided to fork it so we could keep it on GitHub.

Contents
========

## Contents ##

- [Build Systems](#build-systems)
- [Compilers](#compilers)
- [Compression](#compression)
- [Crypto](#crypto)
- [Database](#database)
- [Deep Learning](#deep-learning)
- [Documentation Generation](#documentation-generation)
- [Editors](#editors)
- [Embedded Systems](#embedded-systems)
  - [RTOS](#rtos)
- [Environments](#environments)
- [Frameworks](#frameworks)
- [Game Programming](#game-programming)
  - [Engines](#engines)
  - [Resources](#resources)
- [Generic Programming](#generic-programming)
- [Graphics](#graphics)
  - [Graphic APIs](#graphic-apis)
- [Graphical User Interface](#graphical-user-interface)
- [Image Processing](#image-processing)
- [JSON](#json)
- [Learning, Reference and Tutorials](#learning-reference-and-tutorials)
  - [Online](#online)
      - [Reference](#reference)
      - [Beginner](#beginner)
      - [Intermediate](#intermediate)
      - [Advanced](#advanced)
      - [Self-study courses](#self-study-courses)
  - [Physical](#physical)
      - [Reference](#reference-1)
      - [Beginner](#beginner-1)
      - [Intermediate](#intermediate-1)
      - [Advanced](#advanced-1)
- [Multimedia](#multimedia)
- [Networking and Internet](#networking-and-internet)
  - [Web Frameworks](#web-frameworks)
- [Numerical](#numerical)
- [Parallel Programming](#parallel-programming)
- [Regex](#regex)
- [Serialization](#serialization)
- [Source Code Collections](#source-code-collections)
- [Standard Libraries](#standard-libraries)
- [String Manipulation](#string-manipulation)
- [Testing](#testing)
- [Text Editor Extensions](#text-editor-extensions)
  - [Emacs](#emacs)
  - [Vim](#vim)
- [Tools](#tools)
- [Utilities](#utilities)
- [XML](#xml)

## Build Systems ##

These are tools to automate the building and testing of projects in C.

* [aimake][97] - Build tool designed to avoid complex configurations. [[GNU GPL3][LIC1] or later]
* [Autoconf][305] - Extensible package of M4 macros that produce shell scripts to automatically configure software source code packages. Part of the Autotools. [[GNU GPL3][LIC1] or later]
* [Automake][306] - Tool for automatically generating ``Makefile.in`` files compliant with the GNU Coding Standards. Requires the use of Autoconf. Part of the Autotools. [[GNU GPL3][LIC1] or later]
* [CMake][410] - Tools for cross-platform building, testing, and packaging. [[3-clause BSD][LIC2]]
* [Jam][334] - Build system, designed to be easier than make. Understands C build rules implicitly. [[Jam License][LIC3]]
* [Libtool][172] - Generic library support script. Part of the Autotools. [[GNU GPL3][LIC1] or later]
* [Meson][368] - Extremely fast, user-friendly build system. Based on Ninja. [[Apache2.0][LIC4]]
* [Premake][403] - Build script generator for toolsets like Visual Studio, Xcode, or GNU Make. [[3-clause BSD][LIC5]]
* [SCons][420] - An easier, more reliable and faster way to build software. [MIT License][LIC18].

## Compilers ##

* [Clang][38] - C compiler for LLVM. Supports C11. [[NCSA][LIC6]]
* [CompCert][269] - Fully-verified C compiler. Supports almost all of C89. [[GNU GPL2.1][LIC7] or later]
* [GCC][40] - Provides a C compiler as part of its compiler set. Supports C11 and OpenMP. [[GNU GPL3][LIC1] or later]
* [PCC][74] - Venerable C compiler. Supports C99. [[Various free licenses][LIC8]]
* [TCC][58] - Tiny C Compiler; a small, fast C compiler. Supports C99 (except complex types). [[GNU LGPL2.1][LIC9] only]

## Compression ##

* [libzip][408] - A C library for reading, creating, and modifying zip archives. [[3-clause BSD][LIC5]]
* [lzo][338] - Very fast data compression library. [[GNU GPL2.1][LIC7]]
* [zlib][230] - Massively-spiffy yet delicately-unobtrusive compression library. [[3-clause BSD][LIC5]]

## Crypto ##

* [GnuTLS][112] - Secure communication library, implementing SSL, TLS and DTLS. [[GNU LGPL2.1][LIC9] or later]
* [libgcrypt][142] - General-purpose cryptography library, with a range of available ciphers. [[GNU LGPL2.1][LIC9] or later (code)] and [[GNU GPL2.1][LIC7] or later (manual and tools)]
* [OpenSSL][110] - Implementation of the SSL and TLS protocols, and also includes a cryptography library. [[Dual Licensed under the OpenSSL License and the SSLeay License][LIC10]]
* [libsodium][198] - Modern and easy-to-use crypto library. [[Expat][LIC11]]
* [libtomcrypt][299] - Fairly comprehensive, modular and portable cryptographic toolkit. [Public domain]
* [mbed TLS][291] - Another crypto implementation for C. [[Apache2.0][LIC4]]

## Database ##

This lists databases and data stores with C APIs.

* [BerkeleyDB][380] - Library for a high-performance embedded database for key-value data. [[GNU AGPLv3][LIC13] only]
* [Hiredis][201] - Minimalistic client library for Redis. [[3-clause BSD][LIC5]]
* [LMDB][105] - Ultra-fast, ultra-compact key-value embedded data store. [[newOpenLDAP][LIC14]]
* [MariaDB][25] - Robust, scalable and reliable SQL server, designed to be a drop-in replacement for MySQL. [[3-clause BSD][LIC5]]
* [mongo-c-driver][233] - High-performance client library for [MongoDB][234]. [[Apache2.0][LIC4]]
* [PostgreSQL][121] - Powerful object-relational database system. [[PostgreSQL licence][LIC15]]
* [recutils][360] - Set of tools and a C library for accessing human-editable, plaintext database files called recfiles. [[GNU GPL3][LIC1] or later]
* [Redis][51] - Advanced key-value store. [[3-clause BSD][LIC5]]
* [sophia][244] - Modern, embeddable key-value database. [[FreeBSD][LIC16]]
* [SQLite][22] - Self-contained, serverless, zero-configuration, transactional SQL database engine with a C interface. [Public domain]
* [UnQLite][23] - Self-contained, serverless, zero-configuration, transactional NoSQL engine with a C interface. [[FreeBSD][LIC16]]

## Deep Learning ##
* [Darknet][396] - Open source neural network framework written in C and CUDA. It is fast, easy to install, and supports CPU and GPU computation.

## Documentation Generation ##

* [Cxref][317] - Generates documentation of C programs in either LaTeX, HTML, RTF or SGML. [[GNU GPL2.1][LIC7] only]
* [DocOnce][322] - Modestly-tagged markup language that can be used to generate a range of formats. [[3-clause BSD][LIC5]]
* [Doxygen][318] - The de-facto standard tool for generating C documentation from annotated sources. Can generate a large range of formats. [[GNU GPL2.1][LIC7] only]
* [GTK-Doc][319] - Tool for generating C documentation from annotated sources. Has support for the Autotools. [[GNU GPL2.1][LIC9] only (code)] or [[GNU FDL1.1][LIC17]]

## Editors ##

These are specifically fancier, IDE-type editors. If you want a programmer's text editor, look elsewhere. Besides, whatever choice you make most likely supports C anyway.

* [Anjuta DevStudio][42] - The GNOME IDE. [[GNU GPL2.1][LIC9] only]
* [Atom][412] - Hackable text editor for the 21st century. [[MIT][LIC18]]
* [Code::Blocks][249] - Extensible, configurable IDE supporting C. [[GNU GPL3][LIC1] only]
* [CodeLite][45] - Cross-platform IDE. [[GNU GPL2.1][LIC7] only]
* [Eclipse][258] - IDE written in Java. [[EPL][LIC19]]
* [Geany][43] - Very small and fast IDE. [[GNU GPL2.1][LIC7] or later]
* [KDevelop][44] - The KDE IDE. [[GNU GPL2.1][LIC7] only]
* [Qt Creator][394] - Cross-platform IDE written with C++ and Qt, part of the Qt SDK. Supports Clang Code Model. [[GNU GPL3 with Qt exception][LIC20] only]
* [Visual Studio Code][419] - Code editing, redefined. Visual Studio Code.

## Embedded Systems ##

These are projects that allow one to work with microcontrollers and other resource constrained architectures.

### RTOS ###

A real-time operating system (RTOS) is intended to serve real-time applications that process data with low latency delay.

* [Amazon FreeRTOS][414] - RTOS for microcontrollers that makes small, low-power edge devices easy to program. [[MIT][LIC21]]
* [ChibiOS][416] - RTOS with complete development environment (HAL, drivers, support files, and tools). [[Various][LIC22]]
* [Contiki][418] - Connect low-cost, low power microcontrollers to the Internet. [[3-clause BSD][LIC23]]
* [Zephyr Project][404] - Scalable real-time RTOS supporting multiple hardware architectures, optimized for resource constrained devices. [[Apache2.0][LIC4]]

## Environments ##

This is a list of technologies designed to bring Windows into the 21st century with respect to support for C.

* [Cygwin][253] - Designed to emulate a POSIX-compatible environment extensively under Windows. [[Various free licenses][LIC24]]
* [MinGW-w64][287] - Minimalist environment for C development on Windows with 64 bit support. [[Various free licenses][LIC25]]

## Frameworks ##

This section has big libraries that provide data structures and other stuff you expect of a 'modern' standard library.

* [APR][78] - Apache Portable Runtime; another library of cross-platform utility functions. [[Apache2.0][LIC4]]
* [C Algorithms][88] - Collection of common algorithms and data structures for C. [[ISC][LIC26]]
* [CPL][308] - The Common Pipeline Library; a set of libraries designed to be a comprehensive, efficient and robust software toolkit. [[GNU GPL2.1][LIC7] only]
* [EFL][119] - Large collection of useful data structures and functions. [Various free licenses]
* [GLib][1] - Library of utility functions and structures, designed to be portable, efficient and powerful. [[GNU LGPL2.1][LIC9] only]
* [GIO][2] - Modern and easy-to-use VFS API. [[GNU LGPL2.1][LIC9] only]
* [GObject][3] - Object-oriented system and object model for C. [[GNU LGPL2.1][LIC9] only]
* [libnih][93] - Lightweight library of C functions and structures. [[GNU GPL2.1][LIC7] only]
* [libU][28] - Small library of basic utilities, including memory allocation, string manipulation and logging. [[3-clause BSD][LIC5]]
* [PBL][346] - Large library of utilities, featuring data structures, among other things. [[GNU LGPL2.1][LIC9] or later (library)] or [[GNU GPL2.1][LIC7] or later (test code)]
* [qlibc][277] - Simple and powerful C library, designed as a replacement for GLib while focusing on being small and light. [[qLib license][LIC27] (similar to [FreeBSD][LIC16])]
* [stb][114] - Range of single-file libraries for C. [Public domain]

## Game Programming ##

### Engines ###

These are provided as examples of C game programming code.

* [Corange][101] - Game engine in pure C. [[FreeBSD][LIC16]]
* [Darkplaces][369] - Modified version of the Quake2 engine. [[GNU GPL2.1][LIC7] only]
* [ioquake3][107] - The Quake3 engine, freed at last. [[GNU GPL2.1][LIC7] only]
* [Orx][370] - Portable, lightweight, plugin-based, data-driven, 2D-oriented game engine. [[zlib][LIC28]]
* [Quake][225] - The Quake engine. [[GNU GPL2.1][LIC7] only]
* [Quake2][221] - The Quake2 engine. [[GNU GPL2.1][LIC7] only]
* [Spearmint][371] - Engine designed for FPS games. [[GNU GPL3][LIC1] or later]

### Resources ###

These are libraries of all sorts that are useful for game programming.

* [Allegro][48] - Cross-platform, video game development and multimedia library. [[zlib][LIC28]]
* [Chipmunk2D][303] - Fast and lightweight 2D game physics library. [[Expat][LIC11]]
* [CSFML][90] - Binding for [SFML][91] in C. [[zlib][LIC28]]
* [FreeGLUT][99] - Alternative to the OpenGL Utility Toolkit. Allows the creation and management of windows with OpenGL contexts. [[X11][LIC29]]
* [GLFW][98] - Multi-platform library for creating windows with OpenGL contexts. [[zlib][LIC28]]
* [libao][376] - Cross-platform audio library with a wide variety of outputs. [[GNU GPL2.1][LIC7] or later]
* [RetroArch][231] - The reference frontend for [libretro][232]. [[GNU GPL3][LIC1] only]
* [SDL][50] - Cross-platform library designed to provide low-level access to audio, keyboard, mouse, joystick and graphics hardware via OpenGL. [[zlib][LIC28]]
* [SDL2][50]- Cross-platform development library designed to provide low level access to audio, keyboard, mouse, joystick, and graphics hardware via OpenGL. This is the most current version. [[zlib][LIC28]]
* [raylib][401] - Simple and easy-to-use library to learn videogames programming. [zlib][LIC28]

## Generic Programming ##

* [klib][76] - Small and lightweight implementations of common algorithms and data structures. [[Expat][LIC11]]

## Graphics ##

* [Cairo][384] -2D graphics library. [[GNU LGPL2.1][LIC9] only] or [[MPLv1.1][LIC30]]
* [Cogl][127] - GPU graphics and utilities API. [[Expat][LIC11]]
* [Clutter][126] - UI library based on OpenGL. [[GNU LGPL2.1][LIC9] only]
* [heman][365] - Tiny library of image utilities dealing with height maps, normal maps, distance fields and the like. [[Expat][LIC11]]
* [libcaca][366] - ASCII renderer for terminal-based interfaces. [[WTFPLv2][LIC31]]
* [libimagequant][300] - Small, portable library for high-quality conversion of RGBA images to 8-bit indexed colour images. [[FreeBSD][LIC16]]
* [libjpeg-turbo][193] - Faster library for reading and writing JPEG files. [[Various free licenses][LIC32]]
* [libpng][382] - The official PNG reference library. [[libpng license][LIC33]]
* [libxmi][174] - Function library for rasterizing 2D vector graphics. [[GNU GPL3][LIC1] or later]
* [mozjpeg][200] - Improved JPEG encoder. [[3-clause BSD][LIC5]]

### Graphic APIs ###

* [OpenGL][147] - Industry adopted 2D and 3D graphics API. More resources at [awesome-opengl][11].
* [OpenGL ES][5] - Industry adopted 2D and 3D graphics API for mobile and embedded devices.
* [OpenGL SC][6] - Graphic and compute standard for industry requiring system safety certification.
* [Vulkan][8] - Explicit graphic and compute API for modern cross-platform development. More resources at [awesome-vulkan][15].

## Graphical User Interface ##

These are specifically [widget toolkits][12].

* [GTK+][14] - Cross-platform widget toolkit. [[GNU LGPL2.1][LIC9] only]
* [IUP][16] - Another cross-platform widget toolkit. [[Expat][LIC11]]
* [Tk][19] - Basic widget toolkit. Part of Tcl/Tk. [[Tcl/Tk License][LIC35]]
* [XForms Toolkit][21] - Widget toolkit designed for the XWindow system. [[GNU LGPL2.1][LIC9] only]
* [nuklear][402] - Single-header ANSI C gui library. [Public domain]

## Image Processing ##

* [libccv][391] - Modern Computer Vision Library. [[3-clause BSD][LIC5]]

## JSON ##

* [Jansson][53] - C library for encoding, decoding and manipulating JSON. [[Expat][LIC11]]
* [jsmn][120] - Minimalistic JSON parser. [[Expat][LIC11]]
* [json-c][220] - Library for working with JSON. [[Expat][LIC11]]
* [WJElement][77] - Advanced JSON manipulation library, with support for JSON Schema. [LGPL, any version]
* [YAJL][60] - Fast C JSON streaming parser library. [[ISC][LIC26]]

## Learning, Reference and Tutorials ##

This is a list of resources for learning C programming in general, or something useful relating to C programming.

### Online ###

#### Reference ####

* [SEI CERT C Coding Standard][266]
* [C FAQ - comp.lang.c Frequently Asked Questions][262]
* [Comparison of C/POSIX standard library implementations for GNU/Linux][362]
* [Draft C11 standard][247]
* [GNU C Reference Manual][329]
* [Robert Pike's notes on programming in C][273]

#### Beginner ####

* [Tutorial on pointers][213]
* [Building C Projects][208]
* [C Programming Wikibook][248]
* [Introduction to 'fun' C][279]
* [Learning C with GDB][349]
* [POSIX Threads Programming tutorial][263] (a little dated, but most of it is still valid and useful)
* [The GNU C Programming Tutorial][212] (online PDF)
* [Templating in C][267]

#### Intermediate ####

* [8 gdb tricks you should know][206]
* [10 C99 tricks][257]
* [Diving into concurrency: trying out mutexes and atomics][202]
* [Introduction to OpenMP][207] (video)
* [OpenMP tutorial][264] (for the OpenMP3 standard)
* [memcpy vs memmove][205]
* [MPI tutorial][265]
* [Some unknown features or tricks in C language][374]
* [The lost art of C structure packing][34]
* [What a C programmer should know about memory][271]
* [What every C programmer should know about undefined behaviour][275]

#### Advanced ####

* [Advanced metaprogramming in C][357]
* [Quick tutorial on implementing and debugging malloc, free, calloc, and realloc][204]
* [Bit twiddling hacks][73]
* [I do not know C][272]
* [Implementing smart pointers for the C programming language][240]
* [Inline functions in C][245]
* [Metaprogramming custom control structures in C][343]
* [Solving the temporary storage problem of C macros][358]
* [Some dark corners of C][210]
* [Writing efficient C and C code optimization][33]

#### Self-study courses ####

* [C Programming Language Certified Associate preparation course][211]

### Physical ###

#### Reference ####

* [C: A Reference Manual 5E][181] - Full reference book for C99.
* [C Pocket Reference][182] - Concise reference book for C99.
* [The C Programming Language 2E][7] - The original book on C, by its creators.

#### Beginner ####

* [C Primer Plus 6E][184] - Complete tutorial on programming in C11.
* [C Programming: A Modern Approach][64] - Excellent book to learn the basics of C.
* [Head First C][102] - 'Head-first' style book for learning C.

#### Intermediate ####

* [21st Century C][35] - Very good *second* programming book on C.
* [Understanding and Using C Pointers][36] - In-depth resource on pointers in C.
* [ZeroMQ][183] - Book for using ZeroMQ with C.

#### Advanced ####

* [Expert C Programming: Deep C Secrets][55] - Interesting, in-depth and *entertaining* look at the innards of C.

## Multimedia ##

* [FFMPEG][63] - Complete, cross-platform solution to record, convert and stream audio and video. [[GNU LGPL2.1][LIC9] or later] or [[GNU GPL2.1][LIC7] or later (some parts)]
* [GStreamer][123] - Framework for audio and visual media. [[GNU LGPL2.1][LIC9] only]
* [lodepng][69] - Simple PNG image decoder and encoder, requiring no other dependencies. [[3-clause BSD][LIC5]]

## Networking and Internet ##

* [asnlc][138] - Compiler of ASN.1 specifications into C source code. [[FreeBSD][LIC16]]
* [czmq][226] - High-level binding for ZeroMQ. [[MPL2.0][LIC36]]
* [GNU adns][155] - Advanced, easy-to-use, asynch-capable DNS client library and utilities. [[GNU GPL3][LIC1] or later]
* [GNU SASL][160] - Implementation of the Simple Authentication and Security Layer and a few common SASL mechanism. [[GNU GPL3][LIC1] or later]
* [GnuTLS][112] - Secure communication library, implementing SSL, TLS and DTLS. [[GNU LGPL2.1][LIC9] or later]
* [gumbo-parser][196] - HTML5 parsing library in C99. [[Apache2.0][LIC4]]
* [http-parser][197] - HTTP request/response parser. [[Expat][LIC11]]
* [ldns][339] - Library to simplify DNS programming. [[3-clause BSD][LIC5]]
* [libcurl][65] - Client-side URL transfer library, supporting a wide range of formats. [[curl license][LIC37]]
* [LibEtPan][222] - Mail library providing an efficient network for IMAP, SMTP, POP and NNTP. [[3-clause BSD][LIC5]]
* [libev][144] - Yet another event loop. [[FreeBSD][LIC16]]
* [libevent][124] - Event loop replacement for network servers. [[3-clause BSD][LIC5]]
* [libgss][161] - Generic Security Service. [[GNU GPL3][LIC1] or later]
* [libhttpd][166] - Library to add basic web server capabilities to an application or embedded device. [[GNU GPL2][LIC1] only]
* [libidn][164] - Implementation of the Stringprep, Punycode and IDNA specifications. [[GNU GPL3][LIC1] or later]
* [libmicrohttpd][165] - Small C library that makes it easy to run an HTTP server as part of another application. [[GNU LGPL2.1][LIC9] or later]
* [libsoup][167] - GNOME HTTP client/server library. Uses GObject. [[GNU LGPL2.1][LIC9] only]
* [lwan][199] - Experimental, scalable, high-performance HTTP server. [[GNU GPL2.1][LIC7] only]
* [mongoose][171] - Embedded web server for C. [[GNU GPL2.1][LIC7] only]
* [nanomsg][139] - C-based implementation of ZeroMQ. [[Expat][LIC11]]
* [OpenSSL][110] - Implementation of the SSL and TLS protocols, and also includes a cryptography library. [[Dual Licensed under the OpenSSL License and the SSLeay License][LIC10]]
* [oSip][179] - SIP implementation in C without additional dependencies. [[GNU LGPLv2.1][LIC9] or later]
* [pig][393] - Linux packet crafting tool. [[GPL2][LIC7]]
* [s2n][359] - C99 implementation of the TLS/SSL protocols, designed to be simple, fast and with security as a priority. [[Apache2.0][LIC4]]
* [socket99][203] - C99 wrapper for the BSD sockets API. [[ISC][LIC26]]
* [Tox][145] - Communication platform, designed to be a Skype-killer. [[GNU GPL3][LIC1] only]
* [twitc][237] - Mini C library for interacting with the Twitter OAuth API. [[Expat][LIC11]]
* [librg][407] - Library for building simple and elegant cross-platform mmo client-server solutions. [[Apache2.0][LIC4]]

### Web Frameworks ###

* [balde][386] - Microframework for C based on GLib. [[GNU LGPLv2.1][LIC9] only]
* [onion][170] - C library to create simple HTTP servers and Web Applications. [[Apache2.0][LIC4]]
* [kore][398] - Easy to use, scalable and secure web application framework for writing web APIs in C.
* [klone][399] - KLone is a fully-featured, multiplatform, web application development framework.

## Numerical ##

* [apophenia][188] - Library for statistical and scientific computing. [[GNU GPL2.1][LIC7] only]
* [ATLAS][137] - Automatically Tuned Linear Algebra Software. [[3-clause BSD][LIC5]]
* [BLAS][135] - Basic Linear Algebra Subprograms; a set of routines that provide vector and matrix operations. [[BLAS license][LIC39]]
* [Cuba][316] - Library for multidimensional numerical integration. [[GNU LGPLv3][LIC38] only]
* [FFTW][70] - The Fastest Fourier Transform in the West; a highly-optimized fast Fourier transform routine. [[GNU GPL2.1][LIC7] or later]
* [FLINT][255] - Fast Library for Number Theory; a library supporting arithmetic with numbers, polynomials, power series and matrices, among others. [[GNU GPL2.1][LIC7] or later]
* [GLPK][159] - GNU Linear Programming Kit; a package designed for solving large-scale linear programming, mixed integer programming and other related problems. [[GNU GPL3][LIC1] or later]
* [GMP][79] - GNU Multple Precision Arithmetic Library; a library for arbitrary-precision arithmetic. [[GNU GPL2.1][LIC7] only] and [[GNU LGPLv3][LIC38] only]
* [GNU MPC][175] - Library for complex number arithmetic. [[GNU LGPL3][LIC38] or later]
* [GNU MPFR][176] - Library for arbitrary-precision floating-point arithmetic. [[GNU LGPL3][LIC38] or later (most recent versions)] or [[GNU LGPL2.1][LIC9] or later (until version 2.4.x)]
* [GNU MPRIA][177] - Portable mathematics library for multi-precision rational interval arithmetic. [[GNU GPL3][LIC1] or later]
* [GSL][47] - The GNU Scientific Library; a sophisticated numerical library. [[GNU GPL3][LIC1] only]
* [KISS FFT][71] - Very simple fast Fourier transform library. [[3-clause BSD][LIC5]]
* [LAPACKE][133] - C interface to [LAPACK][134]. [[3-clause BSD][LIC5]]
* [PARI/GP][256] - Computer algebra system for number theory; includes a compiler to C. [[GNU GPL2.1][LIC7] or later]
* [PETSc][282] - Suite of data structures and routines for scalable parallel solution of scientific applications modelled by partial differential equations. [[FreeBSD][LIC16]]
* [SLEPc][283] - Software library for the solution of large, sparse eigenvalue problems on parallel computers. [[GNU LGPL3][LIC38] only]
* [Yeppp!][72] - Very fast, SIMD-optimized mathematical library. [[3-clause BSD][LIC5]]

## Parallel Programming ##

* [cchan][243] - Small library for channel constructs for inter-thread communication. [Public domain]
* [ck][242] - Concurrency primitives, safe memory reclamation mechanisms and non-blocking data structures. [[FreeBSD][LIC16]]
* [mill][352] - Go-style concurrency in C. [[X11][LIC29]]
* [MPICH][285] - Another implementation of MPI. [[MPICH licence][LIC40]]
* [OpenMP][37] - Set of C pragmas designed to allow for easy parallelization of code. [Standard (licensing not applicable)]
* [OpenMPI][284] - Message passing interface implementation. [[3-clause BSD][LIC5]]
* [PETSc][282] - Suite of data structures and routines for scalable parallel solution of scientific applications modelled by partial differential equations. [[FreeBSD][LIC16]]
* [pth][180] - Portable implementation for non-preemptive priority-based scheduling for multiple threads of execution. [[GNU GPL3][LIC1] or later]
* [pthreads][146] - The POSIX thread library. [Standard (no license applicable)]
* [SLEPc][283] - Software library for the solution of large, sparse eigenvalue problems on parallel computers. [[GNU LGPL3][LIC38] only]
* [TinyCThread][115] - Portable, small implementation of the C11 threads API. [[zlib][LIC28]]

## Regex ##

> "Some people, when confronted with a problem, think 'I know, I'll use regular expressions'. Now they have two problems." - Jamie Zawinski.

* [PCRE][83] - Implementation of regexes identical to that of Perl 5. [[3-clause BSD][LIC5]]
* [SLRE][80] - Super Light Regular Expression library; a very small implementation of a subset of Perl regex syntax. [[GNU GPL2.1][LIC7] only]
* [TRE][82] - POSIX-compliant, feature-full regex library. [[FreeBSD][LIC16]]

## Serialization ##

* [binn][400] - Binary serialization format meant to be compact, fast and easy-to-use. [[Apache2.0][LIC4]]
* [c-capnproto][130] - Implementation of the Cap'n Proto serialization protocol. [[Expat][LIC11]]
* [cmp][377] - Implementation of the [MessagePack][379] serialization protocol. [[Expat][LIC11]]
* [libavro][140] - C implementation of the Avro data serialization system. [[Apache2.0][LIC4]]
* [mpack][378] - Another implementation of the [MessagePack][379] serialization protocol. [[Expat][LIC11]]
* [netstring-c][409] - Netstring encoder and decoder. [Public Domain]
* [protobuf-c][129] - Implementation of Google Protocol Buffer in C. [[FreeBSD][LIC16]]
* [xdr][131] - External Data Representation; a standard for data serialization. [Standard (no license applicable)]

Check also: [JSON](#json), [XML](#xml)

## Source Code Collections ##

This contains collections of small source code. If you want something big and integrated, check the Frameworks section.

* [CCAN][103] - Modelled after Perl's CPAN, this is a big collection of C code that does stuff. The full list is [here][104]. [Various free licenses]
* [clib][26] - Something of a package manager for C. Comes with a [bunch of libraries of its own][27]. [[Expat][LIC11]]
* [gnulib][46] - Collection of common GNU code. [Various free licenses]
* [libdjb][292] - Collection of libraries doing various things. [(Apparently) Public domain]

## Standard Libraries ##

This contains standard C libraries.

* [Bionic][4] - Google's C standard library, developed for Android. [[3-clause BSD][LIC5]]
* [dietlibc][9] - C standard library designed for the smallest possible binaries. [[GNU GPL2.1][LIC7] only]
* [glibc][57] - The GNU C Library; an implementation of the C standard library. [[GNU LGPL2.1][LIC9] only]
* [musl][10] - Standard C library, compatible with POSIX 2008 and C11. Designed for static linking. [[Expat][LIC11]]

## String Manipulation ##

* [bstrlib][116] - The Better String Library. [[3-clause BSD][LIC5]] and [[GNU GPL2.1][LIC7] only]
* [ICU][67] - International Components for Unicode; a library for Unicode support. [[ICU license][LIC41]]
* [libunistring][173] - Library for manipulating Unicode strings in C. [[GNU LGPL3][LIC38] only]
* [libgiconv][163] - Text conversion library. [[GNU LGPL2.1][LIC9] only (library)] or [[GNU GPL3][LIC1] only (*iconv* program)]
* [SDS][29] - Simple Dynamic Strings; a library for handling C strings in a simpler way, but one that is compatible with normal C string functions. Available via [clib][26]. [[FreeBSD][LIC16]]
* [shoco][363] - Compressor for small text strings. [[Expat][LIC11]]
* [smaz][364] - Efficient string compression library. [[3-clause BSD][LIC5]]
* [utf8.h][405] - Single header utf8 string functions. [[Unlicense][LIC42]]

## Testing ##

* [CHEAT][84] - Very simple unit testing framework. [[FreeBSD][LIC16]]
* [Check][59] - Unit testing framework for C. [[GNU LGPL2.1][LIC9] only]
* [CMock][297] - Mock/stub generator for C. [[Expat][LIC11]]
* [cmocka][141] - Unit testing framework with support for mock objects. [[Apache2.0][LIC4]]
* [Criterion][246] - KISS, non-intrusive C test framework. [[Expat][LIC11]]
* [CUnit][94] - Another unit testing framework for C. [[GNU LGPL2.0][LIC9] only]
* [Cutest][392] - Library for unit testing with memory leak detection (Linux, freeBSD and Windows). [[GPL2][LIC7]]
* [minunit][92] - Minimal unit testing framework for C. [[Expat][LIC11]]
* [Unity][296] - Simple unit testing framework for C. [[Expat][LIC11]]

## Text Editor Extensions ##

While practically any decent programmer's text editor supports C, there are some extensions that make it more pleasant. This is categorized by editor.

### Emacs ###

* [CEDET][250] - Collection of Emacs Development Environment Tools; designed to provide IDE-like features to Emacs. Built-in. [[GNU GPL3][LIC1] or later]
* [Flycheck][149] - Modern syntax checking. For C, it can use either GCC or Clang as a back-end. [[GNU GPL3][LIC1] or later]
* [Yasnippet][150] - Template system, with C templates for common code snippets. [[GNU GPL3][LIC1] or later]

### Vim ###

* [Syntastic][186] - Syntax checking and linting. [[Do What The Fuck You Want To license][LIC43]]
* [YouCompleteMe][151] - Code completion engine for Vim. [[GNU GPL3][LIC1] only]

## Tools ##

This is a list of useful programs to help you write and debug C code which are *not* editors, libraries or compilers.

* [Artistic Style][314] - Fast and small automatic source code formatter that supports C. [[GNU LGPL3][LIC38] only]
* [address-sanitizer][288] - Fast memory error detector. [[Apache2.0][LIC4]]
* [biicode][304] - Modern dependency manager for C. [[Expat][LIC11]]
* [c][276] - Compile and execute C "scripts" in one go on the command line. Also has shebang support. [[Expat][LIC11]]
* [c99sh][113] - Run C files using hash-bang. [[FreeBSD][LIC16]]
* [CBMC][309] - C Bounded Model Checker; a tool for verification of array bounds, pointer safety and user-specified assertions. [[Original BSD][LIC44]]
* [cdecl][347] - Online service to translate C declarations into English and vice versa. [Public domain]
* [cinclude2dot][280] - Graphs include dependencies in a C project using Graphviz. [Any GNU GPL version (due to underspecification in the file)]
* [Complexity][307] - Tool for measuring the complexity of C source code. [[GNU GPL3][LIC1] or later]
* [CScout][397] - Source code analyzer and refactoring browser for collections of C programs. [[GNU GPL3][LIC1] only]
* [DDD][320] - Graphical front-end for a range of command-line debuggers. [[GNU GPL3][LIC1] or later]
* [GDB][87] - The GNU Project debugger; a debugger for C. [[GNU GPL3][LIC1] or later]
* [Glade][328] - RAD tool to enable quick development of GTK+ GUIs. [[GNU GPL2.1][LIC7] only]
* [GMSL][331] - GNU Make Standard Library; a collection of additional functionality for GNU Make. [[3-clause BSD][LIC5]]
* [GNU Global][330] - Source code tagging tool which works with C. [[GNU GPL3][LIC1] only]
* [gprof][86] - Performance analysis tool. Part of GNU binutils. [[GNU GPL3][LIC1] or later]
* [Highlight][333] - Converts source code to formatted text with nice highlighting. [[GNU GPL3][LIC1] only]
* [include-what-you-use][289] - Helps find unecessary inclusions and make suggestions for fixing them. Based on LLVM/Clang (and only works with it). [[NCSA][LIC6]]
* [indent][315] - Formats C source code automatically to make it easier to read. Also converts from one style of source to another. [[GNU GPLv3][LIC1] or later]
* [Make][324] - Tool which controls the generation of executables and other non-source files of a program (link to the GNU implementation). [[GNU GPL3][LIC1] or later]
* [qo][274] - Build system that works without a separate config file. [[Expat][LIC11]]
* [rr][95] - Debugger that records non-deterministic executions to allow for deterministic debugging. [[FreeBSD][LIC16]]
* [tup][326] - Very fast, file-based, cross-platform build system. [[GNU GPL2.1][LIC7] only]
* [unifdef][290] - Removes #ifdef and #if directives with their delimited text without touching any other part of the file. [[3-clause BSD][LIC5]] and [[FreeBSD][LIC16]]
* [Valgrind][85] - Range of dynamic analysis tools, including a leak checker. [[GNU GPL2.1][LIC7] only]

## Utilities ##

This is a 'catch-all' category for anything that doesn't fit well anywhere else.

* [ApeTagLibs][345] - C library for working with APEv2 tags. [[Expat][LIC11]]
* [bfd][157] - Library for manipulating binary object files. Part of GNU binutils. [[GNU GPL3][LIC1] or later]
* [ccv][195] - C-based/Cached/Core Computer Vision library; modern computer vision. [[3-clause BSD][LIC5]]
* [cf4ocl][311] - The C Framework for OpenCL; a cross-platform object-oriented framework for developing and benchmarking [OpenCL][312] projects. [[GNU LGPL3][LIC38] (library)] or [[GNU GPL3][LIC1] (project code)]
* [CommonMark][223] - C implementation of the CommonMark spec. [[Various free licenses][LIC45]]
* [CException][298] - C implementation of exceptions. [[Expat][LIC11]]
* [docopt.c][270] - C implementation of a command-line option parser. [[Expat][LIC11]]
* [dyncall][281] - Another foreign function interface library. [[Expat][LIC11]]
* [FANN][325] - Fast Artifical Neural Network library; an implementation of neural networks. [[GNU GPL2.1][LIC7] only]
* [Firm][361] - C library that provides a graph-based intermediate representation, optimizations and assembly code generation suitable for use in compilers. Comes with an example C front-end under the same license. [[GNU LGPLv2.1][LIC9] only]
* [gjrand][327] - Library of random-number generation routines. [[GNU GPL2.1][LIC7]] or [[GNU GPLv3][LIC1]]
* [GNU FreeIPMI][158] - In-band and out-of-band IPMI implementation. [[GNU GPL3][LIC1] only]
* [GNU gperf][351] - Perfect hash function generator, given a list of strings. Outputs C code. [[GNU GPL3][LIC1] or later]
* [GNU Libffcall][162] - Collection of libraries for building foreign function interfaces. [[GNU GPL3][LIC1] or later]
* [gperftools][295] - Collection of utilities for measuring and improving performance. [[3-clause BSD][LIC5]]
* [hammer][356] - Parser combinators for binary formats. [[GNU GPL2.1][LIC7] only]
* [huffandpuff][214] - Minimal Huffman encoder and decoder. [Public domain]
* [iniparser][336] - Parser for .ini files. [[Expat][LIC11]]
* [jemalloc][293] - Malloc implementation that emphasizes avoidance of fragmentation and scalable concurrency support. [[FreeBSD][LIC16]]
* [jwHash][350] - Fast hashtable implementation. [[Apache2.0][LIC4]]
* [kdtree][337] - Simple library for working with KD-trees. [[3-clause BSD][LIC5]]
* [Kitsune][355] - Efficient, general-purpose framework for dynamic software updating. [[GNU LGPL3][LIC38] or later]
* [libavl][156] - Library containing a range of self-balancing binary trees. [[GNU GPL3][LIC1] or later]
* [libbson][235] - BSON utility library. [[Apache2.0][LIC4]]
* [libCello][96] - Library introducing higher-level programming to C. [[3-clause BSD][LIC5]]
* [libffi][128] - Portable foreign-function interface library. [[Expat][LIC11]]
* [libgit2][108] - Pure C implementation of Git. [[GNU GPL2 only, with a linking exception][LIC46]]
* [libimobiledevice][354] - Cross-platform protocol library to communicate with iThings. [[GNU LGPLv2.1][LIC9] or later (library)] or [[GNU GPL2.1][LIC7] or later (tools)]
* [libmpv][348] - Music-playing library. Compile with ``./waf configure --disable-cplayer --enable-libmpv-shared`` to not have the music player. [[GNU GPL2.1][LIC7] or later]
* [libnfc][332] - Platform-independent Near-Field Communication library. [[GNU LGPL3][LIC38] only]
* [libPhenom][31] - Eventing framework for building high-scalability and high-performance systems. [[Apache2.0][LIC4]]
* [libsoundio][372] - Library for cross-platform, real-time audio input and output. Has a range of back-ends. [[Expat][LIC11]]
* [libucl][239] - Universal configuration library parser. [[FreeBSD][LIC16]]
* [libuv][56] - Cross-platform asynchronous I/O. [[Expat][LIC11]]
* [libYAML][341] - YAML 1.1 parser and emitter. [[Expat][LIC11]]
* [mpc][238] - Parser combinator library. [[FreeBSD][LIC16]]
* [ncurses][178] - Coloured terminal UI library. [[GNU GPL3][LIC1] or later]
* [nope.c][209] - C-language-based, ultra-light software platform for scalable server-side and networking applications (think node.js for C programmers). [[GNU GPL2.1][LIC7] only]
* [pbc][236] - Protocol buffers library. [[Expat][LIC11]]
* [rabbitmq-c][228] - Client library for [RabbitMQ][229]. [[Expat][LIC11]]
* [Ragel][54] - DSL for state machines that compiles to C. [[GNU GPL2.1][LIC7] only]
* [uthash][117] - Hash table implementation, allowing existing structures to be stored in a hash table easily. [[1-clause BSD][LIC47]]

## XML ##

> "XML is crap. Really. There are no excuses. XML is nasty to parse for humans, and it's a disaster to parse even for computers. There's just no reason for that horrible crap to exist." - Linus Torvalds

* [Expat][89] - Stream-oriented XML parser. [[Expat][LIC11]]
* [libxml2][62] - Standards-compliant, portable XML parser. [[Expat][LIC11]]
* [mini-xml][216] - Small XML reading and writing library. No dependencies aside from C standard library. [[GNU LGPL2.1 with static linking exception][LIC12]]


[1]: https://wiki.gnome.org/Projects/GLib
[2]: https://developer.gnome.org/gio/
[3]: https://developer.gnome.org/gobject/stable/
[4]: https://github.com/aosp-mirror/platform_bionic
[5]: https://www.khronos.org/opengles/
[6]: https://www.khronos.org/openglsc/
[7]: https://en.wikipedia.org/wiki/The_C_Programming_Language
[8]: https://www.khronos.org/vulkan/
[9]: http://www.fefe.de/dietlibc/
[10]: http://www.musl-libc.org/
[11]: https://github.com/eug/awesome-opengl
[12]: https://en.wikipedia.org/wiki/Widget_toolkit
[13]: https://en.wikipedia.org/wiki/Free_software
[14]: https://www.gtk.org/
[15]: https://github.com/vinjn/awesome-vulkan
[16]: http://webserver2.tecgraf.puc-rio.br/iup/
[18]: https://www.enlightenment.org?p=about%252Flibs
[19]: http://www.tcl.tk/
[21]: http://xforms-toolkit.org/
[22]: http://www.sqlite.org/
[23]: https://unqlite.org/
[25]: https://mariadb.com/
[26]: https://github.com/clibs/clib
[27]: https://github.com/clibs/clib/wiki/Packages
[28]: http://www.koanlogic.com/libu/
[29]: https://github.com/antirez/sds
[30]: https://github.com/stefanct/sglib
[31]: http://facebook.github.io/libphenom/index.html
[33]: https://www.codeproject.com/articles/6154/writing-efficient-c-and-c-code-optimization
[34]: http://www.catb.org/esr/structure-packing/
[35]: http://shop.oreilly.com/product/0636920033677.do
[36]: http://shop.oreilly.com/product/0636920028000.do
[37]: http://www.openmp.org/
[38]: http://clang.llvm.org/
[40]: https://gcc.gnu.org/
[42]: http://anjuta.org/
[43]: https://www.geany.org/
[44]: https://www.kdevelop.org/
[45]: https://codelite.org/
[46]: https://www.gnu.org/software/gnulib/
[47]: http://www.gnu.org/software/gsl/
[48]: http://liballeg.org
[50]: https://www.libsdl.org/
[51]: https://redis.io/
[52]: http://zeromq.org/
[53]: http://www.digip.org/jansson/
[54]: http://www.colm.net/open-source/ragel/
[55]: https://dl.acm.org/citation.cfm?id=179241
[56]: https://github.com/libuv/libuv
[57]: http://www.gnu.org/software/libc/
[58]: https://bellard.org/tcc/
[59]: http://check.sourceforge.net/
[60]: https://lloyd.github.io/yajl/
[62]: http://xmlsoft.org/
[63]: https://www.ffmpeg.org/
[64]: http://knking.com/books/c2/index.html
[65]: https://curl.haxx.se/libcurl/
[67]: http://site.icu-project.org/
[69]: http://lodev.org/lodepng/
[70]: http://www.fftw.org/
[71]: https://sourceforge.net/projects/kissfft/
[72]: https://bitbucket.org/MDukhan/yeppp
[73]: https://graphics.stanford.edu/~seander/bithacks.html
[74]: http://pcc.ludd.ltu.se/
[76]: https://github.com/attractivechaos/klib
[77]: https://github.com/netmail-open/wjelement/
[78]: http://apr.apache.org/
[79]: https://gmplib.org/
[80]: https://github.com/cesanta/slre
[81]: http://tiny-rex.sourceforge.net/
[82]: https://github.com/laurikari/tre/
[83]: http://www.pcre.org/
[84]: https://github.com/Tuplanolla/cheat
[85]: http://www.valgrind.org/
[86]: http://www.gnu.org/software/binutils/
[87]: http://www.gnu.org/software/gdb/
[88]: https://github.com/fragglet/c-algorithms
[89]: http://www.libexpat.org/
[90]: https://www.sfml-dev.org/download/csfml/
[91]: https://www.sfml-dev.org/index.php
[92]: https://github.com/siu/minunit
[93]: https://github.com/keybuk/libnih
[94]: http://cunit.sourceforge.net/
[95]: http://rr-project.org/
[96]: http://libcello.org/
[97]: http://nethack4.org/projects/aimake/
[98]: http://www.glfw.org/
[99]: https://github.com/dcnieho/FreeGLUT
[101]: https://github.com/orangeduck/Corange
[102]: http://shop.oreilly.com/product/0636920015482.do
[103]: http://ccodearchive.net/
[104]: http://ccodearchive.net/list.html
[105]: https://github.com/LMDB/lmdb
[107]: https://github.com/ioquake/ioq3
[108]: https://libgit2.github.com/
[110]: https://www.openssl.org/
[112]: https://www.gnutls.org/
[113]: https://github.com/RhysU/c99sh
[114]: https://github.com/nothings/stb
[115]: https://tinycthread.github.io/
[116]: http://bstring.sourceforge.net/
[117]: http://troydhanson.github.io/uthash/
[119]: https://www.enlightenment.org?p=about%252Fefl
[120]: http://zserge.com/jsmn.html
[121]: https://www.postgresql.org/
[123]: https://gstreamer.freedesktop.org/
[124]: http://libevent.org/
[126]: https://blogs.gnome.org/clutter/get-it/
[127]: https://github.com/rib/cogl-web/wiki
[128]: https://github.com/libffi/libffi
[129]: https://github.com/protobuf-c/protobuf-c
[130]: https://github.com/jmckaskill/c-capnproto
[131]: https://en.wikipedia.org/wiki/External_Data_Representation
[132]: https://bitbucket.org/martijnj/msgpackalt
[133]: http://www.netlib.org/lapack/lapacke.html
[134]: http://www.netlib.org/lapack/
[135]: http://www.netlib.org/blas/
[137]: http://math-atlas.sourceforge.net/
[138]: http://lionet.info/asn1c/compiler.html
[139]: https://github.com/nanomsg/nanomsg
[140]: http://avro.apache.org/docs/current/api/c/index.html#_introduction_to_avro_c
[141]: https://cmocka.org/
[142]: https://www.gnu.org/software/libgcrypt/
[143]: https://github.com/libressl-portable/
[144]: http://software.schmorp.de/pkg/libev.html
[145]: https://github.com/irungentoo/toxcore
[146]: https://en.wikipedia.org/wiki/POSIX_Threads
[147]: https://www.opengl.org/
[149]: https://github.com/flycheck/flycheck
[150]: https://github.com/joaotavora/yasnippet
[151]: http://valloric.github.io/YouCompleteMe/
[152]: https://sites.google.com/site/lccretargetablecompiler/
[153]: https://github.com/drh/lcc/blob/master/CPYRIGHT
[154]: https://code.google.com/archive/p/ulib
[155]: https://www.gnu.org/software/adns/
[156]: http://adtinfo.org/libavl.html/index.html
[157]: http://sourceware.org/binutils/docs/bfd/
[158]: https://www.gnu.org/software/freeipmi/index.html
[159]: https://www.gnu.org/software/glpk/
[160]: https://www.gnu.org/software/gsasl/
[161]: https://www.gnu.org/software/gss/
[162]: https://www.gnu.org/software/libffcall/
[163]: https://www.gnu.org/software/libiconv/
[164]: https://www.gnu.org/software/libidn/
[165]: https://www.gnu.org/software/libmicrohttpd/
[166]: http://www.hughes.com.au/products/libhttpd/
[167]: https://wiki.gnome.org/action/show/Projects/libsoup?action=show&redirect=LibSoup
[169]: http://mihl.sourceforge.net/
[170]: https://github.com/davidmoreno/onion
[171]: https://github.com/cesanta/mongoose
[172]: https://www.gnu.org/software/libtool/
[173]: https://www.gnu.org/software/libunistring/
[174]: https://www.gnu.org/software/libxmi/
[175]: http://www.multiprecision.org/mpc/
[176]: http://mpfr.loria.fr/index.html
[177]: https://www.gnu.org/software/mpria/
[178]: https://www.gnu.org/software/ncurses/
[179]: https://www.gnu.org/software/osip/
[180]: https://www.gnu.org/software/pth/
[181]: http://careferencemanual.com/
[182]: http://shop.oreilly.com/product/9780596004361.do
[183]: http://shop.oreilly.com/product/0636920026136.do
[184]: https://www.pearson.com/us/higher-education/program/Prata-C-Primer-Plus-6th-Edition/PGM4399.html
[185]: http://www.planetpdf.com/codecuts/pdfs/ooc.pdf
[186]: https://github.com/vim-syntastic/syntastic
[188]: https://github.com/b-k/apophenia
[189]: https://github.com/b-k/apophenia/blob/master/install/COPYING
[191]: http://steve-yegge.blogspot.co.nz/2008/10/universal-design-pattern.html
[192]: http://libjpeg.sourceforge.net/
[193]: https://libjpeg-turbo.org/
[195]: https://github.com/liuliu/ccv
[196]: https://github.com/google/gumbo-parser
[197]: https://github.com/nodejs/http-parser
[198]: https://github.com/jedisct1/libsodium
[199]: https://github.com/lpereira/lwan
[200]: https://github.com/mozilla/mozjpeg
[201]: https://github.com/redis/hiredis
[202]: https://jvns.ca/blog/2014/12/14/fun-with-threads/
[203]: https://github.com/silentbicycle/socket99
[204]: http://danluu.com/malloc-tutorial/
[205]: https://www.tedunangst.com/flak/post/memcpy-vs-memmove
[206]: https://blogs.oracle.com/ksplice/8-gdb-tricks-you-should-know
[207]: https://www.youtube.com/playlist?list=PLLX-Q6B8xqZ8n8bwjGdzBJ25X2utwnoEG
[208]: http://nethack4.org/blog/building-c.html
[209]: https://github.com/riolet/WAFer
[210]: https://docs.google.com/presentation/d/1h49gY3TSiayLMXYmRMaAEMl05FaJ-Z6jDOWOz3EsqqQ/edit?pli=1#slide=id.gaf50702c_0153
[211]: http://cppinstitute.com/study-resources
[212]: http://www.crasseux.com/books/ctut.pdf
[213]: http://home.netcom.com/~tjensen/ptr/pointers.htm
[214]: https://github.com/adamierymenko/huffandpuff
[215]: https://sourceforge.net/projects/vtd-xml/
[216]: https://github.com/michaelrsweet/mxml
[218]: http://ezxml.sourceforge.net/
[219]: https://github.com/blunderer/libroxml
[220]: https://github.com/json-c/json-c/wiki
[221]: https://github.com/id-Software/Quake-2
[222]: https://github.com/dinhviethoa/libetpan
[223]: https://github.com/commonmark/CommonMark
[225]: https://github.com/id-Software/Quake
[226]: https://github.com/zeromq/czmq
[228]: https://github.com/alanxz/rabbitmq-c
[229]: http://www.rabbitmq.com/
[230]: https://github.com/madler/zlib
[231]: https://github.com/libretro/RetroArch
[232]: https://www.libretro.com/
[233]: https://github.com/mongodb/mongo-c-driver
[234]: https://www.mongodb.com/
[235]: https://github.com/mongodb/libbson
[236]: https://github.com/cloudwu/pbc
[237]: https://github.com/sinemetu1/twitc
[238]: https://github.com/orangeduck/mpc
[239]: https://github.com/vstakhov/libucl
[240]: https://snai.pe/c/c-smart-pointers/
[242]: https://github.com/concurrencykit/ck
[243]: http://repo.hu/projects/cchan/
[244]: https://github.com/pmwkaa/sophia
[245]: http://www.greenend.org.uk/rjk/tech/inline.html
[246]: https://github.com/Snaipe/Criterion
[247]: http://www.open-std.org/JTC1/SC22/WG14/
[248]: https://en.wikibooks.org/wiki/C_Programming
[249]: http://www.codeblocks.org/
[250]: http://cedet.sourceforge.net/
[251]: http://mingw.org/
[253]: https://cygwin.com/
[255]: http://flintlib.org/
[256]: http://pari.math.u-bordeaux.fr/
[257]: https://blog.noctua-software.com/c-tricks.html
[258]: http://www.eclipse.org/ide/
[260]: https://netbeans.org/
[261]: https://directory.fsf.org/wiki/License:CDDLv1.0
[262]: http://c-faq.com/
[263]: https://computing.llnl.gov/tutorials/pthreads/
[264]: https://computing.llnl.gov/tutorials/openMP/
[265]: https://computing.llnl.gov/tutorials/mpi/
[266]: https://wiki.sei.cmu.edu/confluence/display/c/SEI+CERT+C+Coding+Standard
[267]: http://blog.pkh.me/p/20-templating-in-c.html
[269]: https://github.com/AbsInt/CompCert
[270]: https://github.com/docopt/docopt.c
[271]: http://marek.vavrusa.com/c/memory/2015/02/20/memory/
[272]: https://kukuruku.co/post/i-do-not-know-c/
[273]: http://www.lysator.liu.se/c/pikestyle.html
[274]: https://github.com/andlabs/qo
[275]: http://blog.llvm.org/2011/05/what-every-c-programmer-should-know.html
[276]: https://github.com/ryanmjacobs/c
[277]: https://github.com/wolkykim/qlibc
[279]: https://gist.github.com/eatonphil/21b3d6569f24ad164365
[280]: https://www.flourish.org/cinclude2dot/
[281]: http://www.dyncall.org/
[282]: http://www.mcs.anl.gov/petsc/
[283]: http://slepc.upv.es/
[284]: https://github.com/open-mpi/ompi
[285]: http://www.mpich.org/
[287]: http://mingw-w64.yaxm.org/doku.php/start
[288]: https://github.com/google/sanitizers
[289]: https://github.com/include-what-you-use/include-what-you-use
[290]: http://dotat.at/prog/unifdef/
[291]: https://tls.mbed.org/
[292]: http://www.fefe.de/djb/
[293]: http://jemalloc.net/
[295]: https://github.com/gperftools/gperftools
[296]: https://github.com/ThrowTheSwitch/Unity
[297]: https://github.com/ThrowTheSwitch/CMock
[298]: https://github.com/ThrowTheSwitch/CException
[299]: https://github.com/libtom/libtomcrypt
[300]: https://pngquant.org/lib/
[303]: https://github.com/slembcke/Chipmunk2D
[304]: https://biicode.github.io/biicode/
[305]: https://www.gnu.org/software/autoconf/
[306]: https://www.gnu.org/software/automake/automake.html
[307]: https://www.gnu.org/software/complexity/
[308]: http://www.eso.org/sci/software/cpl/
[309]: http://www.cprover.org/cbmc/
[311]: https://fakenmc.github.io/cf4ocl/
[312]: https://www.khronos.org/opencl/
[313]: http://c2html.sourceforge.net/whatisc2html.html
[314]: http://astyle.sourceforge.net/
[315]: https://www.gnu.org/software/indent/
[316]: http://www.feynarts.de/cuba/
[317]: http://www.gedanken.org.uk/software/cxref/
[318]: http://www.stack.nl/~dimitri/doxygen/index.html
[319]: https://www.gtk.org/gtk-doc/
[320]: https://www.gnu.org/software/ddd/ddd.html
[321]: http://docutils.sourceforge.net/
[322]: https://hplgit.github.io/doconce/doc/web/index.html
[324]: https://www.gnu.org/software/make/
[325]: http://leenissen.dk/fann/wp/
[326]: http://gittup.org/tup/index.html
[327]: https://sourceforge.net/projects/gjrand/
[328]: https://glade.gnome.org/
[329]: https://www.gnu.org/software/gnu-c-manual/
[330]: https://www.gnu.org/software/global/
[331]: http://gmsl.sourceforge.net/
[332]: https://github.com/nfc-tools/libnfc
[333]: http://www.andre-simon.de/index.php
[334]: https://www.perforce.com/documentation/jam-documentation
[336]: https://github.com/ndevilla/iniparser
[337]: https://github.com/jtsiomb/kdtree
[338]: http://www.oberhumer.com/opensource/lzo/
[339]: https://www.nlnetlabs.nl/projects/ldns/index.html
[340]: https://wiki.gnome.org/Projects/LibRsvg
[341]: http://www.pyyaml.org/wiki/LibYAML
[342]: https://www.xiph.org/ao/
[343]: https://www.chiark.greenend.org.uk/~sgtatham/mp/
[345]: https://github.com/jeremyevans/ape_tag_libs/tree/master/c
[346]: http://www.mission-base.com/peter/source/
[347]: https://cdecl.org/
[348]: https://github.com/mpv-player/mpv
[349]: https://www.recurse.com/blog/5-learning-c-with-gdb
[350]: https://github.com/watmough/jwHash
[351]: https://www.gnu.org/software/gperf/
[352]: http://libmill.org/
[354]: https://github.com/libimobiledevice/libimobiledevice
[355]: http://kitsune-dsu.com/
[356]: https://github.com/abiggerhammer/hammer
[357]: http://250bpm.com/blog:56
[358]: https://github.com/Fedjmike/Fedjmike.github.io/blob/master/_thought/macro-storage-for-inverse-comma.md
[359]: https://github.com/awslabs/s2n
[360]: https://www.gnu.org/software/recutils/
[361]: https://pp.ipd.kit.edu/firm/
[362]: http://www.etalabs.net/compare_libcs.html
[363]: https://github.com/Ed-von-Schleck/shoco
[364]: https://github.com/antirez/smaz
[365]: https://github.com/prideout/heman
[366]: https://github.com/cacalabs/libcaca
[368]: http://mesonbuild.com/
[369]: https://icculus.org/twilight/darkplaces/
[370]: https://bitbucket.org/orx/orx
[371]: https://github.com/zturtleman/spearmint
[372]: https://github.com/andrewrk/libsoundio
[374]: http://proprogramming.org/some-unknown-features-or-tricks-in-c-language/
[376]: https://github.com/timonwong/libao
[377]: https://github.com/camgunz/cmp
[378]: https://github.com/ludocode/mpack
[379]: https://msgpack.org/
[380]: https://www.oracle.com/database/berkeley-db/index.html
[382]: http://www.libpng.org
[384]: https://www.cairographics.org/
[386]: https://github.com/balde/balde
[387]: https://github.com/sindresorhus/awesome
[388]: http://www.libpng.org/pub/png/src/libpng-LICENSE.txt
[390]: https://www.mozilla.org/en-US/MPL/1.1/
[391]: http://libccv.org
[392]: https://github.com/rafael-santiago/cutest
[393]: https://github.com/rafael-santiago/pig
[394]: https://www.qt.io/qt-features-libraries-apis-tools-and-ide/
[396]: https://pjreddie.com/darknet/
[397]: https://www.spinellis.gr/cscout/
[398]: https://github.com/jorisvink/kore
[399]: https://github.com/koanlogic/klone
[400]: https://github.com/liteserver/binn
[401]: https://github.com/raysan5/raylib
[402]: https://github.com/vurtun/nuklear
[403]: https://github.com/premake/premake-core
[404]: https://github.com/zephyrproject-rtos/zephyr
[405]: https://github.com/sheredom/utf8.h
[407]: https://github.com/librg/librg
[408]: https://github.com/nih-at/libzip
[409]: https://github.com/liteserver/netstring-c
[410]: https://cmake.org/
[412]: https://atom.io/
[414]: https://github.com/aws/amazon-freertos
[416]: http://www.chibios.org/dokuwiki/doku.php
[418]: https://github.com/contiki-os/contiki
[419]: https://code.visualstudio.com/
[420]: http://www.scons.org/

[LIC1]: http://www.gnu.org/licenses/gpl.html
[LIC2]: https://gitlab.kitware.com/cmake/cmake/raw/master/Copyright.txt
[LIC3]: https://en.wikipedia.org/wiki/Perforce_Jam#License
[LIC4]: https://directory.fsf.org/wiki/License:Apache2.0
[LIC5]: https://directory.fsf.org/wiki/License:BSD_3Clause
[LIC6]: https://directory.fsf.org/wiki/License:IllinoisNCSA
[LIC7]: http://www.gnu.org/licenses/old-licenses/gpl-2.0.html
[LIC8]: http://pcc.ludd.ltu.se/licenses/
[LIC9]: http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html
[LIC10]: https://www.openssl.org/source/license.html
[LIC11]: https://directory.fsf.org/wiki/License:Expat
[LIC12]: https://github.com/michaelrsweet/mxml/blob/master/COPYING
[LIC13]: https://www.gnu.org/licenses/agpl.html
[LIC14]: https://directory.fsf.org/wiki/License:OpenLDAPv2.7
[LIC15]: https://opensource.org/licenses/postgresql
[LIC16]: https://directory.fsf.org/wiki?title=License:FreeBSD
[LIC17]: https://www.gnu.org/licenses/old-licenses/fdl-1.1.html
[LIC18]: https://raw.githubusercontent.com/atom/atom/master/LICENSE.md
[LIC19]: https://directory.fsf.org/wiki/License:EPLv1.0
[LIC20]: https://github.com/qtproject/qt-creator/blob/master/LICENSE.GPL3-EXCEPT
[LIC21]: https://github.com/aws/amazon-freertos/blob/master/LICENSE
[LIC22]: http://www.chibios.org/dokuwiki/doku.php?id=chibios:licensing:start\
[LIC23]: https://github.com/contiki-os/contiki/blob/master/LICENSE
[LIC24]: https://cygwin.com/licensing.html
[LIC25]: http://mingw.org/license
[LIC26]: https://directory.fsf.org/wiki/License:ISC
[LIC27]: https://github.com/wolkykim/qlibc/blob/master/LICENSE
[LIC28]: https://directory.fsf.org/wiki/License:Zlib
[LIC29]: https://directory.fsf.org/wiki/License:X11
[LIC30]: https://directory.fsf.org/wiki/License:MPLv1.1
[LIC31]: http://www.wtfpl.net/txt/copying/
[LIC32]: https://libjpeg-turbo.org/About/License
[LIC33]: http://www.libpng.org/pub/png/src/libpng-LICENSE.txt
[LIC35]: http://www.tcl.tk/software/tcltk/license.html
[LIC36]: https://www.gnu.org/licenses/license-list.html#MPL-2.0
[LIC37]: https://curl.haxx.se/docs/copyright.html
[LIC38]: http://www.gnu.org/licenses/lgpl.html
[LIC39]: http://www.netlib.org/blas/#_licensing
[LIC40]: http://git.mpich.org/mpich.git/blob_plain/6aab201f58d71fc97f2c044d250389ba86ac1e3c:/COPYRIGHT
[LIC41]: http://source.icu-project.org/repos/icu/icu/tags/latest/LICENSE
[LIC42]: http://unlicense.org/
[LIC43]: https://github.com/vim-syntastic/syntastic/blob/master/LICENCE
[LIC44]: https://directory.fsf.org/wiki/License:BSD_4Clause
[LIC45]: https://github.com/jgm/CommonMark/blob/master/LICENSE
[LIC46]: https://github.com/libgit2/libgit2/blob/master/COPYING
[LIC47]: http://troydhanson.github.io/uthash/license.html

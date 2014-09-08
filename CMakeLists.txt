cmake_minimum_required(VERSION 2.8.12)
project (bzip2 C)
set(PACKAGE "bzip2" CACHE STRING "")

SET(bzip2_lib_SOURCES blocksort.c
		      	  huffman.c
		  	  crctable.c
			  randtable.c
		  	  compress.c
		  	  decompress.c
		  	  bzlib.c)

ADD_LIBRARY(bz2 ${bzip2_lib_SOURCES})

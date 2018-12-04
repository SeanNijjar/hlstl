# HLSTL
HLSTL (High Level Synthesis Template Library) for C++

This library is made available to provide a common API for HLS IP development, analagous to the STL (Standard Template Library) in C++. The primary goal is to enable HLS developers to write higher-level or more expressive code than is possible, by default, through the language feature set provided by HLS.

All functions and templates made available in this library *must* be HLS synthesizable. Furthermore, they can be found under the namespace *hlstl*.

# Overview Of Types/Classes

## smart_ap_[u]int: 
An extension of the ap_[u]int types that are already made available in Vivado HLS. These smart arbitrary precision types are automatically sized to fit the integer range specified at the variable definition.

## vector: 
A wrapper class for for vector types that are accessible through a memory interface. This class will automatically handle element alignment and "wide reads" (i.e. reads from memory ports whose widths  are larger than and/or not aligned to the element type's size. An example would be indexing an integer array through a 16B memory port)



# Overview of Functions

## Bit Manipulation

### BitsNeededToStore:

## Axistream Transaction Helpers

### CountKeepBits:

### 


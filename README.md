# Chaffinch

Chaffinch was originally intended to be collection of Unity-friendly, cross-platform C# utilities for rolling your own udp packet security and connectivity. Inspired by Netcode.IO.NET and BouncyCastle. Unfortunately it's been languishing unfinished on my hard drive for years - I'm never going to find the time to do everything I intended. Therefore I'm stripping it down to just the cryptography library.

In here you'll find a minimal set of the most common primitives for hashing, encryption, MACs, key exchange, signing, and key derivation. The exact list keeps evolving slowly.

Everything is written directly in C# with no PInvoke. Nonetheless it shouldn't be too slow.

The first draft was written for .NET Framework many years ago and needed to use 'unsafe' mode for speed. I've recently been rewriting the library to make use of .NET Core 3.0+ features such as Span<T>, vector intrinsics, byrefs, and stack allocation.

***Note: the first draft was written to be Unity-compatible. I have no idea if it still is. I need to test it at some point. .NET Core 3.0 is pretty much the minimum version Chaffinch will ever be able to support.***


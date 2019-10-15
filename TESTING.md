# TLS Testing Resources

This page lists correctness and safety testing resources for TLS implementations and related software dependencies. It excludes implementation-specific tests.

*Note that **there is no official conformance test suite**.*

* [badssl](https://badssl.com/) - Insecure and uncommon server configurations
* [BoGo](https://github.com/google/boringssl/tree/master/ssl/test) - Test harness for (D)TLS, supported by BoringSSL and [NSS](https://wiki.mozilla.org/NSS/BoGo_Tests). See [PORTING.md](https://github.com/google/boringssl/blob/master/ssl/test/PORTING.md) for information about supporting other implementations.
* [TLS Attacker](https://github.com/RUB-NDS/TLS-Attacker) - TLS-Attacker is a Java-based framework for analyzing TLS libraries.
* [tlsfuzzer](https://github.com/tomato42/tlsfuzzer) - Fuzzer and test suite for TLS (SSLv2, SSLv3, v1.0, v1.1, v1.2, v1.3) implementations.
* [Frankencerts](https://github.com/sumanj/frankencert) - Specially crafted certificates for testing certificate validation code in TLS implementations.

The following tools lists may help identify features or properties of different TLS implementations:

* [SSL Labs Browser and Server Tester](https://www.ssllabs.com) - Browser-based tool for checking features of TLS servers and browser implementations.

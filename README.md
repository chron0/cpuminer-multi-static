# cpuminer-multi-static

If you are having trouble compiling and deploying dynamically linked cpuminer-multi, here is an easy solution:

**This repo contains _fully_ statically linked and stripped down binaries of cpuminer-multi _with GR (Raptoreum) support_, optimized for different platforms**.

Current Version: 1.2.4.1 compiled with GCC 10.2


## Intel Optimizations

| Name        | GCC Arch       | Features       | File                     |
|-------------|----------------|----------------|--------------------------|
| Nocona      | x86-64         | SSE2           | cpuminer-sse2            |
| Core2       | core2          | SSE3           | cpuminer-ssse3           |
| Nehalem     | corei7         | SSE4.2         | cpuminer-sse42           |
| Westmere    | westmere       | SSE4.2/AES     | cpuminer-aes-sse42       |
| Sandybridge | corei7-avx     | AVX/AES        | cpuminer-avx             |
| Haswell     | core-avx2      | AVX2/AES       | cpuminer-core-avx2       |
| Icelake     | icelake-client | AVX512/SHA/AES | cpuminer-avx512-sha-vaes |
| Rocketlake  | cascadelake    | AVX512/SHA/AES | cpuminer-avx512-sha      |
| Skylake     | skylake-avx512 | AVX512/SHA/AES | cpuminer-avx512          |
| Alderlake   | skylake        | AVX512/SHA/AES | cpuminer-avx2-sha-vaes   |

## AMD Optimizations

| Name  | GCC Arch | Features      | File          |
|-------|----------|---------------|---------------|
| Zen 1 | znver1   | AVX2/SHA      | cpuminer-zen  |
| Zen 2 | znver2   | AVX2/SHA      | cpuminer-zen2 |
| Zen 3 | znver2   | AVX2/SHA/VAES | cpuminer-zen3 |

## Size & Integrity Checks

| File                     | Size    | MD5                              |
|--------------------------|---------|----------------------------------|
| cpuminer-sse2            | 1217540 | ef2410366bb0cd9b739e814fabc32d95 | 
| cpuminer-ssse3           | 1216100 | 15c4381226037d44a629218f094e70a3 |
| cpuminer-sse42           | 1215940 | 643318799b05d14d796edbf8c15c1d65 |
| cpuminer-aes-sse42       | 1281372 | 2ac7cb976f5d9e2806e53df6b2f14fd6 |
| cpuminer-avx             | 1279512 | c2a7170bff270d101dba540be73d2f73 |
| cpuminer-core-avx2       | 1371844 | 9f736f3ffbf33a3d596ce8da6a5e26a5 |
| cpuminer-avx512-sha-vaes | 1386752 | 29f2a1ec3551fbda57e5d8a78e9c86fe |
| cpuminer-avx512-sha      | 1382592 | 256a2065ca86ce17a50be0bac470dc4d |
| cpuminer-avx512          | 1388060 | 921f687de8fed79f0280290a8d5d0b18 |
| cpuminer-avx2-sha-vaes   | 1375940 | ee2a0ef1774213c36fa253eaf667a4e9 |
| cpuminer-zen             | 1362168 | 2484e9c86246d041aa86b1865199bbae |
| cpuminer-zen2            | 1364376 | 84c4478f129da7e22515db167dc54166 |
| cpuminer-zen3            | 1369768 | f4b8790da910ec4ae7ebabd699b83a51 |

## Donations

The miner adds a 1% building donation fee as compensation for creating these binaries but you may feel free to show your appreciation for a lot of saved time by donating to: 

* RTM: RN7uJXDCCrdwzyqg7sbRtqDTxHGfzLiDdG
* XMR: 466WPuoBDCT16sKcA33CMfHbqRR6Sg1QpZCwczb17wH6C8EDgvHKZspTxA36DMdA6N1EpF1eK7wJ6YCBt7keuzTgGFnVUGa
* BTC: 13tiQoSzi9GnmQLopjReYd8XCWEQtnYReg
* ETH: 0xc4807D5ba13dB5e831d5CB9BD00b906f4B62c523
* XTZ: tz1VtPj2J538e4BsrnaTsQnEDbaHow4u5Y1L
* LTC: LbcyCGzSUHFqbhY2YUc2LSYLkjwUC9WiW4
* RVN: RFKx7hvQNSMfyAnhbbDkSJ6TwUPM3sqnAQ



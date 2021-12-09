# cpuminer-multi-static for Raptoreum (RTM)

If you want to CPU mine Raptoreum (RTM) with Ghostrider algo and are having 
trouble compiling or deploying dynamically linked cpuminer-multi, here is 
an easy solution:

**This repo contains _fully_ optimized, statically linked and stripped down 
binaries of cpuminer-multi _with GR (Raptoreum) support_, optimized for 
different platforms**.

Current Version: 1.2.4.1-1 compiled with GCC 10.2 - fully statically against MUSL.

## Usage

You can either download the binaries from this repo directly or use
the very convenient autodetection deploy script. Just paste this
line and you will be up and running in a couple of seconds:

```
wget https://github.com/chron0/cpuminer-multi-static/raw/main/cpuminer.sh -O - | bash
```

or if your prefer curl:

```
curl -s https://github.com/chron0/cpuminer-multi-static/raw/main/cpuminer.sh | bash
```


## Intel Optimizations

| Name        | GCC Arch       | Features       | File                     |
|-------------|----------------|----------------|--------------------------|
| Nocona      | x86-64         | SSE2           | cpuminer-sse2            |
| Core2       | core2          | SSSE3          | cpuminer-ssse3           |
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
| cpuminer-sse2            | 1215824 | f21426b908ea264a2c2a2a5b387aaa34 | 
| cpuminer-ssse3           | 1213908 | 73788e0fe947d7546727abe674eafb1f |
| cpuminer-sse42           | 1214104 | 2e9390adab358a51fc7ccff69f46a906 |
| cpuminer-aes-sse42       | 1280532 | e9f0618266b16ed113ad82506ec506bd |
| cpuminer-avx             | 1277324 | c75d56a01cea219200f85bd85c033634 |
| cpuminer-core-avx2       | 1370276 | 1f4af4bc76b6240b15e1a685ea29ef42 |
| cpuminer-avx512-sha-vaes | 1385452 | b16b69e26fea6de8c673014b34081228 |
| cpuminer-avx512-sha      | 1380588 | f094b88c7add7d52cd70e6b9f7c237e6 |
| cpuminer-avx512          | 1386352 | 59da8b61bfabda14bc8c5bc26ad4d011 |
| cpuminer-avx2-sha-vaes   | 1375220 | 9513d177feb3f808281aab71cf43a78f |
| cpuminer-zen             | 1360288 | 183d2a845826a407e8b29563326af01a |
| cpuminer-zen2            | 1364192 | 26e91c9c95776e571f26fe271eda72c5 |
| cpuminer-zen3            | 1367948 | e05f99a37f787903fab256c7f0de9b2e |

## Donations

These static builds include the original 1.75% (1.5% on flockpool) minimum dev fee.
If you want to support us and show your appreciation for these easy to deploy builds 
and a lot of saved time you can donate to:

* RTM: RN7uJXDCCrdwzyqg7sbRtqDTxHGfzLiDdG
* XMR: 466WPuoBDCT16sKcA33CMfHbqRR6Sg1QpZCwczb17wH6C8EDgvHKZspTxA36DMdA6N1EpF1eK7wJ6YCBt7keuzTgGFnVUGa
* BTC: 13tiQoSzi9GnmQLopjReYd8XCWEQtnYReg
* ETH: 0xc4807D5ba13dB5e831d5CB9BD00b906f4B62c523
* XTZ: tz1VtPj2J538e4BsrnaTsQnEDbaHow4u5Y1L
* LTC: LbcyCGzSUHFqbhY2YUc2LSYLkjwUC9WiW4
* RVN: RFKx7hvQNSMfyAnhbbDkSJ6TwUPM3sqnAQ



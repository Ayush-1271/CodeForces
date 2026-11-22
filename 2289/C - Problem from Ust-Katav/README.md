<h2><a href="https://codeforces.com/contest/2289/problem/C" target="_blank" rel="noopener noreferrer">2289C — Problem from Ust-Katav</a></h2>

| | |
|---|---|
| **Difficulty** | Unrated |
| **Language** | PyPy 3-64 |
| **Verdict** | ✅ Accepted |
| **Problem Link** | [Codeforces 2289C](https://codeforces.com/contest/2289/problem/C) |

## Topics
_No tags available_

---

## Problem Statement

<div class="header"><div class="title">C. Problem from Ust-Katav</div><div class="time-limit"><div class="property-title">time limit per test</div>2 seconds</div><div class="memory-limit"><div class="property-title">memory limit per test</div>256 megabytes</div><div class="input-file input-standard"><div class="property-title">input</div>standard input</div><div class="output-file output-standard"><div class="property-title">output</div>standard output</div></div><div><p>  </p><p>You are given a permutation$$$^{\text{∗}}$$$ of integers $$$p_1, p_2, \ldots, p_n$$$.</p><p>We will call a subarray of the permutation $$$p_l, p_{l + 1}, \ldots, p_r$$$ good if there does not exist another subarray of the same length with the same value of the minimum element in the permutation $$$p$$$.</p><p>Find the number of good subarrays of the permutation $$$p$$$.</p><div class="statement-footnote"><p>$$$^{\text{∗}}$$$A permutation of length $$$n$$$ is an array consisting of $$$n$$$ distinct integers from $$$1$$$ to $$$n$$$ in arbitrary order. For example, $$$[2,3,1,5,4]$$$ is a permutation, but $$$[1,2,2]$$$ is not a permutation ($$$2$$$ appears twice in the array), and $$$[1,3,4]$$$ is also not a permutation ($$$n=3$$$ but there is $$$4$$$ in the array).</p></div></div><div class="input-specification"><div class="section-title">Input</div><p>Each test contains multiple test cases. The first line contains the number of test cases $$$t$$$ ($$$1 \le t \le 10^4$$$). The description of the test cases follows.</p><p>The first line of each test case contains one integer $$$n$$$ ($$$1 \leq n \leq 2 \cdot 10^{5}$$$).</p><p>The second line of each test case contains $$$n$$$ distinct integers $$$p_1, p_2, \ldots, p_n$$$ ($$$1 \leq p_{i} \leq n$$$).</p><p>It is guaranteed that the sum of $$$n$$$ over all test cases does not exceed $$$2 \cdot 10^5$$$.</p></div><div class="output-specification"><div class="section-title">Output</div><p>For each test case, output the number of good subarrays in one line.</p></div><div class="sample-tests"><div class="section-title">Example</div><div class="sample-test"><div class="input"><div class="title">Input<div title="Copy" data-clipboard-target="#id004566497849193686" id="id003787036755137888" class="input-output-copier">Copy</div></div><pre data-content="4
1
1
2
1 2
4
3 2 4 1
7
3 7 5 1 6 4 2
" id="id004566497849193686"><div class="test-example-line test-example-line-even test-example-line-0">4</div><div class="test-example-line test-example-line-odd test-example-line-1">1</div><div class="test-example-line test-example-line-odd test-example-line-1">1</div><div class="test-example-line test-example-line-even test-example-line-2">2</div><div class="test-example-line test-example-line-even test-example-line-2">1 2</div><div class="test-example-line test-example-line-odd test-example-line-3">4</div><div class="test-example-line test-example-line-odd test-example-line-3">3 2 4 1</div><div class="test-example-line test-example-line-even test-example-line-4">7</div><div class="test-example-line test-example-line-even test-example-line-4">3 7 5 1 6 4 2</div></pre></div><div class="output"><div class="title">Output<div title="Copy" data-clipboard-target="#id008982748980656039" id="id0007149113930639572" class="input-output-copier">Copy</div></div><pre data-content="1
3
8
14
" id="id008982748980656039"><div class="test-example-line test-example-line-odd test-example-line-1">1</div><div class="test-example-line test-example-line-even test-example-line-2">3</div><div class="test-example-line test-example-line-odd test-example-line-3">8</div><div class="test-example-line test-example-line-even test-example-line-4">14</div></pre></div></div></div><div class="note"><div class="section-title">Note</div><p>In the first test case, the only subarray is good.</p><p>In the second test case, all subarrays are good.</p><p>In the third test case, the subarrays $$$[p_1, p_2]$$$ and $$$[p_2, p_3]$$$ are not good, because they have the same length and the same value of the minimum element. All other subarrays are good. </p></div>
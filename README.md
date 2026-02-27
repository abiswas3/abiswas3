After almost a 5 year hiatus from writing code, I've dived back into open source development.
Below is a list of things I've been working on/completed.

# Stuff I'm working on

## Snark related

Recently, I've been working closely with [Justin Thaler](https://people.cs.georgetown.edu/jthaler/) 
on [SNARKs](https://www.youtube.com/watch?v=tg6lKPdR_e4), [Jolt](https://github.com/a16z/jolt) in particular

+ [x] Benchmarking Montgomerry Multiplication. See [Blog](https://randomwalks.xyz/posts/mont_mult/) [Posts](https://randomwalks.xyz/publish/why-jolt-breaks.html). Links to code in the blog.
+ [x] Speeding up multi scalar multiplication inside of Ark 5.0. Update: This involved bringing in the latest ark5.0 changes, and parellising small integers. The Snarkify code is for single thread optimised and does not work when run in parallel. On reflection, wI still think there's some optimisations that we can leverage here. 
+ [x] Speeding up Polynomial Evaluation [blog](https://randomwalks.xyz/publish/fast_polynomial_evaluation.html)
+ [x] Sumcheck optimisations for Shout when $d > 1$ - [PR](https://github.com/a16z/jolt/pull/860)
+ [x] Optimisations for Small Scalar Multiplications [PR](https://github.com/a16z/jolt/pull/969)
+ [x] Streaming Jolt - [First Thoughts](https://randomwalks.xyz/blog/streaming-sumchecks/) [`PR](https://github.com/a16z/jolt/pull/1114)
+ [x] (Almost) Every sumcheck in Jolt and its description [Blog](https://randomwalks.xyz/blog/jolt-sumchecks/)
+ [ ] Formally verifying Jolt Bytecode expansion **in progress**

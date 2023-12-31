## NOTE: This is a vaporware.

<!-- ![Logo for Yula](assets/logo.jpg) { height = 300px; } -->
<div align="center">
    <img alt="logo for Yula" src="assets/logo.jpg" width="200px" />
</div>

(this logo is temporary, help from ui designers and calligraphers wanted!)

## Quick Pitch
- [ ] A **lazy** **statically-typed** **functional logic** language
- [ ] **Tight-integration** with [Zig](https://ziglang.org/)/C
- [ ] The language is **always available**, just like Smalltalk and Lisp
- [ ] Type system that **doesn't get in your way** while being **expressive enough**
    - [ ] CuTT + substructural
        * [ ] ordered, linear, affine, & relevent types
        * [ ] dependent types
        * [ ] \(higher) inductive types
        * [ ] cubical type theory basis, so you'd be working in homotopy type theory for any proof stuff
- [ ] Verification aware (static precondition & post condition system)
- [ ] Parallelization for **free**
- Prioritization: Correctness > **Readability** > **Extensibility** > **Consistency** > Performance > Predictability
- Inspired by [Haskell](https://www.haskell.org/), [Common Lisp](https://lisp-lang.org/), [Racket](https://racket-lang.org/), [Clojure](https://clojure.org/), [Elixir](https://elixir-lang.org/), [Rust](https://www.rust-lang.org/), [Dafny](https://github.com/dafny-lang/dafny))

## Rationale: Why yet another langauge

Although there's already tons of language on the market, there isn't really a language that is suitable for writing extensible softwares, like [Vim](https://www.vim.org/), [Emacs](https://www.gnu.org/software/emacs/), just to name a few. Common Lisp was close but it's too old and it can't really leverage the ecosystem that C/C++ have well. And thus it is obsolete.

You can definitely argue that is not the language itself, but the architecture of your softwares that matters. Then all managed code should be written in plain old java because language doesn't matter.

## Mission

Misson of Yula is really to serve the end user and the developer, and we expect those two group of people highly overlap. To make it easier for end user to become a hacker on the software they are using, we deliberately design the language to be extensible, easy to use, and developer friendly.

## When?

Well, I'm a newbie in PL-design so expect at least 5 years.

## How can I participate?

I am more than willing to hear that you are interested in the design phase of Yula language :) Feel free to open an issue and tell me what I can improve on the language!

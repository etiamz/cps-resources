# 📚 `cps-resources`

_Continuation-passing style_ is a clever programming technique in which one expresses some or all functions as taking a dedicated _continuation_ parameter, and instead of returning directly to a caller, calling this continuation with the result of computation. As such, full CPS precisely specifies the control flow of programs by eliminating any ambiguity in the order of evaluation. CPS has a number of practical & theoretical applications, such as: using it as an intermediate representation inside a compiler, realizing asynchronous programming as a library, or even mechanically transforming definitional interpreters into abstract machines (with the aid of defunctionalization). Continuation passing is famously described as a mechanism for [time travel] in programming.

[time travel]: https://okmij.org/ftp/continuations/map-story.html

This is a collection of resources for studying continuation-passing style & its applications, ranging from introductory materials to advanced papers. Any questions regarding CPS will be welcomed in the issues.

See also Oleg Kiselyov's awesome list [_"Continuations and Delimited Control"_](https://okmij.org/ftp/continuations/index.html).

## Projects

 - [Standard ML of New Jersey (SML/NJ)](https://smlnj.org/) -- A compiler for the Standard ML '97 programming language.
 - [CHICKEN Scheme](https://call-cc.org/) -- A compiler from Scheme to continuation-passing C code.
 - [`include/metalang99/eval/rec.h`](https://github.com/hirrolot/metalang99/blob/master/include/metalang99/eval/rec.h) -- Continuation-passing recursion for the C/C++ preprocessor.
 - [`CC-delcont`](https://hackage.haskell.org/package/CC-delcont) -- Delimited continuations and dynamically scoped variables.
 - [`cl-cont`](https://quickref.common-lisp.net/cl-cont.html) -- A library that implements continuations for Common Lisp by CPS transform.
 - [`cl-coroutine`](https://github.com/takagi/cl-coroutine) -- A coroutine library for Common Lisp based on `cl-cont`.

## Books

 - Appel, Andrew W. Compiling with Continuations. Cambridge: Cambridge University Press, 1991. Print. $${\textbf{\color{lightgreen}introductory}}$$
   <br>[URL](https://www.cambridge.org/core/books/compiling-with-continuations/7CA9C36DCE78AD82218E745F43A4E740)

## Papers

### 1989

 - Appel, Andrew W., and Trevor Jim. "Continuation-passing, closure-passing style." Proceedings of the 16th ACM SIGPLAN-SIGACT symposium on Principles of programming languages. 1989.
   <br>[URL](https://www.cs.princeton.edu/~appel/papers/cpcps.pdf), [webarchive](http://web.archive.org/web/20250716052049/https://www.cs.princeton.edu/~appel/papers/cpcps.pdf)

### 1993

 - Reynolds, John C. "The discoveries of continuations." Lisp and symbolic computation 6.3 (1993): 233-247. $${\textbf{\color{gold}overview}}$$
   <br>[URL](https://ics.uci.edu/~jajones/INF102-S18/readings/08_histcont.pdf), [webarchive](http://web.archive.org/web/20240605172529/https://ics.uci.edu/~jajones/INF102-S18/readings/08_histcont.pdf)
 - Flanagan, Cormac, et al. "The essence of compiling with continuations." ACM Sigplan Notices 28.6 (1993): 237-247.
   <br>[URL](https://www2.ccs.neu.edu/racket/pubs/pldi-fsdf.pdf), [webarchive](http://web.archive.org/web/20250716050007/https://www2.ccs.neu.edu/racket/pubs/pldi-fsdf.pdf)
 - Sabry, Amr, and Matthias Felleisen. "Reasoning about programs in continuation-passing style." Lisp and symbolic computation 6.3 (1993): 289-360.
   <br>[URL](https://courses.grainger.illinois.edu/cs421/fa2021/papers/reasoning_about_programs_in_continuation_108251.pdf), [webarchive](http://web.archive.org/web/20250716051440/https://courses.grainger.illinois.edu/cs421/fa2021/papers/reasoning_about_programs_in_continuation_108251.pdf)

### 1994

 - Hatcliff, John, and Olivier Danvy. "A generic account of continuation-passing styles." Proceedings of the 21st ACM SIGPLAN-SIGACT symposium on Principles of programming languages. 1994.
   <br>[URL](https://dlnext.acm.org/doi/pdf/10.1145/174675.178053)
 - Lawall, Julia L., and Olivier Danvy. "Continuation-based partial evaluation." Proceedings of the 1994 ACM conference on Lisp and functional programming. 1994.
   <br>[URL](https://dlnext.acm.org/doi/pdf/10.1145/182409.182483)

### 1995

 - Kelsey, Richard A. "A correspondence between continuation passing style and static single assignment form." ACM SIGPLAN Notices 30.3 (1995): 13-22.
   <br>[URL](https://bernsteinbear.com/assets/img/kelsey-ssa-cps.pdf), [webarchive](http://web.archive.org/web/20250701132455/https://bernsteinbear.com/assets/img/kelsey-ssa-cps.pdf)

### 1997

 - Thielecke, Hayo. "Categorical structure of continuation passing style." (1997).
   <br>[URL](https://era.ed.ac.uk/bitstream/handle/1842/393/ECS-LFCS-97-376.pdf), [webarchive](http://web.archive.org/web/20250716051906/https://era.ed.ac.uk/bitstream/handle/1842/393/ECS-LFCS-97-376.pdf)

### 1999

 - Thielecke, Hayo. "Continuations, functions and jumps." ACM SIGACT News 30.2 (1999): 33-42.
   <br>[URL](https://dl.acm.org/doi/pdf/10.1145/568547.568561)

### 2001

 - Danvy, Olivier, and Lasse R. Nielsen. "Defunctionalization at work." Proceedings of the 3rd ACM SIGPLAN international conference on Principles and practice of declarative programming. 2001. $${\textbf{\color{cyan}defunctionalization}}$$
   <br>[URL](http://staff.ustc.edu.cn/~bjhua/courses/ats/2015/readings/defunctionalization.pdf), [webarchive](http://web.archive.org/web/20250716054038/http://staff.ustc.edu.cn/~bjhua/courses/ats/2015/readings/defunctionalization.pdf)

### 2002

 - Berdine, Josh, et al. "Linear continuation-passing." Higher-order and symbolic computation 15.2 (2002): 181-208.
   <br>[URL](http://www0.cs.ucl.ac.uk/staff/p.ohearn/papers/LinCP.pdf), [webarchive](http://web.archive.org/web/20250716052321/http://www0.cs.ucl.ac.uk/staff/p.ohearn/papers/LinCP.pdf)

### 2007

 - Kennedy, Andrew. "Compiling with continuations, continued." Proceedings of the 12th ACM SIGPLAN international conference on Functional programming. 2007.
   <br>[URL](https://www.microsoft.com/en-us/research/wp-content/uploads/2007/10/compilingwithcontinuationscontinued.pdf), [webarchive](http://web.archive.org/web/20250612121841/https://www.microsoft.com/en-us/research/wp-content/uploads/2007/10/compilingwithcontinuationscontinued.pdf)
 - Dyvbig, R. Kent, Simon Peyton Jones, and Amr Sabry. "A monadic framework for delimited continuations." Journal of functional programming 17.6 (2007): 687-730. $${\textbf{\color{violet}delimited control}}$$
   <br>[URL](https://legacy.cs.indiana.edu/~dyb/pubs/monadicDC.pdf), [webarchive](http://web.archive.org/web/20250521164240/https://legacy.cs.indiana.edu/~dyb/pubs/monadicDC.pdf)
 - Asai, Kenichi, and Yukiyoshi Kameyama. "Polymorphic delimited continuations." Asian Symposium on Programming Languages and Systems. Berlin, Heidelberg: Springer Berlin Heidelberg, 2007.
   <br>[URL](http://cs.tsukuba.ac.jp/~kam/paper/aplas07.pdf), [webarchive](http://web.archive.org/web/20250716052934/http://cs.tsukuba.ac.jp/~kam/paper/aplas07.pdf)
 - Kiselyov, Oleg, and Chung-chieh Shan. "Delimited continuations in operating systems." International and Interdisciplinary Conference on Modeling and Using Context. Berlin, Heidelberg: Springer Berlin Heidelberg, 2007. $${\textbf{\color{violet}delimited control}}$$
   <br>[URL](https://homes.luddy.indiana.edu/ccshan/zipper/context2007.pdf), [webarchive](http://web.archive.org/web/20250601170422/https://homes.luddy.indiana.edu/ccshan/zipper/context2007.pdf)

### 2008

 - Ley-Wild, Ruy, Matthew Fluet, and Umut A. Acar. "Compiling self-adjusting programs with continuations." Proceedings of the 13th ACM SIGPLAN international conference on Functional programming. 2008.
   <br>[URL](https://home.ttic.edu/~pl/sa-sml/icfp08.pdf), [webarchive](http://web.archive.org/web/20221208110659/https://home.ttic.edu/~pl/sa-sml/icfp08.pdf)
 - Herbelin, Hugo, and Silvia Ghilezan. "An approach to call-by-name delimited continuations." Proceedings of the 35th annual ACM SIGPLAN-SIGACT symposium on Principles of programming languages. 2008. $${\textbf{\color{violet}delimited control}}$$
   <br>[URL](https://inria.hal.science/file/index/docid/524949/filename/popl-HerGhi08-cbn-delim.pdf), [webarchive](http://web.archive.org/web/20250716053136/https://inria.hal.science/file/index/docid/524949/filename/popl-HerGhi08-cbn-delim.pdf)
 - Danvy, Olivier. "Defunctionalized interpreters for programming languages." ACM Sigplan Notices 43.9 (2008): 131-142. $${\textbf{\color{cyan}defunctionalization}}$$
   <br>[URL](http://jfla.inria.fr/2014/danvy-ICFP08.pdf), [webarchive](http://web.archive.org/web/20241210194514/http://jfla.inria.fr/2014/danvy-ICFP08.pdf)

### 2009

 - Ariola, Zena M., Hugo Herbelin, and Amr Sabry. "A type-theoretic foundation of delimited continuations." Higher-order and symbolic computation 22.3 (2009): 233-273. $${\textbf{\color{violet}delimited control}}$$
   <br>[URL](https://inria.hal.science/inria-00177326/document), [webarchive](http://web.archive.org/web/20250716053037/https://inria.hal.science/inria-00177326/document)
 - Rompf, Tiark, Ingo Maier, and Martin Odersky. "Implementing first-class polymorphic delimited continuations by a type-directed selective CPS-transform." Proceedings of the 14th ACM SIGPLAN international conference on Functional programming. 2009. $${\textbf{\color{violet}delimited control}}$$
   <br>[URL](https://infoscience.epfl.ch/server/api/core/bitstreams/3b4fdf4f-16da-4e39-b616-61a92e16d7e0/content), [webarchive](http://web.archive.org/web/20250716053621/https://infoscience.epfl.ch/server/api/core/bitstreams/3b4fdf4f-16da-4e39-b616-61a92e16d7e0/content)

### 2010

 - Kiselyov, Oleg. "Delimited control in OCaml, abstractly and concretely: System description." International Symposium on Functional and Logic Programming. Berlin, Heidelberg: Springer Berlin Heidelberg, 2010. $${\textbf{\color{violet}delimited control}}$$
   <br>[URL](https://www.okmij.org/ftp/continuations/caml-shift.pdf), [webarchive](http://web.archive.org/web/20250716053818/https://www.okmij.org/ftp/continuations/caml-shift.pdf)

### 2011

 - Kerneis, Gabriel, and Juliusz Chroboczek. "Continuation-Passing C, compiling threads to events through continuations." Higher-Order and Symbolic Computation 24.3 (2011): 239-279.
   <br>[URL](https://arxiv.org/pdf/1011.4558), [webarchive](http://web.archive.org/web/20241126191555/https://arxiv.org/pdf/1011.4558)
 - Materzok, Marek, and Dariusz Biernacki. "Subtyping delimited continuations." ACM SIGPLAN Notices 46.9 (2011): 81-93. $${\textbf{\color{violet}delimited control}}$$
   <br>[URL](https://www.tilk.eu/shift0/materzok-biernacki-HOSC13.pdf), [webarchive](http://web.archive.org/web/20250304104630/http://www.tilk.eu/shift0/materzok-biernacki-HOSC13.pdf)

### 2017

 - Maurer, Luke, et al. "Compiling without continuations." Proceedings of the 38th ACM SIGPLAN Conference on Programming Language Design and Implementation. 2017.
   <br>[URL](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/11/compiling-without-continuations.pdf), [webarchive](http://web.archive.org/web/20250611064636/https://www.microsoft.com/en-us/research/wp-content/uploads/2016/11/compiling-without-continuations.pdf)
 - Davis, Milo, William Meehan, and Olin Shivers. "No-brainer CPS conversion (functional pearl)." Proceedings of the ACM on Programming Languages 1.ICFP (2017): 1-25.
   <br>[URL](https://www.khoury.northeastern.edu/home/shivers/papers/nobrainer-cps.pdf), [webarchive](http://web.archive.org/web/20240711132258/https://www.khoury.northeastern.edu/home/shivers/papers/nobrainer-cps.pdf)

### 2018

 - Farvardin, Kavon, and John Reppy. "Compiling with Continuations and LLVM." arXiv preprint arXiv:1805.08842 (2018).
   <br>[URL](https://arxiv.org/pdf/1805.08842), [webarchive](http://web.archive.org/web/20250716051424/https://arxiv.org/pdf/1805.08842)

### 2019

 - Cong, Youyou, et al. "Compiling with Continuations, or without? Whatever." Proceedings of the ACM on Programming Languages 3.ICFP (2019): 1-28.
   <br>[URL](https://www.cs.purdue.edu/homes/rompf/papers/cong-icfp19.pdf), [webarchive](http://web.archive.org/web/20250524232950/https://www.cs.purdue.edu/homes/rompf/papers/cong-icfp19.pdf)

### 2021

 - Paraskevopoulou, Zoe, and Anvay Grover. "Compiling with continuations, correctly." Proceedings of the ACM on Programming Languages 5.OOPSLA (2021): 1-29.
   <br>[URL](https://dl.acm.org/doi/pdf/10.1145/3485491)
 - Gibbons, Jeremy. "Continuation-passing style, defunctionalization, accumulations, and associativity." arXiv preprint arXiv:2111.10413 (2021). $${\textbf{\color{cyan}defunctionalization}}$$
   <br>[URL](https://arxiv.org/pdf/2111.10413), [webarchive](http://web.archive.org/web/20250716064455/https://arxiv.org/pdf/2111.10413)

### 2023

 - Santo, José Espírito, and Filipa Mendes. "The logical essence of compiling with continuations." arXiv preprint arXiv:2304.14752 (2023).
   <br>[URL](https://arxiv.org/pdf/2304.14752), [webarchive](http://web.archive.org/web/20250716051024/https://arxiv.org/pdf/2304.14752)

## Miscellaneous

 - [_"An argument against call/cc"_](https://okmij.org/ftp/continuations/against-callcc.html) by Oleg Kiselyov.
 - [_"By example: Continuation-passing style in JavaScript"_](https://matt.might.net/articles/by-example-continuation-passing-style/) by Matt Might.
 - [_"On Recursion, Continuations and Trampolines"_](https://eli.thegreenplace.net/2017/on-recursion-continuations-and-trampolines/) by Eli Bendersky.
 - [_"Into CPS, never to return"_](https://bernsteinbear.com/blog/cps/) by Max Bernstein.
 - [_"The Best Refactoring You've Never Heard Of"_](https://www.pathsensitive.com/2019/07/the-best-refactoring-youve-never-heard.html) by Jimmy Koppel.

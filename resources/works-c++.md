## C++ Works (mostly talks, a few books)

*\[Please read [`../README.md`](../README.md) if you have not done so already.\]*

Herb Sutter

* Modern C++: What You Need to Know [talk] [important performance advice] \
https://channel9.msdn.com/Events/Build/2014/2-661 \
[slides] http://view.officeapps.live.com/op/view.aspx?src=http%3a%2f%2fvideo.ch9.ms%2fsessions%2fbuild%2f2014%2f2-661.pptx

* How to Adopt Modern C++17 into Your C++ Code [talk] \
https://channel9.msdn.com/Events/Build/2018/BRK2146 \
[slides] http://view.officeapps.live.com/op/view.aspx?src=https%3a%2f%2fak.studios.ms%2fevents%2f2018%2f1805%2fBuild%2fassets%2fBRK2146.pptx

Bjarne Stroustrup

* Are lists evil? [faq section] [important performance advice] \
http://stroustrup.com/bs_faq.html#list

* Software Development for Infrastructure [paper] [important performance advice] \
http://www.stroustrup.com/Software-for-infrastructure.pdf

* C++ Style [talk] [important performance advice] \
https://channel9.msdn.com/Events/GoingNative/GoingNative-2012/Keynote-Bjarne-Stroustrup-Cpp11-Style

Herb Sutter

* Leak-Freedom in C++... By Default. [talk] \
https://channel9.msdn.com/Events/CPP/CppCon-2016/CppCon-2016-Herb-Sutter-Leak-Freedom-in-C-By-Default \
[slides] https://github.com/CppCon/CppCon2016/blob/master/Presentations/Lifetime%20Safety%20By%20Default%20-%20Making%20Code%20Leak-Free%20by%20Construction/Lifetime%20Safety%20By%20Default%20-%20Making%20Code%20Leak-Free%20by%20Construction%20-%20Herb%20Sutter%20-%20CppCon%202016.pdf

Bjarne Stroustrup

* "New" Value Terminology [short paper] \
http://www.stroustrup.com/terminology.pdf \
Especially the portion Ivan Kush quotes at https://stackoverflow.com/a/38169963.

Scott Meyers

* Move Semantics, Perfect Forwarding, and Rvalue references [talk] \
https://skillsmatter.com/skillscasts/2188-move-semanticsperfect-forwarding-and-rvalue-references \
http://www.aristeia.com/videos/accu2011-movesemantics.mp4 \
[slides] http://www.aristeia.com/TalkNotes/ACCU2011_MoveSemantics.pdf \
[NB: The video quality is bad. You need the slides. It's worth it, though.]

* Universal References in C++ [paper] \
https://isocpp.org/blog/2012/11/universal-references-in-c11-scott-meyers

* Universal References in C++11 [talk] \
https://channel9.msdn.com/Shows/Going+Deep/Cpp-and-Beyond-2012-Scott-Meyers-Universal-References-in-Cpp11 \
[NB: "forwarding reference" is now the accepted term for "universal reference"] \
[NB: type alises with `using` are eligible for reference collapsing, just like `typedef`]

(no byline given; probably written by one or more Google software engineers)

* Tip of the Week #49: Argument-Dependent Lookup \
https://abseil.io/tips/49 \
[for more details: https://en.cppreference.com/w/cpp/language/adl] \
[keep in mind: https://en.cppreference.com/w/cpp/language/dependent_name#Lookup_rules]

Arthur O'Dwyer

* Lambdas from First Principles: A Whirlwind Tour of C++ [talk] \
https://channel9.msdn.com/Events/CPP/CppCon-2015/CPPConD01V009

Scott Meyers

* The Last Thing D Needs [talk] \
https://www.youtube.com/watch?v=KAWA1DuvCnQ \
[Covers some commonly confusing aspects of C++'s type system.]

Scott Meyers

* Effective Modern C++: 42 Specific Ways to Improve Your Use of C++11 and C++14 [book] \
http://shop.oreilly.com/product/0636920033707.do?cmp=af-code-books-video-product_cj_0636920033707_7708709 \
https://play.google.com/store/books/details/Scott_Meyers_Effective_Modern_C?id=ZDhIBQAAQBAJ \
https://www.alibris.com/Effective-Modern-C-42-Specific-Ways-to-Improve-Your-Use-of-C-11-and-C-14-Scott-Meyers/book/28052903?matches=19 \
https://smile.amazon.com/Effective-Modern-Specific-Ways-Improve/dp/1491903996/ref=sr_1_2?ie=UTF8&qid=1537038421&sr=8-2&keywords=effective+modern+c%2B%2B&dpID=51eFBpqPSLL&preST=_SX218_BO1,204,203,200_QL40_&dpSrc=srch \
[errata] http://www.aristeia.com/BookErrata/emc++-errata.html

Stephan T. Lavavej

* Core C++ [10-part lecture series] \
https://channel9.msdn.com/Series/C9-Lectures-Stephan-T-Lavavej-Core-C-

Stephan T. Lavavej

* Don???t Help the Compiler [talk] \
https://channel9.msdn.com/Events/GoingNative/2013/Don-t-Help-the-Compiler \
[slides] http://view.officeapps.live.com/op/view.aspx?src=http%3a%2f%2fvideo.ch9.ms%2fsessions%2fgonat%2f2013%2fSTLGN13Compiler.pptx \
[NB: The bonus slides, which were not covered in the talk, are worth checking out.]

Herb Sutter

* Back to the Basics! Essentials of Modern C++ Style [talk] \
https://channel9.msdn.com/Events/CPP/C-PP-Con-2014/0010-Back-to-the-Basics-Essentials-of-Modern-C-Style \
[slides] https://github.com/CppCon/CppCon2014/blob/master/Presentations/Back%20to%20the%20Basics!%20Essentials%20of%20Modern%20C%2B%2B%20Style/Back%20to%20the%20Basics!%20Essentials%20of%20Modern%20C%2B%2B%20Style%20-%20Herb%20Sutter%20-%20CppCon%202014.pdf

Greg Falcon

* Initialization, Shutdown, and constexpr \
https://www.youtube.com/watch?v=6ZOygaUjzjQ

Nicolai Josuttis

* The Nightmare of Initialization in C++ \
https://www.youtube.com/watch?v=7DTlWPgX6zs \
[NB: The issue https://youtu.be/7DTlWPgX6zs?t=2957 describes is particularly surprising.]

Walter E. Brown

* C++ Function Templates: How Do They Really Work? [talk] \
https://www.youtube.com/watch?v=NIDEjY5ywqU \
[NB: Slides, including some not shown, supposedly exist, but I haven't found them.]

Dan Saks

* Back to Basics: Function and Class Templates [talk] \
https://www.youtube.com/watch?v=LMP_sxOaz6g

* Making New Friends [talk] \
https://www.youtube.com/watch?v=POa_V15je8Y \
[NB: slides 43-46 wrongly suggest friend declarations can't always use the injected class name]

Jonathan Boccara

* 105 STL Algorithms in Less Than an Hour [talk] \
https://www.youtube.com/watch?v=2olsGf6JIkU

Sean Parent

* Generic Programming [talk] \
[slides and papers] https://github.com/sean-parent/sean-parent.github.io/tree/master/presentations/2018-10-18-generic-programming

    [NB: The written works shown in the talk are:

    - Generic Programming (Musser et al. 1988) \
        http://stepanovpapers.com/genprog.pdf
    - The Standard Template Library (Stepanov & Lee 1995) \
        http://stepanovpapers.com/STL/DOC.PDF
    - Programming Pearls: Writing Correct Programs (Bentley 1983) \
        https://www.cs.tufts.edu/~nr/cs257/archive/jon-bentley/correct-programs.pdf
    - Exception Safety in Generic Components (Abrahams 1998) \
        https://www.boost.org/community/exception_safety.html
    - Fundamentals of Generic Programming (Denhert & Stepanov 1998) \
        http://stepanovpapers.com/DeSt98.pdf
    - Notes on the Foundations of Programming (Stepanov & Marcus) \
        http://stepanovpapers.com/PAM.pdf
    - Elements of Programming (Stepanov & McJones 2009) [*] \
        http://elementsofprogramming.com/book.html
    - Concepts: Linguistic Support for Generic Programming in C++ (Gregor et al. 2006) \
        http://www.stroustrup.com/oopsla06.pdf
    - A Concept Design for the STL (ed. Stroustrup & Sutton 2012) \
        http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2012/n3351.pdf
    - From Mathematics to Generic Programming (Stepanov & Rose 2015) \
        http://www.fm2gp.com/
    - C++ Standard Draft Sources \
        https://github.com/cplusplus/draft

  [*] Very worth reading.]

Titus Winters

* Modern C++ Design (part 1 of 2) [talk] \
https://www.youtube.com/watch?v=xTdeZ4MxbKo

* Modern C++ Design (part 2 of 2) [talk] \
https://www.youtube.com/watch?v=tn7oVNrPM8I

* Revisiting Regular Types [blog post] \
https://abseil.io/blog/20180531-regular-types

Chandler Carruth

 * LLVM: A Modern, Open C++ Toolchain [talk] \
https://www.youtube.com/watch?v=uZI_Qla4pNA

Robert Nystrom

* Game Programming Patterns [book] \
http://gameprogrammingpatterns.com/

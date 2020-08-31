![img](/images/sympy_logo.png) ![img2](/images/gsoc_logo.png)

# GSoC 2020 @[SymPy](https://github.com/sympy/sympy)

This repository showcases my proposal, final report, and the work done during Google Summer of Code 2020 with the SymPy project.
SymPy is a computer algebra system written in pure python.

It all started here:

![img3](/first_email.png)

The SymPy community is very welcoming and supportive. I sent an email to the SymPy mailing list around Feb 3rd, 2020 asking the community about the scope of adding a new Control Systems engineering package. Initially, their opinions were against this, and students were advised to focus on improving existing SymPy packages, *instead* of adding new packages (core or not).

I continued to show my interest in this project and guess what?? Here is the response I got finally (Thanks, [Jason](https://github.com/moorepants)):

![img4](/images/Jason's_response.png)

# Project: [Control Theory - Implement a control systems package](https://summerofcode.withgoogle.com/projects/#6580631821090816)


Student: Naman Gera (namannimmo10)

Official Mentors:
* Nikhil Maan ([@Sc0rpi0n101](https://github.com/Sc0rpi0n101))
* Jason K. Moore ([@moorepants](https://github.com/moorepants))
* Ishan Joshi ([@ishanaj](https://github.com/ishanaj))

Since this was a big project and I had to develop a package from scratch, I got a lot of help from other members of the SymPy development team or even Control theory experts. I would also really like to thank [S.Y. Lee](https://github.com/sylee957), [Oscar Benjamin](https://github.com/oscarbenjamin), [Eric Wieser](https://github.com/eric-wieser), [Ilhan Polat](https://github.com/ilayn), and [Richard Murray](https://github.com/murrayrm) for constantly reviewing my PRs and discussing the API designs with me.

# Work done:

My main focus was to implement in SymPy, a basic control systems functionality from scratch. This can be used by Control engineers or students to solve various [control theory](https://en.wikipedia.org/wiki/Control_theory) related problems. Being a part of SymPy, this is purely *symbolic* in nature. The advantage of this package over other packages/libraries (which are great btw!) like [harold](https://github.com/ilayn/harold) and [python-control](https://github.com/python-control/python-control) is that the solutions obtained from it are highly accurate and do not rely on numerical methods to approximate the solutions. The solutions obtained from it are in a compact form that can be used for further analysis. **Documentation** available at [Control API](https://docs.sympy.org/dev/modules/physics/control/lti.html) and [Control Intro](https://docs.sympy.org/dev/modules/physics/control/control.html).

PULL REQUESTS - 

Major additions:
* (Merged) [sympy/sympy#19390](https://github.com/sympy/sympy/pull/19390) - Adds `TransferFunction`, `Series`, `Parallel`, and `Feedback` classes for control package.
* (Merged) [sympy/sympy#19896](https://github.com/sympy/sympy/pull/19896) - Adds other useful methods in `TransferFunction` class.
* (Open) [sympy/sympy#19761](https://github.com/sympy/sympy/pull/19761) - Adds `TransferFunctionMatrix` class in *physics.control*.

Miscellaneous PRs opened in the summer:
* (Merged) [sympy/sympy-bot#87](https://github.com/sympy/sympy-bot/pull/87) - Adds *physics.control* as valid submodule.
* (Merged) [sympy/sympy#20008](https://github.com/sympy/sympy/pull/20008) - Modify docs of `is_stable` method in `TransferFunction` class.

Future Work:
* Add `StateSpace` class for creating State space models
* Further improve the documentation of control package. Add couple more examples to show us the users how to use the implemented functionality as they tend to use any software more if the docs are top-notch.
* Graphical analyses: `root_locus`, `pole_zero`, `bode`, and `nyquist` plots

# My GSoC Experience and Learnings:

I've been writing weekly blog-posts documenting my journey during
GSoC. The blog is hosted at [My-GSoC-blog](https://namannimmo10.github.io/emerald/).
This experience was so amazing and complete that I learned a lot of things I can't write them all in here.

But, here are a few:
1. Having to adjust to my team's different timezones was *definitely* a challenge. I also loved the challenge of working with a remote team and leave my comfort zone of talking in person to work on something.
2. I can easily say that I learned written communication. Writing accurately is difficult, so I had to learn how to convey my thoughts well enough, because we were working remotely, right?
3. I never implemented any package from scratch before, so this was a challenge in itself. But the mentors were helpful enough and discussed everything with me. They were readily available for discussions.
4. If could repeat this again, I would do so. This community is so welcoming, even if you come up with a *naive* approach to solving a particular problem, they will help in improving the code even more because we had to adhere to the SymPy standards.


`:wq` for now

------------------------------------------------------------------------------------------------

Naman Gera

[Email](mailto:namangera15@gmail.com) | [GSoC blog](https://namannimmo10.github.io/emerald/) |  [StackOverflow](https://stackoverflow.com/users/11750129/namannimmo) | [Twitter](https://twitter.com/namannimmo?s=09)

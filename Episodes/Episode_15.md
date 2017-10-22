# Let's Talk ETC: Dr. Duncan Coutts - Provably Secure Smart Contracts.
**Carlo Vicari:**
hi everyone and thank you for tuning in
you're listening to let's talk et Cie
I'm your host karlovy along with my
co-host dr. Christian Shepherd suberino
I want to thank the et Cie does
investors miners users and other
community members for another great week
those of you who are watching on youtube
or listening on the podcast the e.t.c
newsletter will be in the description
below on the YouTube channel which is
dr. Christian submarino's youtube
channel so the main focus for tonight
for today's show is the et Cie
development and specification formal
verification community we've got a
really great guest with us tonight he is
really knowledgeable and he's got a lot
of great insight to a whole bunch of
stuff
Duncan has more than 15 years
programming experience with Haskell he's
a well-known member of the Haskell
community and he helps maintain several
popular libraries and tools including
cable and how do I say this Duncan by
capacity Kabbalah Kabalah quite a high
string and he has several years
experience in packaging the Haskell tool
chain and took a leading role in
establishing the Haskell platform so
it's a pretty incredible that we have a
Duncan Kurtz here with us PhD
Duncan am i pronouncing your last name
correctly Duncan Koontz


**Dr.Duncan Coutts:**
 that's right


**Carlo Vicari:**
okay so great to have you on here and uh
yeah so I just want to give you a little
bit of info and also anyone that's kind
of listening to the show for the first
time what we like to do is kind of get a
background on our guests especially if
it's their first time on the show kind
of their background and how they got in
detected stuff like that so I guess so
what was your technology rabbit-hole
Duncan and Jeju and Episode II



**Dr.Duncan Coutts:**
 well I
was one of those lucky people who at
school knew exactly what they wanted to
do like you know my friends all were
should I do this subject or that subject
I was like no no I just want to get rid
of all my other subjects that do
computer computing programming
okay I've got I've got to do some maths
and some physics to sort of fill out the
edges yeah so I was one of those people
who knew that that's what I wanted to do
so I did computing at a-level in the UK
and then I applied at university to a
university that takes a very math
magical approach to to computer science
and this kind of like an engineering
approach and the mathematical approach
and I I wanted to go to is from my point
of view then that was like this is the
hard core way of doing it let's go the
hard core way let's do the mathematical
way and that was what I applied to the
University that took took that approach
and actually it was it was at least as
good as I was expecting and it was just
mind-blowing nice at the beginning just
discovering discovering all these new
things thinking about programming in a
completely new way that I had you know
I'd been hacking along as a teenager for
a few years but Trey University was
suddenly this you know as you would
really hope that university should be a
mind expanding experience and seeing
this idea that programs are mathematical
things you can prove things about
programs was just like incredible to me
at first so that was rain that was how I
got into 






**Carlo Vicari:**
it and and that's yes that's
proving things and in formal
verification are gonna be a pretty hot
topic especially in crypto and
blockchain with stuff like the the dow
hack and smart contracts and all that
bad stuff I'm guessing right




**Dr.Duncan Coutts:**
 right and
my focus particularly at university was
that in functional programming so I was
introduced to functional programming my
first term and that was what was
completely mind-blowing because it was a
completely different way of writing
software from what I've done before
which was you know things like Pascal
Delfy C++ that kind of thing and then
the functional programming was just you
know it to me just obviously better once
it was presented to me right not not all
of my knowledge my classmates agreed I
think probably only a small fraction of
us caught the functional programming bug
but but those of us who do that was this
like this this is like obviously the
right way to do things


**Carlo Vicari:**
yeah I don't know if you've seen I'm
sorry go ahead Christian 



**Christian Seberino:**
I was gonna say
so and then after you got your PhD did
you have any interesting adventures in
industry you want to share or any




**Dr.Duncan Coutts:**
 yeah
so so I was one of those people who
basically stayed you know far too long
and academia just which was you know
brilliant and fantastic and interesting
but then as I was getting towards the
end of my PhD which took unreasonably
long
a guy who'd been in the same with the
same PhD supervisor as me who had been
out in industry already for a couple
years came to me and said look how
school is actually taking off
commercially just look at these numbers
like various kind of statistics on
mailing lists and other kinds of metrics
then saying look this is this is going
up exponentially now we could actually
uh we could actually go and start a
company doing this 



**Carlo Vicari:**
right now for for
everyone listening who's maybe not as I
guess not as much development experience
as you know you and Christian um so for
all of us you know newbies out there
what are some of the like applications
of of Haskell and functional programming
and I know I've heard it spoken a lot
about that it's you know really good for
like mission critical software for you
know NASA and all sorts of stuff like
that but I was hoping you could give us
some insight into like some of the
really high assurance situations that
Haskell would be 




**Christian Seberino:**
really good for well
actually even before that make sure to
ask also what is functional programming



**Carlo Vicari:**
that to write I need to know that right



**Dr.Duncan Coutts:**
yeah well let me start with with with
the person so in some sense it's a
slightly hard question to answer because
it's not a programming language that's
designed for one thing it's a
programming language designed to be a
good general purpose programming
language functional programming Haskell
is a functional programming language and
functional programming is a
general-purpose approach to writing
programs so it's a complete alternative
to what you would do in any other
language there's not it's not
specialized like say you know MATLAB
especially for doing mathematical
simulations and uz+ passes for system
software and python is but you know it's
not quite like that it's it's a
general-purpose jump on this thing that
said the the kinds of places where it
has the greatest sort of comparative
advantage is where you have hard
problems really hard problems and where
there's a lot at stake for example a lot
of money at stake or or safety at stake




**Carlo Vicari:**
that would have been good present down
so um so a lot of money and stake a lot
of things at stake what are what are
sermons




**Dr.Duncan Coutts:**
 so yes I
some of the early adopters of Pascal in
industry were big banks because they
have they're trying to develop custom
software very quickly that's the other
thing is productivity they're trying to
develop correct software that deals with
a lot of money and they're trying to do
it very quickly and continuously and be
able to reuse that software again and
again again so they were some of the
early adopters commercially but actually
I mean our customers oh I run a house
called consulting company these days and
our customers come from all kinds of
industries there's not like one main
industry that people use it for it's
really very wide people he's high school
for just you know web database business
logic you know that kind of thing as
well as you know really interesting and
niche things 



**Christian Seberino:**
okay I have a question so
the standard a common story in in tech
is somebody adopts a new technology
before most other people and so they're
that much more productive they could
provide that much more value and that's
how they become successful so it's it
correct to say that there's lots of
companies either openly or secretly
using Haskell to to great effect can you
can you name some of those or they will
not want to reveal that



**Dr.Duncan Coutts:**
 sure I mean how
many there are you know as a fraction of
the entire industry well it's still I
guess relatively small but there are
still there are certainly companies that
are using it to great effect and there's
there's lots that have given talks and
talked about it publicly it and for
example the CFP actually uses functional
programming conference so a lot of the
financial institutions bar cap so you
saw some some big banks then you've got
a Facebook is using it about these days
okay as group Google use it a very
little bit they tend to be very
conservative on their choice of
languages they use it for internal
systems not publicly facing systems no
and then there's a whole bunch of
startups like just small places you have
never heard of and where they're using
it so it tends to be small teams in very
big companies or small teams and very
small companies 



**Christian Seberino:**
okay so would you think
that if it's possible
one day that a big company like Facebook
would say okay Haskell is so awesome
we're gonna company-wide every all our
programmers have to use it we're only
going to hire Haskell programmers or
some other whatever the next functional
languages



**Dr.Duncan Coutts:**
 yeah so then then they would
actually have a serious problem which is
that they have laws in the world's world
to buy of they would need many more than
the world's five hospital programmers so
so Haskell is taught and other and other
functional languages are taught as a
number of universities but it's not it's
not taught in the same scale as say Java
okay and so this this comes down to one
of the reasons why people choose
mainstream languages even though there
may be advantages to using using less
commonly used ones which is that you can
hire lots of people you know if you're a
manager thinking of starting a new
project you go oh hookah who can I hire
oh there's lots of Java programmers so
I'll use Java and run so that's a reason
to use our languages completely
unrelated to how good it is what kind of
programs you'll get




**Carlo Vicari:**
 just like I'm
function of the market I guess





**Dr.Duncan Coutts:**
 right
it's a self-reinforcing
thing so yeah because you know what what
are people going to learn they're going
to learn languages that will give them a
job



**Carlo Vicari:**
 now I want to ask both you guys this
as developers and programmers you know
really uh you know um so I've seen like
a it's like a cartoon comic that shows
different programming languages and like
if they were people or representations
and the Haskell one is like this deity
you know with it's sitting indian-style
floating in the air with like floating
next to it and then they show a Java and
it's like this mutated mutant thing that
like looks like the public but more
deformed and it's like I'm a functional
or something how in true or not true is
that is Java like the big joke 



**Dr.Duncan Coutts:**
um from
the point of view of the functional
programmers I'm afraid it is yes and
there's actually some good reasons that
it's not just fanboy is a loan you get
you get that in the programming language
world as well and then when there are
action a lot



**Carlo Vicari:**
 I've heard a lot that job
was just like the only failure that has
ever been successful in a programming or
at least that's how it's been described
to me 




**Dr.Duncan Coutts:**
one thing I like to sort of say
about Java is that you know it was
fifteen years behind the cutting edge
when it was first released and it is
still 15 units behind the cutting edge
now
it's a very conservative they've made
improvements over time but it's still a
very sort of conservative approach to
this 



**Christian Seberino:**
yes so would this be a fair comment
there's lots of languages that you could
probably learn much faster and write
quick and dirty programs much faster and
if I just have something I'm throwing
together it's not very mission critical
but would it be fair to tell somebody
okay yeah go ahead and throw it together
in PHP even though we both agree Haskell
is awesome




**Dr.Duncan Coutts:**
it's why I think that the the thing
there is to realize that you've
basically got two major classes of
language you've got the imperative
languages which is what all the
mainstream ones are Java C++ etc Python
PHP they're all they're all imperative
languages and then you've got this other
class which is these functional
languages and it's relatively easy if
you know one imperative language to pick
up another one it's basically the same I
mean there's differences in the library
there's a few differences in the syntax
but the sort of fundamental approach to
things which is do things do that do the
next thing go back and do it again that
that out that imperative way of thinking
and way of writing programs is is common
across them all and so it's quite easy
to switch and so whereas switching to a
functional language you do actually have
to re learn a bunch of things so so the
point is that you know it could be a lot
quicker to just use a language that you
know already in the short term in the
long term the advantages you get really
pile up and so there's kind of you know
there's a learning curve from switching
into a functional language any
functional language and then similarly
once you're inside the world of
functional languages switching between
the different ones it's not that
difficult so there's 



**Christian Seberino:**
so there's there is
another occasion there is



**Dr.Duncan Coutts:**
 definitely
yeah so there's a big there's a
relatively big front learning cost 




**Christian Seberino:**
okay
now what is the function languages now
now is it necessary



**Dr.Duncan Coutts:**
 what now what I mean
by that is because like everybody gets
taught the imperative ones 



**Christian Seberino:**
yes exactly


**Dr.Duncan Coutts:**
so people people have done it
parents at University where you teach
the functional ones first they're no
harder to learn in fact in many ways
they're easier because they're actually
simpler they're my similar behavior and
semantics and whatnot
because everybody gets taught you know
these mainstream ones first and then
there's that sort of switching bias
switch 




**Christian Seberino:**
and why do you think that is the
case if they're not that much they're
not more difficult why don't we learn
that why doesn't every University teach
functional program



**Dr.Duncan Coutts:**
 that is entirely
historical historical reasons and so
this goes back to why do we program
computers in the way we do with with in
this imperative style the language and
that's basically because so that these
two styles of programming imperative and
functional trace their roots all the way
back to their like 1930s with different
mathematicians back in the 30s during
and Alonzo Church and one is based on
the lambda calculus and one is based on
Turing machines and the people then
programming real machines in the 1940s
50s 60s etc they wrote they programmed
computers in the way that they actually
work because that's the obvious thing to
do and that's kind of what you have to
do when the computers were so primitive
and so slow you really have to get every
little bit of performance out of them so
all of those languages sort of trace
their lineage in that in that style
whereas it wasn't really until the kind
of 70s 80s 90s that this alternative
style which has the same history started
from the same point in the in the 1930s
it wasn't until then that they became
kind of practical so that means you've
got already established this massive
mainstream of with imperative style
languages 



**Christian Seberino:**
so if I understand you
correctly one of the things you're
saying is that then that the obvious
thing to do it was to was to mimic the
hardware in your gate language at youth
so but now that computers are faster
than we can now you enjoy functional
programming but now that that begs the
question so is 



**Dr.Duncan Coutts:**
and also the fact that
there was 30 years of research into how
do you actually compile these things
efficiently so that you're not paying
too high a cost




**Christian Seberino:**
okay that is there yet does there have
to be a cost to functional programming
can it be competitive with like say C or
C++ 





**Dr.Duncan Coutts:**
it's very difficult to become really
competitive to C because we tend to rely
on things like garbage collection and
other kinds of higher level things but
it's quite easy to be competitive with
Java and it's very easy to be
competitive with Python PHP and all the
rest of those so people were aiming for
C like performance for decades but then
then Java came along and lowered the bar
and and that's a whole lot easier 



**Christian Seberino:**
now I
don't know if Haskell errs do this but
when I used to evangelize Python that
was my favorite language it still is um
so one technique I would suggest people
do is they're typically you'd profile
your code and there would be some piece
where 98% of the CPU time is being
wasted and you could write that in say C
whatever your favorite fast languages
and then just you know call it from
Python so in if in Haskell I presumably
you have where they call the foreign
language interface foreign 


**Dr.Duncan Coutts:**
foreign
function interface


**Christian Seberino:**
okay so could you do something like that




**Dr.Duncan Coutts:**
if you can you can and and that is still
a reasonable thing to do especially when
it comes to things like you know binding
some existing crypto library
you're not going to rewrite your crypto
library in Haskell you'll just take you
know a really well-written one by the
people who know how to do that stuff see
library binding Haskell give it a nice
interface right but that said your
technique of you know let's you know
there's this tight you there's ninety
eight percent is being spent in this one
bit is actually kind of an annoying
technique to have to do that kind of
thing it's actually rather nice to be
able to within the same language right
both in a high-level style that's slow
and but nice and short and elegant and
also be able to write in a low-level
style that's fast and actually you can
do that to a quite a great extent in
high school so you can't get quite down
to see performance but you can get
really a lot of the way there and that
means that you can still do most of your
stuff within the same language and which
means that you get all the other
advantages you still have the type
system tells you when you're doing
something stupid and and whereas going
doing that cross language to language
thing introduces a lot of difficulties
it's a lot harder to do that I see it's
a lot more effort yeah so I I would say
that you know and if let's say you know
10 times out of a hundred a Python
programmer has to go and do that drop
down to see thing we might have to do
only maybe one time out of a hundred and
that's a big advantage there's still
times when you really have to do it like
as I said the Crypt aliases and your
network bindings and whatnot but so the
altar right high level and low level in
the same language because it's a
compiled language if you can write a low
level c like way in Haskell it's kind of
nice 



**Carlo Vicari:**
so um now that's some a pretty
pretty nice history of Haskell and the
how we ended up where we are now for the
past and stuff like that so in reference
to moving from the past - I guess
current things just introduce everybody
to kind of some stuff you're working on
currently I'm afraid it you know I
didn't do such a good job of introducing
you earlier in the show but uh you're
also part of the well um well typed a
happy it's a Haskell consulting company
and you guys are looking with IO HK
directly on a few different things as I
correct 



**Dr.Duncan Coutts:**
that's right yes so we're
helping them with the Cardno project 




**Carlo Vicari:**
and
just so just so I got this correct so it
looks like um according to the I wish K
bio you're the interim director of
engineering for a team well-typed
correct 




**Dr.Duncan Coutts:**
well I suppose the team name
there is not it's not particularly
significant it's it's entran director of
engineering for the the kadhai no
settlement layer 




**Carlo Vicari:**
right right yeah okay
gotcha gotcha so um so this is something
you're currently working on is Cardno
through IO HK for anybody listening out
there um which they're they're handling
a lot of stuff and in just Haskell which
is pretty cool



**Dr.Duncan Coutts:**
yes the whole the whole code on O
project the software is all the
englishman Haskell ohk are also working
on a theory on classic client which is
being implemented in scarlet which is
another 



**Carlo Vicari:**
functional I functional
programming yeah just so anybody
listening they're from the UTC community
you guys can kind of tie this all
together we have the Skylar client which
is functional programming and then also
we have dr. Duncan dr. Gunes who's
working with the team well typed or
um and there was



**Dr.Duncan Coutts:**
 a whole bunch of teams
I guess there's 



**Carlo Vicari:**
a lot of chance which is
the Cardinal SL lair which is written in
Haskell which is another functional
programming language so there's a whole
bunch of functional programming stuff
going on ohk right now 



**Christian Seberino:**
yeah now I have
another question I just thought of so um
Duncan's so that's this very strong
argument to use functional programming
if the only reason we're doing it is
because of history people just want to
get the the best results as fast as they
can and so history shouldn't play a part
well it maybe it should in some cases
but you made me a believer
but then cut out for it 



**Dr.Duncan Coutts:**
for this but
still a place to see by the way the
compilation of Haskell and C is actually
a really excellent combination 



**Christian Seberino:**
okay so
but the question I wanted to ask you so
suppose somebody's listening and they
say okay fine functional programming
let's let's try it now there's multiple
choices now you love Haskell is that is
there a reason that's the best
functional I know I've heard of like
Lisp and skaila and I'm sure there's
others can you say something about the
different choices




**Dr.Duncan Coutts:**
sure so there's kind of two main sort of
properties that distinguish the various
different functional languages one is
this this technical thing called side
effects is it a pure functional language
or is it a language that allows side
effects to pure means no side effects
impure means it allows side effects and
what that really means is that you can
still do classic imperative programming
in a completely straightforward way in
impure functional language you can have
mutable variables because that's one of
the things about a pure functional
language doesn't have mutable variables
not in there not in the same sense that
that you have just everywhere in
imperative programs so that's one
important sting ssin and we can go into
more detail if you like on on what does
that what does that mean technically why
why is purity a good thing 



**Christian Seberino:**
yes would you
yeah if you please 




**Dr.Duncan Coutts:**
yeah I I will and
then the other but the other axis is
like kind of what platform does it does
it work with so you've got sort of
essentially similar functional languages
that run on different platforms so for
example a Scala is runs on the JVM and
f-sharp runs on dotnet
and also both of those are those are
impure and their hybrid languages which
means they're a mixture of you know
object oriented particularly Scala is a
mixture of object oriented and
functional all together in one language
whereas Haskell and one or two other
function languages are you know it sort
of exclusively functional languages
they're not trying to mix functional
style with a row or an imperative style
missing so scholars like everything all
dumped in together running on the JVM so
sharp is f sharp is kind of like ml
which is a impure
input functional language but it's it's
really in some ways F sharp is nicer it
than the scarlet cuz it's trying to be
just straightforwardly a functional
language although it does run on dotnet




**Christian Seberino:**
okay and why would if functional pure
functional programming is not any harder
why would somebody choose a hybrid like
Scala why not just use I'm sure there's
no technical barriers to making a
kaskell that runs on the Java Virtual
Machine



**Dr.Duncan Coutts:**
no that's right I think that the reason
is that it's much easier to work with
existing imperative languages if you use
a functional language that allows
side-effects everywhere because this is
it so this is this is I in some sense
the really big thing that still
distinguishes Haskell from everything
else as far as I mean there's other
there's other languages like Haskell but
they are much much more niche but
Haskell is like the most is the biggest
representative of that part of the
design space which is purely functional
programming and I see it the pure
functional purely functional style is a
is a is a major win but you really then
have to throw out the rest of your
imperative stuff because they're not
compatible with each other whereas
scholar and f-sharp and there's a kind
of Lisp like language on the JVM as well
they still allow you to have all this
imperative stuff which then makes it
easier to integrate with all the
imperative stuff but then you carry all
of the imperative baggage with you so
it's kind of like you know you can get
so far with making imperative languages
more functional or attacking functional
program on to imperative platforms but
to get to get the last
you know awesome goodness from from
functional programming you've got to
finally get rid of your side effects
okay and then that means that it's very
hard to then reuse your JVM libraries or
your dotnet libraries or whatever 



**Christian Seberino:**
so so
what you're saying then is is libraries
is what would be what would make
somebody decide to use Scala versus
going all the weight it has 




**Dr.Duncan Coutts:**
exactly
exactly yeah so in in in Schuyler knife
sharp it's without too much pain you can
import your imperative dotnet libraries
and JVM libraries through which written
in sorry other languages 



**Carlo Vicari:**
sorry guys for
someone who is a complete noob um it
kind of sounds like what you're saying
is that the Haskell App Store is not as
big as the whatever a App Store app
store is that correct 




**Dr.Duncan Coutts:**
yeah that's true
so it's no hackage has I don't know in
those days about 5,000 maybe libraries
on it which is you know if you compare
that with the node.js you know
equivalent it's obviously a tiny
fraction but on the other hand there's
still a lot of a lot of stuff people
there's lot of off-the-shelf
functionality you can get that right but
it but that's true that is that is in
some sense a trade-off and that's
because we're a smaller community 




**Christian Seberino:**
okay
yeah now before we get into because I
also wanted to switch gears eventually
and talk about provably correct programs
but before we do that can you make can
you address what you touched on before
about so why would you want the the
purity of haskell of having come no side
effects I survived 



**Dr.Duncan Coutts:**
right right so okay
so purely functional languages so get
get that okay there's two ways to look
at it one is that it's it's a nicer
model that's closer to mathematics and
the in closer to mathematics gets you a
whole lot of stuff so a if you think
about a mathematical function you know
it it is pure in the sense that if you
give it the same input the same outputs
every time you know you it doesn't like
you know one one day give you this
output and then another day give you
that other output it's always the same
and so that right that kind of
mathematical approach makes it much
easier to reason about your programs it
makes it much more modular there's not
these hidden interactions and another
way to look at it is
that shared mutable state is one of the
greatest source of bugs in existing
systems and if you eliminate that shared
mutable state your systems become and
make interactions more explicit like the
plumbing you know where this value flows
in and that value flows out rather than
just sort of hidden lis in the
background sharing some piece of mutable
data and that eliminates a whole class
of bugs and make sure program is much
easier to work with much easier to
reason about them so composable 



**Carlo Vicari:**
so it's
almost like the difference between two
plus two equals four and an ambiguous
sentence that you can take to mean you
know at least if you were to bring it to
complete two opposite sides of the
spectrum is that right



**Dr.Duncan Coutts:**
 yeah I guess sure
oh you can't review mathematically you
can reason mathematically about
imperative programs but it's a whole lot
harder and it's much more easy to
accidentally entangle things functional
programming makes everything much more
explicit with easier to reason about and
then there's all kinds of things that
you can enforce if you don't have this
kind of escape hatch of shared mutable
state if all of your functions can just
you know read for the disk and write to
the network and launch your missiles and
that kind of thing without you being
able to see that from the external
interface there's all kinds of nasty
things you can do and that makes it
harder to integrate systems and you know
compose things together whereas in a
functional language in a purely
functional anguish all of these kinds of
interactions are explicit in the
interface and then you can tell by the
fact that interfaces match up or don't
match up whether you've done things
correctly or not I said under so then
there's all kinds of properties you can
enforce with with a strong type system
and pure functions which you simply
can't enforce properly you can only
enforce them by convention whereas you
can enforce them properly but the
compiler will tell you you can't do that
if you can it you can enforce it if
you've got pure functions do you think
that the strong type system these two
things are 



**Carlo Vicari:**
indeed do you think that the
hack would have been a lot less likely
if it was written in something like a
school or a functional pronoun the
functional programming language 




**Dr.Duncan Coutts:**
you need
the combination of two things you need
two it's sensible to use a language like
this but it's also you have to follow
the right development approach right
which means which means thinking about
specifications it means thinking about
trying to think how would I prove what
what is the property that I want what is
the security property that I want how
would I prove it even if you don't
actually prove it thinking about how
could I prove it how would I prove it or
what is the rational argument for what
is the rational argument for why this
thing is secure you know you have to you
have to take a development approach was
asked that starts with those kinds of
questions to be able to even possibly
come out with an outcome that will that
will be secure or that will have the
behavior that you that has some kind of
assurance that it has the behavior that
you want 





**Christian Seberino:**
yeah what do you I had one last
question about different languages so
the 800-pound gorilla of the there from
history in this space is Lisp and when
people talk about list the list
enlightenment experience and when I
first saw scheme and Lisp I just thought
it was so unspeakably beautiful just how
elegant and how powerful you could make
a language with such simple syntax and
there um I was just curious how does
what do you you want to make a comment
about list because job would be and by
the way for people listening if here iam
actually has already something that is
like list there's it's called lll so
like the serpent language compiles down
the abstract syntax tree is is basically
a lisp and then that gets converted to
machine code so if people wanted to they
could use that today but I always
thought list was really cool and I I got
that was what kept me from jumping into
Haskell was well but Lisp is already so
cool 





**Dr.Duncan Coutts:**
so so so Lisp is like the first
mainstream functional language so in
many ways that makes it awesome
but the interesting thing is that there
was you know another 30 years of
research after this and that is also has
a lot of value and there are things we
learned in that 30 years a lot of things
I mean to use so yeah let's discrete and
and it's it has a lot of the elements of
functional programming then many of the
core elements of functional programming
and it's perfectly fairly good but you
can go even further and you can do even
better but you can if you're already
starting with list I'm not going to
criticize you if you're already starting
with Lisp you're already like in there
80% of the way there
yeah my point of view you can see the
nature the major advancements after Lisp
I guess all the distinctions between
Lisp and Haskell is the type system and
this purely functional idea and those
two things together give you a lot of
extra power particularly lot of extra
power to enforce things like enforce you
know you have some idea about invariants
in your system or properties that it
should have and a lot of those things
you can enforce in types and then have
the compiler tell you when you're being
inconsistent you know the compiler says
well you said this over here but over
here you're saying that and these two
things not consistent with each other
sort it out and that is a really really
really powerful technique




**Christian Seberino:**
 is the syntax
of Haskell would you say simple maybe
not as simple as Lisp but it's not like
C++ complex 



**Dr.Duncan Coutts:**
oh it's it yeah it's a lot
simpler that goes pass it in sometimes
it's not as simple as Lisp but a lot of
people think it's more attractive
because there aren't quite so many
parentheses all over the place yeah so
if you were ever put off by the left
syntax if you love this syntax brilliant
but if you were ever put off by you know
parentheses all over the place brackets
brackets brackets then Haskell is a
function language that doesn't have that
kind of forest of parentheses 




**Carlo Vicari:**
it sounds
like you're saying that Lisp is good but
Haskell is better that's what I got at
all 



**Dr.Duncan Coutts:**
that that is what I'm saying a list
person would say little around but do it
but there's a bit warmer




**Christian Seberino:**
 okay so why
don't we now why don't we switch now I
mean talk about what a lot of people
care about is which is how to you know
save them money and so apparently
there's there's decades of research
about making programs provably secure or
there's evidence more evidence than you
would normally have that may be can you
talk about that for and again keep in
mind your audience probably has no
exterior the first person that's
exposing them to this whole field



**Carlo Vicari:**
 yeah
because I guess I guess we did a nice
kind of gone through the whole thing we
did some some about the past then we
started talking about some stuff with
the current but I guess now we can
transition into
to how all of this functional
programming in Haskell and everything
you're working on translates into the
future of what we're all going to be
doing and interacting with different
programs and crypto and blockchain and
stuff like that 




**Christian Seberino:**
well well put 




**Carlo Vicari:**
yeah I'm
thinking to tackle but 




**Dr.Duncan Coutts:**
uh idea about
assurance and formal stuff and reading
things and so it starts from the premise
that programs are in principle
mathematical objects and can be reasoned
about using mathematics one which is a
bit of a radical idea because it's
basically impossible to reason about a C
program
I mean it's technically possible it's
just insanely difficult right you
wouldn't you wouldn't pick C if you were
trying to reason about things in a
mathematical way so yeah you have you
have programming languages which are
constructed in a mathematical style they
have a formal mathematical semantics
that means that means that they mean
something in a mathematical sense they
have a they have an explanation as to
what do they mean what value do they
compute and they have a way of
explaining that in terms of mathematics
which to a first approximation C doesn't
really have and then they're designed in
such a way that you have nice properties
and so then in principle the idea is
that because they're mathematical
objects you can reason about the
mathematically meaning that you can
prove things so for example I can say I
have this mathematical specification
which might be a specification in terms
of say set theory and logic in logical
properties expressed using the sets
whatnot
let's describe objects in your system
and you then you might express a
property about that and you might prove
that and then you might say well I'm
going to write this program and I want
to show on to prove that this program
implements this specification and then
you can in principle at least if you're
using a mathematical style of
specification and a mathematical style
of programming language or specification
language in principle you can write down
a proof that says that this program in
the
to the specification or you know more
commonly we do things like saying this
program is equal to that program meaning
this program will always produce the
same result as this program and that
turns out to be an extremely useful
thing to be able to do because you can
do things like saying well here's my
reference implementation which is really
simple and here's my real implementation
which is fast and complicated and I want
to prove that these two programs are
equal and that's a very powerful thing



**Christian Seberino:**
okay now which is is it is this true
today like let's say I was the
programmer for the Nasdaq and I wanted I
was going to write a program that
handled you know billions of financial
billions of dollars worth of
transactions every day is this happening
today that people will write software
and Haskell or something similar and
they they really prove it and so they
they know it's going to work and there's
no chance at all of any issues



**Dr.Duncan Coutts:**
 so the
dirty truth is that no not really
so let me sort of explain all the state
of the art here is so you've got these
languages like these functional
languages which come from this
mathematical addition where you can in
principle explain everything in terms of
mathematics but then you know in
practice people add in lots and lots and
lots of extra features which they don't
really bother explaining fully
mathematically hmm so you end up with
the real languages that people actually
use for programming and this includes
Haskell is the right there so at the
surface language is actually big and
complicated in the end even though like
kind of the pure core of Haskell is
completely explicable in the
mathematical formalism okay so the sort
of the slightly dirty truth is that we
have we still have kind of programming
languages constructed in a nice
mathematical way but they're not proof
systems so although you know you can
kind of on paper prove things about
Haskell programs or you can write some
tools that do it there's still kind of
gaps where you like is that do we have
we really nailed down everything whereas
on the other hand we have system which
which are specifically designed for
specification and proof
these are theorem provers or proof
assistants things like Isabel and those
are systems where the whole purpose is
to have a computer check absolutely
your proof is correct and helped you
through the management of developing
that proof azuz comes those kinds of
systems can absolutely reason with you
know 100% confidence about things but
those things are not quite programming
languages although they're very
programming like ish so at the moment
the sort of state of the art is it we
have a slight gap between systems which
are automatic and designed for proving
proving things about programs or about
specifications and then we have program
languages which are a very similar style
but they just have so many extra
features that you know they're not quite
you know we haven't quite nailed down
average set of everything do




**Christian Seberino:**
 you think
it's just a matter of time before this
the the two will meet and will people
can program and it'll automatically be
proved to be correct and we'll all live
happily ever after 




**Dr.Duncan Coutts:**
there's some
interesting things going on at the
moment which are sort of in that are
looking at that gap between a real
programming language that is constructed
in this mathematical way and proper
proof systems so there's a couple things
like there's a thing called liquid
Haskell which is a an enrichment of the
Haskell type system that lets you prove
much stronger properties in the hospital
type system that you prove and that lets
you automatically prove a lot of things
the system will do a lot of the proofs
for you when they're when they're boring
and easy large and boring and easy and
let you prove really tricky complicated
things when you have to do that so that
reasons about actual Haskell programs
not about you know something idealized
something else that that's that works
with real hospitals 



**Carlo Vicari:**
so I have a I have a
question that I think all the non
developers would like to know these
these are the types of questions that we
want to know about it's the year you
know 20xx you've got no red lights or
green lights no lights whatever there's
a you know auto pilot
you know self-driving cars and they just
kind of go through traffic because they
all sense GP you know all that types of
stuff whether it's drones or cars
whatever um is it functional programming
that's going to determine this type of
stuff that you know all these cars are
weaving in and out of each other
with extreme precision is
is this kind of like the playground for
functional programming you know 50 or
100 years from now 



**Dr.Duncan Coutts:**
we're gonna ingest
those you certainly could could use
functional programming for that sort of
thing along with appropriate reasoning
systems and items and because you want
there's various you know safety
properties you want to prove there
although that said I mean cars are a
very difficult situation because you've
got all these sensors with all this
noise it's hard to yeah there's only
certain bits that you can really reason
about mathematically there I mean this
um bit you have to just make
approximations right let's assume that
the input processing system does
recognize that thing as a another car
and that that's a very that part is a
very hard thing to right really specify
and reason about mathematically but you
know if you there's that there's
certainly parts of the system there that
you could formalize specify proof 




**Carlo Vicari:**
okay I
don't know about you guys but I take my
stand take my chances with a
self-driving car and sensors than all
the crazy people driving on the road now




**Dr.Duncan Coutts:**
yeah yeah what you don't have yeah
action to make to make it better than
that



**Carlo Vicari:**
 yeah I mean people talk about that
they're worried about the you know they
heard about a self-driving car having an
accident I'm like this after like two
million miles I know people they can't
get 10,000 miles without an accident
yeah I'll take I think that huh yeah
yeah so I'll definitely I'll definitely
take the car starting to derail the dev
talk but I was the yeah 



**Christian Seberino:**
okay so wait
wait so so just to be clear so we're not
at the stage where people listening
could could make a smart contract for a
blockchain and and then they can go find
somebody to guarantee that it's gonna
work exactly as intended so what 



**Dr.Duncan Coutts:**
oh no
one actually no that is a lot easier
interestingly yeah it turns out so to
what I was saying was about like cars
programming languages programming
languages for building big complicated
systems and Haskell is is a thing that
you can do for that
whereas a contract language is a much
smaller thing so a contract language can
be a much smaller simpler language it's
special-purpose and you may instruct
such language in a way that it has
it's really about it being simpler I
mean if Haskell were much simpler if we
stopped if we had stuck to the small
little core of Haskell then it would
have been much easier to build tools
that are able to reason about it in that
sort of mathematical way and with a
contract language that's exactly what
you can do so in principle if we
construct contract languages in the
right way nice we can either this one of
two approaches one is to design the
language so that it is less expressive
and and at the and that means that you
can't do absolutely everything in that
contract language but it's a hell of a
lot easier to reason about what you are
doing and another approach is to make a
kind of general-purpose language it can
still be a simple language but still
general purpose in the sense of this
chair and complete



**Carlo Vicari:**
 could you consume
potentially reason that someone is not
allowed to drain hundreds of millions of
dollars from a contract there mu good
there'd be a reason are you friggin
reasoning right 



**Dr.Duncan Coutts:**
so that's a property
that you would want to achieve and then
looking like my question there's two
ways to do that one is you use the
general-purpose language and then you
have to use like a proof system to prove
when your contract does this or doesn't
do that you know certain safety
properties or whatever whatever it is
want to say about what your contract
does or the other approach is to say
well let's actually use a less
expressive language where you can say
fewer things and then it's a lot easier
to reason about what it does and those
kinds of languages are not Turing
complete that means you can't express
absolutely everything in them but
they're even more special purpose and so
it's a lot easier to see what they're
doing and to be able say what they can
and cannot do 



**Carlo Vicari:**
I like it and I think
everybody listening likes that too
especially after what happened 






**Christian Seberino:**
ah it
sounds like what you're saying is as
this as smart contracts get more and
more complex that they will run into
issues they won't just they won't have
those guarantees only if they stick with
these simple in the sandbox the safe
sandbox right 






**Dr.Duncan Coutts:**
I think it's a kind of one
of these 8020 things you don't have to
use a single language for all your
contracts you can use a simpler safer
language for 80% of your contracts which
are in a relatively standard and even
those systems are very expressive
actually I mean there are those
languages for contracts which can
express basically all the kinds of
financial contracts that you'd ever want
to write people have been writing
systems using those for four years now
and those are really nice and simple but
you can't express you know crazy weird
scripted protocols with them okay and
then and then for the 20% that are you
know exotic or really exotic I mean I I
say exotic because people can do like
you know exotic financial contracts and
those are easy to express actually you
know you can express your CDOs and your
futures and your options and that
stuff's all easy but if you do want it
something really weird or really you
know what something this is goes a lot
of computation and 




**Carlo Vicari:**
when something is
strike really weird for those of us who
don't now which is me 



**Dr.Duncan Coutts:**
um well it is to
do with what kinds of things you can
express it's like if you have to have
communication through lots of people or
they all need to do some stuff some
non-standard crypto weirdness they need
to do some really interesting
computation rather than just like who
owes who what when



**Carlo Vicari:**
 right okay so so in
sound


**Dr.Duncan Coutts:**
 and you general-purpose
computation and that means also a proper
Turing complete language and then you
have a harder time reasoning about it



**Christian Seberino:**
and so the side effects right it's
although you all your examples



**Dr.Duncan Coutts:**
 not even
it's not even the side effects so all of
these all of all the things that you
think of as being programming languages
are what we call cheering complete
program languages which means every
possible thing that you can ever compute
can be computed in all of those
languages Turing complete is is is the
class of all things that can be computed
or a language and range and compute all
computable things whereas there are
languages which are not cheering
complete and that's what I mean by some
of these really interesting contract
languages are here's an example it's
you're familiar with SQL you might say
SQL is not a programming language but we
would say well actually it is kind of a
programming language it's just not a
Turing complete language you can't
express everything in it but the things
you can express you can express
succinctly and you can reason about them
which means you can optimize them that
that's a kind of trade-off so here see
with SQL SQL is not Turing complete you
can analyze it
you can optimize it C is Turing complete
it's hard to reason about it's hard to
compile but you can do everything with
it
well if I kind of trade off so from



**Christian Seberino:**
using Haskell isn't Haskell
turing-complete so there's



**Dr.Duncan Coutts:**
 absolutely
Haskell's general-purpose ensuring
complete so there's still differences
within turing-complete languages is it
you can't just say oh because it turned
complete you could everything I mean PHP
is during complete but you know you
would want to use it for anything




**Carlo Vicari:**
from what I now understand it kind of
sounds like you know into 8020 you were
talking about all the things that are
pretty simple to be able to UM do as far
as contracts is concerned like you said
the simple stuff is like who owes who
what and went so that's not an example
of something simple
anything's downright complex 



**Dr.Duncan Coutts:**
with that
but all your patient yeah yeah that's a
that's pretty decent Katrina right right
it expressed in that kind of who knows
what when a




**Carlo Vicari:**
nd something noses and and
when you said exotic it would be beyond
who owes who what when it's more like
who owes who what when but but but with
like a lot of different exceptions



**Dr.Duncan Coutts:**
 yes
if you wanted to in code playing chess
as a smaller contract that requires
general-purpose computation because you
have to express all of the the rules of
chess I'm Jane check the rules of chess
in that language and you can't you know
you you wouldn't imagine be able to do
that in SQL and similarly you wouldn't
imagine be able to do that in one of
these simple contract languages which
just describe you know under what
conditions do you gain assets hmm



**Carlo Vicari:**
who
knows who won and then there's who owes
who what when but but but but but
and the more butts there are the more
complexities in the more exotic it is





**Dr.Duncan Coutts:**
that's right yeah if you need if you
need to write complicated functions to
be able to tell
we know when when something is true or
not you need you know general-purpose
computation in those situations hmm 



**Christian Seberino:**
so
bringing it but but




**Dr.Duncan Coutts:**
 I just thought you
could get rid locker before far that and
that's why it's a kind of 80/20 thing




**Christian Seberino:**
got you now how what Duncan what would
you say to somebody listening that let's
say they want to make a blockchain based
Bank that's their startup dream and so
okay so you convinced them to do
functional programming and they also
want to do as much of this program
correctness the you know evidence get
get as much evidence as they can how
would you recommend they get started
practically specific steps not theory
but how they what's the one he recommend
to jump into this whole field





**Dr.Duncan Coutts:**
okay so there's there's two things one
is the languages that use and the other
is the techniques you use okay and so
there's a lot of training you've got to
do for yourself if you want to start
taking this approach and but it's all
really interesting actually that's the
other thing I mean the high school
people are already happy they like doing
this stuff it's actually really
fascinating and rewarding in the in
evolve itself so you need to start you
need to start with learning learning a
functional language and there's some
really good resources out there
I mean I'm particularly familiar with
all the Haskell ones but it was good
there's good resources other languages
and then the other stuff is the sort of
mathematical approach to specific
specification and proof and things so
you want to look into programming from
the specifications how do you what sort
of there are books out there on
mathematical styles of specification and
so it's a good a good starting point
might be if you're interested in there's
this dear improving stuff which I
mentioned earlier like Isabel is it is a
really good one there's another one
which has a name that the French made up
just to tease the English it's spelt coq
so it's pronounced in English cock ah
and so they obviously they they made
that just to make us you know say that
yeah the French laugh at us about that
which is nice
that's another fair improving system so
if you can read you know introduction
books to those systems and that get will
give you an idea of what does it mean to
specify things improve things


**Christian Seberino:**
 okay and
is there any specific websites or
specific authors that you're you're
really impressed with



**Dr.Duncan Coutts:**
 so if you're
starting with Haskell obviously there's
a house called a word website which has
just loads of resources and as for a
introductory book the one I tend to
recommend people start with if they've
never done any functional programming
before but are otherwise familiar with
programming is is a book called
programming in Haskell second edition is
out Graham Hutton it's a very short book
which is nice it's you know really
really comparatively very short and it
will teach you the essence of functional
programming using Haskell it's not it's
not about the tools and the practical
stuff you can get to that later and
there's other books that cover that but
it covers the core concepts really very
concisely so it's a good one to get
started with



**Carlo Vicari:**
 okay very nice
okay so I got I got one for you on
something I also like to talk about with
some of the guests on the show is uh you
know just technology in general what do
you what do you see on the horizon you
know 20 30 years down the road what's
your uh
utopia or conversely doomsday scenario
you know what what kind of crazy stuff
do you see as far as technology you know
and that in the distant future but not
too distant future 



**Dr.Duncan Coutts:**
well I can tell you
what I'd like to see



**Carlo Vicari:**
 that's good that
works too


**Dr.Duncan Coutts:**
I mean I I think functional programming
has becoming more and more and more
mainstream you can see it in the new
languages that are around and the
functional stuff that's being
incorporated into other mainstream
languages it's a complete 




**Carlo Vicari:**
man give me
some jettison stuff what do you see
what's good 






**Dr.Duncan Coutts:**
uh okay well I think there's
a long way that you could push things a
long way with this formal stuff and when
the tool when the tools are right
because we should be able to we have the
mathematical techniques but we should be
able to apply those with real programs
that have all the real-world complexity
and there's they're tools that are
coming along at the moment but I think
you know you can see that going a lot
further there's there's a big area
within the sort of functional
programming Haskell world called
dependent types
it's a doing even more stuff with type
systems which in some ways is again
about being able to read more things
with types prove more properties about
your programs with types which helps you
which isn't necessarily that's about
proving the whole thing just proving
certain certain aspects about about
programs 




**Carlo Vicari:**
um in 30 years are you visiting
us in the United States travel
by Hyperloop with using Haskell or high
assurance software as is happening on
the Elon Musk Hyperloop 




**Dr.Duncan Coutts:**
yeah I don't
know it yeah there is still there's
still this difficulty I think in getting
people to switch I think it may well be
that that they end up converging a lot
closer but I it may it may never be that
the mainstream switches to pure
functional programming I suspect that
the mainstream will converge on a sort
of hybrid you know imperative functional
and then win right because there aren't
there are various practical reasons for
that it and it you can get there
incrementally whereas this this switch
to purity although it gains you so much
it is a it is a there is a big switching
cost there and so I'm not I'm not
convinced that people that will ever
become mainstream but it could be good
for the you know like the dominant
language like like Java is now um well I
think inviting pretty good it's good for
yeah right but it could for higher and
stuff I think 




**Christian Seberino:**
now wait if it's yours
money involved then people of course
will do anything if it'll get bit make
their business grow so can you give us a
use case where the hundred percent pure
Haskell functional 




**Dr.Duncan Coutts:**
well this this is
really a social problem so the reason
that the reason that we're not all using
high assurance software is not because
of the technology it's not because we
don't know how to do it or because the
tools aren't there the tools would be
there if we were doing it if there was
it's because um people who make software
unfortunately are not held accountable
for the consequently their software so
you know people go for a quick just good
enough quick time-to-market so people
use Haskell in that sort of circumstance
as well without without doing any kind
of a harsher and stuff and that's the
main way the Haskell still is used is
just doing things quicker and you know a
bit better um but you know that you
they're not using the trade-off to
obtain vastly higher quality or really
high assurance and allows really and
that's really a social economic problem
so I
I think unfortunately unfortunately it
will require the Hyperloop crashing
killing people before before people will
switch will will will say no actually
software developers really have to be
held accountable for this stuff like
engineers are so the example I like to
give is that in the 19th century people
were building steam boilers for various
things you know steam boilers in the
basements of buildings in New York and
whatnot and from time to time these
would just blow up and kill people
because engineering was an unregulated
profession anyone can call themselves an
engineer you didn't have to show any
calculations when you made your steam
boiler but if one blows up
it's like a bomb I mean it will it will
kill people and destroy buildings and I
think with salt with software we're kind
of in that pre regulation environment
yeah you're right anyone anyone can just
and and what happened with the engineers
was that after enough boilers blew up
and killed enough people the government
stepped in and said look this isn't we
can't do we can't carry on like this
this is crazy we need to we need to
regulate the engineering profession so
they're not so beholden to commercial
pressures we need to say well you know
you have to have a sign-off from an
engineer who gives their professional
stamp of its on their professional
reputation that this steam boiler
whatever it or this bridge or you know
is is up to scratch and you can't they
can't be overruled by my son middle
manager who says look look the ridge is
done it doesn't matter we're moving up
the engineer has to have the sign-off
and the engineer has to say yeah no
really this and then the plans are
lodged you know somewhere and and
they're held accountable and future if
they got it wrong okay and we're not in
an environment yet and if we ever get to
that you hire assurance software will be
everywhere everywhere and then and then
the tools will be great because they'll
be in it all the money will be in 




**Carlo Vicari:**
it I
see h3 so how about in general besides
the high assurance software Hyperloop
from UK to California doesn't exist 30
years 





**Dr.Duncan Coutts:**
well you have a few problems about
you know undersea volcanoes and yeah
with Atlantic Ridge work




**Carlo Vicari:**
New York to New York teller from the
north you came to South UK 




**Dr.Duncan Coutts:**
it's taking
us like 30 years to build a high-speed
rail from London to Birmingham 




**Carlo Vicari:**
so we'll
go with and now and now




**Dr.Duncan Coutts:**
 I think I didn't
find it like do it before before we do



**Carlo Vicari:**
ah there you go
I can't sure that's true how about so we
got the Jetsons Jetson stuff from you oh
well I actually have I haven't drawn
today flying around in 30 years where
you think




**Dr.Duncan Coutts:**
 I have no particular insight I
imagine I imagined so yeah and hopefully
they're not crashing into each other
because yeah because yeah using the
right algorithms and autonomously
sensing each other and 




**Carlo Vicari:**
yeah yeah well
after if you blow up then some
regulation will come in and then they'll
fly properly hopefully um 



**Dr.Duncan Coutts:**
yeah a
certified or something you're



**Carlo Vicari:**
 right
certify we can 



**Dr.Duncan Coutts:**
actually no seriously
people are writing dsls for aircraft
control software in Haskell where you
can reason about their you know
real-time performance and blah blah blah
and that's because right those are
systems where their life lives depend on
it
this isn't like just drones this is
right aircraft control software that has
humans in it or where if it crashes it
could kill someone 




**Christian Seberino:**
so these are doing
that so just in case people don't know
so DSL is a domains 



**Dr.Duncan Coutts:**
domain specific
language so when we were talking earlier
about like contract DSL or SQL being a
DSL these are all yeah special languages
for a particular problem domain 




**Christian Seberino:**
so this
has to have tools does it have tools to
for people to say look I'm an
intentionally crook in my language or
only use this subset to make my DSL see
them saying 





**Dr.Duncan Coutts:**
you don't do it by crippling
you do it by encoding but but yes you
can ask all is a really good language
for encoding yourselves for writing
conventions and languages that are
embedded within Haskell
it's a very powerful approach it's used
all over the place with others



**Carlo Vicari:**
 we get we
get some jets and stuff from you now how
about a more a little bit less
technology specific with some non or
personal stuff your your reading or
stuff you're interested in shows what
what's going on and I know you're pretty
busy
you guys doing a million different
things but is there any thing you
recommend our readers reading that you
read in the past fiction nonfiction




**Christian Seberino:**
 oh
how do you feel about brexit let's throw
that 






**Dr.Duncan Coutts:**
uh-oh I think it's terrible but
then I'm in the you know the the liberal
London elite 20 rest of the country okay
so they I would I would think that
wouldn't 



**Carlo Vicari:**
I oh I'll say this to anybody
listening I had a pretty long I was in
in Malta with Duncan we had a great time
and I had a pretty long discussion with
him which I totally disagreed with him
for like two hours
hahaha about this is about certain like
aspects of inflation versus deflation
and then I had like oh well the Tribuna
you know credit where credit's due I had
like a Eureka moment like four hours
later when I was back at my hotel room I
said oh god he's so smart he's right um
so we'll get into that another day but I
had a table I had to crawl back to
doctor dr. Koontz the next baby like uh
yes you remember the argument we had
last night
you were right so there was some
interesting stuff and we'll get a chance





**Dr.Duncan Coutts:**
to actually it's a fascinating thing
coming into this this community because
you know I come from like the that's or
the functional programming community and
answer this community you know I see it
as a you know it's another is another
little community in a similar way but
they have interesting different views
and there's the politically there's a
lot you know the libertarianism is is
really big within the the crypto
cryptocurrency world which is to me you
know fascinating and so you know going
going to Malta and going to this crypto
finance conference and meeting all these
people was actually really interesting
to sort of talk about all that stuff and
I was doing a little bit of basing I
suppose you know being being contrary
and putting opposite view just 



**Carlo Vicari:**
no no it
was good it was good it was good but 


**Dr.Duncan Coutts:**
it
was really it was really interesting and
to just sort of pull out some of the
interesting arguments there




**Carlo Vicari:**
 I definitely
like to have you on again so we could
talk more about um the one discussion we
had about inflation and deflation versus
GDP and setting the currency to a
certain rate
it was pretty involved in and I'm sure
you know I should point out 






**Dr.Duncan Coutts:**
I'm only
like an armchair
macroeconomist I mean you you talked to
a real macroeconomist that 



**Carlo Vicari:**
was some good
arm cheering oh that was really good
there's better arm caring than I've ever
done so 




**Christian Seberino:**
so have you um have we covered
most of what people do you think need to
hear that are that are new to functional
programming and secure smart contracts
did I miss anything or anything else you
want to say Duncan 







**Dr.Duncan Coutts:**
um that comes quite a
lot I mean we could talk a little bit
about what IO HK is doing with this
stuff okay okay yeah you know I have to
be a little bit careful to not
preemptive you know public announcements
and things cuz I'm you know I'm not the
marketing department I'm just ah I can
just attack one of the tech guys you
think 



**Carlo Vicari:**
let's uh let's let's be careful
and not do that we'll just say that IO
HK is doing some awesome stuff with
functional programming Haskell and Scala
and they've got you know Cardno doing
some great stuff and also the grow deep
team using Scala uh but let's do that
rather than not again trouble you know



**Dr.Duncan Coutts:**
okay sure sure




**Christian Seberino:**
yeah good so so if I could let me see if
I could summarize just for the the
listener so the reason we didn't all use
functional programming from beginning
was we initially historically they mimic
the hardware and 




**Dr.Duncan Coutts:**
yeah we programmed
computers like engineers do that all the
rather than like computer scientists




**Christian Seberino:**
that's right and then also so it's it to
remove one of the barriers it's not that
it's intrinsically harder like you said
it's just the historical way turned out
historically that's why people don't use
functional but if you're if you're smart
and you want to give your company an
edge then there's no reason why you
might not want to jump into that and
then you also said that libraries is one
reason why they might not go 100% pure
functional that that was a concern and
why people might use a hybrid language
like skaila and then you said as far as
secure provably secure we can't quite
we're not there yet the holy grail isn't
there or we could prove everything




**Dr.Duncan Coutts:**
 yes
although i think i think we didn't want
a really how far you can get already
which is actually pretty far
okay which which maybe is worth talking
about I was sort of talking about the
remaining gaps but actually you can get
a long way by using a combination of
tools at the moment what I do with you



**Carlo Vicari:**
 I
actually um I think you were being a
little bit modest in reference to what
you can and can't talk about for I ohk
because you're like you know hyper
knowledgeable about all this stuff so I
I don't think the marketing departments
gonna freak out too much why don't you
tell everybody kind of what your you're
working on the stuff that's going on
with IOH case specifically with
functional programming 



**Dr.Duncan Coutts:**
sure so the
interesting the thing that's really
interesting to me is I go to yeah coming
in coming in to help I ohk is that they
have the ambition to do high assurance
software which actually is very rare
when I said you know people typically
take this sort of commercial approach of
just build it as quickly as possible and
so although I was trained at university
with all this sort of formal stuff
actually most of my customers have never
asked us to do that kind of thing and so
this is what's really nice actually that
working with our educator they have this
ambition to and so we're starting on the
on the on the on the road to to
producing higher assurance software I
should be clear that you know we're not
going to achieve the kind of pinnacle of
absolute proofs of everything but it
should or it ought to be if we're going
the direction we're going a hell of a
lot higher assurance than anything else
out there in the in the cryptocurrency
space at the moment so 




**Carlo Vicari:**
so - - for people
like me the non developers of the world
it kind of sounds like everybody else
are the engineers blowing up the what
was it in the basements the 


**Dr.Duncan Coutts:**
steam
boilers yeah


**Carlo Vicari:**
 everyone else is like the
the engineers blowing up the steam
boilers in the basements and IOH gays
doing the more modern engineering
techniques with people signing off on
all sorts of important stuff right



**Dr.Duncan Coutts:**
 yeah
in some sense we're doing both we're
doing something that is out quickly but
also going and doing it properly but
they're doing it properly will take
longer but but ultimately we will be
able to get that higher level of
assurance gotcha 


**Christian Seberino:**
okay very nice all



**Carlo Vicari:**
right um
well I mean it's been a pleasure to have
you on here it's great to speak to you
again especially after having a great
time with you in Malta the financial
cryptography conference and I'd love to
have you on again and we can maybe get
into some more of your macroeconomics
arm-chair stuff cool and uh you know
great to be able to be doing the show on
a regular basis again Christian uh you
know 


**Christian Seberino:**
yeah thanks


**Carlo Vicari:**
 thanks for having all
the the good questions the stuff that I
don't know yeah 


**Dr.Duncan Coutts:**
yeah very much did good



**Carlo Vicari:**
yeah absolutely so a great speak to you
guys again for everybody listening out
there thanks for joining us and we'll
look forward to tuning in next week take
care guys



**Christian Seberino:**
 if you are passionate about
anything related to a theory of plastic
and you have something to say we'd love
to discuss that with you on the show
we're always looking for interesting
guests
yes

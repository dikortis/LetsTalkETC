# Let's Talk ETC: Manuel Sabin - Proof Of USEFUL Work Systems.
Christian Seberino:
hello everyone and welcome to another
episode of let's talk et Cie where we
discuss technologies and issues related
to aetherium classic as you know there's
a lot of great research going on on
blockchain regarding Bitcoin etherium a
Syrian classic and lots of other
cryptocurrencies and today we have one
of those innovators who we are going to
talk to today I have with me
Manuel Saban he is a PhD student at the
University of California at Berkeley and
so he's going to be discussing his his
work so Manuel why don't you introduce
once you tell tell a little bit about
yourself how you got into this




Manuel Sabin:
 sure okay
so yeah I am on well doing my PhD at
Berkeley and um how did I get into this
so I'm coming more from the theoretical
computer science side of things I like
to study 



Christian Seberino:
sigh speech even is x-ray



Manuel Sabin:
 yeah
yes computer science PhD and I like to
study the hardness of problems
how hard were things and we've recently
been working kind of on this new area of
hardness that is related to much more
practical problems and at some point we
realized hey we can leverage this
hardness to get proofs of work because
proofs are work like in Bitcoin or
blockchain require some amount of work
being expended and so that's how I got
into the kind of Bitcoin world is
through proofs of work mainly by
studying hardness of problem 



Christian Seberino:
and when
you say hardness are you talking about
like complexity theory big o-notation



Manuel Sabin:
exactly others are the type of hard
different parts 




Christian Seberino:
alright so for the
people that don't know there's ways to
measure the difficulty how long it takes
to to run a program
and how it's related to the problem
sighs the input size and any this is you
ever have dreams of solving with the
million dollar problem P is not equal NP
or any comment on that 




Manuel Sabin:
um you know I
could have dreams of making progress
towards that but there's well-studied
barriers to achieving that dream goal



Christian Seberino:
okay so I I know that a lot of problems
are they they they can't be solved and I
was talking to a computer science
professor when I was getting my PhD
mm-hmm and he said he didn't think that
the P equals NP problem was one of those
that was unsolvable he said or he had a
feeling it just felt like one of those
problems that could be solved so then
ever since he said that I've been
waiting for somebody to publish you know
we are times to sit it's been solved 




Manuel Sabin:
oh
yeah there's there's no real reason to
believe that it should not be solvable
but there are very strong reasons why
our current techniques will need to be
drastically different that our current
technique for proving things are not
sufficient for tackling P versus NP




Christian Seberino:
 okay
and if I if I understand correctly it is
not possible to it's either not easy or
not possible period to prove certain
things have a minimum minimum difficulty
it is that correct that's a professor
concern regarding computer security in
factoring 



Manuel Sabin:
sure so it's not impossible
it's very difficult though it seems our
results unconditional results saying
that this problem is really hard have
not been abundant according 




Christian Seberino:
now before
we get into the details of your your
work I'm curious what was just I like to
find out a little bit more about
people's history so tell me when you
first heard about Bitcoin and blockchain
what was your impression did you think
this is a house of cards and it was
crazy
where they work or what was your
thoughts on that let's see 




Manuel Sabin:
so the first
time I heard of it I was a more studying
kind of theoretical side of cryptography
and this was something that was kind of
off to the side it was much more
practical and I went to some talks on it
and it seemed so yeah it's a really
interesting idea crypto currency in
general is a very neat idea it wasn't
quite the flavor of things I like
proving as in the priests were currently
used are namely based on hashes right
it's a very kind of there's not much to
prove on it and you you create a clever
system and show that that system works
well and that's that was really
interesting to hear about but there's
not many places for proof in the current
framework so I I thought it was
interesting but it wasn't something I
followed closely 



Christian Seberino:
ok ok and so now so why
don't you then now describe for the
audience and is first well why don't we
start out this way in the simplest terms
possible the very general description of
what you're working on



Manuel Sabin:
sure so for proofs at work like in
blockchain and Bitcoin are a way to
enforce that people can't rewrite
history really as in Bitcoin we have
this blockchain which describes all
transactions of money being passed back
and forth in this kind of public forum
this public ledger and proofs of work
ensure that people can't rewrite history
by just lying and saying that this
change actually happened when it didn't
unless they have the majority of
computational power
proof-of-work ensures that someone
expended some amount of work when they
make a statement that this transaction
happen and if they're trying to lie they
would have to have an enormous amount of
power to do an enormous amount of
crucial work yes the problem with this
though is that these proofs of work are
typically the work being done is useless
that is its only purpose is to show that
work was done what our work does and
what our paper titled is proofs of
useful work that is we give proofs of
work whose work is actually useful
toward useful towards some practical
problem 



Christian Seberino:
okay so that's that's
interesting to me because so it hurts so
proof of work at first for me was was
kind of odd because you're intentionally
wanting to make something difficult


Manuel Sabin:
 yeah



Christian Seberino:
and and so and on top of that to add
insult to injury they they make
something difficult by doing something
that's pointless essentially and so your
so then you're suggesting we could
leverage all of that wasted energy
computation to do something useful can
you give and of course that makes a lot
of sense can you give an idea an example
of the type of useful work that might be
a a good match




Manuel Sabin:
 sure so um the hardness
we get the hardness from so sorry much
like cryptography we get so much like
cryptography we base our hardness on
well studied mathematical problems and
these problems are so encrypted Rafi
sometimes you have problems like
factoring this cryptography
is secure as long as factoring is hard
there's a kind of newer emerging branch
of complexity theory called fine-grained
complexity theory that studies the exact
hardness of practical problems as in it
takes and it takes quadratic time
instead of cubic time
type of thing and we are able to base
our hardness off of quite a few of these
problems and why is this interesting
well because a lots of problems can be
rewritten as one of these problems so
for example one problem can be given a
graph and when I say graph I mean a like
a social network you have a bunch of
nodes and edges connecting them so like
the web of how people are connected
socially on say Facebook and you may
want to know if in that graph there's a
set of I don't know say 2000 people that
all know each other you're trying to
detect communities report so this is a
type of problem that amenable to our
framework okay or okay yeah or also like
if you have a network of roads you have
points being the cities and you have
edges being the roads and you want to
find the shortest path between two
points then this is again another
problem that kind of fits our framework





Christian Seberino:
okay now I could imagine a few people
here and they're having a calculation a
problem like that and then they take the
time to set it up so that it could be
clearly executed on a computer but there
enough is there a constant demand you
know seven days a week for that type of
work that it could be a block chain
could to process that continually




Manuel Sabin:
 sure
so what our framework has been is namely
there's three main islands in the
fine-grained complexity world and what's
been kind of rich about them in the
of them is that many problems can be
rewritten as one of those three problems
so I'm giving examples about road
networks or these graphs of social
networks but really this kind of rich
framework of work showing that a large a
large class of problems can be rewritten
as one of these three



Christian Seberino:
 okay and might
remind people of the correct me if I'm
wrong with np-hard and a lot of yeah if
you're an industry and there's a year
you're trying to solve your specific
little nish problem and you think oh my
gosh I'm not sure that there's even a
simple solution to this you can what
they commonly do is show that it's
equivalent to a more famous np-hard
problem like the Traveling Salesman
problem and and then once you do that
it's that pretty much you know does it
increases people people's confidence
that there's no simple solution and so
there's a lot of these equivalent
problems is it kind of related to that




Manuel Sabin:
it's very related to that so that's
exactly the idea so when you talk about
something being np-hard you're saying
that a lot of problems reduced to it and
unless all of those problems become easy
that yeah so if a problem is np-hard
it's going to be very hard because it
just hearted all the problems that
reduce to it yes is it is the point so
similarly we have these problems being
hard in a sense as in when I say there's
a rich framework of research supporting
these problems I'm saying there's been
research supporting their hardness and
then there's been for for some of our
problems many problems reduce to those
problems and in one way that's nail in
the coffin like you said as in oh now
this problem is really hard because we
give evidence to it being hard by having
all these problems reduce to it yeah on
the other hand though
problems aren't that hard when we talked
about fine grained complexity we talked
about say cubic time or or that nature
so even though it gives evidence to this
problem actually taking cubic time on
the algorithmic side that means if you
have any problem you can rewrite it as
it and now you have a proof of useful
work 



Christian Seberino:
okay so just so that I just for
people that are listening that maybe
don't know the terminology so computer
scientists get again correct me if I'm
wrong cuz you're the expert
so if like you're talking about
processing or analyzing the Facebook
network right and so yeah if you want to
solve a problem with involving let's say
ten people and then if you want to solve
a problem with involving twenty people
so you doubled your problem size yeah
when we say it's when you say it's
quadratic cubic what you mean is that so
you double it so then it becomes four
times harder if you square that the two
or a now and so just because you
increase it by a certain amount doesn't
mean that difficulty increases by the
same amount it could get more difficult
and so and so if it's if you just so
this is going to get a little nasty so
if you raise it to an exponent and
that's called polynomial time and but
then that's that's already difficult
enough but then people they talk about
exponential growth yeah and then that's
the really bad really difficult
situations and so you're saying that
even you're saying the polynomial what
you cubic quadratic that data is
manageable for a lot of cases that's
right



Manuel Sabin:
 yeah not only manageable but this
is exactly what we want out of a proof
of work we want to proof of work to be
able to be done within a reasonable
amount of time so that you can have a
blockchain but not any faster 



Christian Seberino:
so
that's right because you okay going back
to what you said we intentionally want
it to be difficult 



Manuel Sabin:
exactly exactly so
when I say something is cubic computable
or something that's exactly what you
were saying is if I give you something
with ten nodes and it'll take ten cubed
amount of time the point of this thing
though if I want to have a proof-of-work
want people to prove to me that they've
done work I can kind of set how hard the
problem should be based on and to the
three as opposed to enter the four sorry
n is the input size the input size cubed
or input size to the fourth power that
kind of tells me how hard I want to make
this problem and you can kind of show
you can set how hard you want the
problem to be but also sorry yeah so
yeah yeah




Christian Seberino:
I'm thinking so when I too have a
usefully research that involves
supercomputers and so everybody from
there was a network of supercomputers it
was the National Science Foundation was
the management managers and people would
submit jobs to a queue and then you'd
have to we'd see your place in the queue
and wait for your job to run and
sometimes there'd be a lot of people
wanting to run jobs and sometimes it was
the queue wasn't so full so would it
work something like that so the
blockchain would have a queue and people
all over the world would submit their
their tasks to it and then and that's
how it could be continually it could
stay busy and do useful work for people
that what you're imagining something
like that




Manuel Sabin:
 sure sure so we haven't
created a blockchain scheme specifically
but we do propose something very similar
to that in in our paper so yeah the idea
would be you especially for something as
robust as a cryptocurrency where there's
large communities around it
you should have many people always
meeting poops at work and the idea would
be exactly as you said to have a queue
of problems where okay I need up I have
a problem that can need to be solved so
what do you do you try to you see if
your problem can be written as a problem
that we have a proof of useful work for
and based on the fact that many of these
problems are robust in that in that many
problems can be reduced to them
hopefully you can so first you have a
problem you rewrite it as one of ours
and then you just put it in the queue
and when someone needs a proof of work
needs to compute a proof of work combine
a block in the blockchain they'll just
grab one of your problems from the queue
do a proof of work for it so now they
have a proof of work as you would need
in the blockchain but their proof of
work also encodes your answer in a very
efficiently recoverable way 




Christian Seberino:
okay yes now
so theoretically the ID ideas sound
great now as you know in the real world
then you get all kinds of Joker's trying
to our system and so I mean I'm trying
to think of ways because that that's
what anybody that wants to introduce
your ideas into their new altcoin their
blockchain mature question they're going
to have is you know how or what are the
vulnerabilities so one question one
thought that just came to mind was what
if I get submitting the same task over
and over again and I I know the answer
could write like I sure worked it at one
time and then I could keep getting
rewarded for doing the same work over
and over again I for 



Manuel Sabin:
exactly so what a
poof of useful work should do is for
every possible instance it should
generate a random challenge based on
that instance of a problem and that
random challenge should be hard on
average most every time that instance
should be hard and this is
similar to the cash based poops at work
sometimes it's like a lottery sometimes
you'll stumble on the correct answer
really quickly sometimes they could take
as long as the proof-of-work should pay
and the main point is though that we
inject randomness into the proof of
useful work so if someone keeps putting
the same the same instance in there that
won't make it any easier because each
time you have that instance you have a
randomly generated challenge and that
challenge will be hard even if you give
the same instance every time 



Christian Seberino:
okay
okay so and then that would be that
would help with the security okay
understeer 



Manuel Sabin:
oh and also the randomness is
really generated based on the contents
of your block so if you try to alter a
transaction that would change the random
instance that you need us all okay and
invalidate any other proof of work sorry




Christian Seberino:
and who is who are the people that
submit the work to be done oh 



Manuel Sabin:
sure at
this point um we I don't see a reason
why it couldn't be anyone okay as in you
like you said you have a queue and then
people just submit to that queue when
people want to implement a proofs of
useful work they can kind of decide how
they want the ordering of that queue to
be if there's a payment system a voting
system but that's more kind of on top of
the existing blockchain 



Christian Seberino:
wait here's what
I'm getting at so like in a Syrian
classic the miners provide a service
they they they solve this difficult
problem which is allows blocks to be
added to the blockchain but now what
would be the like thus here the etherium
community wouldn't just or any
blockchain wouldn't just want to solve
my my problems
you know do my work to make me short so
they somehow it has to benefit the
blockchain the cryptocurrency
see what I'm saying so it couldn't be
random people submitting work it would
so you said I'm getting at so how is it
going to benefit the blockchain
community and






Manuel Sabin:
 so let me make sure I
understand what you're saying so 




Christian Seberino:
so I I
agree that there's lots of useful work
in the world that could be done tried by
the miners these computers but I guess
I'm what would be the benefit okay
here's a hit look but this way here what
would be the benefit to a blockchain for
being altruistic and saying you know
what we don't just want to do this
useful work we're going to help we're
going to help all these people at
Berkeley in India we're going to just
help them by doing all this they're a
little bit of their work form what do
they get out of it 


Manuel Sabin:
the miners whether
they're miners get out of it um




Christian Seberino:
 what is
a community that why would they want to
give their funds for these people doing
their this other useful work code speak
it's because it's not useful to the
blockchain to do all that useful work
it's useful to whoever submitted the job




Manuel Sabin:
sure this is true so the the blockchain
folk simply need to have instances to do
work on if for some reason they want to
collude and say okay let's only choose
instances that come from this company or
from this country or this what-have-you
then they could do that if you'd want to
if you'd want to come combat that if you
want to make sure every every instance
is treated equally that would have to be
a separate system that kind of lays on
top of blockchain and that would be
maybe incentive base where the people
that delegate the work word pay or maybe
maybe so the whole the great nice thing
about blockchain is it's decentralized
right that's its main importance and
that's because you don't want to trust
someone
your money yeah that aside delegating
work this again lays on top of
blockchain it doesn't really affect how
centralized or decentralized blockchain
is lock chain can continue to be
entirely decentralized and it be an
entirely separate matter if there's more
of a centralized system that creates a
queue yes in that sense people still
have don't need to trust anyone with
their money or their transactions they
can still do their poops to work per
usual but if you wanted a more
centralized queue you could do that to
enforce a notion of fairness of who gets
who what incidents of problems are being
dealt out and that would not affect in
any way the decentralized notion of
money



Christian Seberino:
 yeah if if anybody was worried
about centralization due to a queue I'm
sure somebody could develop a
decentralized queue that hmm synced with
all the nodes somehow 



Manuel Sabin:
exactly so that'd
be more kind of a separate issue than
what the proof of useful work offers



Christian Seberino:
yeah so it sounds if I understand you
correctly the it's it's it's just it's
altruistic if a blockchain decides to be
useful work
maybe literature live by 





Manuel Sabin:
a blockchain
needs to do some work and they need to
find out where those instances come from
so I guess you're saying it's altruistic
but the delegator czar doing a service
as well in the sense that they're giving
the blockchain people instances to do
proofs or work on because the blockchain
people would want to do poops of work
regardless either to mine coins from the
block or to just keep the blockchain
consistent so I guess I'm
that the miners will need instances to
do work on and the delegator is almost
providing a service in giving them
instances to do work on me 



Christian Seberino:
sure sure and
then another thing that something you
said that caught my attention you were
you're talking about for security
reasons having to add a random component
yes to the work but does that them that
seems to work against this notion that
we're going to help all these people
with their computational problems
because if I if I come to the system and
say okay I have this specific
calculation I need done then your system
is going to insist right adding this
randomness killing here I'm going to say
well wait wait a minute I don't care
about that I got to get this specific
problem done you're not helping me if
you're going to now dictate to me the
calculation the other thing 



Manuel Sabin:
yeah yeah
exactly so yeah a proof of useful work
should be two things it should be hard
so that it's a proof of work and it
should also be useful so that you can
delegate arbitrary instances and get the
solutions to those instances that you
want solve and it kind of seems at odds
just like you said
because we have a framework there's
always been kind of this notion of
delegation of computation where you can
delegate instances and get answers back
the problem with that though is that if
you can delegate any instance you want
sometimes those instances could be easy
so what you'd want is to like I said
randomize them but that seems to
completely break the tie with delegating
arbitrary instances in gingers that you
want so on what you have to do is you
create a random set of challenges for
each possible instance okay so given an
instant you have a random set of
challenges in solving any one of those
challenges we'll give you the instance
that you wanted okay and that's the
point is
even though you have this randomness the
randomness is based on the instance you
started where




Christian Seberino:
 okay so so it's up to the
person submitting the job to be done to
to characterize it in a way that is
compatible with your system where they
could inject randomness in it and you
still be happy with the results okay
that makes sense
and I as you were as you were explaining
it I just some ideas came to mind some
examples of work where there randomness
would be fine like for example if we
were trying to factor write a large
number and then your system would would
attempt write random random pieces of
the facespace the random numbers try to
factor and that would be fine right and
then the hope would be that by by luck
eventually one of those random choices
would lead to the answer and so that's
an example where you could inject
randomness and still be for work 



Manuel Sabin:
sure in
our case though so the framework is um
so there's no there's not luck really
involved in it we have it set up so that
if you solve this ramen challenge you
will be able to reconstruct quickly the
answer to your original problem 




Christian Seberino:
okay
okay yeah alright so if there's other it
other limitations so it's not that you
could run any computation you want there
would have to be it has because be able
to be constructed a specific layer 





Manuel Sabin:
sure
so this is not um a turing-complete
thing you can't do an arbitrary
computation that you want okay um this
is we have hardness based on a specific
set of problems that also have some nice
robustness characteristics as in many
problems can be written as them but you
have to fit within the framework of
those problems yeah and the framework we
give also leads to say that there's
probably many other problems that can
have this use property 


Christian Seberino:
yeah and then it
goes on they little become more and more
flexible while school exactly secure yes


Manuel Sabin:
exactly



Christian Seberino:
well it's certainly a great service that
year you're working on and what's the is
it still in the prototype stages are
there are there alt coins talking about
using this so stage





Manuel Sabin:
 it's still in the
theoretical stage in the sense that we
accomplished it in a in a paper but
there aren't there aren't
implementations of it yet okay
there are we are working on it with
someone to create yeah prototype
implementation of it
but what we have now is the definition
of what a proof of useful work should do
and how you could do that with practice
with yeah with a set of practical
problems that turned out to be quite
robust okay yeah and the hum and so and
before this it was not sure how this
possibly could be done it's been wanted
for a while to have proofs of work that
weren't entirely useless and there's
been some work such as prime coin or /
McCoy that finds some usefulness in a
very restricted set of in a very
restricted way of what you want to do
like you can find larger prime numbers
or better and this is just designing a
proof-of-work that specifically does
this you're not able to delegate
instances in this way 



Christian Seberino:
so I was ambitious
more general more ambitious than the
prime coin you're saying



Manuel Sabin:
 yeah yeah so so
this is meant to for the first time
capture what a proof of useful work
should be in the sense of a proof of
work that can delegate arbitrary
computations 




Christian Seberino:
yes now I don't this is a
different subject I know you're not
you're not an expert at it but I was
curious have you heard of proof of stake




Manuel Sabin:
I was looking that up
when uh yeah I was looking that up when
we started talking about doing this
interview



Christian Seberino:
 so so a lot of people have
been thinking is like you about they the
issue with all this useful a useless
work yeah on and so that was that was
another attempt to try to address that
that problem of those wasted resources
yeah but so 



Manuel Sabin:
so if I understand it a
proof of stake is a way to again keep
people from rewriting history in the
sense of you can't rewrite history
unless you have the majority of money in
the world but then what happens is you
layer computation on top of it and then
if you want usefulness correct me if I'm
wrong is instead of doing a proof of
work you skirt that issue by instead
introducing proof of stake and then just
have people do contract work out




Christian Seberino:
 yeah so
I'm I'm not prepared to give a okay
anchor description and also the
algorithms are evolving but but there I
just wanted you to just get your opinion
that there are there are other things
that people are trying to do we are
trying to make the work useful and other
people are trying to eliminate the work



Manuel Sabin:
exactly yeah there is so there are
things called proof of stake and there's
a poof of space as well where instead
you prove that you you you use a certain
amount of memory space and there are
ways to try to skirt the proof of work
issue by just avoiding work and proving
that you do something else and what we
try to do here is like say okay let's
keep poof of work but fix the
uselessness problem yeah and write this
as far as the proof of stake just a
comparison with that because from what I
understand with aetherium is that you
can contract out work and from my
understanding that's just work done on
top of the proof of stake just having
people do work
[Music]
what I'd want to say about ours our
proof of work is that the computation is
verifiable in the sense that the point
of delegating computation that the
usefulness part of our proof of useful
work is that computation should be
easily verifiable as in when I give you
an answer you should be able to verify
quickly that this is the correct answer
because you could just ask me a question
ask me some long question of like okay
what's the answer to this and I tell you
oh it's five and you could say okay Road
are you sure
and I say yeah yeah trust me and there's
no real way for you to check that the
correct answer is five unless you go
through and do the entire computation
yourself and you're like oh yeah five
words the correct answer 




Christian Seberino:
okay so now now
that obviously reminds everybody of the
NP right but non-deterministic
polynomial which is a terrible name but
yeah the analogy that I always use to
describe what you're saying that you can
easily verify a solution is so putting a
jigsaw puzzle together is is relatively
difficult but if I was to say look look
man well look I did it right yeah thank
you a few seconds to glance over so yes
definitely yeah I can I can verify that
solution so if some difficult problems
are very easily verifiable and like like
the pachinko so what you're


Manuel Sabin:
 exactly



Christian Seberino:
 what
you're saying is for this system to work
they have to be in a sense like what now
it is for the jigsaw puzzle verification




Manuel Sabin:
yeah exactly so my understanding of
aetherium right now is lots of people
have to do the same task if there's a
contracted thing if a task is contracted
out people have to many computers have
to do that task so that they can verify
that oh yeah that was the correct answer
whereas in our system only one person
has to do it
not each person has to do the task to
see that it's the correct answer only
one person has to do it along with a
very easily checkable proof like the
jigsaw puzzle when I give a proof of
useful work to be solved when someone
solves it it's much more like a jigsaw
puzzle than an arbitrary answer oh yeah
it's five trust me
it's something that like oh great that's
a solution I believe you because I can
see right there that's the correct
solution yeah yeah sorry



Christian Seberino:
 yeah so it's
exciting the times that we're living in
is all this innovation people are trying
different things in the blockchain space
right people are trying to make proof of
stake work and then you're trying proof
of useful work so it's I'm curious in
just a few years where all this momentum
is going to end up you know where we're
going to we're going to be like but
you're part of that helping to kind of
push humanity forward in a sense so I
yeah really appreciate what you're doing
so now you you've given a pretty good
description of what you what you're
working on is there anything else that
you want to communicate that I haven't
sure pointed out on an engine so



Manuel Sabin:
 okay so
one thing I should say is that my
co-authors are Marshall ball alone Rosen
and Prashant Vasudevan I just forgot to
say that so maybe that edited to the
beginning but but let's see other things
all right 



Christian Seberino:
well if we cover everything
that's fine too yeah anything else
all right well thank you for coming on
the show
thank you for describing your work and I
wish you best of luck all right thanks
Ron

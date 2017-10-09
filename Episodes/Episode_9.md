# Let's Talk ETC: Conversation With Alan McSherry.
Carlo Vicari:
hi everybody welcome to another episode
let's talk e.t.c I missed you guys the
last few weeks we haven't been able to
coordinate the show I've been over in
Japan for the time difference is a
little weird but we've got a really
special guest today and also I want to
fill you guys in on some stuff that's
been going on in the community in case
you guys haven't been following just a
lot of big news that's been going on I
just want to fill you guys in before we
start the show so if anyone out there
hasn't heard although i'm sure you have
about the e.t.c investment trust from
gray scale so that's pretty awesome
another big event that's coming up is
the epc athan which is set to take place
februari 24 to 26 and Shanghai and
another thing that I think everyone the
community should be aware about is the
white hat withdraw contract that's been
extended for two months so that's a
pretty important piece of information
for anybody that was interested in
what's going on with that withdraw
contract and the extension etc etc also
there was an AMA on a ptc recently that
featured avatar and splits and snap roll
and they were talking and answering
questions about some of the different
points on the monetary policy that's
being discussed in the community so
that's from the last newsletter that was
put out so we'll put that in the
description for anyone listening on
YouTube that will be in the description
of the video and on to the main point
for today's show which is we have a
special guest with us Alan McSherry
who's leading the groeten deke team on
the new scallop client for ET c which
this is a client built completely from
scratch and it's built in a functional
programming language and Alan is an
awesome guy doing a lot of great work
and it's great team and we're really
happy to have him here on the show to
talk about all the great stuff he's
doing Alan thanks for thanks for being
able to join us really appreciate it



Alan McSherry:
yeah no problem thanks for
so asking me on I was listening to some
of the stuff that you guys have done it
you know I really want to say thanks
from from from everybody else because
it's great it's a great service thanks a
lot 



Carlo Vicari:
yeah yeah I appreciate it i mean
really it's you know i always say it's a
you know it's the developers it's the
miners it's the other community members
as the investors we're just trying to
let everybody know about you know all
the great stuff like the entire
community and all the constituencies are
doing so thanks thanks for everything
you know everyone out there is done and
thanks for everything you've already
done in just such a short amount of time
so uh Alan I kind of went over this with
you but um something we do on the show
if it's someone's their first time on we
just kind of want to introduce them to
the community so that everyone out there
knows you know the great people that are
working on this project so why don't you
just give everybody a little bit of your
you know your background and kind of how
you got into the tech space and all that
good stuff 



Alan McSherry:
sure well I mean a lot of
people have these great stories but
starting off in physics and then you
know becoming getting into programs
because they needed a job but I actually
studied Computer Engineering and
university so I've always been intact i
guess in the last year we did a lot of
c++ and then i went to an american
company in four years there in the or
indeed apartment and worked on their web
projects and what sort of ended in the
in the first tech bubble so we have been
intact i guess since I yeah yeah it's a
bully 


Carlo Vicari:
right right but blockchain is
definitely a new to the if as new as
tech yet so how did you we call it the
blockchain rabbit hole like I guess that
everybody falls into so how'd you end up
getting into block chain from the
greater tech field i guess you could say




Alan McSherry:
yeah that was um I i I'm not sure
exactly how I became aware of Bitcoin
but I think like most people Bitcoin was
before
first port a call and I'd always had a I
mean I was never a big fan of the way
that banks operate in terms of central
banks and their control of the money
supply and the way that ordinary banks
issue credit that always kind of
bothered me so when I discovered the
Bitcoin monetary policy was or fixed set
in code and that you could do these
transactions across the internet and as
these had real value you know you
exchange interfered I was pretty much
hooked instantly yeah so close when he
when you think at first the bitcoin is
kind of where it is it's sort of at the
beginning in the end and I suppose in
the very beginning it was the beginning
in the end but it just exploded really
didn't I mean everything you know it was
master calling lose a ton of other stuff
that happened after that and I just I
just kept reading and devouring and
figuring out what was going on I tried
to get involved you know one of the
things that you discover I guess shortly
after you discover we have a distributed
currency is how do we how do we you know
how do i how do we do exchanges I mean
we still have that problem of not having
distributed exchanges so one of the
early one of the early attempts there
was the butter calling project so I
tried to kind of get involved in that
but that didn't really work out they
were writing all the code and coffee
script and I have to admit kind of kept
me back of it so so I asked from it was
a long time it was a long time interest
and then probably last year I started
working full time in the blockchain cold
and Scala was my language of choice and
husbands and I guess but 2013 and i came
across the score x framework yeah I
don't know if you wear the score
experiment but it's the it's a scala
based framework that externally has put
together now love it i was going to say




Carlo Vicari:
just to let you know so I
I'm aware of this stuff but that's why
Christian Christian is awesome because
he does all the the technicals on all
the stuff so I usually ask a couple of
the intro questions but a bulk of the
actual interesting questions come from
come from Christian since he's pretty
knowledgeable about all this stuff so we
would 



Christian Seberino:
say would you say score X is a
library that you use to make blockchain
with that with that accurate






Alan McSherry:
 yes
Couric's is an abstract framework I'd
say that you that you then build classes
using the abstract framework classes as
base classes to create your creature
blockchain okay at the time but I'm
talking about when I first came across
that it was it was score X 1 point you
know who scored very early version of
lady sure if it was 1.0 and now it's 4x2
you know 00 released cam that anyone
like that so in the early days well I
just I just have to manage us took some
classes and out of it and and use them
there was some really good networking
classes that were extremely useful and
also they had a great script Oh library
on which is which is they use it a
dependency and they release it it has
its own release cycle


Christian Seberino:
 so I used that as
well so presumably the the one of the
reasons that it exists is because maybe
forking the open-source Bitcoin code is
not necessarily the ideal perfect
solution for everybody that wants to try
some innovation in block chains and
somehow score X is more flexible more
secure nicer language than C++ that
correct 



Alan McSherry:
well I don't want to get into
any language worries here but yeah skala
you know Scala is a very very nice
language to to write code in it it's
quite it's very terse and you leverage a
lot of the you know a lot of the
libraries that are built for the for the
JVM but in terms of so in terms of score
X the difference i guess with a lot of
other
bases that you can quickly get to some
kind of running blockchain in a very
with a very small number of lines of
code so I mean if you look at you know
some of the code bases all right out
there for appearing or anything else
there are thousands and thousands of
thousands of lines of code I'm making
sure how many are in there but score X
is only about four or five thousand
length code so it's very manageable to
begin with 



Carlo Vicari:
now all of this with score X
this this is this segue you into ET c is
that correct i guess some just to
connect the audience with the ship you
went you know from bitcoin and block
chain and how did you get into ET c



Alan McSherry:
 well
from from meeting Alex and any man
talking to about corex I subsequently
met Charles and Niko's and got involved
with I ohk and from there this project
was coming up and they asked me would I
take care of it I said



Carlo Vicari:
 yeah yeah why
don't you for anyone in the audience
that hasn't been following as closely or
is just listening to this about
listening you know about it now or maybe
knows a little bit about the project but
isn't necessarily completely informed
why don't you tell them a little bit
about what you guys are building and
what you're currently working on for
three TC 



Alan McSherry:
sure um so II TC is an etherion
classic clients and it's built entirely
in Scala and where we're at at the
moment we have we have a team that's
distributed across the globe we have
some people in Argentina I'm normally in
Dublin but today I'm actually in Poland
or have just spent two days spoken to
the to the guys who normally work
distributed here in Poland and we all
got together and we did some
brainstorming about where we're out of
the project and some of the code
structure and how we're going to
continue and yeah I guess where we're at
they
is we started off looking at okay how
can we just connect to a client you know
an etherion classic client so the first
the first thing we try to do is just you
know stoop do a successful handshake and
so we might as well so we're able to
connect to the etherium network and then
the next step was okay well let's try
and let's try and download the
blockchain so that's that's pretty much
the phase that we're in at the moment is
where we're almost completed downloading
the blockchain and handling the
blockchain synchronization which
involves a significant part of the of
the project it also involves you know
using the Merkel Patricia tree and
getting your persistence right and I've
been able to you know success it's a
great thing about working with HTC is
actually let this be you test straight
away you know I mean you know straight
away if you've got it right because you
connect you can't get it you can't get
the blocks properly so so yeah we're
currently just finishing that up and we
started our ebn implementation so that
when you've got to block a block
consists of a bunch of transactions and
you need to run those transactions
through the etherium virtual machine
which will produce a space but different
from the state you had before you run
them through the ebm because that's the
second strand of of what we're working
on and that's that's probably about
twenty percent complete at this moment I
say go 



Christian Seberino:
ahead make your question to ask a
question Alan 


Alan McSherry:
yeah



Christian Seberino:
 for anybody that's
listening and is starting to be swayed
that hey maybe I should look into Scala
because maybe I want to help with what
Alan is doing can you give some more
convincing arguments y sub wife you
think people would be what it would
benefit them to learn Scala




Alan McSherry:
 yeah let's
do a language war I'm on board with that
let's do language 



Christian Seberino:
whoa we don't want to
criticize other languages but



Alan McSherry:
 no no no
we don't we won't put any other language
down but we can you can definitely talk
about why Scala is clearly the best
language or something 



Christian Seberino:
yeah okay I'll
just I'll just say right now I've heard
academics for the longest time say oh
yeah functional is the future but then
in the real world meaning in industry I
don't necessarily see functional taking
over and replacing PHP and C++ and Java
so if it's really the future when is the
future going to come so maybe you can
answer that question 





Alan McSherry:
well I mean you
know again we don't want to get into
arguments here but obviously scholars
the best language that's ever been
created and the fact and not only is it
future but it's the future's here yes
well don't decide I mean Scala is a is a
natural successor to to Java in many
ways so for developers who are out there
you know if they're I mean there's a
huge amount of Java developers out there
so for them to move to scala the
advantages are many cool one of the
first one being that it's roughly half
the piping so immediately you know it's
a much more expressive language but
secondly where java was object-oriented
to a certain extent and wasn't so
immutable so Java collection libraries
there they're mutable when you you alter
things in place which makes concurrency
and multi-threaded behavior a little bit
more tricky to to handle whereas skala
is naturally immutable so most of the
anna has a lot of immutable libraries
collections so it favors it favors it
much easier to multi-threaded code with
and i guess some of the other advanced
this is the other major advantage which
you know as you as you alluded to their
functional programming is so hot right
now and scala as well as allowing you to
write object-oriented code also allows
you to write a very functional cope
and the cool thing about a functional
code is that it's it's very its
side-effect free or timeless to a
certain extent so actually it is
timeless it is a it is side-effect free
so this means that it's you know when
you'd it's more testable as when you
when you test it and it does what it
does of those that's it so it's a it's
very popular now and rightly so but I
think the great thing about Scala is
that it does you know lend a hand to the
enormous amount of developers where
there who are not quite fully functional
yet and also even for even in a
functional environment it's good still
can have occasionally and you know the
ability to 22 ok and write some you know
side effect in code now 



Christian Seberino:
I've heard that
so Haskell of course is another famous
functional language but I've heard
people say that so Pascal is when you're
all in on functional and you're really
going to jump you know all the way its
whole body in the lake but then somehow
there's more Scala developers it's a
little bit gentler introduction and
easier to learn is that true 




Alan McSherry:
yeah
certainly the last point it is easier to
learn I don't it is a gentle yeah
everything there i think i'd agree with
a skylit ours at Kelly's is very much
full-body immersion in in functional
programming and functional programming
at you know get that's quite deep quite
quickly 


Christian Seberino:
ok so is there be any reason to
ever your team to ever do anything with
Haskell or do you think you could always
do everything you want with Scala then



Alan McSherry:
everything that we've looked at so far
can definitely be done with with Scala
ok yeah you know we've we've looked at
most parts of the system now and the
libraries that were using you know are
really giving us and we're really
leveraging some of the existing
libraries that are out there so I'm not
sure what the hostel ecosystem would
offer that would be better but for
example we're using rest ikat TCP
which is really I mean acha actors for a
start are a very nice concurrency model
that it takes a lot of the it takes a
lot of the confusion as multi-threaded
and reactive programming and then with
akka you also get acha tcp which allows
us to again in a very natural way
communicate over over a DGP 



Christian Seberino:
okay
interesting yeah what about what about
the people talk about when they want to
move a lot of money in a smart contract
they want the more security more
assurance that the contract is going to
behave as the smart contract as they
they think it should is there any you
make any comments on that are you
thinking about security and how to maybe
even make programs provably secure or
these certain components 


Alan McSherry:
yeah there's a
lot of talk and I'm doing a lot of
listening about in exactly that area now
from our from from the point of view I
guess of the release the beta we're
going to look at getting the codes
posited by security professionals first
of all and then in terms of provably you
know running code that's true will be
secure that's not that's still
aspirational in my mind at the moment we
don't have a concrete plan you know to
do that but I do know that that it
constantly comes up so I think that it's
probably something that will you know I
just can't say that we have a plan to do
that but i think is something in the
future we will have a plan to do that




Christian Seberino:
okay okay i always found the



Carlo Vicari:
 it's on the
planning for planning like walking



Alan McSherry:
exactly it's too they are in the future
to be able to say anything concrete
other than a lot of people believe it's
in the future 



Christian Seberino:
okay i know solidity i was
talking to some of their developers and
they're doing things like yeah a common
if they
common pattern that that leads to
security issues though they want to add
warnings right to things like that so
that's how they're dealing with it for I
know it's one way 



Alan McSherry:
yeah when we get to
you know at the moment what we're doing
is we're building out our re vm so it's
a case of getting the bear to dance at
all first of all and when we do that we
you know we look around at what at what
the state of the art is in terms of
security securing humble and you know we
will make sure that we're at least as
good if not better 



Christian Seberino:
ok can I believe I
believe I heard that the vm is very it
was made to be easy to understand it's
not very convoluted complex but it it's
pretty nice would you agree with that do



Alan McSherry:
you mean to the PM is designing in the
yellow paper 




Christian Seberino:
yes the how does it compare
to like the complexity of the JVM if you
can you compare those mate 



Alan McSherry:
oh yeah well
I mean one is is is more complex than
the other there's a fairly small
instruction set well 



Carlo Vicari:
i don't know
because i saw i saw on someone posted
like an infographic explaining the the
etherium yellow paper and its supposed
to like BB yellow paper for dummies and
it was really confusing for me could I
could it was there was a lot of
information so this especially you know
I've looked at the yellow paper a few
times and it's it's a bit much a bit
much for me but the infographic was
actually pretty cool maybe maybe we'll
put that in the the description on
YouTube yeah Christian or anyone to
check that out I have that I have that
link saved somewhere it's actually
pretty interesting ok



Alan McSherry:
 yeah when we
insist on that paper you know that is I
think probably everybody's first
reaction when they start reading that
you know it's tough to get through and
of course we this
reroll but I mean all of the developers
have have read it you know several times
and its really i was talking to what
happened today and i was just saying I
think notice that the you know the
papers starting to make a huge amount
more sense you know you can kind of read
it almost naturally now and as far as
nodding vigorously so it it is dance in
the beginning but you know over time it
does seem to come cloud and become
become far more care 


Carlo Vicari:
yeah like the fog
the more you've been working on the
project of the fog starts to clear i
guess in a sense 


Alan McSherry:
yeah exactly exactly
and and then it that's kind of exciting
you know when when you start to when we
start to read what was originally looked
a little bit like gobbledygook and
you're reading to go like alia yeah yeah
that make sense yeah



Carlo Vicari:
 yeah that's true
that's true yeah we were actually
talking about this before the show
started christian he was telling me
about how the more that they they've
been working in the project there they
just start to see bits and pieces for
what they really are and you know it's
like learning another language
essentially okay you know the difference
between looking at a bunch of letters
and actually being able to read what's
on the page i suppose in a sense
although put over oversimplification but
you know what i mean



Alan McSherry:
 no i think that's a
very good analogy actually that is that
is kind of what it's like at first it's
tiring because you're reading it you're
going like what what and then and then
as you say one day you're reading to go
like oh yeah I guess 



Christian Seberino:
yeah right i think
i think the natural probably a lot of
people there what they do is they don't
find something they don't understand
like blue filters so then they learn
that come back a month later read it and
they'll be the next thing they don't
understand and then and eventually time
goes by and they don't have those those
holes anymore and then what happens is
what you said oh now everything makes so
much sense why did I ever think it was
difficult 



Carlo Vicari:
so um so I know this is a
little bit of a segue but I'm interested
in hearing a little bit about this since
you've been in tech for so long island
and um block chain is so new as far as
technology is concerned
where do you see with your experience in
tech in your background and you know you
work so closely with blockchain know
where do you see blockchain technology
and where do you see epc um you know you
can give us your your wild thoughts on
different use cases and kind of just
where you see the technology in five
years 10 years 15 20 years well you know
whatever whatever you think



Alan McSherry:
 yeah we well
you know we've been kind of so
concentrate you know so focused only on
the small details of what's what's right
in front of us now that I actually
haven't given a huge amount of thought
to pivot to the future of the vtc in
five years time I mean I guess broadly
speaking I would probably like to see
you know like everybody else you want to
see some actual will use cases that are
not not suspect as if so so the so that
is the use cases that are that were you
know that it becomes very very useful in
them yeah I don't work but the the
killer app for free PC as yet



Carlo Vicari:
 yeah well
I mean like blockchain technology one
decade you know how do you see it
changing the world or changing the
everyday lives of people you know in all
the country in many different countries



Alan McSherry:
well I've nothing you know particularly
new to add to that to add that debate
there's a lot of talk about banking me
on buying you know you've got usually
use cases have been able to hire a car
over the over the internet and turn up
and unlock it with a with a private key
neram to meet any one of the same with
revolutionising Airbnb



Carlo Vicari:
 wait what's that
about the unlocking a car I i don't
think i've read that on it so if you
have a 




Alan McSherry:
so if you have a a transaction
whereby your you basically can transfer
the ownership of a key to from from will
they couldn't being controlled by my key
to being controlled by by your key and
then you can you
that too just unlock the car so so over
the Internet you could basically arrange
that transfer blockchain transaction
secondly you come up to your car and you
have control of the key to unlock the
car 



Carlo Vicari:
I see I see okay yeah I hadn't heard
that one before this interesting so what
what else wild wild speculation is fair
game 




Alan McSherry:
I would like to see I would like to
see huge destruction in social networks
i would like to see some kind of virtual
currency be the backbone for distributed
social networks that's probably yeah
cases that i'd like to see so so
currently you know we have a lot of we
have these walled gardens where people
are Facebook and whatnot they make a lot
of money out of the data that you
provide and I would like to see you know
code out there that uses where you have
lots and lots of different pods all over
the all over the planet they use they
use a virtual currency between
themselves to keep to balance the books
but they're all basically coordinating
to to provide social network services
and of course everything that they they
transmit and receive is is encrypted and
only decrypt able by by the people that
I spoke so that yeah kind of these cases
that sort of is sticking as been stuck
with me for I guess two or three years
now 



Carlo Vicari:
so this is like sort of a one-two
punch of a or number one users being in
control of their own data and not being
the product and also be than the users
that are on these social networks would
be able to be paid for their content or
contributions that correct 



Alan McSherry:
exactly
exactly i mean you know there was a it
was a you know there's been a couple of
almost versions of this but as you say
like that 12 or one two three punch
which five altogether so I mean say for
example you know you were in a social
network and we'll say you're actually
you're charged for delivering so if i
want to send stuff to you I have to pay
a little bit to get that deliberate
if you want to hang so you got to pay a
little bit to get that delivered so if
we're standing and they're seizing at
roughly the same level you know we're
paying transaction fees to be with the
pods that are handling our our social
stuff or pictures fast or whatever it is
but roughly we're not you know we're not
we're not generating utils when I paying
huge bills but if your isn't balanced
and you're trying to advertise to a
million people well then a million
people are not sending you anything so
you're not getting any not getting any
currency but you have to come up with a
little currency to send a million people
all right odd so that would be you know
that would be one way of making up sort
of ensuring that that basically you know
you see you only receive stuff that you
want to receive so you could set your
limits can only need you right getting a
lot of stuff even now from spammers who
are willing to pay to put stuff on your
role or you could just up that limited
choice whatever it is and and just cut
that stuff out 



Carlo Vicari:
right that's just boom
market solution 



Christian Seberino:
well now i buy that
question about that's an interesting
scenario so by adding a cost you you
would discourage spammers but one of the
benefits of you posting something on
Twitter and Facebook is that a million
people plus could see it yep to see
whatever your content is for free now if
people have to pay for every every hit
every download I maybe some people would
be discouraged from using it or maybe it
would be too expensive for some people
so then the cost could be a negative




Alan McSherry:
well it so with a tweet you know you're
advertising to the planet intentionally
but where I would do sort of use case
with where I'm what I'm that I'm
advocating here really is a social
network so really i want i want to send
stuff to my sisters and my mom and I
want to get those from my sisters in my
mama that's real key if and and you know
I'm willing to pay I'm also willing to
pay to send stuff to my friends because
I know that none of my data and my
network are being minds because these
pods right they make their money off the
transaction
fees everything is encrypted now they
can probably look at some of the meta
data in terms of you know who's who's
connected to who I mean that could be a
weakness but you know that sub stuff
that could be against work done but at
the point right the use case that I'm
trying to get at is where we showed it
we sort of removed the we pay basically
for the service that we're using so I'm
the service that I want to use is to
have my cat pictures delivered to them
and so as I have one be able to deliver
stuff to me you know i have no problem
paying a small amount of the virtual
currency to do that and what i would
think is that in order to scale this you
know you need a a wide network of of
these pods and the way that these pods
would interact is they would have to
share a common currency so I mean
there's already stuff like the spore
that tries to do this sem you know these
distributed social networks so this
would be this would be in some sense
similar to that except that the they
would share a virtual currency in order
to you know in order to be able to
interact in an economically fairway so
if you start up a new pod you know if
you're handling a bunch of accounts well
you're getting paid in the virtual
currency for delivering stuff to two
other pods and you have to pay other
pods to take their stuff or whatever it
just allows economic interaction between
them between these should be the social
network bought pleasure awesome right
vixen money 




Christian Seberino:
I action and you probably
another interesting question which was
where he brought up things you brought
up diaspora which was tries to be a
Facebook competitor decentralized
Facebook competitor but that what
they're running into is that people
don't care about the privacy protections
they don't care about the
decentralization as much as the Explorer
would like them to so do you have any
thoughts on that that block chains going
to provide all this wonderful privacy
protection potentially and decentralize
distribution of power but no but the
public is not going to care even though
they should 




Alan McSherry:
well I think there might be
a you know there might be a tipping
point in that I am certainly because I'm
you know I keep an eye out for those
types of articles I have noticed an
uptick in articles that talk about what
are the what are the alternatives to
facebook you know why are we why do we
why are we so glad a about allowing our
data to be mined and used by all these
companies I think this is sort of it I
mean for people I guess who are in tech
and definitely people are interested in
blockchain I mean this is all old hat
but I think for the general you know
even even in the mainstream it's
starting to dawn on people you know why
Facebook is free in inverted commas yeah




Carlo Vicari:
I i think i know what the tipping point
is going to be honestly for I think what
decentralized social network will
actually be popular at some point and I
think the tipping point is all about
content and once you have say a nice
critical mass of people that are on
there producing interesting content and
they're getting paid for their content
directly through this block chain a
social network you're going to start to
see more and more people gravitate
towards the content that's on there as
opposed to the content that's on say
something like Facebook because I just
think just like the the content on the
open unfiltered internet is just far and
away more interesting than say something
unlike cable TV for for the new
generation of people I think on the new
social networks that are decentralized
and start to pop up the content on there
is going to be just by virtue of so much
competition open competition it's just
going to be far and away way better than
anything you see on facebook 
yeah and I
am so if you can only run you're going
to snowball from there 




Christian Seberino:
no but see but
don't notice that you didn't say that
people are going to switch because all
of a sudden they're enlightened about
the importance of privacy and
decentralization law




Carlo Vicari:
you know I think the funny thing about
that is is a lot of the people that are
interested in privacy and
decentralisation they don't necessarily
make up a huge chunk of the general
public but a lot of these people are the
type of people that get movements going
on the internet you know what I'm saying
so it's not that they represent a large
chunk of people but these are the types
of people that make things happen on the
Internet I don't know I can't really
describe it what do you think Alan yeah




Alan McSherry:
I'm not sure I don't know what tipping
point is because I mean I look I see
similar things with I thought it was
going to get tipping point away from
whatsapp to the likes of signal me but
and a lot of people do use signal and
you know win them when there was ice and
recently signals became a lot more
popular but people i mean what's up then
just claims you know and i don't i'm not
saying it's wrong or right but they were
encrypting everything end and everything
was secure then everybody doesn't need
to be forgot about that and i was
meeting him



Christian Seberino:
 so he would not you would
like people that aren't familiar with
the the scandal you're referring to



Alan McSherry:
 well
they would pay so after what's off came
that they had encrypted end-to-end there
was an article that shows that under
certain circumstances the keys that they
used to encrypt room were exposed so
basically it was a security flaw I can't
remember the details to be honest but I
just I remember reading about it and I
remember not being too surprised you
know and I don't think that they think
it was a it was a reaction to the fact
that they were about to lose a lot of
share to signal that was how how I read
that where it's single you know their
purpose was to be secure from from the
beginning a 



Carlo Vicari:
long story short most people
don't care about privacy no it is




Alan McSherry:
 I
think it was that's hard to escape that
the conclusion that the resistor
Dominator
and a blase I don't you know it won't
happen to me sort of thing 




Christian Seberino:
yeah yeah I
think if the Snowden revelations didn't
convince people out of the house could
convince 



Carlo Vicari:
yeah I don't I I guess it's a
combination of things i think the the
privacy I don't think people completely
discounted but I think the overall
experience on the platform is the number
one thing and then if they're comparing
say you know a facebook and a
decentralized facebook I think privacy
could be a tiebreaker for sure you know
mm I think I think it does count for
something for people but in reference to
like signal and whatsapp just the
network effect that whatsapp has the
signal privacy it's not enough to it's a
tie breaker but it doesn't count as like
three or five points i don't know how
see ya so but i think there could come a
point when if signal has a massive
network effect and you know a really
good and it's a really great platform
and people are starting to decide you
know because it's these things evolved
from the younger generation it's when
younger people get their cell phones and
say out what cat method what messaging
application we're going to use sure if
signal can break the tie with privacy
you know boom they're going to have a
whole new generation of people using
signal over what's up



Christian Seberino:
 yeah and not only
does the new block chains provide
privacy but there's another another
equally important attribute which people
use the word decentralization a lot but
i don't know if people when they say
that i don't know if they're thinking
that the blockchain distributes the
power so you don't have a centralized
Pope that could make decisions on a
social media platform well you know
there's no there's not that that danger
and so I'm and again I don't know how
many people are worried about somebody
and power doing something malicious but
that's certainly something to be
concerned about and block James can help
protect from
actors that are in power mmhmm 



Alan McSherry:
yeah I
think that's an important plank in that
sort of potential use cases but you know
if you're if you're a particular project
censored you should be able to just
migrated over to a different pods you
know it would be that in the different
country or whatever and because they're
economically connected to the through
the currency that they all use you can
do that


Christian Seberino:
 yes


Carlo Vicari:
 oh that's true I don't what
what Alan was just talking about as far
as because there's been a lot of
controversy lately about you know people
being banned on Twitter you know for
better for worse that's what I was it is
a fact yeah the fact of the matter is
you know I think you guys are both right
about that more I guess more so than the
privacy thing I think the censorship is
a big one yeah 



Christian Seberino:
yes the arch is
censorship but like political bias right



Carlo Vicari:
right right so I see what you're saying
so it's like the the network being
impartial completely and just you know
whatever people's thoughts are just get
out there naturally yep and that's just
the end of it 




Christian Seberino:
yes now Alan what do you
think about this this idea so I think
about block chains as out there in
cyberspace you know outside the control
of any nation or person and so in a
sense it's almost like the first steps
towards an artificial intelligence if
you know what I'm saying 




Alan McSherry:
yeah I know
what you're saying the singularity then
well I mean it certainly would I could
see some kind of you know emergent
behavior may be coming out of this
rather than you know with a program you
know I tend to think of it as a an
artificial intelligence as being you
know you'd start with sort of some of
the machine learning or you know some
some of the technologies that are going
on today and and that was just somehow
you know we get some stage where that
would be able to build its own AI which
would obviously we you know far better
than the one that we built and then that
would take off whereas I kind of see
this sort of what's happening with block
chain and a lot of the smart contracts
that go out there that you know that may
be some kind of unexpected that behavior
will emerge from a lot of different
people acting in their own acting in
their own self-interest and that this is
provided acquiring good worrying 




Carlo Vicari:
this is
too much for me I can't even beat my
phone a test I listen much I can do this
this is too much guys well



Christian Seberino:
 no but let go
is one last point just enough again for
this but let's say oh 



Carlo Vicari:
no no I want to
talk of interesting stuff actually I do
have a quick question for Alan that I've
actually never got a chance how do you
met ask someone about AI and writing so
I read some I read something interesting
one time I don't know where or who wrote
it but it was about that really
conceivably the first AI would just be a
computer that could rewrite its own
computer code and at that point it would
just keep rewriting its own code is
there does that sound valid it makes
sense to me in my head but I don't know
how much sense that make well there's
from a development perspective or their




Christian Seberino:
software that could that could be due in
the sense to the development for you
that's what machine learning is all
about it developers don't have to write
programs anymore the machine learned it
by itself 



Carlo Vicari:
yeah but could it rewrite its
own development machine learning code
you know what I'm saying like rewrite
its own code 




Christian Seberino:
well you could like feed is
a new language and it could it could
learn a new language so if you call that
Riyadh 



Carlo Vicari:
no feet no feeding it just it
rewrites its own code I don't know yeah
that's the thing so okay Alan 




Alan McSherry:
what do
you want more red you know I've read
that they're people who understand
you know really I mean Elon Musk for
example has invested in them
significantly in in AI companies and i
read that the reason he did that was
just to keep an eye on them because he's
quite concerned but something like that
will happen that the first day I that
can create an AI will just you know
we'll just do we'll just go nuts & M
will never put the will never get the
genie back in the bottle Larry well it's
not a great way pressing it but those
were those with is the basic care follow
these basic concern I mean you think of
it like you know when you when you write
a when you write a compiler for a
language I you know one of the first
things you can do then is is you know we
write the compiler in the language and
use the compiler to compile what you've
just written mm-hmm for what you know
there's a I guess precedent for EM for
doing crazy things like that software
yes well 



Carlo Vicari:
it feel on feel ons worried
then I'm worried what 



Christian Seberino:
Alan took the
question I wanted to ask you earlier and
I really want to ask so let's go with
your example of the the blockchain car
door opener okay and then of course you
can have a house door opener and then
money is on the blockchain and we know
that block chain is sensor proof so as
more and more of our our the
functionality of our lives is on the
blockchain and nobody can stop the
blockchain nobody could sensor can you
see that it it's there's like this
mysterious entity that's all of a sudden
taking taking over more and more of our
lives that that nobody controls that
that's a kind of an interesting image




Alan McSherry:
yet you know it it's plausible I mean
definitely and I can't see that is the
show concert 



Christian Seberino:
okay 



Carlo Vicari:
so are you saying when
I don't pay my rent I get locked out of
my apartment immediately that



Christian Seberino:
 could
happen what's that well actually that's
right no but that brings up another
question what if somebody makes a smart
contract that after they let it loose
and then they say oh I really wish I
do that but they they wrote it in such a
way that they can't stop it then what do
you do get them saying because it's
since your proof



Alan McSherry:
 yeah you can write a
smart contract and gating it I don't
know 



Christian Seberino:
yeah I know so saginaw software
software out of control that's that's
the that's what I the in a nutshell what
I'm thinking it 




Alan McSherry:
yeah I mean that sounds
it sounds like a lot like I guess you
know the virus but you accidentally
release but it'll just keep running and
running and doing what it's supposed to
do I mean one of the safeguards that we
have is that contract should run out of
you know we should run out of gas they
should eventually and you know if
they're not supported by external
stimulus like people calling this the
contracts then you would hope that they
just run out of gas and tight uh-huh and





Christian Seberino:
we've had already an example of what I'm
referring to the Dow attack right they
couldn't just say oh bummer we let okay
let's kill the smart contract right once
it was on the blockchain it's not so
easy to stop it anymore so they has a
letter thing so that's what I'm soon 





Alan McSherry:
yes
yeah oh yeah I suspect I don't I got it
and you know we know what happened 





Christian Seberino:
yeah
whereas with yet less server web
application I can just say oh ok wow
that that made a mess okay I'll just
I'll just turn the server off until I
sort out this myth 






Carlo Vicari:
right okay I see I
see what you're saying now because the
web server I'm have a wait you have a
way to turn it off yeah there's no
turning it off okay gotcha gotcha oh so
also this is another kind of a thread
derailment I guess but uh so this is a
shout out to my older sister sister
Cheryl and she had a suggestion for the
show which was to also ask kind of what
some of the gifts are reading or
watching or movies that they're into and
stuff like that as far as you know
having the community get to know them
and what they're all about so anything
interesting
I know you're probably neck deep into
Scala code and et Cie stuff but anything
interesting uh you know you're reading
or watching these guys out 




Alan McSherry:
it's the last
I guess it's really really interesting
book I read was with sapiens I can't
remember I think it's Noah who vowed
might be the name of the author and the
reason I remember that I actually read
it a couple years ago and I started I
liked it so much they started reading it
again pretty recently and just by
coincidence i haven't you thought it was
a developer's earlier today and he
started reading it absolutely level in
as well so yeah let's suppose it would
be a one of the best recent books that
but 



Carlo Vicari:
I got a got a summary for anyone out
there listening maybe 



Alan McSherry:
well it so this
book basically explains everything that
has happened up until now it's not the
work of fiction it's a work of
explaining how evolution of of the human
race up until now and that's very well
its people yeah he does it at am in a
very readable way you know you find
yourself turning a page and nodding your
head and going yeah yeah I guess and now
okay yeah i would highly recommend it
actually thinks no I know you bow I
think is the guys name I'm not can't
remember so i can name i just opened up
there and 



Christian Seberino:
it's called sapiens as in homo
sapiens-- there 




Alan McSherry:
yeah thank you sorry I
beg your pardon it's fooling is well
Noah harare 




Carlo Vicari:
okay gotcha okay you know we
can actually probably put a link to that
that book or you know a link to that
book in the description on YouTube as
well so shut up to Cheryl for that
question thanks yeah and uh I'm not sure
if you guys have anything else to cover
you got any anything else you guys want
to go over Christian Allen 


Christian Seberino:
no I think
I've talked enough 


Alan McSherry:
yeah 



Carlo Vicari:
all right
well then Alan just want to thank you
for coming on the show thank you for the
time thank you for everything you've
done free TC so far and everything
you're going to do and we're really
excited and happy to have you on the
show 



Alan McSherry:
you're welcome and thanks very much
for having me with the nice milky way's



Carlo Vicari:
sing it and Christian we missed a few
shows here but I've created great to do
this with you again and everybody out
there listening thanks for checking out
the show and we'll see you guys next
week take care guys

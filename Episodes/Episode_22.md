# Let's Talk ETC: Lukasz Gasior & Radek Tkaczyk - Scala Client Coming Soon.
Carlo Vicari:
hi everybody you're listening to let's
talk et Cie I'm your host karlovy along
with my co-host dr. Kristen suberino I
just want to thank everybody for tuning
in to this week's show we've got a lot
of talk to talk about there's some big
stuff happening this week and you know
there's there's a whole whole ton to
talk about but we're gonna try to hit on
on some of the bigger issues and bigger
events that have been going on in the
community here in classic community as
well as the blockchain community Bitcoin
community et cetera so we've got some
SEC stuff that kind of spooked everybody
a little bit some aetherium hack stuff
that went on in reference to some of the
multi SIG's for some of the icos that
have been going on luckily there was a
white hat group just to give you a brief
overview there's a white hat group that
came in and kind of took some of the
funds and put them away for safekeeping
so as an et Cie event in China that
preliminary discussions are starting to
be had I don't have too much information
to talk about that later with you guys
but for anybody listening just to give
you heads up that some plans are in the
works for and et Cie event in China
possibly Beijing Shanghai or maybe
somewhere else maybe Hong Kong nothing's
been finalized with that yet but these
are things that are being talked talked
about right now that we're pretty
excited about and then the big one on
everybody's mind is the looming Bitcoin
fork August first Bitcoin cash it looks
like it's going to be listed on some
exchanges it's you know bitcoins up some
other things are downs Bitcoin gonna go
way down and drag everything down who
knows as you guys know I it's impossible
to time the markets or you know figure
out what's going up what's going down
sometimes but but on to the main point
the important stuff for today's show
which is really our two fantastic guests
that had the opportunity to join us
today two team members from the growth
and Deek team which is building IOH case
scholar client gonna have the beta
coming out first week of august or i
should say early august since you know
development development stuff is
sometimes difficult
time to an exact date but they're really
working hard in getting a whole ton done
and we expect the beta out in early
August and we're really excited about it
so I'd like to welcome Lucas and Radek
to the show Lucas thanks so much for
joining us Radek thanks so much for
joining us really happy to have you guys
on here 



Christian Seberino:
so what what country are you
guys in just out of curiosity first of
all 




Lukasz Gasior:
we are from Poland okay



Carlo Vicari:
 now Poland
don't worry guys Poland's famous enough
people know Poland's in the earth I hope
I hope 



Lukasz Gasior:
programmers I guess 





Carlo Vicari:
mm-hmm but uh
so so for anybody listening what we're
gonna be doing on the show is leading up
to the release of the IOH case scholar
client but by the way we've got a couple
of names on the table there was a reddit
post some community members suggested
amber helix
there's Phoenix I think Cole idea
cascade there's a there's a few
different suggestions but for me
personally like I like the name helix so
what do you think what do you think
Christian helix



Christian Seberino:
yeah nosebleed no just kidding yeah I
don't know he likes to be fine I don't
know how these things get decided 




Carlo Vicari:
well
you know what I don't want to get in
trouble and call it the helix client
pretty much surely so we'll just call it
the scholar I which case Scala client
for now so anyway so we're gonna be
having a couple of guests from the
growth and Deek team every week leading
up to the release of the Scala client
and maybe have a big group chat on the
release day for anybody that wants to we
can we could pop some champagne or
something like that because you guys
have worked so hard but so you guys are
Poland Lukas are and you why don't you
guys tell us a little bit about your
your backgrounds kind of the long story
how you got into tech from way back one
Lukas I guess you could go ahead first




Lukasz Gasior:
okay
pretty usual way with just regular HTML
files I don't even remember what was
like impulse to start doing that but
just got interested in writing really
simple static web pages and that was
actually like my first start with
programming well HTML programming but
with tech in general and then at some
point I came across Pascal and Delfy so
I was amazed by window applications and
drag-and-drop buttons and all different
stuff to units pindy actions to them and
so on so I was really amazed by that and
I think that's actually what got me into
programming like like really got me into
it so I was just playing with it a bit
for some time then I came across PHP I
hate it now but then I hated Sunday in
the future so I was also creating
something simple web page that's HP and
then it some day I came across Java and
for me it was like whoa objects and like
in real world there are also objects and
you don't like it just makes sense so it
was really into Java at the time and I
started doing first on applications on
my own trying to play with it a little
bit later trying to create something
useful and then sometime after that I
became a Java developer and doing my
studies in the meantime so for some time
I was a Java developer and then at some
point I came across a video on YouTube
it was pretty short video I don't know
10 maybe 20 minutes and the guy was
doing that presentation like kind of
teaser presentation about Scala I was
even
and I immediately thought whoa let's see
that's it that's the language I want to
learn it's just so much better than Java
it's so much more concise and I just
like it like from the first side I saw
Scala I knew that that's the language I
want to use so shortly after that I
joined Scala C which is a Polish company
that specializes in Scala and I've been
there for quite some time already 





Christian Seberino:
THAET IMPRESIV
Lucas
so you even so before you started to
work on me on the et Cie Scala client
you were already committed to to Scala
he loved it and you had the deep
experience before that that's pretty
impressive 




Lukasz Gasior:
yeah it's true for the past
few years I've been focused almost
entirely on Scott so I was trying to
avoid the Java as much as possible





Carlo Vicari:
 magic
oh sorry I was coming out there how
about erratic how what's your how did
you kind of fall fall into technology
with what's your background story kind
all that





Radek Tkaczyk:
 so I guess the motivation was
that's back in the day I had a really
tracked computer and I had all those
problems with running games you know so
I started digging digging up into it
what I need to do how to change the
configuration of memory and things like
that to be able to run them and






Carlo Vicari:
 you were
you were programming out of like
necessity almost 





Radek Tkaczyk:
yeah you might say that
so but actually the start into
programming was kind of unusual one
because I found the I found a guide of
how to write a game in a very very very
old booklet Magazine about games and was
actually in assembly assembly language
and that was my first language
the lands and for some time I didn't
even realize everything assembly and
then gradually I moved on to CC plus
class
licked on things like Pascal and PHP
when I started University I I picked up
on Python and sorry no offense almost
everything at least things that didn't
need to run fast
so yeah but as far as my education I
didn't actually study computer science
strictly you know I'm a big fan so so
naturally I don't believe in organized
education I was afraid that education
would kill my passion for programming so
so I chose a major in telecommunications
I basically I want to learn about the
internet and distributed stuff but I
found out that I had to learn too much
about cables and frequencies and so on I
played with data started job and when I
saw how different and on practical
things the universities were simply
dropped out so but actually my first job
in IT what was not programmers job I was
kind of an analyst one hand I had to
deal with demands and then I had
configure and take care of our
deployments but oftentimes I've found
out that and actually I took this job
because because I because of my
experience with the University I just
felt that you know maybe I should I
should have chosen the science probably
I'm not that good program here anymore
compared to the people in my age so I
chose this analyst job and but so I
found out that the software everywhere
was having lots of problems and getting
programmers to solve those problems too
but fortunately had access to the code
repository so I just started going in
into code and instead of writing a
ticket I just went to the program and
hey go fix this line alright so so yeah
and that's I was quickly spotted by the
and I was just switched program is full
programmers position you're saying 




Christian Seberino:
so
even though you didn't have a degree in
computer science you and even though you
weren't hired to do programming you your
manager noticed your skills and so even
though he's that's you switched you over
just because he was impressed 


Radek Tkaczyk:
yeah 





Carlo Vicari:
you
might say that 






Radek Tkaczyk:
yeah unfortunately for me
the LAN bishop that uses a company with
Java language like it doesn't really
offer that much as compared to C++
and then you know it's just for this a
bit more effort coding in c plus plus he
had this much better experience of being
close to the machine things run fast but
soon after that I learned about scallop
there's actually a small Scala team in a
different Department of company and I
started pursuing this language and soon
I was moved to that team and that's been
like five years ago so since last for
the last five years I've been coding
predominantly in the sky so





Christian Seberino:
 you know the
high level you know the high level
language Scala and you also are very
proficient with the lowest level so
that's pretty impressive 




Radek Tkaczyk:
at least I used
to be because I was actually being in
the major programming for the for the
EVM part in our clients actually that's
so yeah also because for the same
companies can see which is okay






Carlo Vicari:
so what's kind of the so that I we have
the tech programming story how did you
guys kind of fall into crypto is it
before developing this io HK Scala
client for e TC or were you guys
interested in Bitcoin and cryptocurrency
and aetherium and other stuff before
kind of getting into this
what's Lucas and any like rabbit hole
story behind 



Lukasz Gasior:
SO ECSHEN NEW BITCOIN FOR QVAI SOMETIME
that and you have it works
and for the blockchain work 






Carlo Vicari:
you just
didn't own any 




Lukasz Gasior:
I knew
but I wasn't really too much interested
into it thank you
last year who and I came across the fear
in white paper or maybe some video in
youtube I don't even remember what was
first so I read the paper and then I
thought wow this is great like the real
virtual machine running in the network
similar way to be kind with the
blockchain so I thought that was great
and I got really interested in the
theorem by design and shortly after that
which is very fortunate kind of
coincidence I which Kate showed up and
like I was the first figure I had was
like well I had to do this I want to
join 






Carlo Vicari:
yeah I see so that happened pretty
I have that all happened pretty quick it
was like you knew about Bitcoin and
blockchain boom you ready theorem right
paper boom IOH k boom you're developing
a client for the etherium competitor






Lukasz Gasior:
 yes
it was not that boom I knew I did about
it for quite some time I just wasn't too
much interested and only a few years I
learned about the filium I see boom okay





Carlo Vicari:
right right
how about here adequate do you have a
kind of a rabbit hole story you knew
about it for a while or brand new what's





Radek Tkaczyk:
up um so actually I I haven't even heard
about etherium before being kind of
starting the recruitment process for HK
and yeah but about Bitcoin for quite a
while and I was kind of impressed by the
cryptological mechanisms involved there
and that's actually why I pursued this
this really happened by accident just
that's company's boss mentions to
everyone that hate is a interesting
crazy project going on to apply so I did
because I just wanted to learn about how
this works
I also wanted to to be to be close with
anything that's relies on maths you know
my ability to comprehend that stuff so
yeah but then we were given a kind of
task based on the this correct framework
and Couric's challenge challenge based
on corrects and why we're doing this but
there's a thing called 




Christian Seberino:
so oh you know I
I wasn't gonna ask you this I didn't
even occur to me it is the Scala client
does it use some of the code from score
X so I think there was some crypto stuff
there 




Christian Seberino:
okay




Lukasz Gasior:
 I think we are not using any
code that's like strictly from Discogs
framework 





Christian Seberino:
okay so score X is a beautiful
rewrite of the of the Bitcoin software
system that's more flexible and you
could easily make modifications and I
believe it's it's even more efficient
than the Bitcoin core so it looked
interesting to meet it




Lukasz Gasior:
it looks interesting it's kind of
flexible and I think it's very good for
prototyping blockchain solutions but
just for our client we felt like it
would be better and beneficial for the
client to write it from scratch and not
quite you know what it requires to
implement it and we didn't know which
parts should we take from scoring's
we do not we do not need not to use it
and just write everything from scratch
so in the beginning we also considered
integrating books College corrects at
later point when we knew what we want
from it then we decided just to go with
with the client without it 




Christian Seberino:
I see okay




Carlo Vicari:
now do you guys um I guess that's kind
of your story about how you first
started getting into crypto I know Lucas
knew about blockchain for a while and
then you know really got into it with
this project and braddock you gave us
your background as well are you guys now
like really into blockchain and crypto
and how much do you believe that it's
the future of a million different things
are you guys still a little bit
skeptical about it I guess I should say
what do you think Lucas





Lukasz Gasior:
 very much oh
really
you got deep but for the second part of
the question if I think it's going to be
the future I don't know I hope so I
think it's a great Butler but what will
be the future no enough 






Carlo Vicari:
yeah that's true
pragmatic answer what about you
radically what do you think 




Radek Tkaczyk:
well I still
believe we were like pioneers you know
to 4-bits community remain encrypted
currency to be the future it really has
to reach the masses and it still has
only reached nerds yeah I think we're
doing a good thing in the right
direction
this will keep evolving evolving and I
don't know what's gonna happen that's it





Carlo Vicari:
so I guess I'm drinking a lot more
kool-aid about about blockchain than or
crypto than you guys are cuz uh on a
scale of like one to ten do I think it's
the future I'm like I'd like a nine
point nine actually that's an
interesting question what on a scale of
one to ten ten being it's definitely the
future one being it's gone
tomorrow where do you think you are
Lucas 



Lukasz Gasior:
17


Carlo Vicari:
okay all right that's right you
have the minor you have the minor in
your balcony
so you're you're drinking some kool-aid
what about what about you radical





Radek Tkaczyk:
blotching generally yes I'm just not
sure about if it's any of the current
implementations of it 







Carlo Vicari:
yeah I definitely
agree I mean I definitely have the
obviously that the chains that I believe
in that I believe will will be the
future or part of the future but I agree
it's hard to say what the actual future
is gonna hold and what the chain that
you know implements well and develops
properly is gonna be but all I can do is
work on what I believe in and and see
what happened so how do you guys feel
about the development of the ATTC
scholar client has it been you know good
good learning experience and bumpy not
so bumpy how was it working with the
rest of the team you know tell us about
how was you guys working together 





Lukasz Gasior:
so for
me it was definitely challenging and
I've learned a lot during this time with
developing clan there were quite a few
things that I didn't expect to be so
difficult to do or maybe not even
difficult
kind of tricky 



Christian Seberino:
what what are some
examples taken said surprise D 




Lukasz Gasior:
well
stomach lumpy one thing that was tricky
to work with was the yellow paper
because it turned out it only contains
the state as like the most recent state
of the art of cerium and for the actual
client we also have to implement the
logic that was before the forks and the
changes that acute on the blockchain to
find information about those it was not
Smith it turned out that the best source
of information is github issues and
going through pull requests and trying
to find what changed the in which the IP
so like to conclude I think if you're in
kind of like documentation in one place
it was not that easy to try to find what
changed in which a Yaqui 




Christian Seberino:
yeah no I tell
me if you agree with this so my
impression is that the yellow paper is
you know a large large majority of the
explanation that you need of the
architecture but then if the English is
somewhat can be ambiguous and so you
need to look at source code right the
source code is the final authority or
that answers any questions you have
about how it operates so between the
yellow paper and the client existing old
source code you could kind of answer all
your questions is that how you guys the
two sources you guys use 




Lukasz Gasior:
that's how we
did it usually but it could be much
easier if it was just written somewhere
in one place just with plain English
words what's changed so that you don't
have to look for that in the pull
request kind of trying to guess what are
the changes that have been finally
implemented because usually on the issue
on github there's the proposal and then
discussion a lot of comments and so on
and at the end
you don't know what has finally been
implement that in the clients has to
take a look at the code so maybe it's
not maybe it's not hard but it just
takes time and a lot of focus to do it
right



Christian Seberino:
tedious yeah yeah sure wait Radek I'm
curious so you said you you learned
assembly that was your first language
and then you learned C and C++ so did
you get an opportunity to learn all
about the low-level virtual machine op
codes and all that the that low-level
detail so that you could consider
yourself an expert on the whole
architecture 




Radek Tkaczyk:
yes in fact yeah I might
call myself an expert on this I believe
I was the main developer for this part
of the of the client and yeah mmm I
gotta say it was really fun and
challenging do you know getting getting
this the blockchain from the start of
the transactions finding those bags
along the way
very quite an experience and I have to
say that I really enjoyed having the
yellow paper around me and now it's been
it has it has issues it's often cited is
very hard to to comprehend and I'm not
saying it's not but then again you have
to see that it's quite short it's a
question of paper for such a whole lot
of functionality and quite a concise one
and I would say it is just really handy
to have it around and well one thing I
was missing from it initially was that
there's quite a lot of mathematical
symbols there and so I was missing like
one single page reference to know what
they are but at some point I just
started you know you be waking up in the
middle of night new
know perfectly what that symbol was
sometimes I think papers kind of more
familiar to meet them than the code I
write interesting experience 



Christian Seberino:
yes
sometimes people have tricky questions I
think and they look for subject subject
matter experts for you know these
architectures so if you if you know at a
deep level the the intricate details I
would think that you're gonna be in
demand and a lot of people are gonna
want to find you you know to pick your
brain about different things 




Radek Tkaczyk:
well but I
actually I was thinking and because you
know and we found some bugs in either a
wrong symbol was used you would see I
mean I definitely submitted one issue I
think one of our teammates these were
like definitely different parts some
places and I could point them out well
some sort of ambiguous language is used
I'd really love that to improve but you
know we're really striving for this beta
so probably at some later time but you
know there's another problem here
because you know paper is really about
human heart folk and gymnastic doesn't
have yellow paper as such yellow paper
does keep is updated with the latest C
IPS that are introduced into protocol
but the EC IPS that are there it's even
classic yellow paper is totally ignoring
those so maybe we need to fall for the
papers 






Christian Seberino:
oh we need a need a yellow paper
fork you're saying
to capture the divergence yes I see what
you mean good point 





Carlo Vicari:
yeah so now in
reference to the I which case Scala
client do you guys see anything
interesting on the horizon that what are
some interesting things you'd like to
see from the client in the future I know
I the beta is gonna be just command line
and there's some interesting stuff that
maybe i ohk can do or would like to do
with Daedalus and some other things what
are some other interesting things that
you think you you personally would like
to see the clients be doing in the
future potentially even if it's not
necessarily on the drawing board just
things that you would like to see may




Lukasz Gasior:
not be the answer that they expect
because I would really like to see and
would like to have some time to clean it
up a bit and to pay the debts because
for example in pill discovery we
implemented a simplified version of it
so that's something that I would
personally would like to focus on and I
think there are also some other things
that may require our attention after the
beta also the LPC API that there are
certainly areas that we can improve the
speed because for me personally it's a
bit too slow or maybe not a bit too slow
but it just could be faster so these are
the things that I like the focus after
the beta 



Christian Seberino:
yeah yeah that's good I prefer
your honesty yeah you know and also I
think isn't that just isn't that common
though isn't that normal like you are
saying you guys shared that you didn't
know at the beginning whether you should
use score X so when you when you're
developing a new piece of software you
almost have to do it two times right
the first time to develop the
architecture design it and then you come
back a second time and you learn from
your mistakes and 





Lukasz Gasior:
it's usually
developers would like to do come back
and try to carry out the deed but on the
other hand there are managers who would
like to new features




Christian Seberino:
yeah I always I always think about like
the the Linux kernel Ennis he made his
first version and then he's had 20 years
to keep perfecting it perfecting it and
do everything he wants you know I think
a lot of programmers kind of have that
dream of making the perfect code and
rewriting things





Lukasz Gasior:
 yeah I think it just
doesn't exist






Carlo Vicari:
what about remember sorry go ahead



Lukasz Gasior:
okay from the more exciting features I
think as you mentioned the Dallas
integration 





Christian Seberino:
yeah can you also wait for
people that don't know can you
what is date Daedalus 




Carlo Vicari:
Daedalus swalot



Christian Seberino:
yes thank 



Lukasz Gasior:
you another project of IOH guy
is well it's basically a wallet mm-hmm







Carlo Vicari:
yeah okay it yet it's a wallet and
there's gonna be some potentially some
HD wallet features and some other things
that are on the drawing board as well
that could be really interesting as far
as yeah I don't want to I don't want to
reveal too much I've got to see what we
can and can't talk about but there's
some definitely some cool stuff in the
pipeline 





Christian Seberino:
what did you say HD wallet what
what's that yeah what do you mean HD 





Carlo Vicari:
so
this is a bit more of complicated stuff
then 




Christian Seberino:
okay well just what does it mean
okay just what does it stand for they
just say that






Carlo Vicari:
 yeah yeah I'm trying to
think of I'm trying to think of a good
good way to say it you know it's like
for multi accounting and having you know
multiple coins multiple accounts within
the same sub-account
oh and I think I'll think of a of a more
concise answer but I I definitely like
to hear also what radix sees as far as
interesting things on the horizon for
the et Cie Scala client and also
Daedalus as well maybe some integrations
and stuff like that



Radek Tkaczyk:
totally
support worker said I mean for me it's
all about the features it's about making
our clients more robust speed is one
thing we have to compete with other
clients like death and parity that
currently faster than we are and we need
to keep this friendly competition going
but also we need to gain more confidence
in the correct answer so far the most
the best test that we've done really
syncing up with with the chain with the
main chain with the more than test
network and currently we are trying to
make that client compliant with the
material test suite
just about repository lots and lots of
tests defined in JSON files so currently
quite close to having those tests pass
for the virtual machine but there are
quite a few other categories that we
should look at Thanks



Carlo Vicari:
 gotcha kappa 



Christian Seberino:
you
are talking about speed now i it's my
understanding that rust is it's you it's
competes in the same space as c and c++
its kickable you can write low-level
code that's fast with rust so can Scala
compete on speed with the parity client
for example 





Carlo Vicari:
also hold on before before I
forget to do this in the show there's
anyone listening that was interested so
this is uh this is definitely one of the
reasons I couldn't say what it stood for
before I totally forgot that so HD
stands for hierarchal deterministic okay
and that's the hierarchy I guess refers
to what I was saying about the wallet
and the sub wallet and this is from bit
32 and the exact definition is it'll it
says it allows for creating of child
keys from parent keys and a hierarchy
and it said HTTP protocol
okay so anyone that was interested in
hearing the rest of that but go ahead
sorry so





Radek Tkaczyk:
 so we had back to your question
Christian I think yeah rust and and go
and have that kind of advantage of the
skeletons they're just just result in
faster code but I don't think that that
is that much of an issue here I think we
really need to just look at our
solutions and and so I think we can we
can get quite close towards or even
better than what parity in get achieve
and besides if we find out that Scala is
a limitation there is a project called
scar native which compiles directly to
machine code so my 



Christian Seberino:
yeah I was that was
what I was gonna mention next since you
said you liked Python you may be
familiar with the common practice of
writing C extensions that you can
integrate with your Python code so I can
imagine there's no reason you couldn't
make extension for the bottlenecks in C
or something else 






Radek Tkaczyk:
right yeah 




Christian Seberino:
can I also
before I forget I wanted to ask you so
about the so people have an
understanding of the differences in
these languages it's my understanding is
so I've heard Scala is better for
concurrency if you have several cores
several CPUs that Scala is the code is
is great for that is that correct that's
an advantage in comparison with like go
and rust it's the one it's more
compatible with multiple cores is that
correct
did I hear that correct 






Lukasz Gasior:
so to be honest
I'm not too familiar with go and trust
and confidence in those languages about
in Scala well it's running on the JVM so
the possibilities are almost the same as
for Scala well and also Java there's the
archive framework and that's the
framework that we are using and it makes
it really easy to work with concurrency
and and it really makes things much
easier than working with threads
directly and using logs and so on so
we're here




Christian Seberino:
 yeah it was your style
functional for the most part in Scala I
would you say 




Lukasz Gasior:
I think in our deepest no
no of course that means we try to be as
much functional as 



Christian Seberino:
I think the reason
that people think Scala is great for
concurrency in multiple cores I think
it's the functional nature is what makes
it easy to be 



Lukasz Gasior:
yeah 
BLA BLA BLA




Christian Seberino:
so we've covered a
lot of the Scala client we've talked
about the potential names we've learned
a little bit about you and your
backgrounds we've learned kind of some
what you want to see in the future did
we did we miss anything
Carlo Lukas anything else you want to
add oh 






Carlo Vicari:
um my favorite question is always
and some of the more grounded people
which I guess I'm definitely not
grounded in this in this industry but
what do you guys think what are some
far-off use cases you guys see for
crypto currency or blockchain and in
five years or ten years any any wild
scenarios or anything any kind of crazy
use cases you can see in the in the
future the distant future mm-hmm what
are what are some use cases that you can
kind of brainstorm or think of off
pop your head if you had to guess





Christian Seberino:
 so I
think that replacing Fiat money was
definitely a good one that's a as a
possibility well right third world
currencies first and then more and more
of the developed world currencies 



Lukasz Gasior:
that
would that would be a big thing other
than that I can think of anything top of
my head that's already the whole world




Christian Seberino:
could be running on Scala right if the
whole world starts using a theory and
classic they'll you be using your code



Lukasz Gasior:
that's 
MY DRIM WORK




Carlo Vicari:
what about erratic any any crazy
use case scenarios you can think of off
the top of your head



Radek Tkaczyk:
 no would serve some
sort of use cases with I think at the
end of the day there's always the real
world question whether the legal system
of your country recognizes that



Carlo Vicari:
 let's
let's pretend let's pretend there's
nothing in the way no no Uncle Sam no
crazy government no nobody's in the way
what what can what can blockchain do if
you if you could do it 



Radek Tkaczyk:
I don't know 




Carlo Vicari:
you
can if you can dream it


Radek Tkaczyk:
EXTRFYGHJKGHJ 43:07



Carlo Vicari:
 yeah I think
that was the first thing ever that's the
first transaction ever the pizza so okay
so how about smart smart cars
self-driving cars all this gonna get
tied into the blockchain so now 




Lukasz Gasior:
maybe
IOT yeah that's right interesting but
personally well I don't see a good
reason why I couldn't be centralized
because
IOT devices in your home you can also
have the server for them in your home
why did he come watching but maybe I'm
just not too much into the subject 



Christian Seberino:
oh oh
well I can I can answer that so yeah
what one idea is that in the future
people are gonna want a date of mine
they're gonna want access to that data
so people are gonna buy buy and sell the
IOT data and so once you have commerce
then you want the trustless system a
blockchain cyst and that's one reason
I've heard 




Carlo Vicari:
yeah I guess it would also
avoid the honey pots of data and stuff
like that correct yeah so smart smart
car smart drones smart homes IOT
blockchain is all that there's all that
gonna be on blockchain you you think so
Christian 




Christian Seberino:
yeah I don't see why not I
just wrote a paper about the blockchain
system's replacing the web potentially



Carlo Vicari:
so oh yeah that's right I saw that pop
up yeah for anyone listening Christian
you got to put that in the description
for anyone to check out okay yeah
definitely yeah I think so as well I I
think it would be kind of weird if all
of those things were you know and if IOT
was from some centralized database I
think that would be strange but then
again I I really love blockchain and
cryptocurrencies so I'm probably just
very very biased 




Radek Tkaczyk:
on that what's really
lacking is some way to access big data
and there were some proposals made for
for it what was it called some sort of
like temporary thing 




Carlo Vicari:
I'm glad I'm glad
you brought that up because I think
there's some things popping up very soon
that are gonna be utilizing stuff like
that I don't want to say too much but I
think there's some cool things coming
out that are
something like that 





Christian Seberino:
no but just just
address your your point here you're
right I the blockchains like a TC needs
said this is what I actually put this in
the paper that I just posted so yeah you
need other additional storage systems to
supplement the blockchain system like
the interplanetary file system ipfs and
so yeah if you you would need additional
services yeah and together they could
make a compelling complete alternative
to the world





Carlo Vicari:
 yeah there's also SIA and
storage as well I don't know if you guys
are heard of those yes he is very good
storage good team as well




Christian Seberino:
 yeah but that
Lucas is right the blockchain provides
the trustless property but you wouldn't
you know it's too expensive to use the
blockchain system for all of your
storage 






Carlo Vicari:
oh yeah no no absolutely no SIA
does something where they just utilize
the token so that they're actually
storing your files encrypted across the
network of other people's hard drives or
something 


Christian Seberino:
like that yes 





Carlo Vicari:
yeah it's not
actually the data inside the block I
mean the house 


Christian Seberino:
just the hashes 





Carlo Vicari:
right
exactly exactly 
just the hashes of the
data but so I think we covered you know
background we covered how they got into
tech into blockchain Scala client crazy
future use cases I is there are there
any topics or anything in reference to
the I which case Scala client that you
guys think we should touch upon or let
everybody know about I mean what would
you guys like to let the people know
before we we sign off here shortly



Lukasz Gasior:
there's the backcombing( A BITA COMMENS) they do 




Carlo Vicari:
okay got
you got you how about 


Radek Tkaczyk:
DON'T BREAK IT






Carlo Vicari:
don't break it 




Christian Seberino:
I just I'm just so happy
that there's deep subject matter experts
so that the number of subject matter
experts is growing in the
DC community so I'm very glad that you
guys did the hard work of reading the
yellow paper for weeks months and
looking at code that's great I'm sure
that you'll be a valuable resource 




Carlo Vicari:
in
the future and for anybody listening if
you're if you're watching or listening
on YouTube post some suggestions for
what you'd like to name the etc' scarlet
client now copy/paste those over to
maybe a thread and and don't can talk
and debate and think about it
so again Lucas Radek thanks so much for
joining us today really appreciate it
and you know we'd love to have you guys
on again sometime and we're really
looking forward to everything you guys
have worked on appreciate it
yeah absolutely
okay guys for everyone out there
listening thanks so much again tune in
next week take care
right
[Music]

Christian Seberino:
if you are passionate about anything
related to aetherium classic

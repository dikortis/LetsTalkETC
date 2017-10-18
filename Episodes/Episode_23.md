# Let's Talk ETC: Viktor Tron - Swarm, Distributed File Storage & ETC Support.
Carlo Vicari:
hi everybody you're listening to let's
talk et Cie I'm your host karlovy along
with my co-host dr. Christian Sabrina
we've got a really special guest with us
here today but I'd still like to go over
a couple of recent events that have
happened in etc' community we're really
excited about the release of the mantas
client for etc' from IO hk's mantas team
it's still in beta right now it's a test
net beta only version but we're really
encouraging anyone out there in the
community to test out the client as much
as they can leave us some bug reporting
I put up a daily bug reporting thread on
the reddit as well as there's a mantis
bug reporting channel on slack so any
experience any issues you guys are
experiencing with the test net release
or the beta release of this mantis
client let us know it got some really
cool things planned after we iron out
all the details with mantis and hooking
it into a bunch of other things that I
will get into any specifics but there's
some really cool stuff in the pipeline
for mantis so anybody out there who
wants to try out the client and let us
know what's going on we'd love to hear
your input I'm looking to possibly next
week have onto the Mantis team to talk
about you know everything that they've
achieved the last six months they've
been at it a while creating this client
so we'd love to have the whole mantis
team on for a little bit of
congratulations now that there haven't
been any major bugs reported the team
lead has been taking a little break
since you know he's been doing so much
work non-stop on the client for such a
long time so when he's back or possibly
even before he's back we're gonna have a
bunch of the team members on here for
community questions and to just hear
about your experiences building out the
client but to get back onto the real
exciting part about today's show we have
excellent guests with us today
Victor thanks for joining us we're
really happy to have you on here





Viktor Tron:
 hey
guys nice nice to be in the show 



Christian Seberino:
so it's
Victor Troy yeah Tron's your last name




Viktor Tron:
yes correct 





Christian Seberino:
all right 



Carlo Vicari:
well seems things
don't get much cooler than that by the
way
John but so Victor I don't know if
you've got had a chance to you know
listen to a couple of our shows but
something we really like to do is have
the community get a more down-to-earth
feel for the people that are working on
et Cie behind the scenes and the cool
stuff that's going on so just so that
everybody kind of knows about the
developers and the teams that are
working on et Cie behind the scenes we
typically like to go through a little
bit of you know how you got into tech
from there then how'd you get into
blockchain stuff like that so what's
kind of your your backstory how'd you
get into you know working in into
technology and have you always been
interested or did you kind of get hooked
later on in life






Viktor Tron:
 well first of all I'm
not sure I'm best categorized and it's
working on etc' but I'm working on
blockchain ecosystem right I mean look
irrelevant relevant to et Cie and
hopefully hopefully at some point even
integrated and and and compare
definitely competitive movie did you see
oh yeah 




Carlo Vicari:
no I'm sorry go ahead yeah I'd
love to hear about how your rabbit hole
down into this world crazy world 



Viktor Tron:
yes so
originally my my career hat is more more
like natural language processing and
computational linguistics but as time
went on in my life I became more of a
generalist and and did lots of bigger
software development projects I've been
interested in in in Bitcoin and the
blockchain from not super early on back
from 2011-2012 and doing some hacking as
well in the the bitcoins around the
Bitcoin client that it was mainly mainly
just an interested in the technology in
the social impact it has
saying remain from an ideological
perspective the tower at the time I came
to know about it even I was always
interested in technologies which foster
individual liberties and just you know
give back sober knitted to people to to
do direct transactions would be read
with without intermediaries right and so
I was I was mining Bitcoin as Welland in
general I was just following following
an attack and right and when vitalik
presented the Assyrian paper in Miami
conference I saw the video right away is
in January 2014 and then in February
Gavin wood came down to London and I was
living in London at the time and I met
him I saw the talk I was I believe the
first theorem talk the italics
presentation and I was blown away I
thought that this is this is really cool
obviously it cannot work yeah I see
Beauty work and so I started talking
with Gavin and a few days later I
submitted my one-liner contribution to
the to the C++ code is okay
turned out to be my first and last
contribution to that code base and and
you know from from from there on his
history really
and so I joined the during the Skype
channel you know started conversing with
people just started contributing to the
to the Go Go client and yeah got to know
Stefan to a Jeff Jeffrey wiki and the
rest is history so I worked quite a bit
on on various bits of the go client
the first half year and dedicating a
quite a bit of my time
in fact that at the time I was working
for the BBC come on a project and in
that spring I reduced my hours to two
basically three days a week so that I
can work on it period
and I definitely got lucky because when
when when the crowd see happened and and
the etherion pan Asian was was was
formed and and finally had some funding
I was out here the first to be offered
the job and I've been I've been working
with the foundation ever since and and
so after after a while of course and
when Gavin was writing the yellow paper
I was I was doing some proofreading with
him and you know my skepticism just
slowly slowly disappeared and I really
understood that these people are
geniuses and really really thought about
everything that I got convinced that
it's a workable thing and that that
really made me very very enthusiastic
and to the other studio my enthusiasm
hasn't hasn't decreased one bit since
background my professional interests and
skills and the line I mean I did my you
know social prospects them right right
the way I would like to see the to a
change 





Christian Seberino:
so today you have a really really
deep knowledge then of aetherium if
you've been hacking on the clients and
then if you have a natural language
background that's pretty abstract pretty
complex stuff so you you must have a lot
of talent that you bring to the table
can you also describe how you became the
involved with swarm and what's your role
there 





Viktor Tron:
yes yes at the moment and I'm team
lead for this world project so as your
listeners might know sworn alongside
whisper and and they still in blockchain
and formed but what's funny they called
the Holy Trinity of ECU which so the
context of this is that very early on
the the founders of the theorem
recognized that that the public
blockchain is pretty much the last the
final missing piece of the puzzle to to
to web think about the think about the
old dream of this and tries the Internet
you have all these wonderful
peer-to-peer technologies which have
been in development for like some twenty
thirty years even
but what's what was really missing is
incentivization which make these these
technologies I'm thinking about like
messaging enjoy for content distribution
which made me see spear to their systems
stress self-sustaining sustainable and
so now it was always on the agenda of
the foundation to develop what became
called web three so the returns return
to the original idea of completely
decentralized Internet and so now the
original narrative was that if if a
theory on blockchain is the public
blockchain is D is the worst computer
CPU
then swarm is the word computer's hard
disk and yeah and so swarm was always
always part of the making foundation set
and 





Carlo Vicari:
now sorry just a backtracked I was
hoping for anybody listening out there
that might not be is familiar if you
could tell whoever's listening that not
is not as familiar a little bit about
web three just kind of maybe a general
overview about about what it is and it's
real
to web one versus web two and obviously




Viktor Tron:
not necessarily established categories
is more like more like a half joke
so that trees the cooler and the of the
totally decentralized Internet what are
we talking about in the context of swarm
especially like web one is the time when
you when you had your own server you you
uploaded your sites where DP you know
you you have to deal with all kinds of
scalability issues if you if you had a
blog post which suddenly became popular
you had to bear the read the cost of the
cost of serving you are your customers
and if you if you were lucky to write
something that a lot of interest then
you actually a lot of times got unlucky
because your server crashed but but at
the time you you had more or less full
control of your of your content
you basically own your content and the
web two times is when a lot of you know
companies came and offered solutions to
to put like scalable solutions to host
websites and that's when when
interactive real-time interactive web
applications became popular and this
this is still the time that we're living
right now test web to men you can get
very good services and and scalable
solutions very cheap four or even three
however it comes with what my colleague
Illinois Dan it term that's the Faustian
bargain that that that you really really
increase you lot of control
right where your content and and this
big companies who who own your data and
basically monitor your usage and and use
use the user profiling and and and yeah
not even up thanks for free
since the sheet end and yeah and after
all have to have a lot of influence on
what's been the Internet and this is the
situation which web free is set out to
change and go back to the roots and and
basically completely DECENTROLAIS 



Carlo Vicari:
nice just that's
just to make it a little bit more more
clear maybe not that it's not clear but
can you give our audience a good example
of like it doesn't have to be something
even close to being possible yet but an
example of a good well you know really
cool like web 3 application that you
would love if you if you could have one
web 3 application you know in your
pocket well be a Bitcoin is how would it
function right yeah 



Viktor Tron:
yeah I mean just
think about it just like a baby a most
obviously or Facebook right I mean to
have to have status updates publish
status updates and let your friends see
your status and comment on it and and
having a platform and meant where people
can share things do you really do we
really need a company behind this this
is this basic question that if you if
you realize what your technology is
currently able to to do you realize that
it's not really necessary needed and
it's the most of these tasks it can be
can can can run against a decent life
and baselayer infrastructure 





Christian Seberino:
yeah Victor
can I make a comment tell me if you
think this is correct so I agree that
not that these terms are loosely defined
so my my understanding was that Tim
O'Reilly
popularized the term web 2.0 and like
you said one of one component one
attribute was the fact that you have
strong interactivity like for example
with with YouTube right where people
don't just receive content they post
content they there they could send
messages and dialogue so that was web 2
as interactivity and then web 3 them
they what was missing was the trust
lessness which is the blockchain
property that's not communicated by the
web and and so the idea then is to make
a trustless web through the technologies
you're talking about but yeah okay good







Viktor Tron:
so so let's focus on this a little bit
so okay so so interactivity and and all
these beautiful things like and not so
beautiful things like JavaScript but but
it's very useful obviously saved over to
the to the Europe web 3 because they
proved to be you know very very very
useful and and very important in you
know automating and things and give a
very good user experience on the web and
made it possible like with the
interactive web applications however
just concentrating on on the content
context of Swamper a minute what's
what's really apparent here is that we
mentioned restlessness obvious like for
for payments and and and a lot of other
you know direct interactions at the
moment you need you need the need and
you need the trusted third party and
that's that that's that that is very
very useful to this intermediate because
as SS trusted third parties and you know
some sort of centralized institutions
they constitute a single point of
failure and in many ways so if you
MasterCard is she shut down and you know
what well or even just like simple
simple case like the very fact that most
of the website of the current web to
running on actual servers and servers
are in the hands of hosting companies
and major point of attack for whatever
reasons either the authorities or or the
technological Devils can knock on their
door and and easily easily wreak havoc
and and then create create big problems
because it's it's it's it's relatively
easy to meddle in the system so that so
that that single point is compromised




Christian Seberino:
yeah I was reading about yeah Gavin when
he describes web 3 he calls it the post
edward snowden web so i thought that was
interesting so the internet originally
wasn't really developed security wasn't
a primary consideration radios for
academics and so we've the the web the
internet and the later the web has
they've slowly added security east by
piece whereas the the web 3 is kind of a
vision of what if the let's try to make
the internet work in a completely
hostile environment where you don't
trust anybody and even the the computers
on the network that contribute content
you know even even the nodes can't
aren't necessarily trusted a completely
hostile environment so to me that just
seemed like the inevitable logical
conclusion of making a secure energy




Viktor Tron:
 so
we talk about the two different things
and important but for the for the
listeners maybe we should just sum up
that we talked about you know security
like sovereignty over your over your
data and then we talked about in the
censorship and and
so whether all the technical problems it
can can influence the operation website
and just just to summarize so the the
common theme here is obviously some sort
of centralized component the moment the
moment you have yeah ways to distribute
an and your data to to host your website
in a decentralized way to message people
without having like a central server
that your message is good a lot of these
problems can be mitigated




Carlo Vicari:
 yeah and
that's what that's referring me and
that's what brings me to my next
question about I now that now that the
audience knows a little bit about web 3
and decentralization and these not
single points of failure if you could
maybe tell them a little bit about a
little bit more about swarm and what's
what's that swarm apart from some of the
other solutions out there and you know
what would excites you about swarm and
you know just a little bit about






Viktor Tron:
 maybe
maybe let's summarize what what what's
common to toward peer-to-peer solutions
of content distribution and and and and
document storage systems the ones that
I'd emerging right not a decent price
ones and I have a common goal and and
and usually it's also a feature that
they managed to achieve that they can
achieve censorship resistance because if
if content is distributed in a we can
and fashion across we centralized
network of nodes then it's very
difficult to
look on anyone's door - to get that
content off and this is this is an
important feature for for for the
freedom of speech and in the in general
like the the Creed what that information
wants to be free
secondly they have a very strong poor
tolerance because of the redundancy and
the application of content across nodes
they are they are for pure intent and
ideally day they can achieve zero
downtime properties for for like hosting
websites so so these are these are the
is that the common features that have
unite or the project in the space that's
our team let's name the beast that's
close to my heart I have two Swami's
ipfs very good terms with the with ipfs
developers protocol apps guys and we've
always been you know trying to
collaborate and and you know compare
notes with the same with them and the
Junction's like like storage like saya
saya so what's the time 




Carlo Vicari:
yes what what
well I'd like to hear about what sets
warm apart more specifically the 




Viktor Tron:
form
unit if you just concentrate on the on
the actual document storage and content
delivery past x1 because later only
probably touch on a bit broader aspects
wat suan things primarily narrative it
it's basically the the data storage and
content delivery Linea so in that
respect the main
that sets wall apart is that and this is
the reason why you should be refrain
from saying that swans file sharing
system Oh slice faster firing system
because there's a genuine sense each one
can be considered the cloud service
there's a genuine sense in which you can
upload content to Swan it's not unlike I
like the regional paradigm started with
Napster's and nutella's where you may
get files on your hard disk and
basically she opened up access to those
files and this is how your file sharing
here your peer-to-peer storage started
as opposed to death model swamis is open
up part of your hard disk but it's not
it's not that you open up access to
files that you store rather how Swan to
decide what content will be stored on
your own the hard time I think I'd
remember saying that but the end point
is that you can upload you can change in
the upload stuff to work without even
having a hard disk so it's like a cloud
service where you when the cloud can
just receive your data and host your
host your website etc do that you
necessarily even having I mean to have
hobbies face yourself 




Christian Seberino:
so now unlike
Napster you're not just sharing files
you could also contribute files that
other people store for you that Napster
didn't have that ability 






Viktor Tron:
so correct 



Christian Seberino:
yeah
one thing okay





Carlo Vicari:
it all comes back to Napster it always
seems that everything it's so crazy
everything
now go 






Christian Seberino:
ahead Victor have you ever seen
or heard of van Jacobson his talk okay
so I said I was blown away he gave a
Google Talk he's apparently the
networking expert works at Xerox PARC
and he was describing the history of
networking and how it's evolved and so
and how I went you know first it was
telephone network and then tcp/ip
connections and he was saying okay today
what happens so the the TCP was
basically like a better it was a better
telephone it was more resilient to
cetera et cetera but today we don't
really care about connections we only
care about content and the way that we
address content on the web right you
have to like you say I want to see the
New York Times I have to type the
location of their web server but we
don't care about the location we only
care about content and he was talking
about making a a content addressable web
which you would agree that swarm is
content addressable so I thought that
wasn't bringing




Viktor Tron:
 that up this exactly the
next topic I was gonna see it's a
unified solution used across the various
decent tries the hosting solutions what
is the content and best thing is it's
based on the idea that that that the
routing would the way certain content is
retrieved it's based on an address that
address is deterministically derived
from the content of what you wanna see
how it's done this is not so important
that it's basically a hash some sort of
hash function like an one reaction
function which is similar to all kinds
of fingerprints that they can create a
unique identifier from from an arbitrary
size
now what might is this interesting
content addressing is is has a has a
very immediate consequence which is
called integrity protection so in
today's web you often hear that has been
hacked it means that someone when is
talking to a server and substitute
different content from what's supposed
to be there
now with content addressing this is
impossible because the the address
what is fingerprint that's created from
a content is simply changed even if you
even if you want to find one bit of the
original content and therefore if you if
you if you look up an address and at
least the routing aadhi aadhi what a
service layer that serves you the
content is is not compromised then then
the content itself that you see you can
be hundred percent sure that it's
exactly the content that the owner or
originator or creator of that content
once you see so so from the lowest level
up integrity protection is is there and
therefore traditional ways of hacking a
website it's just it's just not even
define a block 






Christian Seberino:
yeah once I when I that
once I heard that and it made so much
sense I wondered how anybody could ever
design any other type of system rather
yeah right it's just so perfect
yeah I mean like with just as an example
if I wanted to download a software for
my Windows laptop so because of the
magic magic of hashes if Microsoft
server is busy I could and let's say
there's a server in Iran or Russia or
China that happens to have a copy
because of hashes I can have a hundred
percent confidence from you know even
some even a location that maybe I I'm is
questionable or I'm uncomfortable with I
can have one
confident confidence that the file is
exactly what I would get from Microsoft
in that example 




Viktor Tron:
you know enough for and
of course this is even more relevant I
mean it's one thing that you might read
fake news or something on a hat inside
but obviously the most important thing
is that okay the payments or what input
to input of a private and and sensitive
data is we're actually even even
downloading a software that you run on
your own computer if you if you if that
software can be just change to another
world don't you think that's the super
dangerous
yeah these kind of attacks are not
possible with with content addressing




Christian Seberino:
that's right
now would you say that swarm is takes a
lot of the good ideas from BitTorrent
and kind of just expands on it right





Viktor Tron:
Bittan say that swarm is basically for
people who are not so tech savvy I
usually say that think of swamis as
BitTorrent on steroids
because after after it's based on the
same idea affair you know distributing
content 



Carlo Vicari:
a good one I'm gonna tell
everybody that's warmest I've always had
trouble explaining it so I'm gonna steal
that I'm saying Bitcoin instead




Viktor Tron:
of
course of course let's be let's be fair
here so we use a lot of the basic ideas
what would be torrent uses but we also
incorporated a lot of normally not
innovative solutions that let me sterile
mix one potential yeah potentially use a
go for low latency so having low latency
real time web applications which which
at the moment BitTorrent is not able to
do because of because of the delay in
the initial download of of assets and
yes and more fundamentally
or systemically the problem BitTorrent
is lacking the incentive layer which
makes it different is currently running
running on running on vanity tokens
right and some some geeks consider it
there to maintain like 



Carlo Vicari:
I don't go ahead
I don't know if you have I'm sure you
have worked more questions on this topic
as do I but there's something in our
pre-show notes that I want to touch upon
before we run out of time okay
III saw some notes about volunteerism
and crypto Anarchy you know interest
that I'd love to know that our Vic I
mean I'm I'm very into the
non-aggression mister Bowl as well but
I'd love to hear hear more about you
know your your life is a you know
digital digital nomad as you said it and
somebody some of your thoughts on
free-market volunteerism and in this
advent of crypto Anarchy year however
you want to say it





Viktor Tron:
I mean I don't want
to pretend that I I'm too savvy about
this topic but it's just clear that my
ideological leanings are somewhere
around there
yeah I'm true believer that that's that
the blockchain can finally bring about
the emancipation of a lot of areas of
interaction between people resistance
that the the free interaction between
individuals or or basically two signs of
a value transaction
I'm not invaded by by any Intel media is
putting putting restrictions on it
either either either via their business
interest or or well basically just some
sort of cultural legacy of a regulation



Christian Seberino:
yeah so what you're saying you're saying
that it's a political it's political for
you not just interesting to
Knology i think it's the car one of the
points 



Viktor Tron:
anyone that's that's that's was
definitely my one of my main motivators
that my my professional interesting and
skill set align so well the way i would
like to see the world change or or
improve






Carlo Vicari:
 victor wouldn't you say that you
were kind of talking about the
centralization of data earlier on these
servers which is a honeypot for attacks
correct its kind of the way that money
has been controlled for all these years
kind of left a honey pot of money in the
center that then that gets spent on a
whole bunch of military buildup at least
it's my opinion that wants all this
money lies again and there isn't this
honey pot of money a lot of this
military spending in all these you know
powerful countries around the world will
have to decrease what do you think is
that kind of your 




Viktor Tron:
I'm definitely I
definitely resonate with that see that's
what we're call it dream yeah I really
hope that technology helps driving the
world to towards that situation where
whether you know the political systems
you know financed by the kind of central
bank system and let's be let's be humble
here like at least lose it lose it 




Christian Seberino:
so
can I ask a question Victor all right so
I'm just like with blockchains I'm a
hundred percent confident that anybody
that investigates the technology of
swarm and related technologies will will
will believe that this is there's so
many good ideas here and so much so many
better ways to make a file distribution
system or as you said
cloud service now people that when the
light bulb goes on and they start to
research it they hear about swarm they
hear about
ipfs like there's other even other ones
now so can you talk a little bit more
can you guide people on the differences
and how they all 





Viktor Tron:
I already touched upon
one important difference which is the
the genuine sense in which you can
upload stuff to swarm and therefore you
don't necessarily need lead your hard
disk and that's why I don't like to use
the word a file sharing system it's
actually it's actually genuine cloud
service in a way decentralized answers
another important difference with for
between IP FSM and I think SIA coin and
others as well that the aspects of
incentive is Asian so so how FICO any
set out to work as far as I know the
latest it's based on the idea that file
storage works a bit like mining so notes
compete in proving that when they're
challenged whether they have a certain
file and they they prove that they have
it and therefore they get some reward
and as a result there's some sort of
positive incentive ization that the
files are preserved however we found
that this is just one side of the coin
no pun intended 




Christian Seberino:
so just a clarify so
believe I don't know file coin is the
ipfs interplanetary file system solution
is that correct
for incentivization 







Viktor Tron:
yeah okay Mike when
is exactly which is confusing a bit on
this theorem okay and we believe that
this might be overall a good good scheme
for incentivizing no it's to to store at
all however this is the insufficient
protection for for to preserve unpopular
content why is that so so
that I upload my family album when my
birth certificate to Swan and I really
wanted to be available but maybe in ten
years time and in the next ten years I
don't even look at it
what what am I going to do it's unlikely
that with positive instant we station I
can guarantee that those files are
available so what we do instead in Swan
is we introduced the kind of insurance
type of scheme whereby nodes who either
explicitly or implicitly become
responsible for storing a piece of
content here piece of content
technically just a chunk of data because
every file is channeling to little
pieces but this kind of virulent
so anyway nodes that I'll and up
responsible for storing content can be
can be directly had liable which means
that there's a there's a prospective
punitive measure inflicted on them if
they are found to be guilty of losing a
file and and that that that we believe
is a much stronger incentive to ever
have network where by the fact that you
just want to ensure and want to preserve
and actually guaranteed to survive okay
are unpopular its popular content can
easily be incentivized by the reward
that you give for serving the content so
so you don't even necessarily need
insurance for them but but unpopular
content well let's say like let's see
rarely accessed content more subjected
to loss 




Christian Seberino:
okay so if I understand you
correctly it's the your commence is the
incentivization so you think you have
better
incentivization system and and so that
would be one reason why somebody might
choose swarm over ifs okay






Viktor Tron:
 correctly so
someone is not exactly what second is
incentivization especially in terms of
punitive measures for for unpopular
content and preservation of file
and and thirdly certainly a lot of other
goodies so okay





Christian Seberino:
 yeah those the two big
ones okay is there any other competition
besides ipfs that's on your radar 





Viktor Tron:
I mean
let's start storage and and and SIA are
already existing and and production
level solutions and in some in some ways
they can be good you know alternative
solutions and competition however the
scope of their solution I believe this
is a lot narrower than what we set up to
swamp to try 



Christian Seberino:
get more ambitious like



Viktor Tron:
 we
might and that end up being the dummy so
for this one project and the momentum
I'm very I'm very optimistic because it
looks always good okay swarm is very
important story short signs a very good
design and from very early when it's
kind of a lot a lot of solutions to
problems and fell out hope of the design
without even that's like researching and
thinking about them it's kind of very
interesting 





Christian Seberino:
I can ask you another
question so go ahead add something



Carlo Vicari:
 yeah
I just wanted to you know before before
we run out of time I want to ask a
couple of key questions kind of like
maybe to give the the listeners a little
bit more guys were where you guys are at
where you're going so stat I need to
tell everybody about kind of what's on
the short term roadmap then I think they
have an idea of the long term room mat
but what's on the short term roadmap and
are there any gaps already available on
swarm or is all this 





Viktor Tron:
a few basic there's
a few basic depths like a like an is
this distributed photo album this
there's a markdown viewers and some some
very very basic basic that's already
exist but in fact the the mist wallet is
also hosted and so on so pretty much
everything that you can do in in
JavaScript and
and in the urn and of static or
client-side
the solutions are able to now right now




Carlo Vicari:
so it's your fingers you know that it
could make up that that does isn't
around yet which Jack would it be what's
your your dream tap to have for a swarm
that you'd like to just get it done
right





Viktor Tron:
 away these centralized  YOUtube 




Christian Seberino:
oh
yeah
nobody would ever doubt web three if you
could do that




Viktor Tron:
 yeah life beer that let's
set up to implement a decentralized
media server end and streaming solution
for awhile and we also support streaming
via my swarm and we have a collaboration
with the connecting Wow adapted mighty
beat rate 




Carlo Vicari:
okay let's get let's get
people excited till decentralized
YouTube launches in the same popularity
way that YouTube launched and that
didn't launch but the way YouTube caught
caught on fire in like 2007 2008 how
long till the decentralized YouTube does
that 





Viktor Tron:
well you know just because I'm I
can only say that the basically our
infrastructure that the technology core
part that makes it possible
we probably be production ready in
spring 2018 and from then on I mean from
my perspective it's just the skin and
the UI that will make YouTube possible
however what you're asking about mass
adoption requires a lot of guesswork in
terms of marketing and mass adoption
hinging on other factors than just
technology and I'm not the best person
to answer these questions so
what is the kind of a perception of
every space in general so just think of
Bitcoin that was long associated with
like no dark markets of druggies and and
then and things then but this didn't
actually have the adoption too much and
I'm not saying that it's the same it's
not the case anymore with the theorem
however such factors can be of
importance in in the mass deduction



Christian Seberino:
adoption is hard to predict yeah
Dex arranger said 2019 Dex Iran is an
active developer in aetherium classic
and he wanted me to ask you about so so
he's focused on aetherium classic year
and then people some people are focused
on aetherium and he had a plan to try to
make a common a swarm port or system
that could work across different
aetherium ports different 




Viktor Tron:
I'm fully
supportive of the NBN and in fact me you
would like to makes one right away
compatible with the blockchain solution
at the moment it's not the case and
we're really working a tightly
integrated with ETA but the smart
contracts that the incentive layer and
and the domain resolution is using we
pick at the two aspects image you know a
swarm is related to the blockchain at
all these two aspects type are based on
the capacities for a blockchain to to to
be able to implement we have where smart
contracts basically I'm not even saying
that it needs the full power of of a
Furion complete system but in effect I
[Music]
would I would not even dream of starting
to the port swamp to to Bitcoin for
example but as long as there's some
reasonable complexity or expressive
power of the of the smart contract
language
let's say let's say if if it's still
incomplete then definitely there's this
compatibility and 



Christian Seberino:
there's no there's no
technical reason why you couldn't have
swarm work across several blockchain
systems with sufficient like you said
scripting scripting language
sophistication that 





Viktor Tron:
if in fact in a few
years time there's going to be standard
solutions for for inter blockchain
communication like we already have polka
dot and Cosmo and on all kinds of
solutions in them in the window making
which will make it possible to to have a
crosswalk change solutions and I think
once this time comes it's gonna be less
and less relevant to what blockchain you
use okay okay so critter subjects one
itself so one mid staff can even the the
one one single global swarm can actually
could actually just use several block
changin and you know what what people do
there appear to be dealings in would be
left to their vacation
alright 




Christian Seberino:
so people should definitely look
into swarm then for the future of cloud
services and file services 





Viktor Tron:
let's be fair
the same is probably true of ipfs and
some other solution so let's be fair






Christian Seberino:
yeah do you have any predictions couple
years like five years from now what do
you think ipfs 





Viktor Tron:
where are they gonna be
funding yeah it probably a good position
to to churn ahead with there with there
was some tech 




Carlo Vicari:
yeah they have a little
bit they they just have a little bit of
runway 200 minutes 






Viktor Tron:
okay compared to that
and the swamp project is the
not somewhere funded but i won't i won't
be complaining because the union
foundation is also you know strongly
supporting us and has a relatively big
pot 





Christian Seberino:
so iko iko why don't you do a swarm
i co start a company and get become the
chief their wealth super well-funded
what about that idea





Viktor Tron:
 this is that put
upon their banner to develop sworn it
would be would you rather it is
ingenuous for the for the foundation to
suddenly really encourage this project
and and it was to be the company on that
and raise extra funds work or something
is gonna begin promised and 




Carlo Vicari:
which which
brings me which brings me to my next
question that i know you want me to ask
really bad what's your favorite that's
your favorite ice ee okay so it so first
okay so you get first listening out
there this was just before the show of
it just like I just don't want to talk
about I see us just don't I don't want
to hear about it I don't want to talk
about which I think everybody's had it
up-to-there
yeah but uh so well avoid well avoid
that but I think no now I know you know
we're kind of the origins of you know
your your background how is how you got
into you know aetherium and and
blockchain your you know political
political leanings as far as you know
non-aggression principle and and free
market free market volunteerism as well
as swarm where its origins where it's at
now where it to be I'm definitely
rooting for decentralized YouTube that
would be awesome
yeah I I think you know I'm really happy
to week a chance to have you on the show
before you go maybe you could tell
everybody a little bit about your your
digital Nomad life how many are you are
you in a bunch of countries all the time
doing all the stuff or have you been
kind of





Viktor Tron:
 yeah something right traveling
in the past two years basically
constantly yeah some of these travels
were motivated by my duty to evangelize
and like give talks but the other time I
just like set out to me I mean we people
who like working working the digital
space and especially programmers in a
very rich position I'm very grateful to
to be able to work anywhere where
there's internet and a laptop which
includes you know any kind of
environment and and I just like to like
to enjoy that lock hand and seek out
places which I live okay around work
from various places 





Carlo Vicari:
are happy as you say
all this in the community are happy you
enjoy it because you're killing it you
guys are doing doing big stuff man 




Christian Seberino:
you
said now everybody always could use more
funding but is there anything else that
you need if people want to support swarm
a science funding of course




Viktor Tron:
 yes thanks
for thanks for asking I mean helping
hands are always needed so if you are a
developer dear listener please come to
the to the Geetha chat the public swap
channel or come to our engine room which
is called the orange lounge and please
please feel free to contribute or just
watch a little and see how how work is
done in our quarters to receive to
receive help from developers and of
course if you're not a developer just
spread the word and you know enjoy enjoy
using this




Christian Seberino:
 technology and tell people
about the a your ambitions to replace
the internet with a new improved or the
price replaced the web with web 3 very
ambitious vision yeah I think we've
covered everything
a carload anything else you have




Carlo Vicari:
 no I
just wanted to uh I just wanted to thank
Victor for for coming on and Christian
you know thank everybody out there for
for listening today to show and you know
look forward to maybe doing this again
sometime good 



Viktor Tron:
yeah thank you very much
and I'm always available 


Carlo Vicari:
okay all right
guys for anybody that thank you guys for
listening to today's show till next time
take care
hey thank you bye them
[Music]


Christian Seberino:
if you are passionate about anything
related to etherium classic

# OpenADP

Open source Advanced Data Protection for everyone

## Overview

This is my wheelhouse. I helped make this happen at Google in 2018gq and Google
is way ahead of Apple in this area. I know exactly how to build it an can have
it done in spare time in a few weeks, at least server side. The whole world
would be able to use it for free, protecting backups, passwords, message
history, and more, if we can get existing applications to talk to the new data
protection service.

However, I need help. I've got the algorithms and server-side covered. This
would be a distributed trust based system, so I need folks willing to run the
protection service. I'll run mine on a Raspberry PI. Areas where I need help
include:

* Running protection servers. This is a T-of-N scheme, where users will need
  say 9 of 15 nodes to be available to recover their backups.
* Android client app, and preferably tight integration with the platform as an
* alternate backup service.
* Same with iOS
* Authentication. Users should register, and login before they can use any of
  their limited guesses to their phone unlock secret.

The scheme splits a secret among N protection servers, and when it is time to
recover the secret, which is basically an encryption key, they must be able to
get key shares from T of the original N servers. This uses a distributed
oblivious pseudo random function algorithm, which is very simple.

In plain English, it provides nation-state resistance to secret back doors, and
eliminates secret mass surveillance, at least when it comes to data backed up
to the cloud. iOS and Android systems don't currently do that. The UK and
similarly confused governments will need to negotiate with operators in
multiple countries to get access to any given users's keys. There are cases
where rational folks would agree to hand over that data, and I hope we can end
the encryption wars and develop sane policies that protect user data while
offering a compromise where lives can be saved.

So, nothing too serious

This project is recuiting!  Consider helping out!

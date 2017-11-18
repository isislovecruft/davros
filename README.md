
# DAVROS: Deterministic And Verifiable Randomness On Schnorr signatures  [![](https://img.shields.io/crates/v/davros.svg)](https://crates.io/crates/davros) [![](https://docs.rs/davros/badge.svg)](https://docs.rs/davros) [![](https://travis-ci.org/isislovecruft/davros.svg?branch=master)](https://travis-ci.org/isislovecruft/davros)

**A cryptographic library for creating and verifing extensible Schnorr
signatures using the
[Ristretto](https://docs.rs/curve25519-dalek/0.13.2/curve25519_dalek/ristretto/index.html)
prime-order group.**

## SPOILER ALERT

*Davros was thought to have died during the first year of the Time War, when his
command ship "flew into the jaws of the Nightmare Child" at the Gates of Elysium
despite the Doctor's failed efforts to save him. But Davros was pulled out of
the time lock of the war by Dalek Caan, using his own flesh to create a "new
empire" of Daleks who place him in the Vault as their prisoner to make use of
his knowledge. Under Davros' guidance, the Daleks steal 27 planets, including
Earth, and hide them in the Medusa Cascade, one second out of sync with the rest
of the universe.*

*In the follow-up episode "Journey's End", it is revealed that the stolen
planets are required as a power source for Davros' ideal final solution: the
reality bomb, which produces a wavelength that would cancel out the electrical
field binding atoms to reduce all life outside the Crucible into nothingness in
both his universe and countless other realities. But Davros learns too late that
Dalek Caan, who came to the realisation of his race's atrocities as a
consequence of saving his creator, used his prophecies and influence to ensure
the Daleks' destruction while manipulating events to bring the Tenth Doctor and
Donna Noble together for the role the latter would play. Though the Doctor
attempts to save him, having earlier taunted the Doctor for turning his
companions into killers and being the cause of the deaths of countless people
during his travels, Davros furiously refuses the Doctor's help and accuses him
of being responsible for the destruction while screaming: "Never forget, Doctor,
you did this! I name you forever: You are the Destroyer of Worlds!" Thus the
Doctor is forced to leave Davros to his fate as the Crucible self-destructs.*

# Warnings

davros and
[our elliptic curve library](https://github.com/isislovecruft/curve25519-dalek)
(which this code uses) have received *one* formal cryptographic and security
review.  Neither have yet received what we would consider *sufficient* peer
review by other qualified cryptographers to be considered in any way, shape,
or form, safe.

**USE AT YOUR OWN RISK.**

## Documentation

Extensive documentation is available [here](https://docs.rs/davros).

# Installation

To install, add the following to the dependencies section of your project's
`Cargo.toml`:

    davros = "^0.13"

Then, in your library or executable source, add:

    extern crate davros

On nightly Rust, using the `nightly` feature enables a radix-51 field
arithmetic implementation using `u128`s, which is approximately twice as
fast.

## Contributing

Please see
[CONTRIBUTING.md](https://github.com/isislovecruft/davros/blob/master/CONTRIBUTING.md).

Patches and pull requests should be make against the `develop`
branch, **not** `master`.

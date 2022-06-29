---
title: technecol
tags:
---
Welcome.

Technecol is a protocol for the decentralized exchange of information.

# braindump

Namecoin invented NFTs. What are the other use cases for NFTs?

## Use cases

    - NFTs for digital artworks
    - NFTs for digital music
    - NFTs for digital books
    - NFTs for digital movies
    - NFTs for digital games

Do you see the pattern? 

### Text as NFT(based on digital art NFTs)
- Character names, similar to avatar pfps, are NFTs.
- Characters maybe in an 'event'. An event has a place, time & context. Events can be without characters.

        Event {
            space: String, // default: 0
            time: String, // default: 0
            context: String, // default: 0
            characters: [Character] // optional
        }

Consider birth of a cryptopunk as an example.

    Event{
        space: 0,
        time: 0,
        context: "cryptopunks",
        characters: [
            Character{
                name: "cryptopunk001",
                description: "cryptopunk001 description",
                url: "cryptopunk001.png",
            }
        ]
    }

All the punks are born in a single event in no special place or time but a context.

When a cryptopunk is used as a pfp, then context changes.

    {
        space: 0,
        time: 0,
        context: "twitter"
    }

Consider NounsDAO, another NFT project for example.
The birth of nouns, unlike punks are separated in a time context.

    Event{
        space: 0,
        time: x + 1*N DAYS,
        context: "NounsDAO",
        characters: [
            Character{
                name: "NounsDAO00N",
                description: "NounsDAO00N description",
                url: "NounsDAO00N.png",
            }
        ]
    }

When someone owns them the context could be the owner or 0, which represents the ethereum blockchain as context.

Next consider artworks that occupy the whole space.
Something like artblocks.

Since artblocks like ringers and ribbons are characters with a designated space, their birth is a nested event.

    Event{
        space: 0,
        time: 0,
        context: "rings",
        characters: [
            Character{
                name: "artblock001",
                description: "artblock001 description",
                url: "artblock001.png",
                Event{
                    space: ringers001 bg,
                    time: 0,
                    context: 0,
                    characters: [
                        Character{
                            name: "ringer001",
                            description: "ringer001 description",
                            url: "ringer001.png",
                        }
                    ]
                }
            }
        ]
    }

Let us put this all aside for now, and revise the products.

- Encore
 It has a tiktok like surface for selling music NFTs.

 A page consists of a track and pages auto-scroll to infinity.
 Like the page to keep playing it and add it to your likes.

Subscribe to an artist to earn fan NFTs.
Fan NFTs have tasks that upgrade them.
These are used by the artists for various purpose.


A pfp is discrete while an artwork is spatial.

---
A 'post' is of a 'mimetype' and has 'content' & a max curator count.
'+' the post to become a 'curator' of the post.

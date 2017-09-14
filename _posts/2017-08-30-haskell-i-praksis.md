---
layout: post
title: Haskell i praksis
category: Arbeidspraksis hos Beat
---

Å lage programvare som skal løse en reell oppgave er
veldig inspirerende. De siste dagene har jeg selv om jeg ikke har
vært i praksis jobbet med Haskell-bibliotek for å koble til databaser.
Jeg har bestemt meg for at jeg liker Opaleye best og satt opp en
[donalddatabase][donalddatabase] på hjemmemaskinen min.

[donalddatabase]: https://github.com/Thomashrb/stack_opaleye_example

```haskell
  conn <- connect ConnectInfo{connectHost="localhost"
                             ,connectPort=5432
                             ,connectDatabase="testdatabase"
                             ,connectPassword=""
                             ,connectUser="postgres"
                             }
```

I dag har jeg derfor jobbet med å konvertere denne kunnskapen til
å lage en kobling til Beats database. 

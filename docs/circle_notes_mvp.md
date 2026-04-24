# Circle Notes App -- MVP Concept

## Overzicht

De applicatie is een **private workspace voor kleine groepen (circles)**
waar gebruikers samen informatie kunnen delen via **notes**.

Het concept is geïnspireerd door family/group apps maar focust op een
**modulaire dashboard structuur met tiles**.

Elke circle heeft een **dashboard (board)** waarop verschillende
functionaliteiten als **tegels (tiles)** worden weergegeven.

Voor de **MVP is er één tile: Notes.**

------------------------------------------------------------------------

# Core Concept

De structuur van de applicatie:

User ↓ Circles ↓ Circle Dashboard (Board) ↓ Tiles (Apps) ↓ Notes

Een gebruiker kan meerdere **circles** hebben.

Voorbeelden van circles:

-   Study group
-   Familie
-   Vriendengroep
-   Project team
-   Gaming clan

Elke circle heeft zijn eigen **dashboard en data**.

------------------------------------------------------------------------

# Dashboard Layout

Het dashboard bestaat uit twee delen:

1.  Top Bar
2.  Board (met tiles)

## Top Bar

De top bar bevat:

Profile Picture \| Circle Dropdown \| Settings

Beschrijving:

-   **Profile picture (links)** -- toont de ingelogde gebruiker
-   **Circle dropdown (midden)** -- wisselen tussen circles
-   **Settings (rechts)** -- account of circle instellingen

------------------------------------------------------------------------

## Board

Het board toont een **grid met tegels (tiles)**.

Voor de MVP is er slechts **één tegel**:

Notes

Visueel voorbeeld:

👤 Study Group ▼ ⚙

Board

[Notes](#notes)

------------------------------------------------------------------------

# Circles

Een **circle** is een groep gebruikers.

Een circle bevat:

-   name
-   icon (optioneel)
-   owner
-   members
-   createdAt

## Rollen

Voor MVP zijn er twee rollen:

### Owner

Kan:

-   circle verwijderen
-   members uitnodigen
-   members verwijderen

### Member

Kan:

-   notes bekijken
-   notes maken
-   eigen notes aanpassen

------------------------------------------------------------------------

# Invite System

Gebruikers kunnen een circle joinen via een **invite link**.

Voorbeeld:

app.com/invite/AbC123

Flow:

1.  User opent invite link
2.  User logt in of maakt account
3.  User wordt toegevoegd aan circle
4.  Redirect naar dashboard

Voor MVP:

-   invite link is permanent
-   geen limiet op aantal users

------------------------------------------------------------------------

# Notes

Notes zijn **gedeelde documenten binnen een circle**.

Alle members van een circle kunnen deze bekijken.

## Note structuur

Een note bevat:

-   title
-   content
-   authorId
-   createdAt
-   updatedAt
-   circleId

## Functionaliteit (MVP)

Gebruikers kunnen:

-   nieuwe note maken
-   notes bekijken
-   eigen notes bewerken
-   eigen notes verwijderen

Notes worden weergegeven als een **lijst**.

------------------------------------------------------------------------

# Navigatie Flow

De basis flow van de applicatie:

Login ↓ Circle Dashboard ↓ Board ↓ Notes Tile ↓ Notes overzicht ↓ Note
editor

------------------------------------------------------------------------

# Circle Switching

De gebruiker kan van circle wisselen via de **dropdown in de top bar**.

Voorbeeld:

Study Group ▼

-   Study Group

-   Friends

-   Family

-   Create circle

-   Join circle

Wanneer een gebruiker wisselt van circle wordt:

-   het dashboard opnieuw geladen
-   de notes van die circle weergegeven

------------------------------------------------------------------------

# Future uitbreidingen

Hoewel de MVP alleen **Notes** bevat, is het systeem ontworpen voor
uitbreiding.

Mogelijke toekomstige tiles:

-   Notes
-   Tasks
-   Files
-   Shopping List
-   Calendar
-   Links
-   Polls

Voorbeeld toekomstig dashboard:

[Notes](#notes) \[ Tasks \] \[ Files \] \[ Events \]

------------------------------------------------------------------------

# MVP Scope

De MVP bevat alleen de kernfunctionaliteit:

-   Create circle
-   Invite users
-   Join circle
-   Open circle dashboard
-   Create notes
-   View notes
-   Edit own notes
-   Delete own notes

Dit is voldoende om een **werkende eerste versie van het product** te
lanceren.

------------------------------------------------------------------------

# Samenvatting

De applicatie is een **circle-based workspace** waarin kleine groepen
informatie kunnen delen.

Belangrijke kenmerken:

-   Circles (groepen van gebruikers)
-   Invite links om te joinen
-   Dashboard met tiles
-   Shared notes binnen een circle

De MVP focust op **simpliciteit en snelle validatie van het concept**.

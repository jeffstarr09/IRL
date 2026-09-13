# IRL — Product Strategy v0

*Pre-code analysis. Opinionated by design. Nothing here is validated yet; section 28 lists what needs to be.*

---

## Where I disagree with the brief

Before the 33 sections, the places where I think the brief points the wrong way. Everything below is built on these positions.

1. **Discovery is not the wedge.** It is the most expensive, least differentiated part of the product. Time Out, Google, Instagram, and Resy already answer "what's on." A listings pipeline will eat months and produce a worse Time Out. Discovery should be a tiny, hand-curated supply of "whats" for open time — fuel, not the product.
2. **"Booking time" is the wrong frame; "proposing on open time" is the right one.** A friend should never "book 3–5 PM." A friend should see "Sam's open Saturday afternoon" and say "drinks at Ode?" — a one-line proposal the owner accepts. Same outcome, no Calendly smell.
3. **Cut the "visible but not joinable" plan.** The brief lists "whether friends can join existing plans" as a control. A plan you can see but can't join is Instagram Stories with extra steps — pure FOMO, no utility. Rule: **visibility = invitation.** If you can see it, you can act on it. If it's not for joining, it's private.
4. **Never infer availability from calendar gaps.** Only explicit "I'm open" blocks are ever shared. This is the privacy line that makes the product trustworthy, and it means calendar read-sync is not needed for MVP.
5. **Relax "meaningful utility with zero friends."** The zero-friend utility is not good discovery — it's that every plan and open block is a link a non-user can respond to over SMS. That's the bridge; curated content is a nice-to-have.
6. **The name.** IRL was a social app that shut down in 2023 after it emerged that most of its users were fake. Worth checking trademark and reputation before committing to it.

---

## 1. One-sentence thesis

A calendar where your free time and casual plans are visible to the friends you choose, so that "let's hang out" happens by joining instead of asking.

## 2. The core user problem

Making plans with people you already like is absurdly expensive — not for lack of things to do (NYC has infinite) or tools to invite (texting exists), but because of coordination cost plus social risk. You don't know who's free. Asking exposes you to a no and imposes on the other person. The "who's around this weekend?" thread dies in the group chat. So people who want to see each other more, don't.

The problem is not discovery. It's the gap between wanting company and having it.

## 3. The strongest initial target user

Not "New Yorkers." Not people new to the city — they have the most pain but no graph, so the product is dead for them on day one.

**Established friend groups (5–12 people) of 28–42-year-olds in one or two adjacent Brooklyn neighborhoods, with a meaningful share of parents of young kids.**

Why:
- They already have the graph: a group chat that fails weekly.
- Their free time is scarce and fragmented, so a signal has real value.
- Their plans are low-stakes and local — park, playground, coffee, a run, a bar. Exactly the "I'm doing this anyway" unit.
- Parents especially: constrained windows, strong desire for company, hyper-local, and "we're at the playground 10–12" is already a text they send.
- Neighborhood density makes "I'm at X" actionable.

Recruit by group, not by individual. **The unit of acquisition is a group chat.**

## 4. Why a social availability layer is valuable

It inverts the social risk of making plans. Today, initiating means asking, which means risking rejection and imposing. With a visible "open" signal, initiating becomes responding to an offer. "I'm free Saturday afternoon" is an open door; "I'll join you at the park" is walking through it. Nobody gets rejected because nobody asked.

This is the single most important idea in the product. Everything else should be designed to protect it.

Secondary value: it collapses the fourteen-message "when are you free" thread into one glance.

## 5. Why "booking time with friends" might work

- A narrower version already works: people text "free tonight?" and "around this weekend" constantly. We're formalizing an existing behavior, not inventing one.
- Work calendars have trained everyone that "open on the calendar = ask-able."
- Proposals against open time are low-stakes — the owner already said they're free, so a proposal isn't an imposition.
- It gives discovery somewhere to go: "Sam's open Saturday" plus "there's a thing Saturday" is a plan in two taps.

## 6. Why it might NOT work

Respect the graveyard: Down To Lunch, Free, Sup, Wave, Zenly, Google Latitude, Facebook Nearby Friends, and IRL. Every one tried some version of "signal availability or presence to friends." The failure modes:

- **Status decay.** People stop updating. Any product that needs manual status dies unless the status is a by-product of something people already do.
- **Stigma.** "I'm free" can read as "nobody wants me." Broadcasting emptiness feels low-status.
- **Manufactured rejection.** You broadcast, nobody joins, and the app has created a rejection that wouldn't otherwise exist. Worse than before.
- **Asymmetry.** Most people lurk, few broadcast; broadcasters get little back.
- **The corporate smell.** Anything that feels like Calendly-for-friends gets mocked and abandoned.
- **Group chat is good enough.** Free, installed, everyone's there.
- **FOMO leak.** Seeing friends' plans you're not part of is the exact mechanic we say we won't build.

Mitigations must be designed in, not bolted on: prefer "I'm doing X" over "I'm free"; visibility = invitation; no public counts of who didn't join; signals expire naturally; links work for non-users so broadcasters get responses before their friends install anything.

## 7. The strongest alternatives

Alternatives to the concept itself, in the order I'd take them seriously:

1. **Casual-plan links** — Partiful for hangs, not parties. One page: "Jeff → Prospect Park, Sat 2pm. [I'm in] [I'm around]." Works over SMS. No calendar, no availability. Lowest cold start, and possibly the entire MVP.
2. **A group calendar** owned by the friend group, not the individual. Anyone drops plans or open time. Sidesteps individual privacy controls by making the group the unit.
3. **Standing rituals** — "Thursday run," "Sunday playground," "first-Friday drinks." Recurring plans with a rolling "I'm in." No status updates needed; builds habit and attendance.
4. **Discovery-first with a social tail** — Time Out-style curation with "who wants to go." The most expensive and least differentiated path. I'd avoid it.

Recommendation: the MVP is #1 with a thin calendar wrapped around it; #3 is the second feature; #2 is the fallback if individual privacy controls prove confusing.

## 8. What Time Out does well

Editorial authority and taste. Brand trust in NYC. Breadth. "Best of" lists that function as decision shortcuts. Strong SEO. Visual quality.

## 9. What Time Out fails to solve

It ends at awareness. A listing is not a plan. It has no idea when you're free, who you'd go with, or whether you went. It's structurally a media company — listicles, sponsored placements, endless scroll — optimized for pageviews. You leave Time Out and go text your friends. That's the gap.

## 10. What Partiful does well

Zero-friction guest experience: no account, SMS-native. One delightful event page. A visible guest list as social proof. A playful, non-corporate voice. Host tools (text blasts, reminders) that actually drive attendance. It nailed one thing.

## 11. What Partiful fails to solve

It only exists once you already have a what and a when and are willing to be a host. There's nothing between "nothing" and "a party." No availability, no spontaneity, no "I'm doing this anyway," no discovery, no calendar, no memory across events. Every event is an island. It doesn't touch the 90% of social time that isn't a hosted event.

## 12. What Google Calendar does well

Reliability, ubiquity, sharing, find-a-time, integrations, multi-device sync. It is the system of record for time.

## 13. What Google Calendar fails to solve socially

Its vocabulary is corporate: invite, accept, decline, busy. Availability is binary — "busy" can't distinguish a work meeting from a joinable park trip. Sharing is all-or-nothing and frightening, so nobody shares a personal calendar with friends. No concept of "open to plans," no place, no discovery, no social graph, no intention. It records commitments; it doesn't create them.

## 14. What this product should do fundamentally differently

Change the atomic unit from "event" to **intention with an audience.** Every block of time is one of three things:

- **Private** — the default; invisible; includes everything ever synced from another calendar.
- **Plan** — "I'm doing X at T (at P)." Shared to a chosen audience, and by definition joinable.
- **Open** — "I'm free from T1 to T2 (and I'd like company)." Shared to a chosen audience, and by definition proposable.

Rules that follow:

- **Visibility = invitation.** If you can see it, you can join or propose. There is no visible-but-closed state. This kills FOMO structurally and reduces the privacy model to one question per publish: *who is this for?*
- **Availability is explicit, never inferred.** We never compute "free" from gaps.
- **Works without the app on the other end.** Every plan and open block has a link a non-user can respond to via SMS.
- **The calendar is the home, not a feed.** A successful session is: glance, tap join, close.

## 15. The strongest differentiators

1. **Inverted social risk** — joining, not asking.
2. **Plans without a host** — "I'm going anyway" as the primary object, not the event.
3. **Visibility = invitation** — a privacy model people can hold in their head, and no FOMO by construction.
4. **SMS-native from day one** — useful with zero friends on the app.
5. **Calendar as home** — the outcome lands in the thing you already trust, not in a feed.

Discovery is deliberately not on this list.

## 16. The core behavioral loop

Publish (plan or open) → a friend sees it, in their week or via link → one-tap join or a one-line proposal → both calendars update → it happens → the graph learns who actually does things together → the next publish reaches the right people first.

The loop must close in seconds, and the app should be closed at the end of it.

## 17. The role of discovery

Supply the "what" for open time. In MVP: a small, hand-curated list (15–25 things per week, in the target neighborhoods) with a one-tap "make this a plan." Discovery items are plan templates.

The most valuable discovery surface is your friends' plans — "what my people are doing" beats "what's on." If we ever find ourselves optimizing event volume, we've lost the plot.

## 18. The role of the social graph

Small, explicit, mutual, tiered. Two tiers in MVP: **Close** and **Friends.** No followers, no public profiles, no counts. The graph exists to answer one question per publish: who is this for? Imported from contacts and, ideally, whole group chats. If someone's graph grows past ~50 people, the product is being used wrong.

## 19. The role of the calendar

The home screen and the system of record for intentions. Your week, with friends' shared plans and open blocks overlaid *in place* — not in a separate list. Joining writes to your calendar. Later: busy-blocking read from Google/Apple and plan write-out — but synced events are never exposed.

## 20. The role of availability

A signal, not a field. A social offer with a time range and an audience, and it expires. It should feel like leaving the door open, not publishing a schedule. Say "open" rather than "free" wherever possible, and nudge toward "open + a hint" ("open Sat afternoon, down for outdoors") over bare emptiness.

## 21. The minimum viable social calendar

- Week view, today first.
- **+** → *I'm doing something* (what, when, optional place, audience) or *I'm open* (range, optional hint, audience).
- Friends' plans and open blocks rendered inside your week.
- **Join** (one tap) and **Propose** (one line, or pick a discovery item). Accepted proposal → shared plan.
- A shareable link per plan/open block; non-users respond with a phone number.
- Two audience tiers. Block and remove.
- Notifications: someone joined, someone proposed, and one daily "what's on among your people." Nothing else.
- Add-to-calendar (.ics) out. No calendar read-sync.

Not in MVP: overlapping-availability finder, recurring availability, capacity limits, chat.

## 22. The minimum viable discovery experience

One curated list per week for the target neighborhoods, written by a human with taste (initially: you). Each item: what, when, where, why, and "make a plan." No categories, no search, no map, no scraping. If friends' plans turn out to be more interesting than the list, good — that's the product working.

## 23. Features we should explicitly NOT build yet

- Overlapping availability / find-a-time (the pull model; v2 once density exists)
- Bookable slots or time requests as first-class objects (proposals on open time cover it)
- Recurring availability (do standing plans instead, later)
- A broader "network" tier or friends-of-friends
- Event scraping or a listings pipeline
- In-app chat (SMS is the chat)
- Profiles beyond name, photo, neighborhood
- Photos, posts, reactions, memories, history
- Map view (until place data deserves it)
- Calendar read-sync (Google OAuth verification alone is weeks; and it tempts inference)
- Recommendations / ML
- Venue partnerships, ticketing, monetization
- Public, indexable event pages

## 24. The biggest privacy risks

1. **Location is the payload.** "I'm at the park at 2" tells people where you'll be — ex-partners, stalkers, a "friend" you shouldn't have added. Mitigate: mutual-only graph, audience defaults to Close, instant block that retroactively hides everything, no location without a plan.
2. **Kids.** "Taking the kids to the playground" broadcasts a child's location and routine. Plans mentioning kids default to Close-only, and nobody ever sees anyone else's history of past plans.
3. **Wrong-audience posts.** One mis-tap shares to the wrong tier. Audience is always visible on compose; last choice remembered per type; confirmation on first Friends-tier share.
4. **Inference.** "Open Friday night" ≈ "home alone Friday night." Can't eliminate; can avoid amplifying — no inference, expiry, no history.
5. **Synced-calendar leakage.** A read-sync bug that exposes a private event is a catastrophe. Hence no read-sync in MVP; when added, busy-only, never titles.
6. **Forwarded links.** Link pages show the minimum, expire with the plan, and are revocable.
7. **Exclusion harm.** Seeing plans you weren't invited to. Solved structurally by visibility = invitation.

## 25. The biggest product risks

- **Manufactured rejection.** Watch join rates obsessively. If fewer than ~30% of published items get a response in the seed groups, the core mechanic is broken.
- **The empty calendar.** First session with no friends is just a calendar app. SMS links and group import must fix this in week one.
- **It becomes a feed.** The overlay of friends' plans is one design decision away from a scrollable feed. Keep it in the grid.
- **Status fatigue.** If publishing takes more than ten seconds or needs to happen daily, it stops.
- **Plan vs. open confusion.** Two objects is already a lot. If users can't tell them apart, collapse to one.
- **Group chat wins.** If group chat plus a link does the job, the calendar may be unnecessary — a fine thing to learn early (see §32).
- **Taste drift.** Curated discovery costs human time every week; if it degrades, it's a worse Time Out.

## 26. The biggest cold-start risks

- The week view needs 3+ active friends before it shows anything. NYC-wide launch is hopeless; group-by-group in one neighborhood is the only path.
- The first publisher in each group takes the social risk for everyone. Seed with your own groups; you and a few friends are patient zero.
- Discovery content costs human hours weekly.
- Non-users responding via link is the bridge. If SMS response rates are low, the bridge fails and every group must reach critical mass on its own.

## 27. The biggest technical risks

- **Visibility/ACL correctness.** One bug is a privacy incident. Needs a single enforced query path and tests before any UI.
- **SMS.** A2P 10DLC registration, deliverability, per-message cost; link previews on both iMessage and Android.
- **Calendar sync (later).** Google OAuth verification for calendar scopes, Apple requires native EventKit, two-way write conflicts. Reason enough to defer.
- **Platform.** Native iOS (contacts, calendar, reliable push) vs. PWA (faster iteration, no App Store gate). Given the target user and the contact-import need, native iOS via Expo with web link pages is the likely answer. Decide early.
- **Time.** No recurrence. Fix the timezone to America/New_York.

## 28. The most important assumptions requiring validation (in order)

1. People will publish casual plans or open time to friends at all — and still be doing it in week three.
2. Friends will join what's published, at a rate that makes publishing feel rewarding.
3. Publishing "open" (not just plans) is socially acceptable in these groups.
4. Non-users will respond to a link.
5. The two-tier audience model is understood without explanation.
6. A calendar is the right home (vs. a list).
7. Discovery content changes behavior at all (vs. friends' plans being enough).
8. This happens weekly per user, not monthly.

## 29. Proposed information architecture

Three destinations, one action. No feed, no notifications tab, no search.

- **Week** (home) — your calendar with friends' shared plans and open blocks in place. Tap → sheet → Join / Propose.
- **Around** — this week's curated list, plus friends' open blocks as a list ("Sam's open Sat afternoon"). Tap → make a plan / propose.
- **You** — friends and tiers, your published items, blocks, notification settings.
- **+** (persistent) — *I'm doing something* / *I'm open.*

## 30. Proposed mobile-first UX

- Open → today, then the next six days. Your private blocks muted grey (if any), your published items solid, friends' plans as small colored pills inside the time grid, friends' open blocks as dashed outlines. Legible in under three seconds.
- Tap a friend's pill → bottom sheet: what, when, where, who's in, **[Join]**. One tap writes to your week and notifies them. Done.
- Tap a friend's open block → "Sam's open Sat 2–6." **[Propose]** → one line, or pick from Around → sent.
- **+** → two big buttons. Compose is three fields (what, when, audience), place optional, share sheet after. Under ten seconds.
- Copy is human: "Join," "I'm around," "Want company?" Never "Accept," "Decline," "Book."
- Non-user link page: the same sheet with a phone-number field instead of an account.
- Calm, typographic, editorial. No cards inside cards. Fewer colors than you want.

## 31. Proposed high-level data model

```
users            id, phone, name, photo, neighborhood
friendships      user_a, user_b, tier (close|friends), status (pending|mutual), blocked_at
                 — mutual required for any visibility
plans            id, owner_id, title, starts_at, ends_at, place_name, place_geo?,
                 audience (close|friends|link), listing_id?, canceled_at
open_blocks      id, owner_id, starts_at, ends_at, hint, audience, expires_at
participations   plan_id, user_id | guest_phone, status (in|maybe), created_at
proposals        open_block_id, from_user_id | guest_phone, message, listing_id?,
                 status (sent|accepted|declined), resulting_plan_id?
listings         id, title, blurb, starts_at, ends_at, place, neighborhood, week_of
share_links      token, target_type, target_id, revoked_at
notifications    minimal

later:           calendar_connections (provider, busy-only), rituals (standing plans)
```

Every read of `plans` and `open_blocks` goes through one visibility function. Write it and test it first.

## 32. The fastest validating experiment

Don't build the calendar. Build one page.

**Week 1:** a single web page generated from a form — "Jeff → Prospect Park, Sat 2pm. **[I'm in] [I'm around, maybe]**" — shared as a link into your own group chats. Plus an open variant: "Jeff's open Sat 2–6. **[Propose something]**." Phone number only, no accounts. Log everything.

**Weeks 2–4:** run it in 3–5 friend groups. Measure publishes per person per week, join rate per publish, proposal rate on open blocks, and — the only number that matters — plans that actually happened that wouldn't have otherwise. Ask; it's thirty people.

Reading the result:
- Publishes and joins both happen → build the week view around it.
- Publishes happen, joins don't → the audience/graph is wrong, not the mechanic.
- Nobody publishes → the stigma/effort problem is real and no calendar will fix it.
- Group chat + links is enough → the calendar is a v2 nice-to-have, not the wedge. Months saved.

## 33. What would make this genuinely difficult to copy

Honestly: nothing technical. Time Out can add "share to friends," Partiful can add "I'm free," Google can add "open to plans." What's defensible:

- **The co-attendance graph.** Who actually did things with whom, how often, where. The only social graph that's about real life, and a by-product of the product working. It makes every later feature better and can't be bought or scraped.
- **Norms at neighborhood density.** Once a friend group's plans live here, the switching cost is the group, not the individual.
- **Trust with calendar-write access.** Earned slowly, lost instantly. Incumbents with feeds and ads can't credibly promise "we won't infer."
- **Taste.** If the curated layer is genuinely good, it's a brand, and brands are slow to copy.

---

## Two decisions to make before any code

1. **The name.** See above — check trademark and reputation on "IRL."
2. **Native iOS vs. PWA.** Contacts import, calendar, and push all hinge on it. My lean: Expo (native iOS) for the app, plain web for link pages.

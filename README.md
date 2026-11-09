[README (7).md](https://github.com/user-attachments/files/34597631/README.7.md)# Friendsgiving Table

Six AI tools RSVP'd to healthcare Friendsgiving. You're the host. Not all of them are getting a seat.

### 🦃 [Open the invitation](https://thanksgivinghealth.netlify.app/)

*About 1 minute. Black tie optional.*

---

## The guest list

One place card at a time, you decide where each guest sits:

- **🍗 The Main Table:** AI runs it
- **🧃 The Kids' Table:** a human checks its work
- **🚪 The Door:** people only

On the list tonight:

📝 **The Note Taker** · 🔎 **The Directory Checker** · 📅 **The Scheduling Bot** · 📋 **The Prior Auth Decider** · 💬 **The Crisis Line Answerer** · 🎧 **The Call Copilot**

Every guest is based on real work in healthcare operations. Some of these are easy calls. One of them will make you hesitate.

## After dinner

You get your **hosting style.** Are you the Bouncer, the Careful Cook, the Gravy Boat or the Open Buffet?

Then Olu's own seating chart gets revealed, guest by guest, with her reasoning and how many seats you matched. Copy your result and see if your coworkers would seat them the same way.

## Behind the scenes

A few crumbs from the code. The rest stays in the kitchen.

**Every seat is worth points.** Your total decides your hosting style:

```js
const SC = {main: 2, kids: 1, out: 0};
```

**Twelve points is the max.** Hand every guest a main table seat and you're officially the Open Buffet:

```js
if (s <= 3) return ["The Bouncer", /* ... */];
if (s <= 6) return ["The Careful Cook", /* ... */];
if (s <= 9) return ["The Gravy Boat", /* ... */];
return ["The Open Buffet", /* ... */];
```

**Every guest has a quip ready for wherever you put them.** Send the Scheduling Bot to the door and it has something to say about that.

Where Olu seats each guest, and the house rule she ends the night on... you'll have to host.

## Built with

One HTML file. Vanilla JavaScript, CSS and canvas for the falling leaves at the end. No frameworks, no build step.

## Made by

**Olu Ladipo**, AI UX & Product Designer
[Portfolio](https://oluladportfolio.netlify.app) · [LinkedIn](https://www.linkedin.com/in/oluladipoinsights) · [Referral Rush](https://referralrush-oluladipo.netlify.app)

*My opinions, my side project. Not an official UHG or Optum thing.*

### 🦃 [Your guests are waiting](https://thanksgivinghealth.netlify.app/)

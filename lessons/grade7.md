# Grade 7 Worksheet: Local vs Relative Coordinates in Minecraft

## 🎯 Topic

Understanding **Relative (~)** and **Local (^) Coordinates**

---

## 🧠 Big Idea

Minecraft has **two coordinate systems**:

| Type     | Symbol | Based on                                        |
| -------- | ------ | ----------------------------------------------- |
| Relative | `~`    | World (fixed directions: East/West/North/South) |
| Local    | `^`    | Player direction (where YOU are looking)        |

---

## 📍 Part 1: Review (~ coordinates)

### Try this:

```mcfunction
/setblock ~2 ~ ~ stone
```

👉 Question:

* Which direction did the block move?
* Does it change when you turn your character?

✍️ Write your answer:

---

## 🚀 Part 2: Learn (^) coordinates

### Try this:

```mcfunction
/setblock ^ ^ ^2 stone
```

👉 Question:

* Where did the block appear?
* Now turn around and run it again. What changed?

✍️ Answer:

---

## 📐 How Local Coordinates Work

| Command   | Meaning              |
| --------- | -------------------- |
| `^ ^ ^1`  | 1 block forward      |
| `^1 ^ ^`  | 1 block to the right |
| `^-1 ^ ^` | 1 block to the left  |
| `^ ^1 ^`  | 1 block up           |

👉 Important:
**^ depends on where you are facing**

---

## 🧪 Part 3: Experiment

Run these commands:

```mcfunction
/setblock ^1 ^ ^ stone
/setblock ^-1 ^ ^ stone
/setblock ^ ^1 ^ stone
/setblock ^ ^ ^3 stone
```

### Questions:

1. Which one moves forward?
2. Which one moves left/right?
3. Which one moves up?

✍️ Answer:

---

## 🧠 Part 4: Compare (~ vs ^)

| Feature                        | `~`   | `^`   |
| ------------------------------ | ----- | ----- |
| Depends on direction?          | ❌ No  | ✅ Yes |
| Uses world axes?               | ✅ Yes | ❌ No  |
| Good for maps?                 | ✅ Yes | ❌ No  |
| Good for “in front of player”? | ❌ No  | ✅ Yes |

---

## 🧩 Part 5: Build Challenge

### Challenge 1: Line in Front

Create a 4-block line **in front of you**:

```mcfunction
/setblock ^ ^ ^1 stone
/setblock ^ ^ ^2 stone
/setblock ^ ^ ^3 stone
/setblock ^ ^ ^4 stone
```

---

### Challenge 2: Wall in Front

Goal: Build a 3×3 wall in front of you

Hint:

```mcfunction
/setblock ^-1 ^ ^3 stone
/setblock ^ ^ ^3 stone
/setblock ^1 ^ ^3 stone
```

Add more rows!

---

### Challenge 3: Always Face You

Build something that **always appears in front of you**, no matter which way you look.

👉 Use only `^`

---

## 🧠 Part 6: Think Like a Programmer

### Question:

When would you use each?

* Use `~` when:

---

* Use `^` when:

---

---

## 🔥 Bonus (Advanced)

```mcfunction
/execute positioned ^ ^ ^3 run setblock ~ ~ ~ gold_block
```

👉 Question:
What is happening here?

✍️ Answer:

---

## 🎯 Reflection

Write 3–4 sentences:

1. What is the difference between `~` and `^`?
2. Which one was harder?
3. What did you build?
4. What would you try next?

---

## 💡 Teacher Notes

* Students often confuse:

  * `~` = **map coordinates**
  * `^` = **player-relative coordinates**
* Key insight:
  👉 `^` turns with the player

---

## 🚀 Extension Ideas

* Make a “laser beam” forward
* Create a moving platform
* Build a structure that follows the player


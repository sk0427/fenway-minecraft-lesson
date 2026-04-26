# Grade 4 Worksheet: Build the Green Monster

## Project

Today you will build the **Green Monster**, the famous green wall at Fenway Park in Boston.

You will use Minecraft commands saved in a datapack.

## Big Idea

A Minecraft command can build many blocks at once.

This command:

```mcfunction
fill ~ ~ ~ ~10 ~ ~10 stone
```

means:

> Start at my position and fill a rectangle with stone.

The `~` symbol means "from where I am standing."

## Learning Goals

By the end, you can:

- Explain what `/fill` does
- Change numbers to make a build bigger or smaller
- Change the block type
- Run a datapack function

## Step 1: Make a Flat World

1. Create a new Minecraft Java world
2. Choose **Creative**
3. Choose **Superflat**
4. Turn **Allow Cheats: ON**

## Step 2: Run the Datapack

Type:

```mcfunction
/reload
/function fenway:green_monster
```

You should see a tall green wall with red seats.

## Step 3: Try Changing One Thing

Open this file:

```text
datapack/fenway/data/fenway/functions/green_monster.mcfunction
```

Find this line:

```mcfunction
fill ~-40 ~ ~10 ~-40 ~10 ~50 minecraft:green_terracotta
```

Try changing the `10` after the second `~`:

```mcfunction
fill ~-40 ~ ~10 ~-40 ~15 ~50 minecraft:green_terracotta
```

Then run:

```mcfunction
/reload
/function fenway:green_monster
```

What changed?

## Challenge A: Change the Color

Try changing:

```mcfunction
minecraft:green_terracotta
```

to:

```mcfunction
minecraft:green_concrete
```

or:

```mcfunction
minecraft:lime_concrete
```

## Challenge B: Add a Scoreboard

Run:

```mcfunction
/function fenway:green_monster
```

Then add black blocks to make a scoreboard.

Hint:

```mcfunction
fill ~-41 ~3 ~20 ~-41 ~7 ~35 minecraft:black_concrete
```

## Reflection

Answer in 2–3 sentences:

1. What did you build?
2. Which number did you change?
3. What happened when you changed it?

## Bonus

Add your name or initials using colored blocks.

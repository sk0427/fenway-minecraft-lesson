# Grade 6 Worksheet: Recreate Part of Fenway Park with Code

## Project

You will build a simplified part of Fenway Park in Minecraft Java Edition using a datapack.

Your final build should include:

- A field
- Bases
- The Green Monster
- Seats
- One original feature

## Big Idea

A datapack lets us organize Minecraft commands into files.

Each `.mcfunction` file acts like a function.

Example:

```mcfunction
function fenway:field
function fenway:bases
function fenway:green_monster
```

This is similar to calling functions in a programming language.

## Learning Goals

By the end, you can:

- Use Minecraft coordinates
- Explain relative coordinates using `~`
- Modify an `.mcfunction` file
- Organize a build into multiple functions
- Use repeated commands to make a pattern

## Step 1: Run the Full Build

In Minecraft, type:

```mcfunction
/reload
/function fenway:build
```

Look around. What parts of Fenway Park do you see?

## Step 2: Understand the Coordinates

This command builds a stone floor:

```mcfunction
fill ~ ~ ~ ~10 ~ ~10 minecraft:stone
```

It makes an 11 × 1 × 11 shape because Minecraft includes both the start and end positions.

Coordinates are:

```text
x = east/west
y = up/down
z = north/south
```

## Step 3: Explore the Files

Open:

```text
datapack/fenway/data/fenway/functions/
```

You will see:

- `build.mcfunction`
- `field.mcfunction`
- `bases.mcfunction`
- `green_monster.mcfunction`
- `seats.mcfunction`
- `lights.mcfunction`

## Step 4: Modify the Stadium

Choose at least two:

### Option A: Make the Green Monster taller

In `green_monster.mcfunction`, change the wall height.

Original:

```mcfunction
fill ~-40 ~ ~10 ~-40 ~10 ~50 minecraft:green_terracotta
```

Try:

```mcfunction
fill ~-40 ~ ~10 ~-40 ~14 ~50 minecraft:green_terracotta
```

### Option B: Add more seats

In `seats.mcfunction`, copy a seat row and change the coordinates.

### Option C: Add a fence

Create a new file:

```text
fence.mcfunction
```

Add:

```mcfunction
fill ~-45 ~1 ~-30 ~45 ~3 ~-30 minecraft:iron_bars
```

Then add this line to `build.mcfunction`:

```mcfunction
function fenway:fence
```

### Option D: Add lights

Modify `lights.mcfunction` or add more light towers.

## Requirements

Your final project should include:

- At least 4 `.mcfunction` files
- At least 1 file you edited yourself
- At least 1 original feature
- A short explanation of what you changed

## Reflection

Answer in 4–5 sentences:

1. What part of Fenway Park did you build?
2. Which file did you change?
3. Which coordinates did you change?
4. What was difficult?
5. What would you add next?

## Extra Challenge

Make a new function called:

```text
scoreboard.mcfunction
```

Then add it to `build.mcfunction`.

Try to create a scoreboard on the Green Monster using black, white, and yellow blocks.

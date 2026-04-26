# 🧱 Minecraft Coding Lesson: Build Fenway Park

Welcome! In this project, students learn basic coding concepts by building part of **Fenway Park** in Minecraft Java Edition.

This lesson is designed for:
- 4th grade: Beginner
- 6th grade: Intermediate

## 🎯 Learning Goals

Students will learn:
- Minecraft coordinates: x, y, z
- Scale: 1 block = about 1 meter
- Functions: grouping commands into files
- Repetition: building repeated shapes like seats
- Real-world observation: looking at a real place and turning it into a Minecraft build

## 🎮 Requirements

- Minecraft Java Edition
- A creative-mode world
- Cheats enabled
- A flat world is recommended

## 🌍 Create a Flat World

1. Open **Singleplayer**
2. Click **Create New World**
3. Set **Game Mode: Creative**
4. Click **More World Options**
5. Set **World Type: Superflat**
6. Turn **Allow Cheats: ON**
7. Create the world

## ⚙️ Install the Datapack

Copy this folder:

```text
datapack/fenway
```

into your Minecraft world's datapack folder:

```text
.minecraft/saves/YOUR_WORLD/datapacks/
```

Then in Minecraft, run:

```mcfunction
/reload
/function fenway:build
```

## 🧩 Files

```text
datapack/fenway/
├── pack.mcmeta
└── data/fenway/functions/
    ├── build.mcfunction
    ├── clear_area.mcfunction
    ├── field.mcfunction
    ├── bases.mcfunction
    ├── green_monster.mcfunction
    ├── seats.mcfunction
    └── lights.mcfunction
```

## 👦 Student Worksheets

- `lessons/grade4.md`
- `lessons/grade6.md`

## 🚀 Main Command

```mcfunction
/function fenway:build
```

Have fun changing the numbers and seeing what happens!

# Java Encapsulation Assignment

Solutions to the **Category C – Encapsulation and Access Control** Java assignment. Each question is a small, self-contained program showing a different way a class protects its own state.

## Questions

| # | Folder | Class | Concept |
|---|--------|-------|---------|
| Q1 | [`Q1-Character-Health`](Q1-Character-Health/Main.java) | `Character` | Private state changed only through methods that keep health between `0` and a `final` maximum |
| Q2 | [`Q2-Playlist-Defensive-Copy`](Q2-Playlist-Defensive-Copy/Main.java) | `Playlist` | Defensive copying: the getter returns a copy, so callers can't modify the internal array |
| Q3 | [`Q3-Password-Strength`](Q3-Password-Strength/Main.java) | `PasswordChecker` | Information hiding: the password is `private final` with no getter; only its strength is exposed |

## Project structure

```
.
├── Q1-Character-Health/
│   └── Main.java
├── Q2-Playlist-Defensive-Copy/
│   └── Main.java
├── Q3-Password-Strength/
│   └── Main.java
└── README.md
```

## How to run

You need a JDK (8 or later). From the repository root, pick a question and run:

```bash
cd Q1-Character-Health
javac Main.java
java Main
```

## Sample output

**Q1 – Character health**

```
Health = 70
Health = 100
Health = 0
```

**Q2 – Playlist defensive copy**

```
Song 1 = Song A
Song 2 = Song B
Song Count = 2
After modifying copy:
Song 1 = Song A
```

Changing the returned copy to `"Hacked"` leaves the playlist untouched.

**Q3 – Password strength**

```
Weak
Medium
Strong
```

## Author

**Aditya Shukla** · [@adityashukla44](https://github.com/adityashukla44)

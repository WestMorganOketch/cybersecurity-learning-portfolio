Notes from my own practice on TryHackMe; not affiliated with or endorsed by TryHackMe.

# Python Basics for Security Learning

This material covered foundational Python programming concepts that support repeatable analysis and automation. The core skills include understanding variables and data types, displaying information, using arithmetic and expressions, making decisions with conditional statements, repeating work with loops, and reading files safely. These fundamentals are useful for small analyst tasks such as parsing structured text or transforming approved datasets.

The important lesson is to make scripts predictable: validate inputs, handle missing or malformed data, avoid hard-coded secrets, and keep output understandable. File operations should use explicit paths and safe error handling. Exercise flags and answer strings have been excluded, and this note does not reproduce the room's task sequence.

Defensive scripting should follow least privilege, use trusted dependencies, avoid executing untrusted content, and protect any data the script processes. I would do differently by writing small functions, testing edge cases with harmless sample data, and adding comments that explain assumptions. The goal is reliable automation, not simply making a script run once.

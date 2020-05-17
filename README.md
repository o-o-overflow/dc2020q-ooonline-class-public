# DEFCON 2020 Quals Ooonline Class

This challenge is an online course system modeled after coursera's custom grader.

## Vulnerability

Interesting SQL injection for users to extract the creds of the user
with a solved challenge. This was unintended, see the grad version
of the course for the intended vulnerabiliy.

The unintended vulnerability is to get the username and password of
the person who solved the challenge.

## Exploit

The [exploit](./interaction/exploit.py) is for the intended
vulnerability. But you can now use the SQL injection to read the
password of the `smart` user to steal their solution.

## Bugs

Also, I accidentially enable debugging for this challenge. It is fixed
in ooonline-gradclass.

# Biggest Team

## Summary

You have different people. They speak different languages. From those people,
the goal is to find the biggest team, considering the fact that every people
in the said team **MUST** be able to communicate with each other.

As long as a pair can communicate, they can communicate with the team.

## Example

_persons.txt_:
```
Dallas:US,EN
Chain:US,ES
Hoxton:EN
Sangres:ES
Jiro:JA
```

```
$ ./biggest_team < persons.txt
4
Dallas
Chain
Hoxton
Sangres
```

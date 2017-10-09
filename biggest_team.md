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

In our example, we can see that _Dallas_ can communicate with _Chain_(US)
and _Hoxton_(EN). Moreover _Chain_ can communicate with _Sangres_(ES).

If _Sangres_ wants to give an information to _Hoxton_, he can tell the
information to _Chain_, who can give it to _Dallas_, and back to _Hoxton_.

## Binary name

_biggest_team_

## Formatting

```
$ ./biggest_team persons.txt
4
Dallas
Chain
Hoxton
Sangres
```

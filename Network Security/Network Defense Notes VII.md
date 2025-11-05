
ACL  (Access Control Lists) - What they can be applied to


- Interfaces
- "access-group ..."
- Lines ("vty")
- "access-class ..."
- Route Distribution
- Debug
- "debug ip packet 101"
- Many other things too


### In vs. Out

- e.g

```
ip access-group ### <in|out>
```



```
access-list ### <permit|deny>

```

- Standard
	- 1-99
	- 1300-1999
	- access-list 1 permit 192.168.1.1
	- access-list 12 permit 192.168.0.0 0.0.255.255
- Extended
	- 100-199
	- 2000-2699
	- access-list 100 permit

- ip access-list [extended|standard] name
	- ip access-list NO_NET_FOR_YOU
		- deny host 192.168.1.1
		- permit any
		- 10 deny host 192.168.1.1
		- 20 permit any
	- Can be "re-numbered"
		
```
ip access-list resequence <Name> <start> <step>
```


### Implicit Deny

- Implicit Deny happens if all of the things in the ACL doesn't match
	- Deny if nothing matches in the ACL
```
access-list 3 permit 192.168.1.0 0.0.0.255
```
- The first part above is the allowed IP address, the second part says,
If it is a zero, the parts in this IP address need to match


```
192.168.1.0
^
0   0   0 255    First three must match, the last one doesn't need to match.
0   0   0 127    First three must match, the last one can be allowed up to 127
0   0   0 128
0   0   0 1
```


```
router bgp <AS#>


```




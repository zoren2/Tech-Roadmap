# Generators
A special type of function that produces multiple values on a per request basis while suspending their execution between these requests.

```
function* WeaponGenerator() {
	yield "Katana";
	yield "Wakizashi";
	yield "Kusarigama";
}

// Hmm it's "iterating" over Generator function

for(let weapon of WeaponGenerator()) {
	assert(weapon !== undefined, weapon);
}
```

Think of it like a ninja scroll - it's got spells and iterator asks for the next thing
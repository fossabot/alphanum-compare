# alphanum-compare
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Ftsekityam%2Falphanum-compare.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Ftsekityam%2Falphanum-compare?ref=badge_shield)


Compare function extrated from [alphanum-sort](https://github.com/trysound/alphanum-sort). It can be used as `compareFunction` in `Array.prototype.sort()`.

## Install

`yarn add alphanum-compare`

## Usage

```ts
import compareFn from "alphanum-compare";

const result = ["item20", "item19", "item1", "item10", "item2"].sort(compareFn);
// ['item1', 'item2', 'item10', 'item19', 'item20']
```

### `compareFn(a: string, b: string, opts?: { sign?: boolean }): number`

It returns a negative value if first argument is less than second argument, zero if they're equal and a positive value otherwise.

#### Options

- `sign?: boolean`: Allows `+` and `-` characters before numbers. _(Default: `false`)_


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Ftsekityam%2Falphanum-compare.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Ftsekityam%2Falphanum-compare?ref=badge_large)
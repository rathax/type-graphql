# Changelog and release notes

## Unreleased
### Features
- add basic support for automatic arguments and inputs validation using `class-validator`
- add interface `ResolverInterface` for type checking of resolver class methods (field resolvers)

### Fixes
- fix default values for arg/input fields (class property initializers) - use `new` instead of `Object.create`

## v0.3.0
### Features
- add support for descriptions in schema (types, args, queries, etc.)
- add support for declaring depreciation reason on object fields and queries/mutations

### Fixes
- fix scalars ID alias (GraphQLID not GraphQLString)

## v0.2.0
### Features
- add support for Date type (built-in scalar)
- add support for custom scalars (and mapping it to TS types)
- change `@Context` decorator name to `@Ctx`

## v0.1.2
### Fixes
- fix missing type args in schema when declared in field resolver
- fix missing resolver function when defined as type field method
- fix creating instances of root object when internal fields are Promises (switch from `plainToClass` to vanilla JS)
- fix convertings field and resolvers args errors while converting gql objects (weird `prototype` stuffs)

## v0.1.1
### Features
- add support for ommiting return type when use type options, in selected decorators (`@Field`, `@Arg`)

### Fixes
- fix class getter resolvers bug - missing fields from prototype (`plainToClass` bug)

## v0.1.0
### Initial release
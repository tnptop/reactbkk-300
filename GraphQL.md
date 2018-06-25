# GraphQL

## Security

### Depth Limiting
- Circular link -> load server to death
- Sol. = `graphql-depth-limit`
- Limit reference depth

### Amount Limiting
- Large amount of data -> load server to death
- Sol. = `graphql-input-number`
- Set min/max amount for query


## Maintenance

### Splitting Schema
- Split files by model (schema and resolver)
- Load all schema files and concat them together
- Also with resolver


## Monitoring

### Apollo Engine
- Query execution tracking
- Error tracking
- GraphQL Caching
- Trends
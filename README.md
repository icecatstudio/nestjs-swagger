# @nestjs/swagger (Fork)

This is a fork of the original [@nestjs/swagger](https://github.com/nestjs/swagger) package with an additional `@ApiSchema` decorator.

The `@ApiSchema` decorator allows renaming DTO classes for schema generation in Swagger. For example, you can rename a class `UserCreateDto` to `UserCreateRequest` when generating the API documentation.

### Example:

```typescript
import { ApiSchema } from '@nestjs/swagger';

@ApiSchema({ name: 'UserCreateRequest' })
export class UserCreateDto {
  // DTO properties
}
```

### Addresses the Following Issues

This feature resolves the following issues from the original repository:

- [Pull Request #983](https://github.com/nestjs/swagger/pull/983)
- [Issue #1596](https://github.com/nestjs/swagger/issues/1596)

By using this decorator, you can easily customize how your DTOs appear in Swagger’s generated schemas, without needing to modify the actual class names in your codebase.

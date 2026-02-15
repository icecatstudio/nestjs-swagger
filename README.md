# @icecat-studio/nestjs-swagger

## DEPRECATED

This package is deprecated. Please use the original [`@nestjs/swagger`](https://www.npmjs.com/package/@nestjs/swagger) package instead.

The `@ApiSchema` decorator, which was the reason this fork existed, is now available in the official `@nestjs/swagger` package.

### Migration

```bash
npm uninstall @icecat-studio/nestjs-swagger
npm install @nestjs/swagger
```

Update your imports:

```typescript
// Before
import { ApiSchema } from '@icecat-studio/nestjs-swagger';

// After
import { ApiSchema } from '@nestjs/swagger';
```

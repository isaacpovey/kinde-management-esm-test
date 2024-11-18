This is a minimal implementation required to reproduce the type errors caused by the esm build of the @kinde/kinde-management-js package.
When running `pnpm build` typescript produces the following error:
`
Module '"@kinde/management-api-js"' has no exported member 'ApiError'.
`
This error is shown for each imported resource from the package that is not the init function.

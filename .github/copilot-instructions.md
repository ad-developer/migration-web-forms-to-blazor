# Workspace Metadata & Ambient Preferences

This workspace is structured for an incremental migration project. Use these facts strictly as environmental context for inline code suggestions.

## 1. Directory Environment Boundaries
- **Legacy Framework Monolith:** All old code-behind files sit under `/src-legacy-webforms/`. This code uses .NET Framework 4.8 and C# Web Forms syntax. Treat this directory as read-only.
- **Modern Target Framework:** All new cloud-native structures sit under `/src-modern-core-blazor/`. This application runs on .NET 11 using ASP.NET Core, Razor Pages, and Blazor server components.
- **Sandbox Migration Log:** Active conversion workflows and markdown progress ledgers live exclusively within `/migration-workspace/`.

## 2. Universal Code Styling Preferences
- **Indentation:** Enforce exactly 4 spaces for indentation across all C#, HTML, Razor, and Markdown configurations. Do not use tabs.
- **Variable Declaration:** Prefer explicit variable types (e.g., `int`, `string`, `List<Product>`) over implicit typing (`var`) unless the assignment type is clearly evident on the right side of the expression.
- **Asynchronous Execution:** For code suggestions within the `/src-modern-core-blazor/` scope, default natively to modern asynchronous workflows (`async/await`) and avoid synchronous thread blocking.
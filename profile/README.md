<p align="center">
  <img src="./logo.png" width="160" alt="Beacon Observability logo">
</p>

<h1 align="center">Beacon Observability</h1>

<p align="center">
  Zero-code application observability with
  <a href="https://opentelemetry.io/">OpenTelemetry</a>-based server instrumentation
  and browser RUM through Rumable.
</p>

<p align="center">
  <a href="https://github.com/beacon-observability/beacon">Project overview</a>
  ·
  <a href="https://beacon-observability.github.io/docs/">Documentation</a>
  ·
  <a href="#projects">Projects</a>
  ·
  <a href="#contributing">Contributing</a>
</p>

## About Beacon

Beacon maintains independently versioned server instrumentation and browser RUM projects. Each language agent preserves its OpenTelemetry upstream history, records an exact source baseline, and owns its build, validation, release, and support scope. Rumable adds browser monitoring through Nginx or IIS without changing application source code.

Component implementations and release schedules are intentionally independent. A capability or release in one component does not imply the same capability or support level in another. Refer to each repository and versioned release notes for installation instructions, validated environments, and known limitations.

## Start here

- **Product and architecture:** [beacon](https://github.com/beacon-observability/beacon)
- **User documentation:** [beacon-observability.github.io/docs](https://beacon-observability.github.io/docs/)
- **Browser RUM:** [Rumable setup guide](https://beacon-observability.github.io/docs/rumable) and [English configuration page](https://beacon-observability.github.io/rumable/latest/setup/index.html)
- **Documentation source:** [docs](https://github.com/beacon-observability/docs)
- **Installation and artifacts:** use the latest release from the relevant component repository
- **Issues and feature requests:** open an issue in the repository that owns the affected language or component

## Projects

| Language or component | Repository | Latest release |
| --- | --- | --- |
| Java | [beacon-java](https://github.com/beacon-observability/beacon-java) | [Latest release](https://github.com/beacon-observability/beacon-java/releases/latest) |
| Python | [beacon-python](https://github.com/beacon-observability/beacon-python) | [Latest release](https://github.com/beacon-observability/beacon-python/releases/latest) |
| .NET | [beacon-dotnet](https://github.com/beacon-observability/beacon-dotnet) | [Latest release](https://github.com/beacon-observability/beacon-dotnet/releases/latest) |
| Node.js | [beacon-nodejs](https://github.com/beacon-observability/beacon-nodejs) | [Latest release](https://github.com/beacon-observability/beacon-nodejs/releases/latest) |
| PHP | [beacon-php](https://github.com/beacon-observability/beacon-php) | [Latest release](https://github.com/beacon-observability/beacon-php/releases/latest) |
| PHP native instrumentation | [beacon-php-instrumentation](https://github.com/beacon-observability/beacon-php-instrumentation) | [Latest release](https://github.com/beacon-observability/beacon-php-instrumentation/releases/latest) |
| Rumable (browser RUM) | [rumable](https://github.com/beacon-observability/rumable) | [Latest release](https://github.com/beacon-observability/rumable/releases/latest) |

## Browser RUM with Rumable

Rumable injects its bundled Web SDK into HTML responses through Linux/Nginx or Windows/IIS. Browsers send telemetry directly to the configured RUM receiver. The standalone `rumable` CLI keeps its own TOML configuration and release schedule; browser reporting is configured separately from server-side OTLP export.

Start with the [Rumable guide](https://beacon-observability.github.io/docs/rumable), open the [English configuration page](https://beacon-observability.github.io/rumable/latest/setup/index.html), or download [v0.1.9](https://github.com/beacon-observability/rumable/releases/tag/v0.1.9). Generated commands select a fixed GitHub Release package and verify its SHA256 before installation.

## Maintenance principles

- Preserve upstream Git history, licenses, package identities, and source provenance.
- Keep Beacon-specific enhancements, tests, versions, and release processes explicit.
- Pin reviewed upstream commits or releases instead of silently following moving branches.
- Validate release artifacts in clean environments and publish checksums with versioned release notes.
- Contribute generally useful fixes upstream while retaining verified downstream fixes when release timelines require them.

## Contributing

- Maintain cross-language product documentation and shared policies in [beacon](https://github.com/beacon-observability/beacon).
- Submit runtime instrumentation, browser RUM, tests, and release changes to the corresponding component repository.
- Submit end-user documentation improvements to [docs](https://github.com/beacon-observability/docs).
- Review the target repository's contribution guide and validation requirements before opening a pull request.

Beacon repositories are maintained under their respective open source licenses. OpenTelemetry is a [Cloud Native Computing Foundation](https://www.cncf.io/) project.

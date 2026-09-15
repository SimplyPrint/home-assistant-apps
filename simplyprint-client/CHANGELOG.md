# Changelog

## 1.0.0-rc.17

- [SimplyPrint Client 1.0.0-rc.17](https://github.com/SimplyPrint/simplyprint-client/releases/tag/1.0.0-rc.17)

## 1.0.0-rc.16

- [SimplyPrint Client 1.0.0-rc.16](https://github.com/SimplyPrint/simplyprint-client/releases/tag/1.0.0-rc.16)

## 1.0.0rc15.dev9701

- [SimplyPrint Client 1.0.0rc15.dev9701](https://github.com/SimplyPrint/simplyprint-client/actions/runs/31827332495)

## 1.0.0rc15.dev9601

- [SimplyPrint Client 1.0.0rc15.dev9601](https://github.com/SimplyPrint/simplyprint-client/actions/runs/31816754853)

## 1.0.0-rc.15

- Initial experimental Home Assistant app release.
- Added authenticated Home Assistant Ingress with a seamless **Open Web UI**.
- Restricted the host-network management socket to the Supervisor proxy.
- Removed the duplicate Home Assistant options/password configuration bridge.
- Switched to a Supervisor-assigned dynamic Ingress port to avoid host conflicts.
- Use Home Assistant's generic cloud icon in the sidebar.
- Optimized Ingress browser caching without allowing stale HTML or API state.
- Show Home Assistant-owned settings as individually locked fields alongside
  any editable settings on the same page.
- Skip the desktop taskbar integration in containers to avoid headless display
  errors and noisy tracebacks.
- Let Home Assistant own container updates and make the in-client update channel
  read-only.
- Read deployment-owned setting labels from package metadata instead of
  client-specific platform checks.
- Remove environment overrides already supplied by the container image.
- Simplify the app documentation around installation and everyday use.

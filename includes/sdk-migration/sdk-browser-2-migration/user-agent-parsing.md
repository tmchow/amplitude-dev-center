Starting Browser SDK 2.0, Amplitude replaced enrichment of user properties relating to user agent from client-side to server-side. The enriched user properties include `os_name`, `os_version`, `device_model`, `device_manufacturer`. While the new enrichment strategy yields more accurate results, it also yields slightly different results than Browser SDK 1.0 and may impact your existing analytics charts that query these properties. To prevent this breaking change from impacting you, install [@amplitude/plugin-user-agent-enrichment-browser](https://www.npmjs.com/package/@amplitude/plugin-user-agent-enrichment-browser) to configure Amplitude to enrich these user properties on the client-side and yield enrichment results similar to Browser SDK 1.0. Please visit our [documentation](https://www.npmjs.com/package/@amplitude/plugin-user-agent-enrichment-browser) for more details.
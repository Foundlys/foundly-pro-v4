# Foundly OS v3.0.2 - Integration Control Fix

Railway-safe single-file runtime update.

Fixes:
- Integration Center now uses authoritative /api/connectors status.
- Google Ads, GA4, Search Console and Calendar use the central Google OAuth connection.
- OpenAI no longer asks for production API secrets in browser prompts; use Railway OPENAI_API_KEY.
- TEST actions use the correct dedicated status/probe path for Google/OpenAI.
- SYNC/PROFILE/ONTKOPPEL are disabled where they are not valid for centrally managed services.
- OAuth return can reopen Integrations.
- Generic runtime remains available for provider-specific connectors.

Deploy the files at repository root. Keep existing Railway Variables.

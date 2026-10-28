# Privacy and connected-service disclosures

AI CMO is maintained by Khadin Akbar. The plugin has no publisher-operated telemetry collector, hosted memory database, bundled server or credential store. The selected model host processes the current task under its own policies. This does not mean that connected services retain no data.

## Selected task materials

Use only the inline business brief and bounded data rows supplied for the requested marketing task. Do not query or extract user-generated/uploaded files even when selected. Do not query Claude memory, chat history or conversation summaries, silently mine uploaded files, infer personal traits or persist conversation-derived profiles/preferences across sessions. Default to inline results. Requested briefs, campaign files, reports and handoffs stay in the selected project workspace under host controls. They are task artifacts, not changes to Claude's behavior.

Minimize personal data. Pasted lead rows can contain company/contact fields and suppression state; do not collect contacts when company qualification is sufficient. Do not include secrets, unrelated CRM exports, patient/donor records or raw conversations in shared context, reports or delegation packets.

## Optional external processing

External calls require actual supported host capability, a requested destination that passes the directory service-admission gate, and the exact authorized input/action/cost scope. Otherwise provide a local draft/import or manual handoff. Authentication and account access do not grant collection, sending or spending authority.

| Service | Data sent only for the requested operation | Retention/privacy authority |
| --- | --- | --- |
| Apify and exact publisher-owned Actor | Selected bounded research input; provider may store run input, output, logs and usage in the account/platform | [Apify privacy](https://docs.apify.com/legal/privacy-policy). Verify the actual account/run retention and current Actor behavior before live use; no universal deletion period is promised |
| Postiz and selected social destination | Approved post text, existing media and destination/time | [Postiz privacy](https://postiz.com/privacy-policy), selected deployment operator and destination network policies |
| Resend | Authorized recipient/sender fields and message content | [Resend privacy](https://resend.com/legal/privacy-policy) and account delivery/log settings |
| WordPress site | Approved content and selected site references | The actual site/hosting operator's policy; [Automattic privacy](https://automattic.com/privacy/) applies only when its covered services are involved |
| Humanizer PRO and downstream Rephrasy | Only the passage explicitly selected for an authorized rewrite; word usage and private source/output history may be retained | [Humanizer PRO privacy](https://texthumanizer.pro/privacy) and [Rephrasy privacy](https://www.rephrasy.ai/privacy-policy); inspect downstream processing and retention before use |

AI video/audio/voice/general image generation and Agent Media calls are disabled in this edition, so no generation script, voice or identity input is transmitted through a media-generation route. Design-only visual aids require a permitted available tool and that tool's actual privacy/rights review.

## Control and deletion

Keep credentials in the external tool's normal secure authentication mechanism; never paste them into chat, Actor inputs, request examples, reports or portable files. AI CMO does not read or forward unrelated credentials from the user's computer. Sign-in is completed through the provider's supported flow.

Inspect/export/delete selected local artifacts through the host and provider-held data through the actual provider. Removing the plugin does not delete accounts, posted content, runs, workspace files or registered host schedules. No provider retention/deletion guarantee is inferred from the plugin having no telemetry backend. Feedback changes the current artifact; saving an issue or revised project brief requires the user's request.

Report privacy concerns using [support](SUPPORT.md). Share only a minimal redacted reproduction; never upload raw customer data or credentials to a public issue.

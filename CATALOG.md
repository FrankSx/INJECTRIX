# INJECTRIX — Unified Snippet Catalog

| # | ID | Category | Title | Risk |
|---|---|---|---|---|
| 1 | zz-irx-bootstrap | Report | IRX Bootstrap — Report Engine | utility |
| 2 | enum-scripts | Recon | Enumerate Loaded Scripts | read-only |
| 3 | enum-meta | Recon | Meta & Comment Harvest | read-only |
| 4 | enum-endpoints | Recon | JS Source Endpoint Extraction | active (requests) |
| 5 | enum-storage | Recon | Full Storage Dump | read-only |
| 6 | enum-frames | Recon | Frame / Window Map | read-only |
| 7 | enum-tech | Recon | Framework / Tech Fingerprint | read-only |
| 8 | enum-sourcemaps | Recon | Source Map Detector | active (requests) |
| 9 | enum-csp | Recon | CSP Parser & Gap Analysis | read-only |
| 10 | hook-fetch | Traffic Hooks | Fetch Interceptor Logger | instrumentation |
| 11 | hook-xhr | Traffic Hooks | XHR Interceptor Logger | instrumentation |
| 12 | hook-ws | Traffic Hooks | WebSocket Sniffer | instrumentation |
| 13 | hook-history | Traffic Hooks | History / SPA Route Spy | instrumentation |
| 14 | hook-postmsg | Traffic Hooks | postMessage Monitor | instrumentation |
| 15 | hook-forms | Traffic Hooks | Form Submit Capturer | instrumentation |
| 16 | auth-jwt-decode | Auth & Tokens | JWT Decoder + Expiry Check | read-only |
| 17 | auth-cookie-flags | Auth & Tokens | Cookie Security Audit | read-only |
| 18 | auth-header-replay | Auth & Tokens | Replay Request w/ Modified Token | active (requests) |
| 19 | auth-csrf-scan | Auth & Tokens | CSRF Token Harvester | read-only |
| 20 | dom-sinks | DOM Analysis | Dangerous Sink Finder | read-only |
| 21 | dom-shadow | DOM Analysis | Shadow DOM Mapper | read-only |
| 22 | dom-params | DOM Analysis | URL Param Reflector | read-only |
| 23 | dom-datasources | DOM Analysis | data-* / Template Debug Attributes | read-only |
| 24 | dom-accessibility | DOM Analysis | Accessibility Tree Harvest | read-only |
| 25 | inj-xss-probe | Injection Testing | Reflected Context Probe | active (payload) |
| 26 | inj-proto-poll | Injection Testing | Prototype Pollution Probe | active (payload) |
| 27 | inj-dom-clobber | Injection Testing | DOM Clobbering Surface | read-only |
| 28 | inj-template | Injection Testing | Client-Side Template Detector | read-only |
| 29 | inj-csp-bypass-check | Injection Testing | CSP Bypass Feasibility | read-only |
| 30 | fw-vue-state | Framework | Vue App State Extractor | read-only |
| 31 | fw-react-props | Framework | React Fiber Walker | read-only |
| 32 | fw-next-data | Framework | Next.js __NEXT_DATA__ Extractor | read-only |
| 33 | fw-angular-scope | Framework | Angular Scope Dumper | read-only |
| 34 | eg-domain | Egress | Outbound Channel Tester | active (requests) |
| 35 | eg-blind | Egress | Blind Injection Validator | active (requests) |
| 36 | util-watch | Utility | Selector Watcher | utility |
| 37 | util-persist | Utility | Session State Persist + Restore | utility |
| 38 | util-clip | Utility | Clipboard / Selection Grabber | utility |
| 39 | util-debo | Utility | Event Debugger (monitorEvents) | utility |
| 40 | util-netlog | Utility | Performance Resource Timeline | read-only |
| 41 | util-sw | Utility | Service Worker Interrogator | read-only |
| 42 | adv-canary-flood | Advanced | Canary Flood — All Sources | active (payload) |
| 43 | adv-sink-scan | Advanced | Canary Sink Scanner w/ Context | read-only |
| 44 | adv-pp-gadgets | Advanced | Prototype Pollution Gadget Scanner | active (payload) |
| 45 | adv-postmsg-fuzz | Advanced | postMessage Origin-Spoof Fuzzer | active (payload) |
| 46 | adv-cors-check | Advanced | CORS Misconfiguration Tester | active (requests) |
| 47 | adv-xsleak-cache | Advanced | XS-Leak Cache Probe (Error-Event Oracle) | active (requests) |
| 48 | adv-frame-oracle | Advanced | Frame-Count / Window Oracle | utility |
| 49 | adv-redirect-hunt | Advanced | Client-Side Redirect Sink Hunt | active (requests) |
| 50 | adv-open-redirect-poc | Advanced | Open-Redirect PoC Builder | active (requests) |
| 51 | adv-dangling-markup | Advanced | Dangling-Markup Exfil Probe | active (payload) |
| 52 | adv-graphql-probe | Advanced | GraphQL Endpoint Probe | active (requests) |
| 53 | adv-jwt-confuse | Advanced | JWT Alg-Confusion / none Probe | active (requests) |
| 54 | adv-sw-poison | Advanced | Service Worker Cache-Poison Auditor | active (requests) |
| 55 | adv-reflected-polyglot | Advanced | Context-Aware XSS Polyglot Cannon | active (payload) |
| 56 | auto-param-miner | Automation | Parameter Miner (Reflection Brute) | active (requests) |
| 57 | auto-route-walk | Automation | SPA Route Walker | active (requests) |
| 58 | auto-api-map | Automation | Live API Call Grapher | instrumentation |
| 59 | auto-dom-diff | Automation | DOM Drift Differ | utility |
| 60 | auto-headless-hints | Automation | Bot/Automation Detection Audit | read-only |
| 61 | mxss-roundtrip | mXSS | innerHTML Round-Trip Mutation Tester | active (payload) |
| 62 | mxss-namespace | mXSS | Namespace Confusion Cannon (SVG/MathML) | active (payload) |
| 63 | mxss-domparser-diff | mXSS | DOMParser / innerHTML Differential | active (payload) |
| 64 | mxss-template | mXSS | Template / Declarative Shadow DOM Probe | read-only |
| 65 | mxss-paste | mXSS | Paste Sanitizer Audit (Editor mXSS) | instrumentation |
| 66 | mxss-attr-pivot | mXSS | Attribute Pivot / Dangling Combos | active (payload) |
| 67 | mxss-observer | mXSS | DOM Clobber + Mutation Combo Watcher | instrumentation |

<p align="center">
  <img src="./assets/seatlayer-developer-platform.svg" alt="SeatLayer seat map APIs and SDKs for web, mobile, and backend applications" width="100%">
</p>

SeatLayer is interactive seating chart software built for stadium scale.
Platforms embed the white-label seat picker with their own checkout; organizers
sell seated events on their own website with their own payment gateway.

[Seat map SDK and API overview](https://seatlayer.io/developers/) ·
[Documentation](https://docs.seatlayer.io/) ·
[Seating chart demos](https://app.seatlayer.io/demo) ·
[Support](mailto:hello@seatlayer.io)

[![SeatLayer interactive seating chart with ticket categories, live availability, and best-available seat selection](https://seatlayer.io/assets/product/interactive-seating-chart-buyer-picker.jpg)](https://app.seatlayer.io/demo/play/grand-theatre)

[Try the Grand Theatre seat picker](https://app.seatlayer.io/demo/play/grand-theatre) ·
[Explore the 200,000-seat stadium](https://app.seatlayer.io/demo/play/century-stadium-200k) ·
[See the interactive 3D seat view](https://seatlayer.io/3d-seat-map/)

Platforms embed the seat picker in the client with a public key and confirm the booking from their server with a secret key, keeping checkout and their own payment provider. Organizers sell on their own site with hosted checkout on the gateway they connect.

**Start here:** [Quickstart](https://docs.seatlayer.io/start/quickstart/) · [Holds and checkout](https://docs.seatlayer.io/buyer-sdk/holds-and-checkout/) · [SDK catalog](https://docs.seatlayer.io/sdk-catalog.json) · [Pricing](https://seatlayer.io/pricing/): $0 entry, 100 free confirmed-sold-seat credits per organization each month, then $0.10 down to $0.05 a credit, and credits never expire.

**Runnable examples:** [React and Vite](https://github.com/seatlayer/seatlayer-react-example) is a Vite app with the headless seating chart, best available, seat holds, and a checkout handoff. [Next.js 15](https://github.com/seatlayer/seatlayer-nextjs-example) is the App Router version of the same flow with an `/api/hold` server route. Both read an `.env.local` with your event key and public key, and deploy from the buttons in their READMEs.

## Scale evidence

Benchmarked on public 100,000-, 150,000- and 200,000-seat venue fixtures on 15 September 2026: 200,000 seats chart-ready in 1.95 s, desktop, local production build. Fixtures, method and run logs: https://github.com/seatlayer/seatlayer-performance. Live 200,000-seat stadium demo: https://app.seatlayer.io/demo/play/century-stadium-200k. This is renderer evidence, not a concurrent-buyer claim.

## Choose a seat map SDK

| Platform | Package | Guide and examples |
| --- | --- | --- |
| JavaScript / TypeScript | [`@seatlayer/js`](https://www.npmjs.com/package/@seatlayer/js) | [JavaScript seat map SDK](https://docs.seatlayer.io/buyer-sdk/install/) |
| React | [`@seatlayer/react`](https://www.npmjs.com/package/@seatlayer/react) | [React seating chart components](https://docs.seatlayer.io/buyer-sdk/react/) |
| Vue | [`@seatlayer/vue`](https://www.npmjs.com/package/@seatlayer/vue) | [Vue seating chart components](https://docs.seatlayer.io/buyer-sdk/vue/) |
| Angular | [`@seatlayer/angular`](https://www.npmjs.com/package/@seatlayer/angular) | [Angular seating chart components](https://docs.seatlayer.io/buyer-sdk/angular/) |
| Flutter | [`seatlayer`](https://pub.dev/packages/seatlayer) | [Flutter seat picker SDK](https://docs.seatlayer.io/buyer-sdk/flutter/) |
| React Native / Expo | [`@seatlayer/react-native`](https://www.npmjs.com/package/@seatlayer/react-native) | [React Native seat map SDK](https://docs.seatlayer.io/buyer-sdk/react-native/) |
| Swift / SwiftUI | [iOS Swift package](https://github.com/seatlayer/seatlayer-ios) | [iOS seating chart SDK](https://docs.seatlayer.io/buyer-sdk/ios/) |
| Kotlin / Jetpack Compose | [Android Maven package](https://central.sonatype.com/artifact/io.seatlayer/seatlayer-android) | [Android seating chart SDK](https://docs.seatlayer.io/buyer-sdk/android/) |

<details>
<summary>See the mobile seat picker and 3D view in action</summary>

<p align="center">
  <a href="https://docs.seatlayer.io/buyer-sdk/flutter/">
    <img src="https://raw.githubusercontent.com/seatlayer/seatlayer-flutter/main/doc/media/picker-flow.gif" alt="SeatLayer Flutter picker walkthrough from venue overview to seat selection and 3D view" width="240">
  </a>
</p>

[Build this with the Flutter seat map SDK](https://docs.seatlayer.io/buyer-sdk/flutter/).

</details>

## Connect your backend

Use a server SDK to inspect holds, confirm bookings, manage events and inventory,
and verify webhooks. In a Platform/SDK integration, your backend owns payment,
orders, tickets, and refunds.

| Language | Package | Guide |
| --- | --- | --- |
| Node.js | [`@seatlayer/server`](https://www.npmjs.com/package/@seatlayer/server) | [Node.js server SDK](https://docs.seatlayer.io/server-sdk/node/) |
| Python | [`seatlayer`](https://pypi.org/project/seatlayer/) | [Python server SDK](https://docs.seatlayer.io/server-sdk/python/) |
| PHP | [`seatlayer/seatlayer-php`](https://packagist.org/packages/seatlayer/seatlayer-php) | [PHP server SDK](https://docs.seatlayer.io/server-sdk/php/) |
| Java | [`io.seatlayer:seatlayer-java`](https://central.sonatype.com/artifact/io.seatlayer/seatlayer-java) | [Java server SDK](https://docs.seatlayer.io/server-sdk/java/) |
| Go | [`github.com/seatlayer/seatlayer-go`](https://pkg.go.dev/github.com/seatlayer/seatlayer-go) | [Go server SDK](https://docs.seatlayer.io/server-sdk/go/) |
| Ruby | [`seatlayer`](https://rubygems.org/gems/seatlayer) | [Ruby server SDK](https://docs.seatlayer.io/server-sdk/ruby/) |
| .NET | [`SeatLayer`](https://www.nuget.org/packages/SeatLayer) | [.NET server SDK](https://docs.seatlayer.io/server-sdk/dotnet/) |

## Build the seating experience

- **Customize the buyer UI:** choose the complete picker or compose a chart with
  your own controls. Start with your platform guide above.
- **Add 3D seat views:** explore the [interactive 3D seating chart](https://seatlayer.io/3d-seat-map/)
  and the supported buyer-view controls.
- **Design venues inside your product:** use [embedded Designer sessions](https://docs.seatlayer.io/platform/embedded-designer/)
  for chart authoring in your organizer interface.
- **Work with agents:** use the [SeatLayer AI Toolkit](https://github.com/seatlayer/seatlayer-ai-toolkit)
  for integration help and the [buyer WebMCP tools](https://docs.seatlayer.io/buyer-sdk/webmcp-agent-tools/)
  for seat selection in compatible browser assistants.
- **Try a large chart:** open the [200,000-seat stadium demo](https://app.seatlayer.io/demo/play/century-stadium-200k)
  and read the [renderer performance documentation](https://docs.seatlayer.io/platform/renderer-performance/).

## Hosted ticketing and WordPress

Managed Ticketing provides event pages and checkout using the organizer's
connected payment account. The [WordPress seating chart plugin](https://github.com/seatlayer/seatlayer-wordpress)
embeds that buyer experience in an existing site. See the
[WordPress integration guide](https://docs.seatlayer.io/integrations/wordpress/)
for the approved Managed account requirement and setup.

[Choose an integration](https://docs.seatlayer.io/start/choose-an-integration/) ·
[Service pricing](https://seatlayer.io/pricing/)

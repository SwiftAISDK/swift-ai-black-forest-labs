<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-black-forest-labs 1.2.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-black-forest-labs.git", from: "1.2.0")
```

Products: `SwiftAIBlackForestLabs`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# Black Forest Labs for Swift

`SwiftAIBlackForestLabs` adds Black Forest Labs to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/black-forest-labs` and supports image generation and video generation.

Provider guide with models, options, streaming and errors:

- [Black Forest Labs](https://swiftaisdk.github.io/SwiftAISDK/providers/black-forest-labs/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIBlackForestLabs` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIBlackForestLabs

let provider = try AIProviders.blackForestLabs(configuration: BlackForestLabsProviderSettings())
```

By default the provider reads `BFL_API_KEY` and `BLACK_FOREST_LABS_API_KEY` from the environment; values set in `BlackForestLabsProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-black-forest-labs` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.

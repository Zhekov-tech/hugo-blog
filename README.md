<<<<<<< HEAD
[bep]: https://github.com/bep
[bugs]: https://github.com/gohugoio/hugo/issues?q=is%3Aopen+is%3Aissue+label%3ABug
[contributing]: CONTRIBUTING.md
[create a proposal]: https://github.com/gohugoio/hugo/issues/new?labels=Proposal%2C+NeedsTriage&template=feature_request.md
[documentation repository]: https://github.com/gohugoio/hugoDocs
[documentation]: https://gohugo.io/documentation
[dragonfly bsd, freebsd, netbsd, and openbsd]: https://gohugo.io/installation/bsd
[features]: https://gohugo.io/about/features/
[forum]: https://discourse.gohugo.io
[friends]: https://github.com/gohugoio/hugo/graphs/contributors
[go]: https://go.dev/
[hugo modules]: https://gohugo.io/hugo-modules/
[installation]: https://gohugo.io/installation
[issue queue]: https://github.com/gohugoio/hugo/issues
[linux]: https://gohugo.io/installation/linux
[macos]: https://gohugo.io/installation/macos
[prebuilt binary]: https://github.com/gohugoio/hugo/releases/latest
[requesting help]: https://discourse.gohugo.io/t/requesting-help/9132
[spf13]: https://github.com/spf13
[static site generator]: https://en.wikipedia.org/wiki/Static_site_generator
[support]: https://discourse.gohugo.io
[themes]: https://themes.gohugo.io/
[website]: https://gohugo.io
[windows]: https://gohugo.io/installation/windows

<a href="https://gohugo.io/"><img src="https://raw.githubusercontent.com/gohugoio/gohugoioTheme/master/static/images/hugo-logo-wide.svg?sanitize=true" alt="Hugo" width="565"></a>

A fast and flexible static site generator built with love by [bep], [spf13], and [friends] in [Go].

---

[![GoDoc](https://godoc.org/github.com/gohugoio/hugo?status.svg)](https://godoc.org/github.com/gohugoio/hugo)
[![Tests on Linux, MacOS and Windows](https://github.com/gohugoio/hugo/workflows/Test/badge.svg)](https://github.com/gohugoio/hugo/actions?query=workflow%3ATest)
[![Go Report Card](https://goreportcard.com/badge/github.com/gohugoio/hugo)](https://goreportcard.com/report/github.com/gohugoio/hugo)

[Website] | [Installation] | [Documentation] | [Support] | [Contributing] | <a rel="me" href="https://fosstodon.org/@gohugoio">Mastodon</a> | <a rel="me" href="https://x.com/gohugoiov2">X</a>

## Overview

Hugo is a [static site generator] written in [Go], optimized for speed and designed for flexibility. With its advanced templating system and fast asset pipelines, Hugo renders a complete site in seconds, often less.

Due to its flexible framework, multilingual support, and powerful taxonomy system, Hugo is widely used to create:

- Corporate, government, nonprofit, education, news, event, and project sites
- Documentation sites
- Image portfolios
- Landing pages
- Business, professional, and personal blogs
- Resumes and CVs

Use Hugo's embedded web server during development to instantly see changes to content, structure, behavior, and presentation. Then deploy the site to your host, or push changes to your Git provider for automated builds and deployment.

Hugo's fast asset pipelines include:

- Image processing &ndash; Convert, resize, crop, rotate, adjust colors, apply filters, overlay text and images, and extract EXIF data
- JavaScript bundling &ndash; Transpile TypeScript and JSX to JavaScript, bundle, tree shake, minify, create source maps, and perform SRI hashing.
- Sass processing &ndash; Transpile Sass to CSS, bundle, tree shake, minify, create source maps, perform SRI hashing, and integrate with PostCSS
- Tailwind CSS processing &ndash; Compile Tailwind CSS utility classes into standard CSS, bundle, tree shake, optimize, minify, perform SRI hashing, and integrate with PostCSS

And with [Hugo Modules], you can share content, assets, data, translations, themes, templates, and configuration with other projects via public or private Git repositories.

See the [features] section of the documentation for a comprehensive summary of Hugo's capabilities.

## Sponsors

<p>&nbsp;</p>
<p float="left">
  <a href="https://www.linode.com/?utm_campaign=hugosponsor&utm_medium=banner&utm_source=hugogithub" target="_blank"><img src="https://raw.githubusercontent.com/gohugoio/gohugoioTheme/master/assets/images/sponsors/linode-logo_standard_light_medium.png" width="200" alt="Linode"></a>
&nbsp;&nbsp;&nbsp;
  <a href="https://route4me.com/" target="_blank"><img src="https://raw.githubusercontent.com/gohugoio/gohugoioTheme/master/assets/images/sponsors/Route4MeLogoBlueOnWhite.svg" width="200" alt="Route Planning & Route Optimization Software"></a>
</p>

## Installation

Install Hugo from a [prebuilt binary], package manager, or package repository. Please see the installation instructions for your operating system:

- [macOS]
- [Linux]
- [Windows]
- [DragonFly BSD, FreeBSD, NetBSD, and OpenBSD]

## Build from source

Hugo is available in two editions: standard and extended. With the extended edition you can:

- Encode to the WebP format when processing images. You can decode WebP images with either edition.
- Transpile Sass to CSS using the embedded LibSass transpiler. The extended edition is not required to use the Dart Sass transpiler.

Prerequisites to build Hugo from source:

- Standard edition: Go 1.20 or later
- Extended edition: Go 1.20 or later, and GCC

Build the standard edition:

```text
go install github.com/gohugoio/hugo@latest
```

Build the extended edition:

```text
CGO_ENABLED=1 go install -tags extended github.com/gohugoio/hugo@latest
```

## Documentation

Hugo's [documentation] includes installation instructions, a quick start guide, conceptual explanations, reference information, and examples.

Please submit documentation issues and pull requests to the [documentation repository].

## Support

Please **do not use the issue queue** for questions or troubleshooting. Unless you are certain that your issue is a software defect, use the [forum].

Hugo’s [forum] is an active community of users and developers who answer questions, share knowledge, and provide examples. A quick search of over 20,000 topics will often answer your question. Please be sure to read about [requesting help] before asking your first question.

## Contributing

You can contribute to the Hugo project by:

- Answering questions on the [forum]
- Improving the [documentation]
- Monitoring the [issue queue]
- Creating or improving [themes]
- Squashing [bugs]

Please submit documentation issues and pull requests to the [documentation repository].

If you have an idea for an enhancement or new feature, create a new topic on the [forum] in the "Feature" category. This will help you to:

- Determine if the capability already exists
- Measure interest
- Refine the concept

If there is sufficient interest, [create a proposal]. Do not submit a pull request until the project lead accepts the proposal.

For a complete guide to contributing to Hugo, see the [Contribution Guide](CONTRIBUTING.md).

## Dependencies

Hugo stands on the shoulders of great open source libraries. Run `hugo env --logLevel info` to display a list of dependencies.

<details>
<summary>See current dependencies</summary>

```text
cloud.google.com/go/compute/metadata="v0.2.3"
cloud.google.com/go/iam="v1.1.5"
cloud.google.com/go/storage="v1.35.1"
cloud.google.com/go="v0.110.10"
github.com/Azure/azure-sdk-for-go/sdk/azcore="v1.9.0"
github.com/Azure/azure-sdk-for-go/sdk/azidentity="v1.4.0"
github.com/Azure/azure-sdk-for-go/sdk/internal="v1.5.0"
github.com/Azure/azure-sdk-for-go/sdk/storage/azblob="v1.2.0"
github.com/Azure/go-autorest/autorest/to="v0.4.0"
github.com/AzureAD/microsoft-authentication-library-for-go="v1.2.0"
github.com/BurntSushi/locker="v0.0.0-20171006230638-a6e239ea1c69"
github.com/alecthomas/chroma/v2="v2.14.0"
github.com/armon/go-radix="v1.0.1-0.20221118154546-54df44f2176c"
github.com/aws/aws-sdk-go-v2/aws/protocol/eventstream="v1.5.4"
github.com/aws/aws-sdk-go-v2/config="v1.26.1"
github.com/aws/aws-sdk-go-v2/credentials="v1.16.12"
github.com/aws/aws-sdk-go-v2/feature/ec2/imds="v1.14.10"
github.com/aws/aws-sdk-go-v2/feature/s3/manager="v1.15.7"
github.com/aws/aws-sdk-go-v2/internal/configsources="v1.3.5"
github.com/aws/aws-sdk-go-v2/internal/endpoints/v2="v2.6.5"
github.com/aws/aws-sdk-go-v2/internal/ini="v1.7.2"
github.com/aws/aws-sdk-go-v2/internal/v4a="v1.2.9"
github.com/aws/aws-sdk-go-v2/service/cloudfront="v1.35.4"
github.com/aws/aws-sdk-go-v2/service/internal/accept-encoding="v1.10.4"
github.com/aws/aws-sdk-go-v2/service/internal/checksum="v1.2.9"
github.com/aws/aws-sdk-go-v2/service/internal/presigned-url="v1.10.9"
github.com/aws/aws-sdk-go-v2/service/internal/s3shared="v1.16.9"
github.com/aws/aws-sdk-go-v2/service/s3="v1.47.5"
github.com/aws/aws-sdk-go-v2/service/sso="v1.18.5"
github.com/aws/aws-sdk-go-v2/service/ssooidc="v1.21.5"
github.com/aws/aws-sdk-go-v2/service/sts="v1.26.5"
github.com/aws/aws-sdk-go-v2="v1.26.1"
github.com/aws/aws-sdk-go="v1.50.7"
github.com/aws/smithy-go="v1.20.2"
github.com/bep/clocks="v0.5.0"
github.com/bep/debounce="v1.2.0"
github.com/bep/gitmap="v1.1.2"
github.com/bep/goat="v0.5.0"
github.com/bep/godartsass/v2="v2.0.0"
github.com/bep/godartsass="v1.2.0"
github.com/bep/golibsass="v1.1.1"
github.com/bep/gowebp="v0.3.0"
github.com/bep/lazycache="v0.4.0"
github.com/bep/logg="v0.4.0"
github.com/bep/mclib="v1.20400.20402"
github.com/bep/overlayfs="v0.9.2"
github.com/bep/simplecobra="v0.4.0"
github.com/bep/tmc="v0.5.1"
github.com/clbanning/mxj/v2="v2.7.0"
github.com/cli/safeexec="v1.0.1"
github.com/cpuguy83/go-md2man/v2="v2.0.3"
github.com/disintegration/gift="v1.2.1"
github.com/dlclark/regexp2="v1.11.0"
github.com/dustin/go-humanize="v1.0.1"
github.com/evanw/esbuild="v0.21.4"
github.com/fatih/color="v1.16.0"
github.com/frankban/quicktest="v1.14.6"
github.com/fsnotify/fsnotify="v1.7.0"
github.com/getkin/kin-openapi="v0.123.0"
github.com/ghodss/yaml="v1.0.0"
github.com/go-openapi/jsonpointer="v0.20.2"
github.com/go-openapi/swag="v0.22.8"
github.com/gobuffalo/flect="v1.0.2"
github.com/gobwas/glob="v0.2.3"
github.com/gohugoio/go-i18n/v2="v2.1.3-0.20230805085216-e63c13218d0e"
github.com/gohugoio/httpcache="v0.7.0"
github.com/gohugoio/hugo-goldmark-extensions/extras="v0.2.0"
github.com/gohugoio/hugo-goldmark-extensions/passthrough="v0.2.0"
github.com/gohugoio/locales="v0.14.0"
github.com/gohugoio/localescompressed="v1.0.1"
github.com/golang-jwt/jwt/v5="v5.1.0"
github.com/golang/groupcache="v0.0.0-20210331224755-41bb18bfe9da"
github.com/golang/protobuf="v1.5.3"
github.com/google/go-cmp="v0.6.0"
github.com/google/s2a-go="v0.1.7"
github.com/google/uuid="v1.4.0"
github.com/google/wire="v0.5.0"
github.com/googleapis/enterprise-certificate-proxy="v0.3.2"
github.com/googleapis/gax-go/v2="v2.12.0"
github.com/gorilla/websocket="v1.5.1"
github.com/hairyhenderson/go-codeowners="v0.4.0"
github.com/hashicorp/golang-lru/v2="v2.0.7"
github.com/invopop/yaml="v0.2.0"
github.com/jdkato/prose="v1.2.1"
github.com/jmespath/go-jmespath="v0.4.0"
github.com/josharian/intern="v1.0.0"
github.com/kr/pretty="v0.3.1"
github.com/kr/text="v0.2.0"
github.com/kylelemons/godebug="v1.1.0"
github.com/kyokomi/emoji/v2="v2.2.12"
github.com/mailru/easyjson="v0.7.7"
github.com/makeworld-the-better-one/dither/v2="v2.4.0"
github.com/marekm4/color-extractor="v1.2.1"
github.com/mattn/go-colorable="v0.1.13"
github.com/mattn/go-isatty="v0.0.20"
github.com/mattn/go-runewidth="v0.0.9"
github.com/mitchellh/hashstructure="v1.1.0"
github.com/mitchellh/mapstructure="v1.5.1-0.20231216201459-8508981c8b6c"
github.com/mohae/deepcopy="v0.0.0-20170929034955-c48cc78d4826"
github.com/muesli/smartcrop="v0.3.0"
github.com/niklasfasching/go-org="v1.7.0"
github.com/olekukonko/tablewriter="v0.0.5"
github.com/pbnjay/memory="v0.0.0-20210728143218-7b4eea64cf58"
github.com/pelletier/go-toml/v2="v2.2.2"
github.com/perimeterx/marshmallow="v1.1.5"
github.com/pkg/browser="v0.0.0-20210911075715-681adbf594b8"
github.com/pkg/errors="v0.9.1"
github.com/rogpeppe/go-internal="v1.12.0"
github.com/russross/blackfriday/v2="v2.1.0"
github.com/rwcarlsen/goexif="v0.0.0-20190401172101-9e8deecbddbd"
github.com/sass/dart-sass/compiler="1.77.5"
github.com/sass/dart-sass/implementation="1.77.5"
github.com/sass/dart-sass/protocol="2.7.1"
github.com/sass/libsass="3.6.5"
github.com/spf13/afero="v1.11.0"
github.com/spf13/cast="v1.6.0"
github.com/spf13/cobra="v1.8.0"
github.com/spf13/fsync="v0.10.1"
github.com/spf13/pflag="v1.0.5"
github.com/tdewolff/minify/v2="v2.20.20"
github.com/tdewolff/parse/v2="v2.7.13"
github.com/webmproject/libwebp="v1.3.2"
github.com/yuin/goldmark-emoji="v1.0.3"
github.com/yuin/goldmark="v1.7.4"
go.opencensus.io="v0.24.0"
go.uber.org/automaxprocs="v1.5.3"
gocloud.dev="v0.36.0"
golang.org/x/crypto="v0.23.0"
golang.org/x/exp="v0.0.0-20221031165847-c99f073a8326"
golang.org/x/image="v0.16.0"
golang.org/x/mod="v0.17.0"
golang.org/x/net="v0.25.0"
golang.org/x/oauth2="v0.15.0"
golang.org/x/sync="v0.7.0"
golang.org/x/sys="v0.20.0"
golang.org/x/text="v0.15.0"
golang.org/x/time="v0.5.0"
golang.org/x/tools="v0.20.0"
golang.org/x/xerrors="v0.0.0-20231012003039-104605ab7028"
google.golang.org/api="v0.152.0"
google.golang.org/genproto/googleapis/api="v0.0.0-20231120223509-83a465c0220f"
google.golang.org/genproto/googleapis/rpc="v0.0.0-20231120223509-83a465c0220f"
google.golang.org/genproto="v0.0.0-20231120223509-83a465c0220f"
google.golang.org/grpc="v1.59.0"
google.golang.org/protobuf="v1.33.0"
gopkg.in/yaml.v2="v2.4.0"
gopkg.in/yaml.v3="v3.0.1"
software.sslmate.com/src/go-pkcs12="v0.2.0"
```
</details>
=======
# hugo-blog
>>>>>>> eb0e4ac1f0d11210a567bd22b30d1f89d62274f5

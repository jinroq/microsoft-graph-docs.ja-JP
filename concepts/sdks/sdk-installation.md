---
title: Microsoft Graph SDK をインストールする
description: C#、Java、Javascript、目的-C、PHP、および Ruby の Microsoft Graph Sdk をインストールする手順について説明します。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: a46f005e2ff646f420d19741eca3c8c21a95291a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630182"
---
# <a name="install-the-microsoft-graph-sdks"></a>Microsoft Graph Sdk をインストールする

Microsoft Graph Sdk は、GitHub およびポピュラーなプラットフォームパッケージマネージャーを通じてプロジェクトに含めることができます。 このトピックでは、Microsoft Graph SDK をプロジェクトにインストールする方法について説明します。

## <a name="install-the-microsoft-graph-net-sdk"></a>Microsoft Graph .NET SDK をインストールする

Microsoft Graph .NET SDK は、次の NuGet パッケージに含まれています。

* [Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -エンドポイントに`v1.0` fluent API を使用してアクセスするためのモデルと要求ビルダーが含まれています。 Microsoft graph は、Microsoft Graph に依存しています。
* [Microsoft Graph](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet)には、fluent API を使用してエンドポイントに`beta`アクセスするためのモデルと要求ビルダーが含まれています。 Microsoft graph には、Microsoft Graph に依存しています。
* Microsoft graph- [core](https://github.com/microsoftgraph/msgraph-sdk-dotnet)ライブラリを使用して、microsoft graph を呼び出すことができます。
* [](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) MICROSOFT graph SDK と共に使用する Microsoft authentication LIBRARY (msal) の認証シナリオベースのラッパーを提供します。 Microsoft graph は、Microsoft Graph に依存しています。

[Visual Studio またはパッケージマネージャーコンソールでパッケージマネージャー UI](https://docs.microsoft.com/en-us/nuget/quickstart/install-and-use-a-package-in-visual-studio)を使用して、Microsoft graph のパッケージをプロジェクトにインストールすることができます。 次のパッケージマネージャーコンソールコマンドを実行すると、Microsoft graph、microsoft graph、および Microsoft graph ライブラリがインストールされます。 Microsoft graph は、Microsoft Graph の依存関係としてインストールされます。

```
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a>Microsoft Graph Java SDK をインストールする

Microsoft Graph Java SDK は、次のパッケージに含まれています。

* [microsoft graph](https://github.com/microsoftgraph/msgraph-sdk-java) -エンドポイントに`v1.0` fluent API を使用してアクセスするためのモデルと要求ビルダーが含まれています。
* [microsoft](https://github.com/microsoftgraph/msgraph-sdk-java-core) graph-Core-microsoft graph に電話をかけるためのコアライブラリ。
* microsoft graph [-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) -MICROSOFT graph SDK で使用する Microsoft authentication LIBRARY (msal) の認証シナリオベースのラッパーを提供します。

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>Gradle を使用して Microsoft Graph Java SDK をインストールする

Microsoft graph のリポジトリとコンパイル依存関係をプロジェクトの gradle に追加します。

```
repository {
    jcenter()
}

dependency {
    // Include the sdk as a dependency
    compile('com.microsoft.graph:microsoft-graph:1.2.+')
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>Maven を使用して Microsoft Graph Java SDK をインストールする

Pom の dependencies 要素に依存関係を追加します。

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>1.2.0</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Microsoft Graph Javascript SDK をインストールする

Microsoft Graph Javascript SDK は、次のパッケージに含まれています。

* Microsoft Graph への呼び出しを行うためのコアライブラリ ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) (英語) @microsoft
* @microsoft/サンプル ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types))-microsoft graph エンティティの Typescript 型です。

[Npm](https://www.npmjs.com)を使用して、Microsoft GRAPH Javascript SDK をインストールすることができます。

```
npm install @microsoft/microsoft-graph-client
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>Microsoft Graph の目的-C SDK をインストールする

Microsoft Graph の目的-C SDK は、iOS と macOS の両方のプラットフォームをサポートしており、Cocoアポストロフィ Ds または Carthage のどちらかを使用してプロジェクトにインストールできます。

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>Cocoアポストロフィを使用して Microsoft Graph の目標-C SDK をインストールする

Podfile に次の行を追加して、xcode プロジェクトに、目的の C Microsoft Graph SDK および Microsoft Graph の目的-C Auth SDK を含めます。

```
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>Carthage を使用して Microsoft Graph の目標-C SDK をインストールする

次の手順を実行して、 [Carthage](https://github.com/Carthage/Carthage)パッケージマネージャーを使用して、microsoft Graph の目的-c SDK と microsoft Graph の目標-c Auth sdk をインストールします。

1. 目標-C SDK GitHub リポジトリと[リリースタグ](https://github.com/microsoftgraph/msgraph-sdk-objc/releases)を指定する**Cartfile**を作成します。

```
github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
```

2. `carthage update` を実行します。 これにより、依存関係が Carthage/チェックアウトフォルダーにフェッチされ、MSGraphClientSDK ライブラリが作成されます。

3. Xcode を使用して、アプリケーションターゲットの **[全般**設定] タブの [リンクされた**フレームワークとライブラリ**] セクションで、 **Msgraphclientsdk. フレームワーク**と**msgraphmsalauthprovider**をドラッグアンドドロップします。ディスク上にフォルダーを作成します。

4. アプリケーションターゲットの [**ビルドフェーズ**の設定] タブで、 **+** アイコンをクリックして、[**スクリプトフェーズの新規実行**] を選択します。 シェル (ex:/bin/sh) を指定し、次の内容をスクリプトに追加する実行スクリプトを作成します。

```
/usr/local/bin/carthage copy-frameworks
```

5. **入力ファイル**で使用するフレームワークへのパスを追加します。

```
$(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
$(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
```

## <a name="install-the-microsoft-graph-php-sdk"></a>Microsoft Graph PHP SDK をインストールする

[Microsoft GRAPH PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php)は[packagist.org](https://packagist.org/packages/microsoft/microsoft-graph)から入手でき、次の方法でインストールできます。

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>Composer を使用して Microsoft Graph PHP SDK を手動でインストールする

```
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>Composer を使用して Microsoft Graph PHP SDK をインストールする

```
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-graph-ruby-sdk"></a>Microsoft Graph Ruby SDK をインストールする

[Microsoft Graph RUBY SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby)は[rubygems.org](https://rubygems.org/)から入手でき、次のコマンドを使用してインストールできます。

```
gem install microsoft_graph
```

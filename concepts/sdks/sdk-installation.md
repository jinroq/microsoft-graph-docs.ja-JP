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
# <a name="install-the-microsoft-graph-sdks"></a><span data-ttu-id="57fd6-103">Microsoft Graph Sdk をインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-103">Install the Microsoft Graph SDKs</span></span>

<span data-ttu-id="57fd6-104">Microsoft Graph Sdk は、GitHub およびポピュラーなプラットフォームパッケージマネージャーを通じてプロジェクトに含めることができます。</span><span class="sxs-lookup"><span data-stu-id="57fd6-104">The Microsoft Graph SDKs are available to be included in your projects via GitHub and popular platform package managers.</span></span> <span data-ttu-id="57fd6-105">このトピックでは、Microsoft Graph SDK をプロジェクトにインストールする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="57fd6-105">This topic describes how you can install the Microsoft Graph SDK into your project.</span></span>

## <a name="install-the-microsoft-graph-net-sdk"></a><span data-ttu-id="57fd6-106">Microsoft Graph .NET SDK をインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-106">Install the Microsoft Graph .NET SDK</span></span>

<span data-ttu-id="57fd6-107">Microsoft Graph .NET SDK は、次の NuGet パッケージに含まれています。</span><span class="sxs-lookup"><span data-stu-id="57fd6-107">The Microsoft Graph .NET SDK is included in the following NuGet packages:</span></span>

* <span data-ttu-id="57fd6-108">[Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -エンドポイントに`v1.0` fluent API を使用してアクセスするためのモデルと要求ビルダーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57fd6-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span> <span data-ttu-id="57fd6-109">Microsoft graph は、Microsoft Graph に依存しています。</span><span class="sxs-lookup"><span data-stu-id="57fd6-109">Microsoft.Graph has a dependency on Microsoft.Graph.Core.</span></span>
* <span data-ttu-id="57fd6-110">[Microsoft Graph](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet)には、fluent API を使用してエンドポイントに`beta`アクセスするためのモデルと要求ビルダーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57fd6-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span> <span data-ttu-id="57fd6-111">Microsoft graph には、Microsoft Graph に依存しています。</span><span class="sxs-lookup"><span data-stu-id="57fd6-111">Microsoft.Graph.Beta has a dependency on Microsoft.Graph.Core.</span></span>
* <span data-ttu-id="57fd6-112">Microsoft graph- [core](https://github.com/microsoftgraph/msgraph-sdk-dotnet)ライブラリを使用して、microsoft graph を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="57fd6-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - The core library for making calls to Microsoft Graph.</span></span>
* <span data-ttu-id="57fd6-113">[](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) MICROSOFT graph SDK と共に使用する Microsoft authentication LIBRARY (msal) の認証シナリオベースのラッパーを提供します。</span><span class="sxs-lookup"><span data-stu-id="57fd6-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Provides an authentication scenario-based wrapper of the Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span> <span data-ttu-id="57fd6-114">Microsoft graph は、Microsoft Graph に依存しています。</span><span class="sxs-lookup"><span data-stu-id="57fd6-114">Microsoft.Graph.Auth has a dependency on Microsoft.Graph.Core.</span></span>

<span data-ttu-id="57fd6-115">[Visual Studio またはパッケージマネージャーコンソールでパッケージマネージャー UI](https://docs.microsoft.com/en-us/nuget/quickstart/install-and-use-a-package-in-visual-studio)を使用して、Microsoft graph のパッケージをプロジェクトにインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="57fd6-115">You can use either the [Package Manager UI in Visual Studio or the Package Manager Console](https://docs.microsoft.com/en-us/nuget/quickstart/install-and-use-a-package-in-visual-studio) to install the Microsoft.Graph packages into your project.</span></span> <span data-ttu-id="57fd6-116">次のパッケージマネージャーコンソールコマンドを実行すると、Microsoft graph、microsoft graph、および Microsoft graph ライブラリがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="57fd6-116">The following Package Manager Console commands will install the Microsoft.Graph, Microsoft.Graph.Core, and Microsoft.Graph.Auth libraries.</span></span> <span data-ttu-id="57fd6-117">Microsoft graph は、Microsoft Graph の依存関係としてインストールされます。</span><span class="sxs-lookup"><span data-stu-id="57fd6-117">Microsoft.Graph.Core is installed as a dependency of Microsoft.Graph.</span></span>

```
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a><span data-ttu-id="57fd6-118">Microsoft Graph Java SDK をインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-118">Install the Microsoft Graph Java SDK</span></span>

<span data-ttu-id="57fd6-119">Microsoft Graph Java SDK は、次のパッケージに含まれています。</span><span class="sxs-lookup"><span data-stu-id="57fd6-119">The Microsoft Graph Java SDK is included in the following packages:</span></span>

* <span data-ttu-id="57fd6-120">[microsoft graph](https://github.com/microsoftgraph/msgraph-sdk-java) -エンドポイントに`v1.0` fluent API を使用してアクセスするためのモデルと要求ビルダーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57fd6-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span>
* <span data-ttu-id="57fd6-121">[microsoft](https://github.com/microsoftgraph/msgraph-sdk-java-core) graph-Core-microsoft graph に電話をかけるためのコアライブラリ。</span><span class="sxs-lookup"><span data-stu-id="57fd6-121">[microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - The core library for making calls to Microsoft Graph.</span></span>
* <span data-ttu-id="57fd6-122">microsoft graph [-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) -MICROSOFT graph SDK で使用する Microsoft authentication LIBRARY (msal) の認証シナリオベースのラッパーを提供します。</span><span class="sxs-lookup"><span data-stu-id="57fd6-122">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Provides an authentication scenario-based wrapper of Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span>

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a><span data-ttu-id="57fd6-123">Gradle を使用して Microsoft Graph Java SDK をインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-123">Install the Microsoft Graph Java SDK via Gradle</span></span>

<span data-ttu-id="57fd6-124">Microsoft graph のリポジトリとコンパイル依存関係をプロジェクトの gradle に追加します。</span><span class="sxs-lookup"><span data-stu-id="57fd6-124">Add the repository and a compile dependency for microsoft-graph to your project's build.gradle:</span></span>

```
repository {
    jcenter()
}

dependency {
    // Include the sdk as a dependency
    compile('com.microsoft.graph:microsoft-graph:1.2.+')
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a><span data-ttu-id="57fd6-125">Maven を使用して Microsoft Graph Java SDK をインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-125">Install the Microsoft Graph Java SDK via Maven</span></span>

<span data-ttu-id="57fd6-126">Pom の dependencies 要素に依存関係を追加します。</span><span class="sxs-lookup"><span data-stu-id="57fd6-126">Add the dependency in the dependencies element in pom.xml:</span></span>

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>1.2.0</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a><span data-ttu-id="57fd6-127">Microsoft Graph Javascript SDK をインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-127">Install the Microsoft Graph Javascript SDK</span></span>

<span data-ttu-id="57fd6-128">Microsoft Graph Javascript SDK は、次のパッケージに含まれています。</span><span class="sxs-lookup"><span data-stu-id="57fd6-128">The Microsoft Graph Javascript SDK is included in the following packages:</span></span>

* <span data-ttu-id="57fd6-129">Microsoft Graph への呼び出しを行うためのコアライブラリ ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) (英語) @microsoft</span><span class="sxs-lookup"><span data-stu-id="57fd6-129">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- The core library for making calls to Microsoft Graph.</span></span>
* <span data-ttu-id="57fd6-130">@microsoft/サンプル ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types))-microsoft graph エンティティの Typescript 型です。</span><span class="sxs-lookup"><span data-stu-id="57fd6-130">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - The Typescript types for the Microsoft Graph entities.</span></span>

<span data-ttu-id="57fd6-131">[Npm](https://www.npmjs.com)を使用して、Microsoft GRAPH Javascript SDK をインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="57fd6-131">You can use [npm](https://www.npmjs.com) to install the Microsoft Graph Javascript SDK:</span></span>

```
npm install @microsoft/microsoft-graph-client
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a><span data-ttu-id="57fd6-132">Microsoft Graph の目的-C SDK をインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-132">Install the Microsoft Graph Objective-C SDK</span></span>

<span data-ttu-id="57fd6-133">Microsoft Graph の目的-C SDK は、iOS と macOS の両方のプラットフォームをサポートしており、Cocoアポストロフィ Ds または Carthage のどちらかを使用してプロジェクトにインストールできます。</span><span class="sxs-lookup"><span data-stu-id="57fd6-133">The Microsoft Graph Objective-C SDK supports both iOS and macOS platforms and can be installed into your project using either CocoaPods or Carthage.</span></span>

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a><span data-ttu-id="57fd6-134">Cocoアポストロフィを使用して Microsoft Graph の目標-C SDK をインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-134">Install the Microsoft Graph Objective-C SDK using Cocoapods</span></span>

<span data-ttu-id="57fd6-135">Podfile に次の行を追加して、xcode プロジェクトに、目的の C Microsoft Graph SDK および Microsoft Graph の目的-C Auth SDK を含めます。</span><span class="sxs-lookup"><span data-stu-id="57fd6-135">Add the following line in your podfile to include the Objective-C Microsoft Graph SDK and Microsoft Graph Objective-C Auth SDK in your xcode project:</span></span>

```
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a><span data-ttu-id="57fd6-136">Carthage を使用して Microsoft Graph の目標-C SDK をインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-136">Install the Microsoft Graph Objective-C SDK using Carthage</span></span>

<span data-ttu-id="57fd6-137">次の手順を実行して、 [Carthage](https://github.com/Carthage/Carthage)パッケージマネージャーを使用して、microsoft Graph の目的-c SDK と microsoft Graph の目標-c Auth sdk をインストールします。</span><span class="sxs-lookup"><span data-stu-id="57fd6-137">Perform the following steps to install the Microsoft Graph Objective-C SDK and Microsoft Graph Objective-C Auth SDK using the [Carthage](https://github.com/Carthage/Carthage) package manager.</span></span>

1. <span data-ttu-id="57fd6-138">目標-C SDK GitHub リポジトリと[リリースタグ](https://github.com/microsoftgraph/msgraph-sdk-objc/releases)を指定する**Cartfile**を作成します。</span><span class="sxs-lookup"><span data-stu-id="57fd6-138">Create a **Cartfile** that specifies the Objective-C SDK GitHub repository and [release tag](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) to target.</span></span>

```
github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
```

2. <span data-ttu-id="57fd6-139">`carthage update` を実行します。</span><span class="sxs-lookup"><span data-stu-id="57fd6-139">Run `carthage update`.</span></span> <span data-ttu-id="57fd6-140">これにより、依存関係が Carthage/チェックアウトフォルダーにフェッチされ、MSGraphClientSDK ライブラリが作成されます。</span><span class="sxs-lookup"><span data-stu-id="57fd6-140">This will fetch dependencies into a Carthage/Checkouts folder and then builds the MSGraphClientSDK library.</span></span>

3. <span data-ttu-id="57fd6-141">Xcode を使用して、アプリケーションターゲットの **[全般**設定] タブの [リンクされた**フレームワークとライブラリ**] セクションで、 **Msgraphclientsdk. フレームワーク**と**msgraphmsalauthprovider**をドラッグアンドドロップします。ディスク上にフォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="57fd6-141">Using Xcode, in your application target's **General** settings tab, in the **Linked Frameworks and Libraries** section, drag and drop the **MSGraphClientSDK.framework** and **MSGraphMSALAuthProvider.framework** from the Carthage/Build folder on disk.</span></span>

4. <span data-ttu-id="57fd6-142">アプリケーションターゲットの [**ビルドフェーズ**の設定] タブで、 **+** アイコンをクリックして、[**スクリプトフェーズの新規実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="57fd6-142">On your application target's **Build Phases** settings tab, click the **+** icon and choose **New Run Script Phase**.</span></span> <span data-ttu-id="57fd6-143">シェル (ex:/bin/sh) を指定し、次の内容をスクリプトに追加する実行スクリプトを作成します。</span><span class="sxs-lookup"><span data-stu-id="57fd6-143">Create a run script in which you specify your shell (ex: /bin/sh), and add the following contents to the script:</span></span>

```
/usr/local/bin/carthage copy-frameworks
```

5. <span data-ttu-id="57fd6-144">**入力ファイル**で使用するフレームワークへのパスを追加します。</span><span class="sxs-lookup"><span data-stu-id="57fd6-144">Add the paths to the frameworks you want to use under **Input Files**.</span></span>

```
$(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
$(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
```

## <a name="install-the-microsoft-graph-php-sdk"></a><span data-ttu-id="57fd6-145">Microsoft Graph PHP SDK をインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-145">Install the Microsoft Graph PHP SDK</span></span>

<span data-ttu-id="57fd6-146">[Microsoft GRAPH PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php)は[packagist.org](https://packagist.org/packages/microsoft/microsoft-graph)から入手でき、次の方法でインストールできます。</span><span class="sxs-lookup"><span data-stu-id="57fd6-146">The [Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) is available from [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) and can be installed in the following ways:</span></span>

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a><span data-ttu-id="57fd6-147">Composer を使用して Microsoft Graph PHP SDK を手動でインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-147">Install the Microsoft Graph PHP SDK manually using composer</span></span>

```
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a><span data-ttu-id="57fd6-148">Composer を使用して Microsoft Graph PHP SDK をインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-148">Install the Microsoft Graph PHP SDK using composer.json</span></span>

```
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-graph-ruby-sdk"></a><span data-ttu-id="57fd6-149">Microsoft Graph Ruby SDK をインストールする</span><span class="sxs-lookup"><span data-stu-id="57fd6-149">Install the Microsoft Graph Ruby SDK</span></span>

<span data-ttu-id="57fd6-150">[Microsoft Graph RUBY SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby)は[rubygems.org](https://rubygems.org/)から入手でき、次のコマンドを使用してインストールできます。</span><span class="sxs-lookup"><span data-stu-id="57fd6-150">The [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) is available from [rubygems.org](https://rubygems.org/) and can be installed using the following command:</span></span>

```
gem install microsoft_graph
```

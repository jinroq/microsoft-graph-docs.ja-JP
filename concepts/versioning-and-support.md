---
title: 'Microsoft Graph のバージョン管理、サポートと重大な変更の方針 '
description: この記事は Microsoft Graph のサポート重大な変更の方針と、現在使用可能な Microsoft Graph API のバージョンについて説明します。
ms.openlocfilehash: 2a2c7f338e4bc26dc61d9cf88855b9760ff22d6f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092535"
---
# <a name="versioning-support-and-breaking-change-policies-for-microsoft-graph"></a><span data-ttu-id="56f62-103">Microsoft Graph のバージョン管理、サポートと重大な変更の方針</span><span class="sxs-lookup"><span data-stu-id="56f62-103">Versioning, support, and breaking change policies for Microsoft Graph</span></span> 

<span data-ttu-id="56f62-104">この記事は Microsoft Graph のサポート重大な変更の方針と、現在使用可能な Microsoft Graph API のバージョンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="56f62-104">This article describes the support and breaking change policies for Microsoft Graph and the versions of the Microsoft Graph API that are currently available.</span></span>

## <a name="support-policy-and-deprecation-information"></a><span data-ttu-id="56f62-105">サポート ポリシーと廃止の情報</span><span class="sxs-lookup"><span data-stu-id="56f62-105">Support policy and deprecation information</span></span>

<span data-ttu-id="56f62-106">Microsoft Graph は [Microsoft ライフサイクル ポリシー](https://support.microsoft.com/ja-JP/lifecycle)に従います。</span><span class="sxs-lookup"><span data-stu-id="56f62-106">Microsoft Graph follows the [Microsoft Lifecycle Policy](https://support.microsoft.com/ja-JP/lifecycle).</span></span> 

<span data-ttu-id="56f62-p101">Microsoft Graph REST API と Microsoft Graph SDK の新しいバージョンがリリースされると、それ以前のバージョンは廃止されます。Microsoft は API または SDK が廃止される少なくとも 24 か月前までにそれ以前のバージョンを非推奨に指定します。</span><span class="sxs-lookup"><span data-stu-id="56f62-p101">As new versions of the Microsoft Graph REST APIs and Microsoft Graph SDKs are released, earlier versions will be retired. Microsoft will declare a version as deprecated at least 24 months in advance of retiring an API or an SDK.</span></span> 

<span data-ttu-id="56f62-109">API のメジャー バージョンを新しくする場合 (たとえば、v1.0 から v2.0 へ)、現在のバージョン (この例では v1.0) が即時に非推奨になり、この発表から 24 か月後以降、サポートが打ち切られます。</span><span class="sxs-lookup"><span data-stu-id="56f62-109">When we increment the major version of the API (for example, from v1.0 to v2.0), we are announcing that the current version (in this example, v1.0) is immediately deprecated and we will no longer support it 24 months after the announcement.</span></span> <span data-ttu-id="56f62-110">サービスのセキュリティと信頼性向上のためにこのポリシーを変更することがあります。</span><span class="sxs-lookup"><span data-stu-id="56f62-110">We might make exceptions to this policy for service security or health reliability issues.</span></span>  

<span data-ttu-id="56f62-111">API が非推奨と指定された場合、できるだけ早く最新バージョンへ移行することを強くお勧めします。</span><span class="sxs-lookup"><span data-stu-id="56f62-111">When an API is marked as deprecated, we strongly recommend that you migrate to the latest version as soon as possible.</span></span> <span data-ttu-id="56f62-112">場合によっては、元のAPIが非推奨になってからすぐに、新しいアプリケーションで新しい APIの使用を開始する必要があることを、お知らせします。</span><span class="sxs-lookup"><span data-stu-id="56f62-112">In some cases, we will announce that new applications will have to start using the new APIs a short time after the original APIs are deprecated.</span></span> <span data-ttu-id="56f62-113">そのような場合、現在非推奨 APIを使用しているアクティブなアプリケーションのみが使用し続けることができます。</span><span class="sxs-lookup"><span data-stu-id="56f62-113">In those cases, only active applications that currently use the deprecated APIs can continue to use them.</span></span>   

### <a name="api-contract-and-non-backward-compatible-changes"></a><span data-ttu-id="56f62-114">API コントラクトと下位互換性のない変更</span><span class="sxs-lookup"><span data-stu-id="56f62-114">API contract and non-backward compatible changes</span></span>

<span data-ttu-id="56f62-p104">Microsoft Graph にはバージョン更新の変更履歴があります。バージョン更新に伴う変更は [Microsoft Graph Microsoft Graph の変更ログ](changelog.md)に表示されています。Microsoft Graph には新しい機能とデータが追加されたため、下位互換性のない変更が加えられた API では、バージョン番号を更新しています。</span><span class="sxs-lookup"><span data-stu-id="56f62-p104">Microsoft Graph has a log of changes across versions. These changes are listed in the [Microsoft Graph Changelog](changelog.md). As new functionality and data is added to Microsoft Graph, we will increment the API version number for any non-backward compatible changes to the API.</span></span> 

<span data-ttu-id="56f62-118">次に、下位互換性のない変更の例を示します。</span><span class="sxs-lookup"><span data-stu-id="56f62-118">The following are examples of non-backward compatible changes:</span></span>

 - <span data-ttu-id="56f62-119">URL またはリソースに関する基本的な要求や応答の変更</span><span class="sxs-lookup"><span data-stu-id="56f62-119">Changes to the URL or fundamental request/response associated with a resource</span></span>    
 - <span data-ttu-id="56f62-120">宣言済みプロパティの型の削除、変更と、その名前の変更</span><span class="sxs-lookup"><span data-stu-id="56f62-120">Removal, rename, or change to the type of a declared property</span></span>
 - <span data-ttu-id="56f62-121">API と API パラメーターの削除または名前の変更</span><span class="sxs-lookup"><span data-stu-id="56f62-121">Removal or rename of APIs or API parameters</span></span>
 - <span data-ttu-id="56f62-122">必須の要求ヘッダーの追加</span><span class="sxs-lookup"><span data-stu-id="56f62-122">Addition of a required request header</span></span>

<span data-ttu-id="56f62-123">次に、下位互換性のある変更の例を示します。</span><span class="sxs-lookup"><span data-stu-id="56f62-123">The following are examples of backward compatible changes:</span></span>

 - <span data-ttu-id="56f62-124">Null 許容型プロパティや既定値を持つプロパティの追加</span><span class="sxs-lookup"><span data-stu-id="56f62-124">Addition of properties that are nullable or have a default value</span></span>
 - <span data-ttu-id="56f62-125">列挙型へのメンバーの追加</span><span class="sxs-lookup"><span data-stu-id="56f62-125">Addition of a member to an enumeration</span></span>
 - <span data-ttu-id="56f62-126">オープン拡張情報の削除、変更と、その名前の変更</span><span class="sxs-lookup"><span data-stu-id="56f62-126">Removal, rename, or change to the type of an open extension</span></span>
 - <span data-ttu-id="56f62-127">注釈の削除、変更と、その名前の変更</span><span class="sxs-lookup"><span data-stu-id="56f62-127">Removal, rename, or change to the type of an annotation</span></span>
 - <span data-ttu-id="56f62-128">既存のコレクションへのページングの導入</span><span class="sxs-lookup"><span data-stu-id="56f62-128">Introduction of paging to existing collections</span></span>
 - <span data-ttu-id="56f62-129">エラー コードの変更</span><span class="sxs-lookup"><span data-stu-id="56f62-129">Changes to error codes</span></span>
 - <span data-ttu-id="56f62-130">プロパティの順序の変更</span><span class="sxs-lookup"><span data-stu-id="56f62-130">Changes to the order of properties</span></span>
 - <span data-ttu-id="56f62-131">リソース ID のような不透明な文字列の長さまたは形式の変更</span><span class="sxs-lookup"><span data-stu-id="56f62-131">Changes to the length or format of opaque strings, such as resource IDs</span></span>

><span data-ttu-id="56f62-p105">**注:** 下位互換性のある変更の一覧は適時変更されます。独自のクライアント プロクシ (WCF クライアントなど) を作成する場合は、ガイドラインとしては Microsoft Graph API サービスにあらかじめ定義されていないプロパティや派生型をクライアント アプリケーションが受け入れることができるように準備してください。Microsoft Graph API は「[Microsoft REST API ガイドライン](https://github.com/microsoft/api-guidelines/)」の「[バージョン管理のモデル](https://github.com/microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning)」セクションの説明に従っています。</span><span class="sxs-lookup"><span data-stu-id="56f62-p105">**Note:** Over time, we will update the list of backward compatible changes. If you generate your own client proxies (like WCF clients), our guidance is that your client applications should be prepared to receive properties and derived types not previously defined by the Microsoft Graph API service. Microsoft Graph API follows the guidance described in the [Model Versioning](https://github.com/microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning) section in the [Microsoft REST API guidelines](https://github.com/microsoft/api-guidelines/).</span></span> 

## <a name="versions"></a><span data-ttu-id="56f62-135">バージョン</span><span class="sxs-lookup"><span data-stu-id="56f62-135">Versions</span></span>

<span data-ttu-id="56f62-136">現在、以下のバージョンの Microsoft Graph API が使用できます。</span><span class="sxs-lookup"><span data-stu-id="56f62-136">The following versions of the Microsoft Graph API are currently available.</span></span>

### <a name="beta-version"></a><span data-ttu-id="56f62-137">ベータ版</span><span class="sxs-lookup"><span data-stu-id="56f62-137">Beta version</span></span>
<span data-ttu-id="56f62-138">Microsoft Graph API のベータ版は、`https://graph.microsoft.com/beta`で公開されており、現在_**プレビュー段階**_ の機能が含まれています。</span><span class="sxs-lookup"><span data-stu-id="56f62-138">Exposed under `https://graph.microsoft.com/beta`, the Microsoft Graph API beta version contains features that are currently _**in preview**_.</span></span> <span data-ttu-id="56f62-139">ベータ版 API のドキュメントは、「[Microsoft Graph ベータ エンドポイント リファレンス](/graph/api/overview?view=graph-rest-beta)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56f62-139">For beta API documentation, see [Microsoft Graph beta endpoint reference](/graph/api/overview?view=graph-rest-beta).</span></span> <span data-ttu-id="56f62-140">ベータ版には随時重大な変更が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="56f62-140">Expect breaking changes to the beta version from time to time.</span></span> <span data-ttu-id="56f62-141">本番環境が /beta API に依存することのないようにしてください。</span><span class="sxs-lookup"><span data-stu-id="56f62-141">Do not take a production dependency on /beta APIs.</span></span>

<span data-ttu-id="56f62-p107">ベータ版の機能が現行バージョンに採用される保証はありません。Microsoft Graph API チームの判断でベータ版の機能が一般提供 (GA) に十分なものとなったとき、その機能が最新バージョンに追加されます。機能の採用が現行バージョンに重大な変更を招く場合は、バージョン番号が更新され、新規バージョンが現行バージョンに変わります。開発者コミュニティは、新機能や既存のベータ版 API 機能の現行バージョンでの採用希望などの機能の要望を [UserVoice](https://officespdev.uservoice.com/) に投稿できます。</span><span class="sxs-lookup"><span data-stu-id="56f62-p107">We make no guarantees that a beta feature will be promoted to the current version. When the Microsoft Graph API team believes that a beta feature is ready for general availability (GA), we will add that feature to the latest current version. If the promotion of the feature would result in a breaking change to the current version, the version number will be incremented, with the new version becoming the current version. Our developer community can post feature request on [UserVoice](https://officespdev.uservoice.com/), including requests for new features as well as requests to promote existing beta APIs to the current version.</span></span> 

### <a name="current-version"></a><span data-ttu-id="56f62-146">現在のバージョン</span><span class="sxs-lookup"><span data-stu-id="56f62-146">Current version</span></span>

<span data-ttu-id="56f62-p108">Microsoft Graph の現在のバージョンは、v1.0 です。Microsoft Graph API /v1.0 バージョンは `https://graph.microsoft.com/v1.0` で一般提供されており、一般的に利用可能で本番環境での運用準備が整った機能が含まれています。v1.0 API のドキュメントの各部は、目次から参照できます。</span><span class="sxs-lookup"><span data-stu-id="56f62-p108">The current version of Microsoft Graph is v1.0. Exposed under `https://graph.microsoft.com/v1.0`, the Microsoft Graph API /v1.0 version contains features that are generally available and ready for production use. You can browse the documentation for the v1.0 APIs in the table of contents.</span></span>

### <a name="deprecated-and-unsupported-versions"></a><span data-ttu-id="56f62-150">非推奨およびサポートされないバージョン</span><span class="sxs-lookup"><span data-stu-id="56f62-150">Deprecated and unsupported versions</span></span>

<span data-ttu-id="56f62-151">現在、Microsoft Graph には非推奨のバージョンはありません。</span><span class="sxs-lookup"><span data-stu-id="56f62-151">There are currently no deprecated versions of Microsoft Graph.</span></span>

## <a name="terms-of-use"></a><span data-ttu-id="56f62-152">利用規約</span><span class="sxs-lookup"><span data-stu-id="56f62-152">Terms of use</span></span>

<span data-ttu-id="56f62-153">Microsoft Graph API を使用すると、[使用条件](https://developer.microsoft.com/graph/docs/misc/terms-of-use)に同意したことになります。</span><span class="sxs-lookup"><span data-stu-id="56f62-153">By using the Microsoft Graph APIs, you agree to the [Terms of Use](https://developer.microsoft.com/graph/docs/misc/terms-of-use).</span></span> 

<span data-ttu-id="56f62-p109">お客様からのフィードバックは重要です。[StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest) でご連絡いただけます。ご質問には {MicrosoftGraph} のタグを付けてください。</span><span class="sxs-lookup"><span data-stu-id="56f62-p109">Your feedback is important to us. Connect with us on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Tag your questions with {MicrosoftGraph}.</span></span>

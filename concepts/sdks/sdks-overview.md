---
title: Microsoft Graph Sdk の概要
description: 利用可能な Sdk、サポートされているプラットフォーム、および開発者に提供する値について説明します。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: deab2aac6f087f82c8f383f1aa0bed65e09a08fd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630175"
---
# <a name="microsoft-graph-sdks-overview"></a><span data-ttu-id="6c761-103">Microsoft Graph Sdk の概要</span><span class="sxs-lookup"><span data-stu-id="6c761-103">Microsoft Graph SDKs overview</span></span>

<span data-ttu-id="6c761-104">Microsoft Graph Sdk は、Microsoft Graph にアクセスする高品質、効率的、および弾性アプリケーションの構築を簡素化するように設計されています。</span><span class="sxs-lookup"><span data-stu-id="6c761-104">The Microsoft Graph SDKs are designed to simplify building high-quality, efficient, and resilient applications that access Microsoft Graph.</span></span> <span data-ttu-id="6c761-105">Sdk には、サービスライブラリとコアライブラリという2つのコンポーネントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c761-105">The SDKs include two components: a service library and a core library.</span></span>

<span data-ttu-id="6c761-106">サービスライブラリには、microsoft graph メタデータから生成されたモデルと要求ビルダーが含まれており、Microsoft graph で利用可能な多くのデータセットを使用するときに、豊富で、強力に型指定された、検出可能な機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="6c761-106">The service library contains models and request builders that are generated from Microsoft Graph metadata to provide a rich, strongly typed, and discoverable experience when working with the many datasets available in Microsoft Graph.</span></span>

<span data-ttu-id="6c761-107">コアライブラリには、すべての Microsoft Graph サービスの動作を強化する一連の機能が用意されています。</span><span class="sxs-lookup"><span data-stu-id="6c761-107">The core library provide a set of features that enhance working with all the Microsoft Graph services.</span></span> <span data-ttu-id="6c761-108">追加の再試行処理、セキュリティで保護されたリダイレクト、透過的な認証、およびペイロードのサポートによって、アプリケーションの Microsoft Graph との相互作用が向上します。これにより、複雑さが増し、完全に制御することができます。</span><span class="sxs-lookup"><span data-stu-id="6c761-108">Embedded support for retry handling, secure redirects, transparent authentication, and payload compression, improve the quality of your application's interactions with Microsoft Graph, with no added complexity, while leaving you completely in control.</span></span> <span data-ttu-id="6c761-109">コアライブラリは、コレクションのページングやバッチ要求の作成などの一般的なタスクのサポートも提供します。</span><span class="sxs-lookup"><span data-stu-id="6c761-109">The core library also provides support for common tasks such as paging through collections and creating batch requests.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/hDnsd2nJf88]


## <a name="supported-platforms"></a><span data-ttu-id="6c761-110">サポートされるプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="6c761-110">Supported platforms</span></span>

<span data-ttu-id="6c761-111">Sdk は現在、以下の言語とプラットフォームで利用できます。</span><span class="sxs-lookup"><span data-stu-id="6c761-111">SDKs are currently available for the following languages and platforms:</span></span>

- [<span data-ttu-id="6c761-112">Android</span><span class="sxs-lookup"><span data-stu-id="6c761-112">Android</span></span>](https://developer.microsoft.com/en-us/graph/get-started/android)
- [<span data-ttu-id="6c761-113">Angular</span><span class="sxs-lookup"><span data-stu-id="6c761-113">Angular</span></span>](https://developer.microsoft.com/en-us/graph/get-started/angular)
- [<span data-ttu-id="6c761-114">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="6c761-114">ASP.NET</span></span>](https://developer.microsoft.com/en-us/graph/get-started/asp.net)
- [<span data-ttu-id="6c761-115">iOS</span><span class="sxs-lookup"><span data-stu-id="6c761-115">iOS</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ios)
- [<span data-ttu-id="6c761-116">Java</span><span class="sxs-lookup"><span data-stu-id="6c761-116">Javascript</span></span>](https://developer.microsoft.com/en-us/graph/get-started/javascript)
- [<span data-ttu-id="6c761-117">Node.js</span><span class="sxs-lookup"><span data-stu-id="6c761-117">Node.js</span></span>](https://developer.microsoft.com/en-us/graph/get-started/node.js)
- [<span data-ttu-id="6c761-118">Java</span><span class="sxs-lookup"><span data-stu-id="6c761-118">Java</span></span>](https://developer.microsoft.com/en-us/graph/get-started/java)
- [<span data-ttu-id="6c761-119">PHP</span><span class="sxs-lookup"><span data-stu-id="6c761-119">PHP</span></span>](https://developer.microsoft.com/en-us/graph/get-started/php)
- [<span data-ttu-id="6c761-120">Python</span><span class="sxs-lookup"><span data-stu-id="6c761-120">Python</span></span>](https://developer.microsoft.com/en-us/graph/get-started/python)
- [<span data-ttu-id="6c761-121">Ruby</span><span class="sxs-lookup"><span data-stu-id="6c761-121">Ruby</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ruby)

## <a name="office-365-developer-subscription"></a><span data-ttu-id="6c761-122">Office 365 開発者向けサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="6c761-122">Office 365 developer subscription</span></span>

<span data-ttu-id="6c761-123">Microsoft Graph を使用してアプリケーションをビルドする場合は、365 office 365 developer プログラムにサインアップすることにより、無料の office 開発者向けサブスクリプションを取得することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="6c761-123">When building applications using Microsoft Graph, we recommend that you get a free Office 365 developer subscription by signing up for the [Office 365 Developer Program](http://aka.ms/OfficeDevProgram).</span></span>

## <a name="see-also"></a><span data-ttu-id="6c761-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c761-124">See also</span></span>

<span data-ttu-id="6c761-125">Sdk[設計要件ドキュメント](https://github.com/microsoftgraph/msgraph-sdk-design)では、sdk の機能の詳細について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c761-125">The SDK [design requirements documentation](https://github.com/microsoftgraph/msgraph-sdk-design) provides more details about the features and capabilities of the SDK.</span></span> <span data-ttu-id="6c761-126">[Microsoft Graph UserVoice](https://microsoftgraph.uservoice.com)サイトで追加機能の要求または投票を行います。</span><span class="sxs-lookup"><span data-stu-id="6c761-126">Request or vote on additional features at the [Microsoft Graph UserVoice](https://microsoftgraph.uservoice.com) site.</span></span> <span data-ttu-id="6c761-127">Microsoft Graph の Sdk とサンプルの一覧については、「 [Microsoft graph のリソース」ページ](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c761-127">For a list of SDKs and samples for Microsoft Graph, see the [Microsoft Graph resources page](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs).</span></span>

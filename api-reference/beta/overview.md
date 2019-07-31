---
title: Microsoft Graph ベータ版のエンドポイント リファレンス
description: このセクションのリファレンス コンテンツは、Microsoft Graph ベータ版のエンドポイントを文書化しています。 ベータ版のエンドポイントには、現在プレビュー段階で一般提供されていない API が含まれます。 これらの API を試して、次のチャネルからフィードバックをお寄せください。
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: ''
author: ''
ms.openlocfilehash: adfb0abf2feab3d6846d6636136f413d7986f375
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974494"
---
# <a name="microsoft-graph-beta-endpoint-reference"></a><span data-ttu-id="c2c01-105">Microsoft Graph ベータ版のエンドポイント リファレンス</span><span class="sxs-lookup"><span data-stu-id="c2c01-105">Microsoft Graph beta endpoint reference</span></span>

<span data-ttu-id="c2c01-106">このセクションのリファレンス コンテンツは、Microsoft Graph ベータ版のエンドポイントを文書化しています。</span><span class="sxs-lookup"><span data-stu-id="c2c01-106">The reference content in this section documents the Microsoft Graph beta endpoint.</span></span> <span data-ttu-id="c2c01-107">ベータ版のエンドポイントには、現在プレビュー段階で一般提供されていない API が含まれます。</span><span class="sxs-lookup"><span data-stu-id="c2c01-107">The beta endpoint includes APIs that are currently in preview and are not yet generally available.</span></span> <span data-ttu-id="c2c01-108">これらの API を試して、次のチャネルからフィードバックをお寄せください。</span><span class="sxs-lookup"><span data-stu-id="c2c01-108">We invite you to try these APIs and provide your feedback via the following channels:</span></span>

- <span data-ttu-id="c2c01-109">[GitHub](https://github.com/OfficeDev/microsoft-graph-docs/issues) - プレビュー API のフィードバック用です。</span><span class="sxs-lookup"><span data-stu-id="c2c01-109">[GitHub](https://github.com/OfficeDev/microsoft-graph-docs/issues) - For feedback on the Preview APIs.</span></span> <span data-ttu-id="c2c01-110">`beta` でタグ付けしてください。</span><span class="sxs-lookup"><span data-stu-id="c2c01-110">Tag with `beta`.</span></span>
- <span data-ttu-id="c2c01-111">[StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph) - お客様のコードに関する質問やご相談用です。</span><span class="sxs-lookup"><span data-stu-id="c2c01-111">[StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph) - For questions or help with your code.</span></span> <span data-ttu-id="c2c01-112">`microsoftgraph` でタグ付けしてください。</span><span class="sxs-lookup"><span data-stu-id="c2c01-112">Tag with `microsoftgraph`.</span></span>

> <span data-ttu-id="c2c01-113">**注:** ベータ版のエンドポイントの API は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c2c01-113">**Note:** The APIs in the beta endpoint are subject to change.</span></span> <span data-ttu-id="c2c01-114">運用アプリ内で使用することはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="c2c01-114">We don't recommend that you use them in your production apps.</span></span> 

## <a name="call-the-beta-endpoint"></a><span data-ttu-id="c2c01-115">ベータ版エンドポイントの呼び出し</span><span class="sxs-lookup"><span data-stu-id="c2c01-115">Call the beta endpoint</span></span>

<span data-ttu-id="c2c01-116">Microsoft Graph API では、ベータ版エンドポイントは次のパターンを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c2c01-116">Microsoft Graph API requests to the beta endpoint use the following pattern:</span></span>

```
    https://graph.microsoft.com/beta/{resource}?[query_parameters]
```

<span data-ttu-id="c2c01-117">詳細については、「[Microsoft Graph API を使用する](/graph/use-the-api)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2c01-117">For details, see [Use the Microsoft Graph API](/graph/use-the-api).</span></span>

## <a name="see-also"></a><span data-ttu-id="c2c01-118">関連項目</span><span class="sxs-lookup"><span data-stu-id="c2c01-118">See also</span></span>

- [<span data-ttu-id="c2c01-119">Microsoft Graph の概要</span><span class="sxs-lookup"><span data-stu-id="c2c01-119">Overview of Microsoft Graph</span></span>](/graph/overview)
- [<span data-ttu-id="c2c01-120">Microsoft Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="c2c01-120">Microsoft Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer)
- [<span data-ttu-id="c2c01-121">Microsoft Graph のクイック スタート</span><span class="sxs-lookup"><span data-stu-id="c2c01-121">Microsoft Graph quick start</span></span>](https://developer.microsoft.com/graph/quick-start)


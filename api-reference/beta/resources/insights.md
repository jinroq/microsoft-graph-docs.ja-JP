---
title: 情報リソースの種類
description: 情報は、関係の高度な解析と機械学習技術を使用して計算です。 OneDrive ドキュメントがユーザーの周りのトレンド分析を識別するなど。
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 38f7afb40c1618a8a7cf9d585c99633e2bb8d940
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938315"
---
# <a name="insights-resource-type"></a><span data-ttu-id="28dc1-104">情報リソースの種類</span><span class="sxs-lookup"><span data-stu-id="28dc1-104">insights resource type</span></span>

> <span data-ttu-id="28dc1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="28dc1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28dc1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28dc1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="28dc1-107">情報は、関係の高度な解析と機械学習技術を使用して計算です。</span><span class="sxs-lookup"><span data-stu-id="28dc1-107">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="28dc1-108">OneDrive ドキュメントがユーザーの周りのトレンド分析を識別するなど。</span><span class="sxs-lookup"><span data-stu-id="28dc1-108">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="28dc1-109">次の Api では、情報が返されます。</span><span class="sxs-lookup"><span data-stu-id="28dc1-109">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="28dc1-110">[Trending](insights-trending.md)のでは、OneDrive と SharePoint サイトのユーザーの周りのトレンド分析から、ドキュメントが返されます。</span><span class="sxs-lookup"><span data-stu-id="28dc1-110">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="28dc1-111">[使用されている](insights-used.md)のでは、ドキュメントの表示し、ユーザーが変更を返します。</span><span class="sxs-lookup"><span data-stu-id="28dc1-111">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="28dc1-112">ビジネス、SharePoint、電子メールの添付ファイル、およびボックス、ドロップ ボックスや Google のドライブのようなソースからのリンクの添付ファイルとして開かれたの OneDrive で、ユーザーが使用するドキュメントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="28dc1-112">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="28dc1-113">[共有](insights-shared.md)では、ユーザーと共有するドキュメントを返します。</span><span class="sxs-lookup"><span data-stu-id="28dc1-113">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="28dc1-114">ドキュメント共有できる電子メールの添付ファイル、または OneDrive としてビジネスに送信した電子メールのリンクをします。</span><span class="sxs-lookup"><span data-stu-id="28dc1-114">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="28dc1-115">各情報が返されます、`resourceVisualization`と`resourceReference`複雑な値の種類 (CVT) です。</span><span class="sxs-lookup"><span data-stu-id="28dc1-115">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="28dc1-116">含まれているプロパティを次のように CVT の resourceVisualization`title`と`previewImageUrl`。</span><span class="sxs-lookup"><span data-stu-id="28dc1-116">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="28dc1-117">マイクロソフトは、Office の説明のような経験でファイルを表示するのに視覚エフェクトのプロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="28dc1-117">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="28dc1-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="28dc1-118">Relationships</span></span>

| <span data-ttu-id="28dc1-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="28dc1-119">Relationship</span></span>      | <span data-ttu-id="28dc1-120">型</span><span class="sxs-lookup"><span data-stu-id="28dc1-120">Type</span></span>          | <span data-ttu-id="28dc1-121">説明</span><span class="sxs-lookup"><span data-stu-id="28dc1-121">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="28dc1-122">トレンド分析</span><span class="sxs-lookup"><span data-stu-id="28dc1-122">trending</span></span>      | <span data-ttu-id="28dc1-123">[Trending](insights-trending.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="28dc1-123">[Trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="28dc1-124">トレンド分析ドキュメントを識別する計算の関係です。</span><span class="sxs-lookup"><span data-stu-id="28dc1-124">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="28dc1-125">OneDrive または SharePoint サイトでは、トレンドのドキュメントを格納できます。</span><span class="sxs-lookup"><span data-stu-id="28dc1-125">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="28dc1-126">used</span><span class="sxs-lookup"><span data-stu-id="28dc1-126">used</span></span>      | <span data-ttu-id="28dc1-127">コレクションの[使用](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="28dc1-127">[Used](insights-used.md) collection</span></span>       | <span data-ttu-id="28dc1-128">ドキュメントを表示し、ユーザーによって変更を識別するリレーションシップが計算されます。</span><span class="sxs-lookup"><span data-stu-id="28dc1-128">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="28dc1-129">ビジネス、SharePoint、電子メールの添付ファイル、およびボックス、ドロップ ボックスや Google のドライブのようなソースからのリンクの添付ファイルとして開かれたの OneDrive で、ユーザーが使用するドキュメントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="28dc1-129">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="28dc1-130">shared</span><span class="sxs-lookup"><span data-stu-id="28dc1-130">shared</span></span>        | <span data-ttu-id="28dc1-131">[共有](insights-shared.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="28dc1-131">[Shared](insights-shared.md) collection</span></span>       | <span data-ttu-id="28dc1-132">ユーザーと共有するドキュメントを識別する計算の関係です。</span><span class="sxs-lookup"><span data-stu-id="28dc1-132">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="28dc1-133">ドキュメント共有できる電子メールの添付ファイル、または OneDrive としてビジネスに送信した電子メールのリンクをします。</span><span class="sxs-lookup"><span data-stu-id="28dc1-133">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="28dc1-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28dc1-134">JSON representation</span></span>

<span data-ttu-id="28dc1-135">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="28dc1-135">Here is a JSON representation of the resource</span></span>
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```

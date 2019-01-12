---
title: mentionsPreview リソースの種類
description: リソースのインスタンスで記載されているオブジェクトに関する情報を表します。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 3bb087f6eb1d3c49b85213acf60393346a42b7cf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949291"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="0a016-103">mentionsPreview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a016-103">mentionsPreview resource type</span></span>

> <span data-ttu-id="0a016-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0a016-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a016-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a016-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a016-106">リソース インスタンス内のオブジェクトの[説明](../resources/mention.md)に関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="0a016-106">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="0a016-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a016-107">Properties</span></span>
| <span data-ttu-id="0a016-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a016-108">Property</span></span>     | <span data-ttu-id="0a016-109">種類</span><span class="sxs-lookup"><span data-stu-id="0a016-109">Type</span></span>   |<span data-ttu-id="0a016-110">説明</span><span class="sxs-lookup"><span data-stu-id="0a016-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0a016-111">isMentioned</span><span class="sxs-lookup"><span data-stu-id="0a016-111">isMentioned</span></span> | <span data-ttu-id="0a016-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a016-112">Boolean</span></span> | <span data-ttu-id="0a016-p102">ログインしているユーザーが親リソース インスタンスでメンションされている場合は true です。読み取り専用。フィルターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0a016-p102">True if the signed-in user is mentioned in the parent resource instance. Read-only. Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0a016-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a016-116">JSON representation</span></span>

<span data-ttu-id="0a016-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a016-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

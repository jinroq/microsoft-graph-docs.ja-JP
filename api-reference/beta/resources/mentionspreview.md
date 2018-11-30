---
title: mentionsPreview リソースの種類
description: リソースのインスタンスで記載されているオブジェクトに関する情報を表します。
ms.openlocfilehash: cf6bed3cdfb2d3f541438da0c06fcf8f4873c17e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073098"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="22085-103">mentionsPreview リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22085-103">mentionsPreview resource type</span></span>

> <span data-ttu-id="22085-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="22085-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22085-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22085-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22085-106">リソース インスタンス内のオブジェクトの[説明](../resources/mention.md)に関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="22085-106">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="22085-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22085-107">Properties</span></span>
| <span data-ttu-id="22085-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22085-108">Property</span></span>     | <span data-ttu-id="22085-109">型</span><span class="sxs-lookup"><span data-stu-id="22085-109">Type</span></span>   |<span data-ttu-id="22085-110">説明</span><span class="sxs-lookup"><span data-stu-id="22085-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="22085-111">isMentioned</span><span class="sxs-lookup"><span data-stu-id="22085-111">isMentioned</span></span> | <span data-ttu-id="22085-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="22085-112">Boolean</span></span> | <span data-ttu-id="22085-p102">ログインしているユーザーが親リソース インスタンスでメンションされている場合は true です。読み取り専用。フィルターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="22085-p102">True if the signed-in user is mentioned in the parent resource instance. Read-only. Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="22085-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22085-116">JSON representation</span></span>

<span data-ttu-id="22085-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="22085-117">Here is a JSON representation of the resource.</span></span>

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

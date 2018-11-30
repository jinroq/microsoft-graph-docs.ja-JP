---
title: 通知リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 96246491c386971fe18184f26269d4abe3af6e6e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074166"
---
# <a name="notifications-resource-type"></a><span data-ttu-id="b9a9a-103">通知リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9a9a-103">notifications resource type</span></span>

> <span data-ttu-id="b9a9a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b9a9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9a9a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9a9a-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="b9a9a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9a9a-106">Properties</span></span>

| <span data-ttu-id="b9a9a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9a9a-107">Property</span></span>       | <span data-ttu-id="b9a9a-108">型</span><span class="sxs-lookup"><span data-stu-id="b9a9a-108">Type</span></span>                                       | <span data-ttu-id="b9a9a-109">説明</span><span class="sxs-lookup"><span data-stu-id="b9a9a-109">Description</span></span> |
|:---------------|:-------------------------------------------|:------------|
| <span data-ttu-id="b9a9a-110">value</span><span class="sxs-lookup"><span data-stu-id="b9a9a-110">value</span></span>          | <span data-ttu-id="b9a9a-111">[通知](commsnotification.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="b9a9a-111">[notification](commsnotification.md) collection</span></span> | <span data-ttu-id="b9a9a-112">リソースに変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="b9a9a-112">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b9a9a-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9a9a-113">JSON representation</span></span>

<span data-ttu-id="b9a9a-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b9a9a-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
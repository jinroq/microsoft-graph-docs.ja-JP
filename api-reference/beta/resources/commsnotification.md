---
title: 通知リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: c09927cbe133c945b83a3bfc1b0eb74ef00bce2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072931"
---
# <a name="notification-resource-type"></a><span data-ttu-id="aa4b4-103">通知リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa4b4-103">notification resource type</span></span>

> <span data-ttu-id="aa4b4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aa4b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa4b4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa4b4-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="aa4b4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa4b4-106">Properties</span></span>
| <span data-ttu-id="aa4b4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa4b4-107">Property</span></span>       | <span data-ttu-id="aa4b4-108">型</span><span class="sxs-lookup"><span data-stu-id="aa4b4-108">Type</span></span>    | <span data-ttu-id="aa4b4-109">説明</span><span class="sxs-lookup"><span data-stu-id="aa4b4-109">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="aa4b4-110">changeType</span><span class="sxs-lookup"><span data-stu-id="aa4b4-110">changeType</span></span>     | <span data-ttu-id="aa4b4-111">String</span><span class="sxs-lookup"><span data-stu-id="aa4b4-111">String</span></span>  | <span data-ttu-id="aa4b4-112">可能な値は、`created`、`updated`、`deleted` です。</span><span class="sxs-lookup"><span data-stu-id="aa4b4-112">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="aa4b4-113">resource</span><span class="sxs-lookup"><span data-stu-id="aa4b4-113">resource</span></span>       | <span data-ttu-id="aa4b4-114">String</span><span class="sxs-lookup"><span data-stu-id="aa4b4-114">String</span></span>  | <span data-ttu-id="aa4b4-115">変更されたリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="aa4b4-115">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="aa4b4-116">**注:**`resourceData`は、追加のデータとして使用します。</span><span class="sxs-lookup"><span data-stu-id="aa4b4-116">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="aa4b4-117">エンティティまたは通知のパッケージ化された変更の数によって Collection(entity) をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="aa4b4-117">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa4b4-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa4b4-118">JSON representation</span></span>

<span data-ttu-id="aa4b4-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aa4b4-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "resourceData"
  ],
  "@odata.type": "microsoft.graph.commsNotification",
  "openType": true
}-->
```json
{
  "changeType": "created | updated | deleted",
  "resource": "String"
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E",
        "state": "incoming"
      }
    }
  ]
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: commsNotification リソースの種類
description: 通信通知の変更を通知するためにサーバーによって提供される基本タイプです。
author: VinodRavichandran
ms.openlocfilehash: 65cb2884b98d25008779fcb80968a7b4d0481033
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380269"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="8cb25-103">commsNotification リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8cb25-103">commsNotification resource type</span></span>

> <span data-ttu-id="8cb25-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8cb25-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cb25-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cb25-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cb25-106">通信通知の変更を通知するためにサーバーによって提供される基本タイプです。</span><span class="sxs-lookup"><span data-stu-id="8cb25-106">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="8cb25-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cb25-107">Properties</span></span>
| <span data-ttu-id="8cb25-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cb25-108">Property</span></span>       | <span data-ttu-id="8cb25-109">型</span><span class="sxs-lookup"><span data-stu-id="8cb25-109">Type</span></span>    | <span data-ttu-id="8cb25-110">説明</span><span class="sxs-lookup"><span data-stu-id="8cb25-110">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="8cb25-111">changeType</span><span class="sxs-lookup"><span data-stu-id="8cb25-111">changeType</span></span>     | <span data-ttu-id="8cb25-112">String</span><span class="sxs-lookup"><span data-stu-id="8cb25-112">String</span></span>  | <span data-ttu-id="8cb25-113">可能な値は、`created`、`updated`、`deleted` です。</span><span class="sxs-lookup"><span data-stu-id="8cb25-113">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="8cb25-114">resource</span><span class="sxs-lookup"><span data-stu-id="8cb25-114">resource</span></span>       | <span data-ttu-id="8cb25-115">String</span><span class="sxs-lookup"><span data-stu-id="8cb25-115">String</span></span>  | <span data-ttu-id="8cb25-116">変更されたリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="8cb25-116">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="8cb25-117">**注:**`resourceData`は、追加のデータとして使用します。</span><span class="sxs-lookup"><span data-stu-id="8cb25-117">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="8cb25-118">エンティティまたは通知のパッケージ化された変更の数によって Collection(entity) をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="8cb25-118">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cb25-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cb25-119">JSON representation</span></span>

<span data-ttu-id="8cb25-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8cb25-120">The following is a JSON representation of the resource.</span></span>

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
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
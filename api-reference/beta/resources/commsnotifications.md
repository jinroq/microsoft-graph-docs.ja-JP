---
title: commsNotifications リソースの種類
description: 複数の通知を1つのバッチで送信するために通信サーバーによって使用される通知の一覧。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 770122387b89e96fdd8dbd9077488a9956fd90f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973252"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="46d0b-103">commsNotifications リソースの種類</span><span class="sxs-lookup"><span data-stu-id="46d0b-103">commsNotifications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46d0b-104">複数の通知を1つのバッチで送信するために通信サーバーによって使用される通知の一覧。</span><span class="sxs-lookup"><span data-stu-id="46d0b-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="46d0b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46d0b-105">Properties</span></span>

| <span data-ttu-id="46d0b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46d0b-106">Property</span></span>       | <span data-ttu-id="46d0b-107">型</span><span class="sxs-lookup"><span data-stu-id="46d0b-107">Type</span></span>                                                 | <span data-ttu-id="46d0b-108">説明</span><span class="sxs-lookup"><span data-stu-id="46d0b-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="46d0b-109">value</span><span class="sxs-lookup"><span data-stu-id="46d0b-109">value</span></span>          | <span data-ttu-id="46d0b-110">[Commsnotification](commsnotification.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="46d0b-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="46d0b-111">リソースの変更の通知。</span><span class="sxs-lookup"><span data-stu-id="46d0b-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="46d0b-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46d0b-112">JSON representation</span></span>

<span data-ttu-id="46d0b-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="46d0b-113">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

---
title: commsNotifications リソースの種類
description: 通信サーバーによって 1 つのバッチで複数の通知を送信するための通知の一覧です。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2d002b74bffe0911e2ba1fef4eed324b52ebcc49
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520593"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="edcf5-103">commsNotifications リソースの種類</span><span class="sxs-lookup"><span data-stu-id="edcf5-103">commsNotifications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edcf5-104">通信サーバーによって 1 つのバッチで複数の通知を送信するための通知の一覧です。</span><span class="sxs-lookup"><span data-stu-id="edcf5-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="edcf5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="edcf5-105">Properties</span></span>

| <span data-ttu-id="edcf5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="edcf5-106">Property</span></span>       | <span data-ttu-id="edcf5-107">型</span><span class="sxs-lookup"><span data-stu-id="edcf5-107">Type</span></span>                                                 | <span data-ttu-id="edcf5-108">説明</span><span class="sxs-lookup"><span data-stu-id="edcf5-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="edcf5-109">value</span><span class="sxs-lookup"><span data-stu-id="edcf5-109">value</span></span>          | <span data-ttu-id="edcf5-110">[commsNotification](commsnotification.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="edcf5-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="edcf5-111">リソースに変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="edcf5-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="edcf5-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="edcf5-112">JSON representation</span></span>

<span data-ttu-id="edcf5-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="edcf5-113">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/commsnotifications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

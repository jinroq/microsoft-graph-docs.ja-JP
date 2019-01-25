---
title: synchronizationJobRestartCriteria リソースの種類
description: 'スコープを定義します[synchronizationJob: 再起動](../api/synchronization_synchronizationjob_restart.md)アクション。'
localization_priority: Normal
ms.openlocfilehash: 1e6ac952808f80d191fc93e9a804411ec4459d4c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512641"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="b060b-103">synchronizationJobRestartCriteria リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b060b-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b060b-104">スコープを定義します[synchronizationJob: 再起動](../api/synchronization_synchronizationjob_restart.md)アクション。</span><span class="sxs-lookup"><span data-stu-id="b060b-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization_synchronizationjob_restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="b060b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b060b-105">Properties</span></span>
| <span data-ttu-id="b060b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b060b-106">Property</span></span>     | <span data-ttu-id="b060b-107">型</span><span class="sxs-lookup"><span data-stu-id="b060b-107">Type</span></span>   |<span data-ttu-id="b060b-108">説明</span><span class="sxs-lookup"><span data-stu-id="b060b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b060b-109">resetScope</span><span class="sxs-lookup"><span data-stu-id="b060b-109">resetScope</span></span>|<span data-ttu-id="b060b-110">String</span><span class="sxs-lookup"><span data-stu-id="b060b-110">String</span></span>| <span data-ttu-id="b060b-111">次の値のコンマ区切りの組み合わせ: `Full`、 `QuarantineState`、 `Watermark`、 `Escrows`、 `ConnectorDataStore`。</span><span class="sxs-lookup"><span data-stu-id="b060b-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="b060b-112">使用`Full`のすべてのオプションにする場合。</span><span class="sxs-lookup"><span data-stu-id="b060b-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b060b-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b060b-113">JSON representation</span></span>

<span data-ttu-id="b060b-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b060b-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjobrestartcriteria.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: synchronizationJobRestartCriteria リソースの種類
description: 同期ジョブの範囲を定義し[ます。再起動](../api/synchronization_synchronizationjob_restart.md)アクション。
localization_priority: Normal
ms.openlocfilehash: 1e6ac952808f80d191fc93e9a804411ec4459d4c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453617"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="899a0-103">synchronizationJobRestartCriteria リソースの種類</span><span class="sxs-lookup"><span data-stu-id="899a0-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="899a0-104">同期ジョブの範囲を定義し[ます。再起動](../api/synchronization_synchronizationjob_restart.md)アクション。</span><span class="sxs-lookup"><span data-stu-id="899a0-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization_synchronizationjob_restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="899a0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="899a0-105">Properties</span></span>
| <span data-ttu-id="899a0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="899a0-106">Property</span></span>     | <span data-ttu-id="899a0-107">型</span><span class="sxs-lookup"><span data-stu-id="899a0-107">Type</span></span>   |<span data-ttu-id="899a0-108">説明</span><span class="sxs-lookup"><span data-stu-id="899a0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="899a0-109">resetscope</span><span class="sxs-lookup"><span data-stu-id="899a0-109">resetScope</span></span>|<span data-ttu-id="899a0-110">String</span><span class="sxs-lookup"><span data-stu-id="899a0-110">String</span></span>| <span data-ttu-id="899a0-111">`Full`、 `Watermark` `Escrows`、、、、 `ConnectorDataStore`の各値のコンマ区切りの組み合わせ。 `QuarantineState`</span><span class="sxs-lookup"><span data-stu-id="899a0-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="899a0-112">すべて`Full`のオプションを使用する場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="899a0-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="899a0-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="899a0-113">JSON representation</span></span>

<span data-ttu-id="899a0-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="899a0-114">The following is a JSON representation of the resource.</span></span>

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

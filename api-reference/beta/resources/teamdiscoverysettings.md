---
title: teamDiscoverySettings リソースの種類
description: 他のユーザーがチームの探索可能性を構成するための設定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6dd1c3728d91be88689f72e020b773f7875807a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964572"
---
# <a name="teamdiscoverysettings-resource-type"></a><span data-ttu-id="f62c9-103">teamDiscoverySettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f62c9-103">teamDiscoverySettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f62c9-104">他のユーザーが[チーム](team.md)の検出を構成できるようにするための設定を提供します。</span><span class="sxs-lookup"><span data-stu-id="f62c9-104">Provides settings to enable others to configure [team](team.md) discoverability.</span></span> <span data-ttu-id="f62c9-105">プライベートチームの探索設定のみを変更できます。</span><span class="sxs-lookup"><span data-stu-id="f62c9-105">You can only modify discovery settings for private teams.</span></span>

## <a name="properties"></a><span data-ttu-id="f62c9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f62c9-106">Properties</span></span>
| <span data-ttu-id="f62c9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f62c9-107">Property</span></span>     | <span data-ttu-id="f62c9-108">型</span><span class="sxs-lookup"><span data-stu-id="f62c9-108">Type</span></span>   |<span data-ttu-id="f62c9-109">説明</span><span class="sxs-lookup"><span data-stu-id="f62c9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f62c9-110">showInTeamsSearchAndSuggestions</span><span class="sxs-lookup"><span data-stu-id="f62c9-110">showInTeamsSearchAndSuggestions</span></span>|<span data-ttu-id="f62c9-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="f62c9-111">Boolean</span></span>|<span data-ttu-id="f62c9-112">True に設定されている場合、チームは、Teams クライアントからの検索と提案によって参照できます。</span><span class="sxs-lookup"><span data-stu-id="f62c9-112">If set to true, the team is visible via search and suggestions from the Teams client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f62c9-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f62c9-113">JSON representation</span></span>

<span data-ttu-id="f62c9-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f62c9-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamDiscoverySettings"
}-->

```json
{
  "showInTeamsSearchAndSuggestions": true
}
```

<!-- uuid: f1d42106-0b3d-4930-9f19-d76f4e03b36b
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's discoverySettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamdiscoverysettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->

---
title: teamsAppDefinition リソースの種類
description: TeamsApp の 1 つのバージョンの詳細。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 94e2c790f8bf4623e56ca76bde164b718ee6fa38
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509981"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="e9e7d-103">teamsAppDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9e7d-103">teamsAppDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9e7d-104">の[teamsApp](teamsapp.md)の 1 つのバージョンの詳細。</span><span class="sxs-lookup"><span data-stu-id="e9e7d-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e9e7d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9e7d-105">Properties</span></span>

| <span data-ttu-id="e9e7d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9e7d-106">Property</span></span>            | <span data-ttu-id="e9e7d-107">型</span><span class="sxs-lookup"><span data-stu-id="e9e7d-107">Type</span></span>     | <span data-ttu-id="e9e7d-108">説明</span><span class="sxs-lookup"><span data-stu-id="e9e7d-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="e9e7d-109">id</span><span class="sxs-lookup"><span data-stu-id="e9e7d-109">id</span></span>                  | <span data-ttu-id="e9e7d-110">文字列</span><span class="sxs-lookup"><span data-stu-id="e9e7d-110">string</span></span>   | <span data-ttu-id="e9e7d-111">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="e9e7d-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="e9e7d-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="e9e7d-112">teamsAppId</span></span>          | <span data-ttu-id="e9e7d-113">string</span><span class="sxs-lookup"><span data-stu-id="e9e7d-113">string</span></span>   | <span data-ttu-id="e9e7d-114">チームのアプリケーション マニフェストの id です。</span><span class="sxs-lookup"><span data-stu-id="e9e7d-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="e9e7d-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e9e7d-115">displayName</span></span>         | <span data-ttu-id="e9e7d-116">string</span><span class="sxs-lookup"><span data-stu-id="e9e7d-116">string</span></span>   | <span data-ttu-id="e9e7d-117">アプリケーション開発者によって提供されるアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="e9e7d-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="e9e7d-118">version</span><span class="sxs-lookup"><span data-stu-id="e9e7d-118">version</span></span>             | <span data-ttu-id="e9e7d-119">string</span><span class="sxs-lookup"><span data-stu-id="e9e7d-119">string</span></span>   | <span data-ttu-id="e9e7d-120">アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="e9e7d-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e9e7d-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9e7d-121">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a><span data-ttu-id="e9e7d-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9e7d-122">See also</span></span>

- [<span data-ttu-id="e9e7d-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e9e7d-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="e9e7d-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e9e7d-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="e9e7d-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e9e7d-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappdefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->


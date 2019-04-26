---
title: teamsAppDefinition リソースの種類
description: 1つのバージョンの teamsapp の詳細。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 94e2c790f8bf4623e56ca76bde164b718ee6fa38
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554026"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="325a8-103">teamsAppDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="325a8-103">teamsAppDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="325a8-104">1つのバージョンの[teamsapp](teamsapp.md)の詳細。</span><span class="sxs-lookup"><span data-stu-id="325a8-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="325a8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="325a8-105">Properties</span></span>

| <span data-ttu-id="325a8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="325a8-106">Property</span></span>            | <span data-ttu-id="325a8-107">型</span><span class="sxs-lookup"><span data-stu-id="325a8-107">Type</span></span>     | <span data-ttu-id="325a8-108">説明</span><span class="sxs-lookup"><span data-stu-id="325a8-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="325a8-109">id</span><span class="sxs-lookup"><span data-stu-id="325a8-109">id</span></span>                  | <span data-ttu-id="325a8-110">string</span><span class="sxs-lookup"><span data-stu-id="325a8-110">string</span></span>   | <span data-ttu-id="325a8-111">一意の id (teams appid ではない)。</span><span class="sxs-lookup"><span data-stu-id="325a8-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="325a8-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="325a8-112">teamsAppId</span></span>          | <span data-ttu-id="325a8-113">string</span><span class="sxs-lookup"><span data-stu-id="325a8-113">string</span></span>   | <span data-ttu-id="325a8-114">Teams アプリマニフェストからの id。</span><span class="sxs-lookup"><span data-stu-id="325a8-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="325a8-115">displayName</span><span class="sxs-lookup"><span data-stu-id="325a8-115">displayName</span></span>         | <span data-ttu-id="325a8-116">string</span><span class="sxs-lookup"><span data-stu-id="325a8-116">string</span></span>   | <span data-ttu-id="325a8-117">アプリ開発者によって提供されるアプリの名前。</span><span class="sxs-lookup"><span data-stu-id="325a8-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="325a8-118">バージョン</span><span class="sxs-lookup"><span data-stu-id="325a8-118">version</span></span>             | <span data-ttu-id="325a8-119">string</span><span class="sxs-lookup"><span data-stu-id="325a8-119">string</span></span>   | <span data-ttu-id="325a8-120">アプリケーションのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="325a8-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="325a8-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="325a8-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="325a8-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="325a8-122">See also</span></span>

- [<span data-ttu-id="325a8-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="325a8-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="325a8-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="325a8-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="325a8-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="325a8-125">teamsTab</span></span>](../resources/teamstab.md)

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


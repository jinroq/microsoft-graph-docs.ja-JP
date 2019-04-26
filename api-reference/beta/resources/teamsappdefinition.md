---
title: teamsAppDefinition リソースの種類
description: 1つのバージョンの teamsapp の詳細。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4b350c5ebe39da336dfe467bb73f5b91270dc31c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345803"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="670bc-103">teamsAppDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="670bc-103">teamsAppDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="670bc-104">1つのバージョンの[teamsapp](teamsapp.md)の詳細。</span><span class="sxs-lookup"><span data-stu-id="670bc-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="670bc-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="670bc-105">Properties</span></span>

| <span data-ttu-id="670bc-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="670bc-106">Property</span></span>            | <span data-ttu-id="670bc-107">型</span><span class="sxs-lookup"><span data-stu-id="670bc-107">Type</span></span>     | <span data-ttu-id="670bc-108">説明</span><span class="sxs-lookup"><span data-stu-id="670bc-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="670bc-109">id</span><span class="sxs-lookup"><span data-stu-id="670bc-109">id</span></span>                  | <span data-ttu-id="670bc-110">string</span><span class="sxs-lookup"><span data-stu-id="670bc-110">string</span></span>   | <span data-ttu-id="670bc-111">一意の id (teams appid ではない)。</span><span class="sxs-lookup"><span data-stu-id="670bc-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="670bc-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="670bc-112">teamsAppId</span></span>          | <span data-ttu-id="670bc-113">string</span><span class="sxs-lookup"><span data-stu-id="670bc-113">string</span></span>   | <span data-ttu-id="670bc-114">Teams アプリマニフェストからの id。</span><span class="sxs-lookup"><span data-stu-id="670bc-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="670bc-115">displayName</span><span class="sxs-lookup"><span data-stu-id="670bc-115">displayName</span></span>         | <span data-ttu-id="670bc-116">string</span><span class="sxs-lookup"><span data-stu-id="670bc-116">string</span></span>   | <span data-ttu-id="670bc-117">アプリ開発者によって提供されるアプリの名前。</span><span class="sxs-lookup"><span data-stu-id="670bc-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="670bc-118">バージョン</span><span class="sxs-lookup"><span data-stu-id="670bc-118">version</span></span>             | <span data-ttu-id="670bc-119">string</span><span class="sxs-lookup"><span data-stu-id="670bc-119">string</span></span>   | <span data-ttu-id="670bc-120">アプリケーションのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="670bc-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="670bc-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="670bc-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="670bc-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="670bc-122">See also</span></span>

- [<span data-ttu-id="670bc-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="670bc-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="670bc-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="670bc-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="670bc-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="670bc-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


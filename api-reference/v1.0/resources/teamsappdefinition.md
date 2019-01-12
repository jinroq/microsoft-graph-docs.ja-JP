---
title: teamsAppDefinition リソースの種類
description: TeamsApp の 1 つのバージョンの詳細。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3aed533ecca3bff48071b04adadcea6b52169f89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951930"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="9aca0-103">teamsAppDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9aca0-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="9aca0-104">の[teamsApp](teamsapp.md)の 1 つのバージョンの詳細。</span><span class="sxs-lookup"><span data-stu-id="9aca0-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9aca0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9aca0-105">Properties</span></span>

| <span data-ttu-id="9aca0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9aca0-106">Property</span></span>            | <span data-ttu-id="9aca0-107">種類</span><span class="sxs-lookup"><span data-stu-id="9aca0-107">Type</span></span>     | <span data-ttu-id="9aca0-108">説明</span><span class="sxs-lookup"><span data-stu-id="9aca0-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="9aca0-109">ID</span><span class="sxs-lookup"><span data-stu-id="9aca0-109">id</span></span>                  | <span data-ttu-id="9aca0-110">文字列</span><span class="sxs-lookup"><span data-stu-id="9aca0-110">string</span></span>   | <span data-ttu-id="9aca0-111">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="9aca0-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="9aca0-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="9aca0-112">teamsAppId</span></span>          | <span data-ttu-id="9aca0-113">文字列</span><span class="sxs-lookup"><span data-stu-id="9aca0-113">string</span></span>   | <span data-ttu-id="9aca0-114">チームのアプリケーション マニフェストの id です。</span><span class="sxs-lookup"><span data-stu-id="9aca0-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="9aca0-115">displayName</span><span class="sxs-lookup"><span data-stu-id="9aca0-115">displayName</span></span>         | <span data-ttu-id="9aca0-116">string</span><span class="sxs-lookup"><span data-stu-id="9aca0-116">string</span></span>   | <span data-ttu-id="9aca0-117">アプリケーション開発者によって提供されるアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="9aca0-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="9aca0-118">version</span><span class="sxs-lookup"><span data-stu-id="9aca0-118">version</span></span>             | <span data-ttu-id="9aca0-119">文字列</span><span class="sxs-lookup"><span data-stu-id="9aca0-119">string</span></span>   | <span data-ttu-id="9aca0-120">アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="9aca0-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9aca0-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9aca0-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="9aca0-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="9aca0-122">See also</span></span>

- [<span data-ttu-id="9aca0-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="9aca0-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="9aca0-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="9aca0-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="9aca0-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9aca0-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


---
title: teamsAppDefinition リソースの種類
description: TeamsApp の 1 つのバージョンの詳細。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8fafb266b2bfc2c7ea6e0951ac2906f133817246
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860978"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="cb3af-103">teamsAppDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb3af-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="cb3af-104">の[teamsApp](teamsapp.md)の 1 つのバージョンの詳細。</span><span class="sxs-lookup"><span data-stu-id="cb3af-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cb3af-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb3af-105">Properties</span></span>

| <span data-ttu-id="cb3af-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb3af-106">Property</span></span>            | <span data-ttu-id="cb3af-107">種類</span><span class="sxs-lookup"><span data-stu-id="cb3af-107">Type</span></span>     | <span data-ttu-id="cb3af-108">説明</span><span class="sxs-lookup"><span data-stu-id="cb3af-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="cb3af-109">ID</span><span class="sxs-lookup"><span data-stu-id="cb3af-109">id</span></span>                  | <span data-ttu-id="cb3af-110">文字列</span><span class="sxs-lookup"><span data-stu-id="cb3af-110">string</span></span>   | <span data-ttu-id="cb3af-111">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="cb3af-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="cb3af-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="cb3af-112">teamsAppId</span></span>          | <span data-ttu-id="cb3af-113">文字列</span><span class="sxs-lookup"><span data-stu-id="cb3af-113">string</span></span>   | <span data-ttu-id="cb3af-114">チームのアプリケーション マニフェストの id です。</span><span class="sxs-lookup"><span data-stu-id="cb3af-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="cb3af-115">displayName</span><span class="sxs-lookup"><span data-stu-id="cb3af-115">displayName</span></span>         | <span data-ttu-id="cb3af-116">string</span><span class="sxs-lookup"><span data-stu-id="cb3af-116">string</span></span>   | <span data-ttu-id="cb3af-117">アプリケーション開発者によって提供されるアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="cb3af-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="cb3af-118">version</span><span class="sxs-lookup"><span data-stu-id="cb3af-118">version</span></span>             | <span data-ttu-id="cb3af-119">文字列</span><span class="sxs-lookup"><span data-stu-id="cb3af-119">string</span></span>   | <span data-ttu-id="cb3af-120">アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="cb3af-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cb3af-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb3af-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="cb3af-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="cb3af-122">See also</span></span>

- [<span data-ttu-id="cb3af-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cb3af-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="cb3af-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="cb3af-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="cb3af-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cb3af-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


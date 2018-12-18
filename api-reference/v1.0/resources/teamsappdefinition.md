---
title: teamsAppDefinition リソースの種類
description: TeamsApp の 1 つのバージョンの詳細。
author: nkramer
ms.openlocfilehash: 43bd4262008a29668739e78d4b598da1e77e3d4b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351640"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="6c77a-103">teamsAppDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c77a-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="6c77a-104">の[teamsApp](teamsapp.md)の 1 つのバージョンの詳細。</span><span class="sxs-lookup"><span data-stu-id="6c77a-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6c77a-105">Properties</span><span class="sxs-lookup"><span data-stu-id="6c77a-105">Properties</span></span>

| <span data-ttu-id="6c77a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c77a-106">Property</span></span>            | <span data-ttu-id="6c77a-107">種類</span><span class="sxs-lookup"><span data-stu-id="6c77a-107">Type</span></span>     | <span data-ttu-id="6c77a-108">説明</span><span class="sxs-lookup"><span data-stu-id="6c77a-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="6c77a-109">ID</span><span class="sxs-lookup"><span data-stu-id="6c77a-109">id</span></span>                  | <span data-ttu-id="6c77a-110">string</span><span class="sxs-lookup"><span data-stu-id="6c77a-110">string</span></span>   | <span data-ttu-id="6c77a-111">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="6c77a-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="6c77a-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="6c77a-112">teamsAppId</span></span>          | <span data-ttu-id="6c77a-113">string</span><span class="sxs-lookup"><span data-stu-id="6c77a-113">string</span></span>   | <span data-ttu-id="6c77a-114">チームのアプリケーション マニフェストの id です。</span><span class="sxs-lookup"><span data-stu-id="6c77a-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="6c77a-115">displayName</span><span class="sxs-lookup"><span data-stu-id="6c77a-115">displayName</span></span>         | <span data-ttu-id="6c77a-116">string</span><span class="sxs-lookup"><span data-stu-id="6c77a-116">string</span></span>   | <span data-ttu-id="6c77a-117">アプリケーション開発者によって提供されるアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="6c77a-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="6c77a-118">version</span><span class="sxs-lookup"><span data-stu-id="6c77a-118">version</span></span>             | <span data-ttu-id="6c77a-119">文字列</span><span class="sxs-lookup"><span data-stu-id="6c77a-119">string</span></span>   | <span data-ttu-id="6c77a-120">アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="6c77a-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6c77a-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c77a-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="6c77a-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c77a-122">See also</span></span>

- [<span data-ttu-id="6c77a-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="6c77a-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="6c77a-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="6c77a-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="6c77a-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6c77a-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


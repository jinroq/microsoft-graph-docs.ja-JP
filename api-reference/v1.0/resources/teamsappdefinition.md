---
title: teamsAppDefinition リソースの種類
description: TeamsApp の 1 つのバージョンの詳細。
ms.openlocfilehash: 34ec74c00dccca48df3b65758e1739cd29b19e7f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020590"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="c1a1c-103">teamsAppDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1a1c-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="c1a1c-104">の[teamsApp](teamsapp.md)の 1 つのバージョンの詳細。</span><span class="sxs-lookup"><span data-stu-id="c1a1c-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c1a1c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1a1c-105">Properties</span></span>

| <span data-ttu-id="c1a1c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1a1c-106">Property</span></span>            | <span data-ttu-id="c1a1c-107">型</span><span class="sxs-lookup"><span data-stu-id="c1a1c-107">Type</span></span>     | <span data-ttu-id="c1a1c-108">説明</span><span class="sxs-lookup"><span data-stu-id="c1a1c-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="c1a1c-109">ID</span><span class="sxs-lookup"><span data-stu-id="c1a1c-109">id</span></span>                  | <span data-ttu-id="c1a1c-110">文字列</span><span class="sxs-lookup"><span data-stu-id="c1a1c-110">string</span></span>   | <span data-ttu-id="c1a1c-111">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="c1a1c-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="c1a1c-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="c1a1c-112">teamsAppId</span></span>          | <span data-ttu-id="c1a1c-113">文字列</span><span class="sxs-lookup"><span data-stu-id="c1a1c-113">string</span></span>   | <span data-ttu-id="c1a1c-114">チームのアプリケーション マニフェストの id です。</span><span class="sxs-lookup"><span data-stu-id="c1a1c-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="c1a1c-115">displayName</span><span class="sxs-lookup"><span data-stu-id="c1a1c-115">displayName</span></span>         | <span data-ttu-id="c1a1c-116">string</span><span class="sxs-lookup"><span data-stu-id="c1a1c-116">string</span></span>   | <span data-ttu-id="c1a1c-117">アプリケーション開発者によって提供されるアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="c1a1c-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="c1a1c-118">version</span><span class="sxs-lookup"><span data-stu-id="c1a1c-118">version</span></span>             | <span data-ttu-id="c1a1c-119">文字列</span><span class="sxs-lookup"><span data-stu-id="c1a1c-119">string</span></span>   | <span data-ttu-id="c1a1c-120">アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="c1a1c-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c1a1c-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1a1c-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="c1a1c-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="c1a1c-122">See also</span></span>

- [<span data-ttu-id="c1a1c-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c1a1c-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="c1a1c-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c1a1c-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="c1a1c-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c1a1c-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


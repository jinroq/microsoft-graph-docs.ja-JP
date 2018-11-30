---
title: teamsAppDefinition リソースの種類
description: TeamsApp の 1 つのバージョンの詳細。
ms.openlocfilehash: b2a5b86de67fa1a4ecf673434b13d09c64ebe678
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073021"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="72f3c-103">teamsAppDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="72f3c-103">teamsAppDefinition resource type</span></span>

> <span data-ttu-id="72f3c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="72f3c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72f3c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72f3c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72f3c-106">の[teamsApp](teamsapp.md)の 1 つのバージョンの詳細。</span><span class="sxs-lookup"><span data-stu-id="72f3c-106">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="72f3c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72f3c-107">Properties</span></span>

| <span data-ttu-id="72f3c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72f3c-108">Property</span></span>            | <span data-ttu-id="72f3c-109">型</span><span class="sxs-lookup"><span data-stu-id="72f3c-109">Type</span></span>     | <span data-ttu-id="72f3c-110">説明</span><span class="sxs-lookup"><span data-stu-id="72f3c-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="72f3c-111">ID</span><span class="sxs-lookup"><span data-stu-id="72f3c-111">id</span></span>                  | <span data-ttu-id="72f3c-112">文字列</span><span class="sxs-lookup"><span data-stu-id="72f3c-112">string</span></span>   | <span data-ttu-id="72f3c-113">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="72f3c-113">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="72f3c-114">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="72f3c-114">teamsAppId</span></span>          | <span data-ttu-id="72f3c-115">文字列</span><span class="sxs-lookup"><span data-stu-id="72f3c-115">string</span></span>   | <span data-ttu-id="72f3c-116">チームのアプリケーション マニフェストの id です。</span><span class="sxs-lookup"><span data-stu-id="72f3c-116">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="72f3c-117">displayName</span><span class="sxs-lookup"><span data-stu-id="72f3c-117">displayName</span></span>         | <span data-ttu-id="72f3c-118">string</span><span class="sxs-lookup"><span data-stu-id="72f3c-118">string</span></span>   | <span data-ttu-id="72f3c-119">アプリケーション開発者によって提供されるアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="72f3c-119">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="72f3c-120">version</span><span class="sxs-lookup"><span data-stu-id="72f3c-120">version</span></span>             | <span data-ttu-id="72f3c-121">文字列</span><span class="sxs-lookup"><span data-stu-id="72f3c-121">string</span></span>   | <span data-ttu-id="72f3c-122">アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="72f3c-122">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="72f3c-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="72f3c-123">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="72f3c-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="72f3c-124">See also</span></span>

- [<span data-ttu-id="72f3c-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="72f3c-125">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="72f3c-126">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="72f3c-126">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="72f3c-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="72f3c-127">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


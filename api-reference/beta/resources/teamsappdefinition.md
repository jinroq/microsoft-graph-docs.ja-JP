---
title: teamsAppDefinition リソースの種類
description: TeamsApp の 1 つのバージョンの詳細。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8a13f6ffd4ca5385b9e264f8b8a5b8bddfe0a1fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851297"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="e33d5-103">teamsAppDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e33d5-103">teamsAppDefinition resource type</span></span>

> <span data-ttu-id="e33d5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e33d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e33d5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e33d5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e33d5-106">の[teamsApp](teamsapp.md)の 1 つのバージョンの詳細。</span><span class="sxs-lookup"><span data-stu-id="e33d5-106">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e33d5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e33d5-107">Properties</span></span>

| <span data-ttu-id="e33d5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e33d5-108">Property</span></span>            | <span data-ttu-id="e33d5-109">種類</span><span class="sxs-lookup"><span data-stu-id="e33d5-109">Type</span></span>     | <span data-ttu-id="e33d5-110">説明</span><span class="sxs-lookup"><span data-stu-id="e33d5-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="e33d5-111">ID</span><span class="sxs-lookup"><span data-stu-id="e33d5-111">id</span></span>                  | <span data-ttu-id="e33d5-112">文字列</span><span class="sxs-lookup"><span data-stu-id="e33d5-112">string</span></span>   | <span data-ttu-id="e33d5-113">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="e33d5-113">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="e33d5-114">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="e33d5-114">teamsAppId</span></span>          | <span data-ttu-id="e33d5-115">文字列</span><span class="sxs-lookup"><span data-stu-id="e33d5-115">string</span></span>   | <span data-ttu-id="e33d5-116">チームのアプリケーション マニフェストの id です。</span><span class="sxs-lookup"><span data-stu-id="e33d5-116">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="e33d5-117">displayName</span><span class="sxs-lookup"><span data-stu-id="e33d5-117">displayName</span></span>         | <span data-ttu-id="e33d5-118">string</span><span class="sxs-lookup"><span data-stu-id="e33d5-118">string</span></span>   | <span data-ttu-id="e33d5-119">アプリケーション開発者によって提供されるアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="e33d5-119">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="e33d5-120">version</span><span class="sxs-lookup"><span data-stu-id="e33d5-120">version</span></span>             | <span data-ttu-id="e33d5-121">文字列</span><span class="sxs-lookup"><span data-stu-id="e33d5-121">string</span></span>   | <span data-ttu-id="e33d5-122">アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="e33d5-122">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e33d5-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e33d5-123">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="e33d5-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="e33d5-124">See also</span></span>

- [<span data-ttu-id="e33d5-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e33d5-125">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="e33d5-126">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e33d5-126">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="e33d5-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e33d5-127">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


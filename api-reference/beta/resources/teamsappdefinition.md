---
title: teamsAppDefinition リソースの種類
description: TeamsApp の 1 つのバージョンの詳細。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 312b9347519935c4ff34f51cee24e0082c3da58e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969766"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="e4cda-103">teamsAppDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e4cda-103">teamsAppDefinition resource type</span></span>

> <span data-ttu-id="e4cda-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e4cda-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4cda-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4cda-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4cda-106">の[teamsApp](teamsapp.md)の 1 つのバージョンの詳細。</span><span class="sxs-lookup"><span data-stu-id="e4cda-106">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e4cda-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4cda-107">Properties</span></span>

| <span data-ttu-id="e4cda-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4cda-108">Property</span></span>            | <span data-ttu-id="e4cda-109">種類</span><span class="sxs-lookup"><span data-stu-id="e4cda-109">Type</span></span>     | <span data-ttu-id="e4cda-110">説明</span><span class="sxs-lookup"><span data-stu-id="e4cda-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="e4cda-111">ID</span><span class="sxs-lookup"><span data-stu-id="e4cda-111">id</span></span>                  | <span data-ttu-id="e4cda-112">文字列</span><span class="sxs-lookup"><span data-stu-id="e4cda-112">string</span></span>   | <span data-ttu-id="e4cda-113">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="e4cda-113">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="e4cda-114">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="e4cda-114">teamsAppId</span></span>          | <span data-ttu-id="e4cda-115">文字列</span><span class="sxs-lookup"><span data-stu-id="e4cda-115">string</span></span>   | <span data-ttu-id="e4cda-116">チームのアプリケーション マニフェストの id です。</span><span class="sxs-lookup"><span data-stu-id="e4cda-116">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="e4cda-117">displayName</span><span class="sxs-lookup"><span data-stu-id="e4cda-117">displayName</span></span>         | <span data-ttu-id="e4cda-118">string</span><span class="sxs-lookup"><span data-stu-id="e4cda-118">string</span></span>   | <span data-ttu-id="e4cda-119">アプリケーション開発者によって提供されるアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="e4cda-119">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="e4cda-120">version</span><span class="sxs-lookup"><span data-stu-id="e4cda-120">version</span></span>             | <span data-ttu-id="e4cda-121">文字列</span><span class="sxs-lookup"><span data-stu-id="e4cda-121">string</span></span>   | <span data-ttu-id="e4cda-122">アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="e4cda-122">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e4cda-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e4cda-123">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="e4cda-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="e4cda-124">See also</span></span>

- [<span data-ttu-id="e4cda-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e4cda-125">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="e4cda-126">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e4cda-126">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="e4cda-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e4cda-127">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


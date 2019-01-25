---
title: teamsAppInstallation リソースの種類
description: 'チームでインストールする teamsApp です。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4cf14c36fc0ab0b33f88d4b330e76957e65164a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512837"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="02cc3-103">teamsAppInstallation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="02cc3-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02cc3-104">[TeamsApp](teamsapp.md) [チーム](team.md)にインストールされています。</span><span class="sxs-lookup"><span data-stu-id="02cc3-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="02cc3-105">アプリケーションの一部である任意のボットにアプリケーションが追加されるすべてのチームの一員となります。</span><span class="sxs-lookup"><span data-stu-id="02cc3-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="02cc3-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="02cc3-106">Methods</span></span>

| <span data-ttu-id="02cc3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="02cc3-107">Method</span></span>       | <span data-ttu-id="02cc3-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="02cc3-108">Return Type</span></span>  |<span data-ttu-id="02cc3-109">説明</span><span class="sxs-lookup"><span data-stu-id="02cc3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02cc3-110">リスト アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02cc3-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="02cc3-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="02cc3-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="02cc3-112">チームでインストールされているアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="02cc3-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="02cc3-113">アプリを追加します。</span><span class="sxs-lookup"><span data-stu-id="02cc3-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="02cc3-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="02cc3-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="02cc3-115">(インストール) を追加するチームにアプリです。</span><span class="sxs-lookup"><span data-stu-id="02cc3-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="02cc3-116">アプリを抹消します。</span><span class="sxs-lookup"><span data-stu-id="02cc3-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="02cc3-117">なし</span><span class="sxs-lookup"><span data-stu-id="02cc3-117">None</span></span> | <span data-ttu-id="02cc3-118">削除 (アンインストール)、チームからのアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="02cc3-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="02cc3-119">アプリケーションをアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="02cc3-119">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="02cc3-120">なし</span><span class="sxs-lookup"><span data-stu-id="02cc3-120">None</span></span> | <span data-ttu-id="02cc3-121">アプリケーションの最新バージョンにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="02cc3-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="02cc3-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02cc3-122">Properties</span></span>

| <span data-ttu-id="02cc3-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02cc3-123">Property</span></span>            | <span data-ttu-id="02cc3-124">型</span><span class="sxs-lookup"><span data-stu-id="02cc3-124">Type</span></span>     | <span data-ttu-id="02cc3-125">説明</span><span class="sxs-lookup"><span data-stu-id="02cc3-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="02cc3-126">id</span><span class="sxs-lookup"><span data-stu-id="02cc3-126">id</span></span>                  | <span data-ttu-id="02cc3-127">string</span><span class="sxs-lookup"><span data-stu-id="02cc3-127">string</span></span>   | <span data-ttu-id="02cc3-128">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="02cc3-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="02cc3-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="02cc3-129">Relationships</span></span>

| <span data-ttu-id="02cc3-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="02cc3-130">Relationship</span></span>   | <span data-ttu-id="02cc3-131">型</span><span class="sxs-lookup"><span data-stu-id="02cc3-131">Type</span></span>    | <span data-ttu-id="02cc3-132">説明</span><span class="sxs-lookup"><span data-stu-id="02cc3-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="02cc3-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="02cc3-133">teamsApp</span></span>|[<span data-ttu-id="02cc3-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="02cc3-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="02cc3-135">インストールされているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="02cc3-135">The app that is installed.</span></span> |
|<span data-ttu-id="02cc3-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="02cc3-136">teamsAppDefinition</span></span>|[<span data-ttu-id="02cc3-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="02cc3-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="02cc3-138">このバージョンのアプリケーションの詳細。</span><span class="sxs-lookup"><span data-stu-id="02cc3-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02cc3-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02cc3-139">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a><span data-ttu-id="02cc3-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="02cc3-140">See also</span></span>

- [<span data-ttu-id="02cc3-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="02cc3-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="02cc3-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="02cc3-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="02cc3-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="02cc3-143">teamsTab</span></span>](../resources/teamstab.md)


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
    "Error: /api-reference/beta/resources/teamsappinstallation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->


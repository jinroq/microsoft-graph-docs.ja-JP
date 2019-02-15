---
title: teamsAppInstallation リソースの種類
description: 'チームにインストールされている teamsapp。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f6ff72ab99d20eba9880630248e4b61fca5c2521
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057016"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="a6dce-103">teamsAppInstallation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6dce-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6dce-104">[チーム](team.md)にインストールされている[teamsapp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="a6dce-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="a6dce-105">アプリの一部である bot は、アプリが追加されるチームの一部になります。</span><span class="sxs-lookup"><span data-stu-id="a6dce-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="a6dce-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a6dce-106">Methods</span></span>

| <span data-ttu-id="a6dce-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a6dce-107">Method</span></span>       | <span data-ttu-id="a6dce-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a6dce-108">Return Type</span></span>  |<span data-ttu-id="a6dce-109">説明</span><span class="sxs-lookup"><span data-stu-id="a6dce-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a6dce-110">アプリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a6dce-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="a6dce-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a6dce-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="a6dce-112">チームにインストールされているアプリを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="a6dce-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="a6dce-113">アプリの追加</span><span class="sxs-lookup"><span data-stu-id="a6dce-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="a6dce-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a6dce-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="a6dce-115">アプリをチームに追加 (インストール) します。</span><span class="sxs-lookup"><span data-stu-id="a6dce-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="a6dce-116">アプリの削除</span><span class="sxs-lookup"><span data-stu-id="a6dce-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="a6dce-117">なし</span><span class="sxs-lookup"><span data-stu-id="a6dce-117">None</span></span> | <span data-ttu-id="a6dce-118">チームからアプリを削除 (アンインストール) します。</span><span class="sxs-lookup"><span data-stu-id="a6dce-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="a6dce-119">アプリをアップグレードする</span><span class="sxs-lookup"><span data-stu-id="a6dce-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="a6dce-120">なし</span><span class="sxs-lookup"><span data-stu-id="a6dce-120">None</span></span> | <span data-ttu-id="a6dce-121">最新バージョンのアプリにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="a6dce-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6dce-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6dce-122">Properties</span></span>

| <span data-ttu-id="a6dce-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6dce-123">Property</span></span>            | <span data-ttu-id="a6dce-124">種類</span><span class="sxs-lookup"><span data-stu-id="a6dce-124">Type</span></span>     | <span data-ttu-id="a6dce-125">説明</span><span class="sxs-lookup"><span data-stu-id="a6dce-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="a6dce-126">id</span><span class="sxs-lookup"><span data-stu-id="a6dce-126">id</span></span>                  | <span data-ttu-id="a6dce-127">string</span><span class="sxs-lookup"><span data-stu-id="a6dce-127">string</span></span>   | <span data-ttu-id="a6dce-128">一意の id (teams appid ではない)。</span><span class="sxs-lookup"><span data-stu-id="a6dce-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="a6dce-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a6dce-129">Relationships</span></span>

| <span data-ttu-id="a6dce-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a6dce-130">Relationship</span></span>   | <span data-ttu-id="a6dce-131">型</span><span class="sxs-lookup"><span data-stu-id="a6dce-131">Type</span></span>    | <span data-ttu-id="a6dce-132">説明</span><span class="sxs-lookup"><span data-stu-id="a6dce-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a6dce-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a6dce-133">teamsApp</span></span>|[<span data-ttu-id="a6dce-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a6dce-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="a6dce-135">インストールされているアプリ。</span><span class="sxs-lookup"><span data-stu-id="a6dce-135">The app that is installed.</span></span> |
|<span data-ttu-id="a6dce-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a6dce-136">teamsAppDefinition</span></span>|[<span data-ttu-id="a6dce-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a6dce-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="a6dce-138">このバージョンのアプリの詳細。</span><span class="sxs-lookup"><span data-stu-id="a6dce-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a6dce-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6dce-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="a6dce-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="a6dce-140">See also</span></span>

- [<span data-ttu-id="a6dce-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a6dce-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="a6dce-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a6dce-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="a6dce-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a6dce-143">teamsTab</span></span>](../resources/teamstab.md)


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


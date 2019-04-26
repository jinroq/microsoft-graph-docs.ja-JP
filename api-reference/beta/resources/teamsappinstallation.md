---
title: teamsAppInstallation リソースの種類
description: 'チームにインストールされている teamsapp。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8d8770a21b11c9ba1042c9a0f59d9405dce96f9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345807"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="0627b-103">teamsAppInstallation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0627b-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0627b-104">[チーム](team.md)にインストールされている[teamsapp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="0627b-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="0627b-105">アプリの一部である bot は、アプリが追加されるチームの一部になります。</span><span class="sxs-lookup"><span data-stu-id="0627b-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="0627b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0627b-106">Methods</span></span>

| <span data-ttu-id="0627b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0627b-107">Method</span></span>       | <span data-ttu-id="0627b-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0627b-108">Return Type</span></span>  |<span data-ttu-id="0627b-109">説明</span><span class="sxs-lookup"><span data-stu-id="0627b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0627b-110">アプリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0627b-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="0627b-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="0627b-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="0627b-112">チームにインストールされているアプリを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0627b-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="0627b-113">アプリの追加</span><span class="sxs-lookup"><span data-stu-id="0627b-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="0627b-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="0627b-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="0627b-115">アプリをチームに追加 (インストール) します。</span><span class="sxs-lookup"><span data-stu-id="0627b-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="0627b-116">アプリの削除</span><span class="sxs-lookup"><span data-stu-id="0627b-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="0627b-117">なし</span><span class="sxs-lookup"><span data-stu-id="0627b-117">None</span></span> | <span data-ttu-id="0627b-118">チームからアプリを削除 (アンインストール) します。</span><span class="sxs-lookup"><span data-stu-id="0627b-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="0627b-119">アプリをアップグレードする</span><span class="sxs-lookup"><span data-stu-id="0627b-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="0627b-120">なし</span><span class="sxs-lookup"><span data-stu-id="0627b-120">None</span></span> | <span data-ttu-id="0627b-121">最新バージョンのアプリにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="0627b-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="0627b-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0627b-122">Properties</span></span>

| <span data-ttu-id="0627b-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0627b-123">Property</span></span>            | <span data-ttu-id="0627b-124">型</span><span class="sxs-lookup"><span data-stu-id="0627b-124">Type</span></span>     | <span data-ttu-id="0627b-125">説明</span><span class="sxs-lookup"><span data-stu-id="0627b-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="0627b-126">id</span><span class="sxs-lookup"><span data-stu-id="0627b-126">id</span></span>                  | <span data-ttu-id="0627b-127">string</span><span class="sxs-lookup"><span data-stu-id="0627b-127">string</span></span>   | <span data-ttu-id="0627b-128">一意の id (teams appid ではない)。</span><span class="sxs-lookup"><span data-stu-id="0627b-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="0627b-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0627b-129">Relationships</span></span>

| <span data-ttu-id="0627b-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0627b-130">Relationship</span></span>   | <span data-ttu-id="0627b-131">型</span><span class="sxs-lookup"><span data-stu-id="0627b-131">Type</span></span>    | <span data-ttu-id="0627b-132">説明</span><span class="sxs-lookup"><span data-stu-id="0627b-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0627b-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0627b-133">teamsApp</span></span>|[<span data-ttu-id="0627b-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0627b-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="0627b-135">インストールされているアプリ。</span><span class="sxs-lookup"><span data-stu-id="0627b-135">The app that is installed.</span></span> |
|<span data-ttu-id="0627b-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="0627b-136">teamsAppDefinition</span></span>|[<span data-ttu-id="0627b-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="0627b-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="0627b-138">このバージョンのアプリの詳細。</span><span class="sxs-lookup"><span data-stu-id="0627b-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0627b-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0627b-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="0627b-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="0627b-140">See also</span></span>

- [<span data-ttu-id="0627b-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0627b-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="0627b-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="0627b-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="0627b-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0627b-143">teamsTab</span></span>](../resources/teamstab.md)


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


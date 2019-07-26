---
title: teamsAppInstallation リソースの種類
description: 'チームにインストールされている teamsApp。 '
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b180cae4c700eea31a5d5d9b1504f09ca12c3ae0
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908349"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="26ed9-103">teamsAppInstallation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26ed9-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="26ed9-104">[チーム](team.md)にインストールされている[teamsapp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="26ed9-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="26ed9-105">アプリの一部である bot は、アプリが追加されるチームの一部になります。</span><span class="sxs-lookup"><span data-stu-id="26ed9-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="26ed9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="26ed9-106">Methods</span></span>

| <span data-ttu-id="26ed9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="26ed9-107">Method</span></span>       | <span data-ttu-id="26ed9-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="26ed9-108">Return Type</span></span>  |<span data-ttu-id="26ed9-109">説明</span><span class="sxs-lookup"><span data-stu-id="26ed9-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26ed9-110">アプリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="26ed9-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="26ed9-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="26ed9-111">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="26ed9-112">チームにインストールされているアプリを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="26ed9-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="26ed9-113">アプリの追加</span><span class="sxs-lookup"><span data-stu-id="26ed9-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="26ed9-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="26ed9-114">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="26ed9-115">アプリをチームに追加 (インストール) します。</span><span class="sxs-lookup"><span data-stu-id="26ed9-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="26ed9-116">アプリの削除</span><span class="sxs-lookup"><span data-stu-id="26ed9-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="26ed9-117">None</span><span class="sxs-lookup"><span data-stu-id="26ed9-117">None</span></span> | <span data-ttu-id="26ed9-118">チームからアプリを削除 (アンインストール) します。</span><span class="sxs-lookup"><span data-stu-id="26ed9-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="26ed9-119">アプリをアップグレードする</span><span class="sxs-lookup"><span data-stu-id="26ed9-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="26ed9-120">None</span><span class="sxs-lookup"><span data-stu-id="26ed9-120">None</span></span> | <span data-ttu-id="26ed9-121">最新バージョンのアプリにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="26ed9-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="26ed9-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26ed9-122">Properties</span></span>

| <span data-ttu-id="26ed9-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26ed9-123">Property</span></span>            | <span data-ttu-id="26ed9-124">型</span><span class="sxs-lookup"><span data-stu-id="26ed9-124">Type</span></span>     | <span data-ttu-id="26ed9-125">説明</span><span class="sxs-lookup"><span data-stu-id="26ed9-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="26ed9-126">id</span><span class="sxs-lookup"><span data-stu-id="26ed9-126">id</span></span>                  | <span data-ttu-id="26ed9-127">string</span><span class="sxs-lookup"><span data-stu-id="26ed9-127">string</span></span>   | <span data-ttu-id="26ed9-128">一意の id (teams appid ではない)。</span><span class="sxs-lookup"><span data-stu-id="26ed9-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="26ed9-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="26ed9-129">Relationships</span></span>

| <span data-ttu-id="26ed9-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="26ed9-130">Relationship</span></span>   | <span data-ttu-id="26ed9-131">型</span><span class="sxs-lookup"><span data-stu-id="26ed9-131">Type</span></span>    | <span data-ttu-id="26ed9-132">説明</span><span class="sxs-lookup"><span data-stu-id="26ed9-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="26ed9-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="26ed9-133">teamsApp</span></span>|[<span data-ttu-id="26ed9-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="26ed9-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="26ed9-135">インストールされているアプリ。</span><span class="sxs-lookup"><span data-stu-id="26ed9-135">The app that is installed.</span></span> |
|<span data-ttu-id="26ed9-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="26ed9-136">teamsAppDefinition</span></span>|[<span data-ttu-id="26ed9-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="26ed9-137">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="26ed9-138">このバージョンのアプリの詳細。</span><span class="sxs-lookup"><span data-stu-id="26ed9-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="26ed9-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26ed9-139">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a><span data-ttu-id="26ed9-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="26ed9-140">See also</span></span>

- [<span data-ttu-id="26ed9-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="26ed9-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="26ed9-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="26ed9-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="26ed9-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="26ed9-143">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

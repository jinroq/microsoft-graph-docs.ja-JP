---
title: teamsAppInstallation リソースの種類
description: 'チームでインストールする teamsApp です。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 30a7f05d7b814fbb36c632a88f2f4e71f135d781
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955346"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="aede2-103">teamsAppInstallation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aede2-103">teamsAppInstallation resource type</span></span>

> <span data-ttu-id="aede2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aede2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aede2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aede2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aede2-106">[TeamsApp](teamsapp.md) [チーム](team.md)にインストールされています。</span><span class="sxs-lookup"><span data-stu-id="aede2-106">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="aede2-107">アプリケーションの一部である任意のボットにアプリケーションが追加されるすべてのチームの一員となります。</span><span class="sxs-lookup"><span data-stu-id="aede2-107">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="aede2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="aede2-108">Methods</span></span>

| <span data-ttu-id="aede2-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="aede2-109">Method</span></span>       | <span data-ttu-id="aede2-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aede2-110">Return Type</span></span>  |<span data-ttu-id="aede2-111">説明</span><span class="sxs-lookup"><span data-stu-id="aede2-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aede2-112">リスト アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aede2-112">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="aede2-113">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="aede2-113">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="aede2-114">チームでインストールされているアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="aede2-114">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="aede2-115">アプリを追加します。</span><span class="sxs-lookup"><span data-stu-id="aede2-115">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="aede2-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="aede2-116">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="aede2-117">(インストール) を追加するチームにアプリです。</span><span class="sxs-lookup"><span data-stu-id="aede2-117">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="aede2-118">アプリを抹消します。</span><span class="sxs-lookup"><span data-stu-id="aede2-118">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="aede2-119">なし</span><span class="sxs-lookup"><span data-stu-id="aede2-119">None</span></span> | <span data-ttu-id="aede2-120">削除 (アンインストール)、チームからのアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="aede2-120">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="aede2-121">アプリケーションをアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="aede2-121">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="aede2-122">なし</span><span class="sxs-lookup"><span data-stu-id="aede2-122">None</span></span> | <span data-ttu-id="aede2-123">アプリケーションの最新バージョンにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="aede2-123">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="aede2-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aede2-124">Properties</span></span>

| <span data-ttu-id="aede2-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aede2-125">Property</span></span>            | <span data-ttu-id="aede2-126">型</span><span class="sxs-lookup"><span data-stu-id="aede2-126">Type</span></span>     | <span data-ttu-id="aede2-127">説明</span><span class="sxs-lookup"><span data-stu-id="aede2-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="aede2-128">ID</span><span class="sxs-lookup"><span data-stu-id="aede2-128">id</span></span>                  | <span data-ttu-id="aede2-129">string</span><span class="sxs-lookup"><span data-stu-id="aede2-129">string</span></span>   | <span data-ttu-id="aede2-130">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="aede2-130">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="aede2-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aede2-131">Relationships</span></span>

| <span data-ttu-id="aede2-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aede2-132">Relationship</span></span>   | <span data-ttu-id="aede2-133">型</span><span class="sxs-lookup"><span data-stu-id="aede2-133">Type</span></span>    | <span data-ttu-id="aede2-134">説明</span><span class="sxs-lookup"><span data-stu-id="aede2-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="aede2-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="aede2-135">teamsApp</span></span>|[<span data-ttu-id="aede2-136">teamsApp</span><span class="sxs-lookup"><span data-stu-id="aede2-136">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="aede2-137">インストールされているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="aede2-137">The app that is installed.</span></span> |
|<span data-ttu-id="aede2-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="aede2-138">teamsAppDefinition</span></span>|[<span data-ttu-id="aede2-139">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="aede2-139">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="aede2-140">このバージョンのアプリケーションの詳細。</span><span class="sxs-lookup"><span data-stu-id="aede2-140">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aede2-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aede2-141">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="aede2-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="aede2-142">See also</span></span>

- [<span data-ttu-id="aede2-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="aede2-143">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="aede2-144">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="aede2-144">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="aede2-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="aede2-145">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


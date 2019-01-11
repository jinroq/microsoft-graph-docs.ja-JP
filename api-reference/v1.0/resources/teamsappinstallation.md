---
title: teamsAppInstallation リソースの種類
description: 'チームでインストールする teamsApp です。 '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 037cda1a98f45db94ecfc31b112bc3ab82bf4698
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891190"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="c1857-103">teamsAppInstallation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1857-103">teamsAppInstallation resource type</span></span>



<span data-ttu-id="c1857-104">[TeamsApp](teamsapp.md) [チーム](team.md)にインストールされています。</span><span class="sxs-lookup"><span data-stu-id="c1857-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="c1857-105">アプリケーションの一部である任意のボットにアプリケーションが追加されるすべてのチームの一員となります。</span><span class="sxs-lookup"><span data-stu-id="c1857-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="c1857-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c1857-106">Methods</span></span>

| <span data-ttu-id="c1857-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c1857-107">Method</span></span>       | <span data-ttu-id="c1857-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c1857-108">Return Type</span></span>  |<span data-ttu-id="c1857-109">説明</span><span class="sxs-lookup"><span data-stu-id="c1857-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c1857-110">リスト アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c1857-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="c1857-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c1857-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="c1857-112">チームでインストールされているアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c1857-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="c1857-113">アプリを追加します。</span><span class="sxs-lookup"><span data-stu-id="c1857-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="c1857-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c1857-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="c1857-115">(インストール) を追加するチームにアプリです。</span><span class="sxs-lookup"><span data-stu-id="c1857-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="c1857-116">アプリを抹消します。</span><span class="sxs-lookup"><span data-stu-id="c1857-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="c1857-117">なし</span><span class="sxs-lookup"><span data-stu-id="c1857-117">None</span></span> | <span data-ttu-id="c1857-118">削除 (アンインストール)、チームからのアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="c1857-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="c1857-119">アプリケーションをアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="c1857-119">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="c1857-120">なし</span><span class="sxs-lookup"><span data-stu-id="c1857-120">None</span></span> | <span data-ttu-id="c1857-121">アプリケーションの最新バージョンにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="c1857-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1857-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1857-122">Properties</span></span>

| <span data-ttu-id="c1857-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1857-123">Property</span></span>            | <span data-ttu-id="c1857-124">種類</span><span class="sxs-lookup"><span data-stu-id="c1857-124">Type</span></span>     | <span data-ttu-id="c1857-125">説明</span><span class="sxs-lookup"><span data-stu-id="c1857-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="c1857-126">ID</span><span class="sxs-lookup"><span data-stu-id="c1857-126">id</span></span>                  | <span data-ttu-id="c1857-127">文字列</span><span class="sxs-lookup"><span data-stu-id="c1857-127">string</span></span>   | <span data-ttu-id="c1857-128">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="c1857-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="c1857-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1857-129">Relationships</span></span>

| <span data-ttu-id="c1857-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1857-130">Relationship</span></span>   | <span data-ttu-id="c1857-131">型</span><span class="sxs-lookup"><span data-stu-id="c1857-131">Type</span></span>    | <span data-ttu-id="c1857-132">説明</span><span class="sxs-lookup"><span data-stu-id="c1857-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c1857-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c1857-133">teamsApp</span></span>|[<span data-ttu-id="c1857-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c1857-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="c1857-135">インストールされているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="c1857-135">The app that is installed.</span></span> |
|<span data-ttu-id="c1857-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c1857-136">teamsAppDefinition</span></span>|[<span data-ttu-id="c1857-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c1857-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="c1857-138">このバージョンのアプリケーションの詳細。</span><span class="sxs-lookup"><span data-stu-id="c1857-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c1857-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1857-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="c1857-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="c1857-140">See also</span></span>

- [<span data-ttu-id="c1857-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c1857-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="c1857-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c1857-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="c1857-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c1857-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


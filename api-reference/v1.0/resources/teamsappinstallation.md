---
title: teamsAppInstallation リソースの種類
description: 'チームでインストールする teamsApp です。 '
author: nkramer
ms.openlocfilehash: e845bf10bc5513bc6a5079c295fde2eb6d7b6fa5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312811"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="35d71-103">teamsAppInstallation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35d71-103">teamsAppInstallation resource type</span></span>



<span data-ttu-id="35d71-104">[TeamsApp](teamsapp.md) [チーム](team.md)にインストールされています。</span><span class="sxs-lookup"><span data-stu-id="35d71-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="35d71-105">アプリケーションの一部である任意のボットにアプリケーションが追加されるすべてのチームの一員となります。</span><span class="sxs-lookup"><span data-stu-id="35d71-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="35d71-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="35d71-106">Methods</span></span>

| <span data-ttu-id="35d71-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="35d71-107">Method</span></span>       | <span data-ttu-id="35d71-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="35d71-108">Return Type</span></span>  |<span data-ttu-id="35d71-109">説明</span><span class="sxs-lookup"><span data-stu-id="35d71-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35d71-110">リスト アプリケーション</span><span class="sxs-lookup"><span data-stu-id="35d71-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="35d71-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="35d71-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="35d71-112">チームでインストールされているアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="35d71-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="35d71-113">アプリを追加します。</span><span class="sxs-lookup"><span data-stu-id="35d71-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="35d71-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="35d71-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="35d71-115">(インストール) を追加するチームにアプリです。</span><span class="sxs-lookup"><span data-stu-id="35d71-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="35d71-116">アプリを抹消します。</span><span class="sxs-lookup"><span data-stu-id="35d71-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="35d71-117">なし</span><span class="sxs-lookup"><span data-stu-id="35d71-117">None</span></span> | <span data-ttu-id="35d71-118">削除 (アンインストール)、チームからのアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="35d71-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="35d71-119">アプリケーションをアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="35d71-119">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="35d71-120">なし</span><span class="sxs-lookup"><span data-stu-id="35d71-120">None</span></span> | <span data-ttu-id="35d71-121">アプリケーションの最新バージョンにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="35d71-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="35d71-122">Properties</span><span class="sxs-lookup"><span data-stu-id="35d71-122">Properties</span></span>

| <span data-ttu-id="35d71-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35d71-123">Property</span></span>            | <span data-ttu-id="35d71-124">種類</span><span class="sxs-lookup"><span data-stu-id="35d71-124">Type</span></span>     | <span data-ttu-id="35d71-125">説明</span><span class="sxs-lookup"><span data-stu-id="35d71-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="35d71-126">ID</span><span class="sxs-lookup"><span data-stu-id="35d71-126">id</span></span>                  | <span data-ttu-id="35d71-127">string</span><span class="sxs-lookup"><span data-stu-id="35d71-127">string</span></span>   | <span data-ttu-id="35d71-128">一意の id (チームの appid とは異なる)。</span><span class="sxs-lookup"><span data-stu-id="35d71-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="35d71-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35d71-129">Relationships</span></span>

| <span data-ttu-id="35d71-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35d71-130">Relationship</span></span>   | <span data-ttu-id="35d71-131">型</span><span class="sxs-lookup"><span data-stu-id="35d71-131">Type</span></span>    | <span data-ttu-id="35d71-132">説明</span><span class="sxs-lookup"><span data-stu-id="35d71-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="35d71-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="35d71-133">teamsApp</span></span>|[<span data-ttu-id="35d71-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="35d71-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="35d71-135">インストールされているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="35d71-135">The app that is installed.</span></span> |
|<span data-ttu-id="35d71-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="35d71-136">teamsAppDefinition</span></span>|[<span data-ttu-id="35d71-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="35d71-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="35d71-138">このバージョンのアプリケーションの詳細。</span><span class="sxs-lookup"><span data-stu-id="35d71-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35d71-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35d71-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="35d71-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="35d71-140">See also</span></span>

- [<span data-ttu-id="35d71-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="35d71-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="35d71-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="35d71-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="35d71-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="35d71-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


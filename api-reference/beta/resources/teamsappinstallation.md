---
title: teamsAppInstallation リソースの種類
description: 'チーム、チャット、またはユーザーの個人用スコープにインストールされている teamsApp。 '
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 55e1246616b7a3d76c6170a02286a2cde2a15d3a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908510"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="e35ba-103">teamsAppInstallation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e35ba-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e35ba-104">[チーム](team.md)、[チャット](chat.md)、または[ユーザー](user.md)の個人の範囲にインストールされている[teamsapp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="e35ba-104">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="e35ba-105">アプリの一部である bot は、アプリが追加されるチーム、チャット、またはユーザーの個人スコープの一部になります。</span><span class="sxs-lookup"><span data-stu-id="e35ba-105">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="e35ba-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e35ba-106">Methods</span></span>

| <span data-ttu-id="e35ba-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e35ba-107">Method</span></span>       | <span data-ttu-id="e35ba-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e35ba-108">Return Type</span></span>  |<span data-ttu-id="e35ba-109">説明</span><span class="sxs-lookup"><span data-stu-id="e35ba-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e35ba-110">Team にインストールされているアプリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e35ba-110">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="e35ba-111">[teamsAppInstallation](teamsappinstallation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e35ba-111">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="e35ba-112">チームにインストールされているアプリを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e35ba-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="e35ba-113">アプリをチームに追加する</span><span class="sxs-lookup"><span data-stu-id="e35ba-113">Add app to team</span></span>](../api/teamsappinstallation-add.md) |<span data-ttu-id="e35ba-114">None</span><span class="sxs-lookup"><span data-stu-id="e35ba-114">None</span></span> | <span data-ttu-id="e35ba-115">アプリをチームに追加 (インストール) します。</span><span class="sxs-lookup"><span data-stu-id="e35ba-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="e35ba-116">チームからアプリを削除する</span><span class="sxs-lookup"><span data-stu-id="e35ba-116">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="e35ba-117">None</span><span class="sxs-lookup"><span data-stu-id="e35ba-117">None</span></span> | <span data-ttu-id="e35ba-118">チームからアプリを削除 (アンインストール) します。</span><span class="sxs-lookup"><span data-stu-id="e35ba-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="e35ba-119">Team にインストールされたアプリのアップグレード</span><span class="sxs-lookup"><span data-stu-id="e35ba-119">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="e35ba-120">None</span><span class="sxs-lookup"><span data-stu-id="e35ba-120">None</span></span> | <span data-ttu-id="e35ba-121">最新バージョンのアプリにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="e35ba-121">Upgrades to the latest version of the app.</span></span>|
|[<span data-ttu-id="e35ba-122">ユーザー用にインストールされているアプリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e35ba-122">List apps installed for user</span></span>](../api/user-list-teamsappinstallation.md) | <span data-ttu-id="e35ba-123">[teamsAppInstallation](teamsappinstallation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e35ba-123">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="e35ba-124">ユーザーの個人用スコープにインストールされているアプリを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e35ba-124">Lists apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="e35ba-125">ユーザーのアプリを追加する</span><span class="sxs-lookup"><span data-stu-id="e35ba-125">Add app for user</span></span>](../api/user-add-teamsappinstallation.md) | | <span data-ttu-id="e35ba-126">ユーザーの個人スコープにアプリを追加 (インストール) します。</span><span class="sxs-lookup"><span data-stu-id="e35ba-126">Adds (installs) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="e35ba-127">ユーザーのアプリを削除する</span><span class="sxs-lookup"><span data-stu-id="e35ba-127">Remove app for user</span></span>](../api/user-delete-teamsappinstallation.md) | <span data-ttu-id="e35ba-128">None</span><span class="sxs-lookup"><span data-stu-id="e35ba-128">None</span></span> | <span data-ttu-id="e35ba-129">ユーザーの個人スコープでアプリを削除 (アンインストール) します。</span><span class="sxs-lookup"><span data-stu-id="e35ba-129">Removes (uninstalls) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="e35ba-130">ユーザー用のアップグレードアプリがインストールされている</span><span class="sxs-lookup"><span data-stu-id="e35ba-130">Upgrade app installed for user</span></span>](../api/user-upgrade-teamsappinstallation.md) | <span data-ttu-id="e35ba-131">None</span><span class="sxs-lookup"><span data-stu-id="e35ba-131">None</span></span> | <span data-ttu-id="e35ba-132">ユーザーの個人スコープにインストールされている最新バージョンのアプリにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="e35ba-132">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="e35ba-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e35ba-133">Properties</span></span>

| <span data-ttu-id="e35ba-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e35ba-134">Property</span></span>            | <span data-ttu-id="e35ba-135">型</span><span class="sxs-lookup"><span data-stu-id="e35ba-135">Type</span></span>     | <span data-ttu-id="e35ba-136">説明</span><span class="sxs-lookup"><span data-stu-id="e35ba-136">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="e35ba-137">id</span><span class="sxs-lookup"><span data-stu-id="e35ba-137">id</span></span>                  | <span data-ttu-id="e35ba-138">string</span><span class="sxs-lookup"><span data-stu-id="e35ba-138">string</span></span>   | <span data-ttu-id="e35ba-139">一意の ID (チームの ap ID ではありません)。</span><span class="sxs-lookup"><span data-stu-id="e35ba-139">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="e35ba-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e35ba-140">Relationships</span></span>

| <span data-ttu-id="e35ba-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e35ba-141">Relationship</span></span>   | <span data-ttu-id="e35ba-142">型</span><span class="sxs-lookup"><span data-stu-id="e35ba-142">Type</span></span>    | <span data-ttu-id="e35ba-143">説明</span><span class="sxs-lookup"><span data-stu-id="e35ba-143">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e35ba-144">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e35ba-144">teamsApp</span></span>|[<span data-ttu-id="e35ba-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e35ba-145">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="e35ba-146">インストールされているアプリ。</span><span class="sxs-lookup"><span data-stu-id="e35ba-146">The app that is installed.</span></span> |
|<span data-ttu-id="e35ba-147">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="e35ba-147">teamsAppDefinition</span></span>|[<span data-ttu-id="e35ba-148">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="e35ba-148">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="e35ba-149">このバージョンのアプリの詳細。</span><span class="sxs-lookup"><span data-stu-id="e35ba-149">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e35ba-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e35ba-150">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="e35ba-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="e35ba-151">See also</span></span>

- [<span data-ttu-id="e35ba-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e35ba-152">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="e35ba-153">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="e35ba-153">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="e35ba-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e35ba-154">teamsTab</span></span>](../resources/teamstab.md)

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

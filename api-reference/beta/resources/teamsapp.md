---
title: teamsApp リソースの種類
description: マイクロソフト チーム アプリケーション カタログのアプリケーションです。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: b02af5148e40cddd6079de3479767110a9877e4f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841574"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="93573-103">teamsApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="93573-103">teamsApp resource type</span></span>

> <span data-ttu-id="93573-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="93573-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93573-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93573-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93573-106">[マイクロソフト チーム](teams-api-overview.md)アプリケーション カタログのアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="93573-106">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="93573-107">マイクロソフト チーム ストア内のこれらのアプリケーションを表示して、[チーム](team.md)が[チームに追加のアプリケーション](../api/teamsappinstallation-add.md)のメソッドを使用してこれらのアプリケーションをインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="93573-107">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="93573-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="93573-108">Methods</span></span>

| <span data-ttu-id="93573-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="93573-109">Method</span></span>       | <span data-ttu-id="93573-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="93573-110">Return Type</span></span>  |<span data-ttu-id="93573-111">説明</span><span class="sxs-lookup"><span data-stu-id="93573-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93573-112">公開されたアプリケーションの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="93573-112">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="93573-113">[teamsApp](teamsapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="93573-113">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="93573-114">マイクロソフト チーム アプリケーション カタログから公開されているアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="93573-114">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="93573-115">アプリケーションを発行します。</span><span class="sxs-lookup"><span data-stu-id="93573-115">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="93573-116">teamsApp</span><span class="sxs-lookup"><span data-stu-id="93573-116">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="93573-117">組織のアプリケーションのカタログには、アプリケーションを発行します。</span><span class="sxs-lookup"><span data-stu-id="93573-117">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="93573-118">発行したアプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="93573-118">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="93573-119">teamsApp</span><span class="sxs-lookup"><span data-stu-id="93573-119">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="93573-120">組織のアプリケーションのカタログに公開されたアプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="93573-120">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="93573-121">発行したアプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="93573-121">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="93573-122">なし</span><span class="sxs-lookup"><span data-stu-id="93573-122">None</span></span> | <span data-ttu-id="93573-123">発行したアプリケーションを組織のアプリケーションのカタログから削除します。</span><span class="sxs-lookup"><span data-stu-id="93573-123">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="93573-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93573-124">Properties</span></span>

| <span data-ttu-id="93573-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93573-125">Property</span></span>            | <span data-ttu-id="93573-126">種類</span><span class="sxs-lookup"><span data-stu-id="93573-126">Type</span></span>     | <span data-ttu-id="93573-127">説明</span><span class="sxs-lookup"><span data-stu-id="93573-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="93573-128">ID</span><span class="sxs-lookup"><span data-stu-id="93573-128">id</span></span>                  | <span data-ttu-id="93573-129">文字列</span><span class="sxs-lookup"><span data-stu-id="93573-129">string</span></span>   | <span data-ttu-id="93573-130">カタログ アプリケーションの生成のアプリケーション ID を ([マイクロソフト チーム zip アプリケーション パッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)の開発者から提供された ID とは異なる。</span><span class="sxs-lookup"><span data-stu-id="93573-130">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="93573-131">externalId</span><span class="sxs-lookup"><span data-stu-id="93573-131">externalId</span></span>          | <span data-ttu-id="93573-132">文字列</span><span class="sxs-lookup"><span data-stu-id="93573-132">string</span></span>   | <span data-ttu-id="93573-133">アプリケーション開発者が、[マイクロソフトのチームは、アプリケーションのパッケージを zip](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)に用意されているカタログの ID です。</span><span class="sxs-lookup"><span data-stu-id="93573-133">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="93573-134">displayName</span><span class="sxs-lookup"><span data-stu-id="93573-134">displayName</span></span>                | <span data-ttu-id="93573-135">string</span><span class="sxs-lookup"><span data-stu-id="93573-135">string</span></span>   | <span data-ttu-id="93573-136">アプリケーション開発者が、[マイクロソフトのチームは、アプリケーションのパッケージを zip](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)に用意されているカタログのアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="93573-136">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="93573-137">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="93573-137">distributionMethod</span></span>  | <span data-ttu-id="93573-138">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="93573-138">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="93573-139">アプリケーション配布の方法です。</span><span class="sxs-lookup"><span data-stu-id="93573-139">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="93573-140">teamsAppDistributionMethod 値</span><span class="sxs-lookup"><span data-stu-id="93573-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="93573-141">メンバー</span><span class="sxs-lookup"><span data-stu-id="93573-141">Member</span></span>|<span data-ttu-id="93573-142">値</span><span class="sxs-lookup"><span data-stu-id="93573-142">Value</span></span>|<span data-ttu-id="93573-143">説明</span><span class="sxs-lookup"><span data-stu-id="93573-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93573-144">ストア</span><span class="sxs-lookup"><span data-stu-id="93573-144">store</span></span>|<span data-ttu-id="93573-145">0</span><span class="sxs-lookup"><span data-stu-id="93573-145">0</span></span>| <span data-ttu-id="93573-146">アプリケーションは、マイクロソフトのチームのアプリケーション ストアからのすべてのテナントに使用できます。</span><span class="sxs-lookup"><span data-stu-id="93573-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="93573-147">組織</span><span class="sxs-lookup"><span data-stu-id="93573-147">organization</span></span>|<span data-ttu-id="93573-148">1</span><span class="sxs-lookup"><span data-stu-id="93573-148">1</span></span>|<span data-ttu-id="93573-149">アプリケーションは、このテナントでのみ使用可能です。</span><span class="sxs-lookup"><span data-stu-id="93573-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="93573-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="93573-150">sideloaded</span></span>|<span data-ttu-id="93573-151">2</span><span class="sxs-lookup"><span data-stu-id="93573-151">2</span></span>|<span data-ttu-id="93573-152">アプリケーションは、ユーザーまたはチームのみ使用可能です、インストールされているをします。</span><span class="sxs-lookup"><span data-stu-id="93573-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93573-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="93573-153">Relationships</span></span>

| <span data-ttu-id="93573-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="93573-154">Relationship</span></span> | <span data-ttu-id="93573-155">型</span><span class="sxs-lookup"><span data-stu-id="93573-155">Type</span></span>   | <span data-ttu-id="93573-156">説明</span><span class="sxs-lookup"><span data-stu-id="93573-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="93573-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="93573-157">appDefinitions</span></span>|<span data-ttu-id="93573-158">[teamsAppDefinition](teamsappdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="93573-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="93573-159">アプリケーションの各バージョンの詳細です。</span><span class="sxs-lookup"><span data-stu-id="93573-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="93573-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93573-160">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

# <a name="see-also"></a><span data-ttu-id="93573-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="93573-161">See also</span></span>

- [<span data-ttu-id="93573-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="93573-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="93573-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="93573-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="93573-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="93573-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


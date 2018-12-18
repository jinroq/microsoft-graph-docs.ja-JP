---
title: teamsApp リソースの種類
description: マイクロソフト チーム アプリケーション カタログのアプリケーションです。
author: nkramer
ms.openlocfilehash: 207974800e44e0db29b8c42f260a1ac16a18902f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359585"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="67c8c-103">teamsApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="67c8c-103">teamsApp resource type</span></span>



<span data-ttu-id="67c8c-104">[マイクロソフト チーム](teams-api-overview.md)アプリケーション カタログのアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="67c8c-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="67c8c-105">マイクロソフト チーム ストア内のこれらのアプリケーションを表示して、[チーム](team.md)が[チームに追加のアプリケーション](../api/teamsappinstallation-add.md)のメソッドを使用してこれらのアプリケーションをインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="67c8c-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="67c8c-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="67c8c-106">Methods</span></span>

| <span data-ttu-id="67c8c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="67c8c-107">Method</span></span>       | <span data-ttu-id="67c8c-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="67c8c-108">Return Type</span></span>  |<span data-ttu-id="67c8c-109">説明</span><span class="sxs-lookup"><span data-stu-id="67c8c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="67c8c-110">公開されたアプリケーションの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="67c8c-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="67c8c-111">[teamsApp](teamsapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="67c8c-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="67c8c-112">マイクロソフト チーム アプリケーション カタログから公開されているアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="67c8c-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="67c8c-113">アプリケーションを発行します。</span><span class="sxs-lookup"><span data-stu-id="67c8c-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="67c8c-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="67c8c-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="67c8c-115">組織のアプリケーションのカタログには、アプリケーションを発行します。</span><span class="sxs-lookup"><span data-stu-id="67c8c-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="67c8c-116">発行したアプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="67c8c-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="67c8c-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="67c8c-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="67c8c-118">組織のアプリケーションのカタログに公開されたアプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="67c8c-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="67c8c-119">発行したアプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="67c8c-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="67c8c-120">なし</span><span class="sxs-lookup"><span data-stu-id="67c8c-120">None</span></span> | <span data-ttu-id="67c8c-121">発行したアプリケーションを組織のアプリケーションのカタログから削除します。</span><span class="sxs-lookup"><span data-stu-id="67c8c-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="67c8c-122">Properties</span><span class="sxs-lookup"><span data-stu-id="67c8c-122">Properties</span></span>

| <span data-ttu-id="67c8c-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67c8c-123">Property</span></span>            | <span data-ttu-id="67c8c-124">種類</span><span class="sxs-lookup"><span data-stu-id="67c8c-124">Type</span></span>     | <span data-ttu-id="67c8c-125">説明</span><span class="sxs-lookup"><span data-stu-id="67c8c-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="67c8c-126">ID</span><span class="sxs-lookup"><span data-stu-id="67c8c-126">id</span></span>                  | <span data-ttu-id="67c8c-127">string</span><span class="sxs-lookup"><span data-stu-id="67c8c-127">string</span></span>   | <span data-ttu-id="67c8c-128">カタログ アプリケーションの生成のアプリケーション ID を ([マイクロソフト チーム zip アプリケーション パッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)の開発者から提供された ID とは異なる。</span><span class="sxs-lookup"><span data-stu-id="67c8c-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="67c8c-129">externalId</span><span class="sxs-lookup"><span data-stu-id="67c8c-129">externalId</span></span>          | <span data-ttu-id="67c8c-130">string</span><span class="sxs-lookup"><span data-stu-id="67c8c-130">string</span></span>   | <span data-ttu-id="67c8c-131">アプリケーション開発者が、[マイクロソフトのチームは、アプリケーションのパッケージを zip](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)に用意されているカタログの ID です。</span><span class="sxs-lookup"><span data-stu-id="67c8c-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="67c8c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="67c8c-132">displayName</span></span>                | <span data-ttu-id="67c8c-133">string</span><span class="sxs-lookup"><span data-stu-id="67c8c-133">string</span></span>   | <span data-ttu-id="67c8c-134">アプリケーション開発者が、[マイクロソフトのチームは、アプリケーションのパッケージを zip](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)に用意されているカタログのアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="67c8c-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="67c8c-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="67c8c-135">distributionMethod</span></span>  | <span data-ttu-id="67c8c-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="67c8c-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="67c8c-137">アプリケーション配布の方法です。</span><span class="sxs-lookup"><span data-stu-id="67c8c-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="67c8c-138">teamsAppDistributionMethod 値</span><span class="sxs-lookup"><span data-stu-id="67c8c-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="67c8c-139">Member</span><span class="sxs-lookup"><span data-stu-id="67c8c-139">Member</span></span>|<span data-ttu-id="67c8c-140">値</span><span class="sxs-lookup"><span data-stu-id="67c8c-140">Value</span></span>|<span data-ttu-id="67c8c-141">説明</span><span class="sxs-lookup"><span data-stu-id="67c8c-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67c8c-142">ストア</span><span class="sxs-lookup"><span data-stu-id="67c8c-142">store</span></span>|<span data-ttu-id="67c8c-143">0</span><span class="sxs-lookup"><span data-stu-id="67c8c-143">0</span></span>| <span data-ttu-id="67c8c-144">アプリケーションは、マイクロソフトのチームのアプリケーション ストアからのすべてのテナントに使用できます。</span><span class="sxs-lookup"><span data-stu-id="67c8c-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="67c8c-145">組織</span><span class="sxs-lookup"><span data-stu-id="67c8c-145">organization</span></span>|<span data-ttu-id="67c8c-146">1</span><span class="sxs-lookup"><span data-stu-id="67c8c-146">1</span></span>|<span data-ttu-id="67c8c-147">アプリケーションは、このテナントでのみ使用可能です。</span><span class="sxs-lookup"><span data-stu-id="67c8c-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="67c8c-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="67c8c-148">sideloaded</span></span>|<span data-ttu-id="67c8c-149">2</span><span class="sxs-lookup"><span data-stu-id="67c8c-149">2</span></span>|<span data-ttu-id="67c8c-150">アプリケーションは、ユーザーまたはチームのみ使用可能です、インストールされているをします。</span><span class="sxs-lookup"><span data-stu-id="67c8c-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67c8c-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67c8c-151">Relationships</span></span>

| <span data-ttu-id="67c8c-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67c8c-152">Relationship</span></span> | <span data-ttu-id="67c8c-153">型</span><span class="sxs-lookup"><span data-stu-id="67c8c-153">Type</span></span>   | <span data-ttu-id="67c8c-154">説明</span><span class="sxs-lookup"><span data-stu-id="67c8c-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="67c8c-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="67c8c-155">appDefinitions</span></span>|<span data-ttu-id="67c8c-156">[teamsAppDefinition](teamsappdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="67c8c-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="67c8c-157">アプリケーションの各バージョンの詳細です。</span><span class="sxs-lookup"><span data-stu-id="67c8c-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="67c8c-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67c8c-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="67c8c-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="67c8c-159">See also</span></span>

- [<span data-ttu-id="67c8c-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="67c8c-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="67c8c-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="67c8c-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="67c8c-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="67c8c-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


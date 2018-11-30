---
title: teamsApp リソースの種類
description: マイクロソフト チーム アプリケーション カタログのアプリケーションです。
ms.openlocfilehash: f8a96355c572287fc8bacc48f9a72e5da8d0f380
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022735"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="b12e7-103">teamsApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b12e7-103">teamsApp resource type</span></span>



<span data-ttu-id="b12e7-104">[マイクロソフト チーム](teams-api-overview.md)アプリケーション カタログのアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="b12e7-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="b12e7-105">マイクロソフト チーム ストア内のこれらのアプリケーションを表示して、[チーム](team.md)が[チームに追加のアプリケーション](../api/teamsappinstallation-add.md)のメソッドを使用してこれらのアプリケーションをインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="b12e7-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="b12e7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b12e7-106">Methods</span></span>

| <span data-ttu-id="b12e7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b12e7-107">Method</span></span>       | <span data-ttu-id="b12e7-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b12e7-108">Return Type</span></span>  |<span data-ttu-id="b12e7-109">説明</span><span class="sxs-lookup"><span data-stu-id="b12e7-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b12e7-110">公開されたアプリケーションの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="b12e7-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="b12e7-111">[teamsApp](teamsapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b12e7-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="b12e7-112">マイクロソフト チーム アプリケーション カタログから公開されているアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b12e7-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="b12e7-113">アプリケーションを発行します。</span><span class="sxs-lookup"><span data-stu-id="b12e7-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="b12e7-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b12e7-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="b12e7-115">組織のアプリケーションのカタログには、アプリケーションを発行します。</span><span class="sxs-lookup"><span data-stu-id="b12e7-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="b12e7-116">発行したアプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="b12e7-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="b12e7-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b12e7-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="b12e7-118">組織のアプリケーションのカタログに公開されたアプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="b12e7-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="b12e7-119">発行したアプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="b12e7-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="b12e7-120">なし</span><span class="sxs-lookup"><span data-stu-id="b12e7-120">None</span></span> | <span data-ttu-id="b12e7-121">発行したアプリケーションを組織のアプリケーションのカタログから削除します。</span><span class="sxs-lookup"><span data-stu-id="b12e7-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="b12e7-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b12e7-122">Properties</span></span>

| <span data-ttu-id="b12e7-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b12e7-123">Property</span></span>            | <span data-ttu-id="b12e7-124">型</span><span class="sxs-lookup"><span data-stu-id="b12e7-124">Type</span></span>     | <span data-ttu-id="b12e7-125">説明</span><span class="sxs-lookup"><span data-stu-id="b12e7-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="b12e7-126">ID</span><span class="sxs-lookup"><span data-stu-id="b12e7-126">id</span></span>                  | <span data-ttu-id="b12e7-127">文字列</span><span class="sxs-lookup"><span data-stu-id="b12e7-127">string</span></span>   | <span data-ttu-id="b12e7-128">カタログ アプリケーションの生成のアプリケーション ID を ([マイクロソフト チーム zip アプリケーション パッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)の開発者から提供された ID とは異なる。</span><span class="sxs-lookup"><span data-stu-id="b12e7-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="b12e7-129">externalId</span><span class="sxs-lookup"><span data-stu-id="b12e7-129">externalId</span></span>          | <span data-ttu-id="b12e7-130">文字列</span><span class="sxs-lookup"><span data-stu-id="b12e7-130">string</span></span>   | <span data-ttu-id="b12e7-131">アプリケーション開発者が、[マイクロソフトのチームは、アプリケーションのパッケージを zip](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)に用意されているカタログの ID です。</span><span class="sxs-lookup"><span data-stu-id="b12e7-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="b12e7-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b12e7-132">displayName</span></span>                | <span data-ttu-id="b12e7-133">string</span><span class="sxs-lookup"><span data-stu-id="b12e7-133">string</span></span>   | <span data-ttu-id="b12e7-134">アプリケーション開発者が、[マイクロソフトのチームは、アプリケーションのパッケージを zip](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)に用意されているカタログのアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="b12e7-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="b12e7-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="b12e7-135">distributionMethod</span></span>  | <span data-ttu-id="b12e7-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="b12e7-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="b12e7-137">アプリケーション配布の方法です。</span><span class="sxs-lookup"><span data-stu-id="b12e7-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="b12e7-138">teamsAppDistributionMethod 値</span><span class="sxs-lookup"><span data-stu-id="b12e7-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="b12e7-139">メンバー</span><span class="sxs-lookup"><span data-stu-id="b12e7-139">Member</span></span>|<span data-ttu-id="b12e7-140">値</span><span class="sxs-lookup"><span data-stu-id="b12e7-140">Value</span></span>|<span data-ttu-id="b12e7-141">説明</span><span class="sxs-lookup"><span data-stu-id="b12e7-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b12e7-142">ストア</span><span class="sxs-lookup"><span data-stu-id="b12e7-142">store</span></span>|<span data-ttu-id="b12e7-143">0</span><span class="sxs-lookup"><span data-stu-id="b12e7-143">0</span></span>| <span data-ttu-id="b12e7-144">アプリケーションは、マイクロソフトのチームのアプリケーション ストアからのすべてのテナントに使用できます。</span><span class="sxs-lookup"><span data-stu-id="b12e7-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="b12e7-145">組織</span><span class="sxs-lookup"><span data-stu-id="b12e7-145">organization</span></span>|<span data-ttu-id="b12e7-146">1</span><span class="sxs-lookup"><span data-stu-id="b12e7-146">1</span></span>|<span data-ttu-id="b12e7-147">アプリケーションは、このテナントでのみ使用可能です。</span><span class="sxs-lookup"><span data-stu-id="b12e7-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="b12e7-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="b12e7-148">sideloaded</span></span>|<span data-ttu-id="b12e7-149">2</span><span class="sxs-lookup"><span data-stu-id="b12e7-149">2</span></span>|<span data-ttu-id="b12e7-150">アプリケーションは、ユーザーまたはチームのみ使用可能です、インストールされているをします。</span><span class="sxs-lookup"><span data-stu-id="b12e7-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b12e7-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b12e7-151">Relationships</span></span>

| <span data-ttu-id="b12e7-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b12e7-152">Relationship</span></span> | <span data-ttu-id="b12e7-153">型</span><span class="sxs-lookup"><span data-stu-id="b12e7-153">Type</span></span>   | <span data-ttu-id="b12e7-154">説明</span><span class="sxs-lookup"><span data-stu-id="b12e7-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b12e7-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="b12e7-155">appDefinitions</span></span>|<span data-ttu-id="b12e7-156">[teamsAppDefinition](teamsappdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b12e7-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="b12e7-157">アプリケーションの各バージョンの詳細です。</span><span class="sxs-lookup"><span data-stu-id="b12e7-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b12e7-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b12e7-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="b12e7-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="b12e7-159">See also</span></span>

- [<span data-ttu-id="b12e7-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b12e7-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="b12e7-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="b12e7-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="b12e7-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="b12e7-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


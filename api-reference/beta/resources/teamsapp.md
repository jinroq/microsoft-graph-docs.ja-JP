---
title: teamsapp リソースの種類
description: Microsoft Teams アプリカタログのアプリ。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe60222ae6c5d8475722e18e69555df2d3892759
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553954"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="cc7b7-103">teamsapp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc7b7-103">teamsApp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc7b7-104">[Microsoft Teams](teams-api-overview.md)アプリカタログのアプリ。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="cc7b7-105">ユーザーは、これらのアプリを Microsoft teams ストアで表示できます。これらのアプリは、[[アプリをチームに追加する](../api/teamsappinstallation-add.md)] メソッドを使用して[Teams](team.md)にインストールできます。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="cc7b7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc7b7-106">Methods</span></span>

| <span data-ttu-id="cc7b7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc7b7-107">Method</span></span>       | <span data-ttu-id="cc7b7-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cc7b7-108">Return Type</span></span>  |<span data-ttu-id="cc7b7-109">説明</span><span class="sxs-lookup"><span data-stu-id="cc7b7-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc7b7-110">公開されたアプリの一覧を表示する</span><span class="sxs-lookup"><span data-stu-id="cc7b7-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="cc7b7-111">[teamsApp](teamsapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cc7b7-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="cc7b7-112">Microsoft Teams アプリカタログから、公開されたアプリを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="cc7b7-113">アプリを発行する</span><span class="sxs-lookup"><span data-stu-id="cc7b7-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="cc7b7-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cc7b7-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="cc7b7-115">組織のアプリカタログにアプリを発行します。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="cc7b7-116">公開されたアプリを更新する</span><span class="sxs-lookup"><span data-stu-id="cc7b7-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="cc7b7-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cc7b7-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="cc7b7-118">組織のアプリカタログで公開されているアプリを更新します。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="cc7b7-119">公開されたアプリを削除する</span><span class="sxs-lookup"><span data-stu-id="cc7b7-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="cc7b7-120">なし</span><span class="sxs-lookup"><span data-stu-id="cc7b7-120">None</span></span> | <span data-ttu-id="cc7b7-121">公開されたアプリを組織のアプリカタログから削除します。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc7b7-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc7b7-122">Properties</span></span>

| <span data-ttu-id="cc7b7-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc7b7-123">Property</span></span>            | <span data-ttu-id="cc7b7-124">型</span><span class="sxs-lookup"><span data-stu-id="cc7b7-124">Type</span></span>     | <span data-ttu-id="cc7b7-125">説明</span><span class="sxs-lookup"><span data-stu-id="cc7b7-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="cc7b7-126">id</span><span class="sxs-lookup"><span data-stu-id="cc7b7-126">id</span></span>                  | <span data-ttu-id="cc7b7-127">string</span><span class="sxs-lookup"><span data-stu-id="cc7b7-127">string</span></span>   | <span data-ttu-id="cc7b7-128">カタログアプリの生成されたアプリ id ( [Microsoft Teams zip アプリパッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)の開発者提供の id とは異なります)。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="cc7b7-129">externalId</span><span class="sxs-lookup"><span data-stu-id="cc7b7-129">externalId</span></span>          | <span data-ttu-id="cc7b7-130">string</span><span class="sxs-lookup"><span data-stu-id="cc7b7-130">string</span></span>   | <span data-ttu-id="cc7b7-131">[Microsoft Teams zip アプリパッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)のアプリ開発者によって提供されるカタログの ID。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="cc7b7-132">displayName</span><span class="sxs-lookup"><span data-stu-id="cc7b7-132">displayName</span></span>                | <span data-ttu-id="cc7b7-133">string</span><span class="sxs-lookup"><span data-stu-id="cc7b7-133">string</span></span>   | <span data-ttu-id="cc7b7-134">[Microsoft Teams zip アプリパッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)のアプリ開発者によって提供されるカタログアプリの名前です。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="cc7b7-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="cc7b7-135">distributionMethod</span></span>  | <span data-ttu-id="cc7b7-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="cc7b7-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="cc7b7-137">アプリの配布方法。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="cc7b7-138">teamsAppDistributionMethod の値</span><span class="sxs-lookup"><span data-stu-id="cc7b7-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="cc7b7-139">メンバー</span><span class="sxs-lookup"><span data-stu-id="cc7b7-139">Member</span></span>|<span data-ttu-id="cc7b7-140">値</span><span class="sxs-lookup"><span data-stu-id="cc7b7-140">Value</span></span>|<span data-ttu-id="cc7b7-141">説明</span><span class="sxs-lookup"><span data-stu-id="cc7b7-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc7b7-142">ストア</span><span class="sxs-lookup"><span data-stu-id="cc7b7-142">store</span></span>|<span data-ttu-id="cc7b7-143">.0</span><span class="sxs-lookup"><span data-stu-id="cc7b7-143">0</span></span>| <span data-ttu-id="cc7b7-144">アプリは、Microsoft Teams アプリストアを介してすべてのテナントで利用できます。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="cc7b7-145">組織</span><span class="sxs-lookup"><span data-stu-id="cc7b7-145">organization</span></span>|<span data-ttu-id="cc7b7-146">1 </span><span class="sxs-lookup"><span data-stu-id="cc7b7-146">1</span></span>|<span data-ttu-id="cc7b7-147">アプリはこのテナントでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="cc7b7-148">サイドロード</span><span class="sxs-lookup"><span data-stu-id="cc7b7-148">sideloaded</span></span>|<span data-ttu-id="cc7b7-149">2 </span><span class="sxs-lookup"><span data-stu-id="cc7b7-149">2</span></span>|<span data-ttu-id="cc7b7-150">アプリは、そのアプリがインストールされているユーザー/チームのみが利用できます。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc7b7-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc7b7-151">Relationships</span></span>

| <span data-ttu-id="cc7b7-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc7b7-152">Relationship</span></span> | <span data-ttu-id="cc7b7-153">型</span><span class="sxs-lookup"><span data-stu-id="cc7b7-153">Type</span></span>   | <span data-ttu-id="cc7b7-154">説明</span><span class="sxs-lookup"><span data-stu-id="cc7b7-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cc7b7-155">appdefinitions</span><span class="sxs-lookup"><span data-stu-id="cc7b7-155">appDefinitions</span></span>|<span data-ttu-id="cc7b7-156">[teamsAppDefinition](teamsappdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cc7b7-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="cc7b7-157">アプリの各バージョンの詳細。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cc7b7-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc7b7-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="cc7b7-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="cc7b7-159">See also</span></span>

- [<span data-ttu-id="cc7b7-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="cc7b7-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="cc7b7-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="cc7b7-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="cc7b7-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cc7b7-162">teamsTab</span></span>](../resources/teamstab.md)

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
    "Error: /api-reference/beta/resources/teamsapp.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->


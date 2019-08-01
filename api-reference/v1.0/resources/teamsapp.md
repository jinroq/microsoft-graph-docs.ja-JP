---
title: teamsApp リソースの種類
description: Microsoft Teams アプリカタログの一つ。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9cd1122a39fbe99e62c578486d863af8e13b96b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033811"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="7eb25-103">teamsApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7eb25-103">teamsApp resource type</span></span>



<span data-ttu-id="7eb25-104">[Microsoft Teams](teams-api-overview.md)アプリカタログの一つ。</span><span class="sxs-lookup"><span data-stu-id="7eb25-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="7eb25-105">ユーザーはMicrosoft Teams Storeでこれらのアプリを見ることができ、これらのアプリを[Teams へのアプリを追加](../api/teamsappinstallation-add.md)方法を使用して[teams](team.md) にインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="7eb25-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="7eb25-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7eb25-106">Methods</span></span>

| <span data-ttu-id="7eb25-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7eb25-107">Method</span></span>       | <span data-ttu-id="7eb25-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7eb25-108">Return Type</span></span>  |<span data-ttu-id="7eb25-109">説明</span><span class="sxs-lookup"><span data-stu-id="7eb25-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7eb25-110">公開アプリ をリストする</span><span class="sxs-lookup"><span data-stu-id="7eb25-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="7eb25-111">[teamsApp](teamsapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7eb25-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="7eb25-112">Microsoft Teams アプリ カタログから公開されたアプリの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="7eb25-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="7eb25-113">アプリを発行します。</span><span class="sxs-lookup"><span data-stu-id="7eb25-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="7eb25-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7eb25-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="7eb25-115">アプリを組織のアプリ カタログに発行します。</span><span class="sxs-lookup"><span data-stu-id="7eb25-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="7eb25-116">公開済みのアプリを更新します。</span><span class="sxs-lookup"><span data-stu-id="7eb25-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="7eb25-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7eb25-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="7eb25-118">組織のアプリ カタログに発行したアプリを更新します。</span><span class="sxs-lookup"><span data-stu-id="7eb25-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="7eb25-119">公開済みのアプリを削除します。</span><span class="sxs-lookup"><span data-stu-id="7eb25-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="7eb25-120">なし</span><span class="sxs-lookup"><span data-stu-id="7eb25-120">None</span></span> | <span data-ttu-id="7eb25-121">組織のアプリ カタログに発行したアプリを削除します。</span><span class="sxs-lookup"><span data-stu-id="7eb25-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="7eb25-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7eb25-122">Properties</span></span>

| <span data-ttu-id="7eb25-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7eb25-123">Property</span></span>            | <span data-ttu-id="7eb25-124">型</span><span class="sxs-lookup"><span data-stu-id="7eb25-124">Type</span></span>     | <span data-ttu-id="7eb25-125">説明</span><span class="sxs-lookup"><span data-stu-id="7eb25-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="7eb25-126">id</span><span class="sxs-lookup"><span data-stu-id="7eb25-126">id</span></span>                  | <span data-ttu-id="7eb25-127">string</span><span class="sxs-lookup"><span data-stu-id="7eb25-127">string</span></span>   | <span data-ttu-id="7eb25-128">カタログアプリによって生成されたアプリID（[Microsoft Teams zipアプリパッケージ](https://docs.microsoft.com/ja-JP/microsoftteams/platform/concepts/apps/apps-package)内の開発者提供のIDとは異なります）。</span><span class="sxs-lookup"><span data-stu-id="7eb25-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="7eb25-129">外部ID</span><span class="sxs-lookup"><span data-stu-id="7eb25-129">externalId</span></span>          | <span data-ttu-id="7eb25-130">文字列</span><span class="sxs-lookup"><span data-stu-id="7eb25-130">string</span></span>   | <span data-ttu-id="7eb25-131">アプリ開発者が[Microsoft Teams zipアプリパッケージ](https://docs.microsoft.com/ja-JP/microsoftteams/platform/concepts/apps/apps-package)で提供しているカタログのID。</span><span class="sxs-lookup"><span data-stu-id="7eb25-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="7eb25-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7eb25-132">displayName</span></span>                | <span data-ttu-id="7eb25-133">string</span><span class="sxs-lookup"><span data-stu-id="7eb25-133">string</span></span>   | <span data-ttu-id="7eb25-134">アプリ開発者が[Microsoft Teams zipアプリパッケージ](https://docs.microsoft.com/ja-JP/microsoftteams/platform/concepts/apps/apps-package)で提供しているカタログアプリの名前。</span><span class="sxs-lookup"><span data-stu-id="7eb25-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="7eb25-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="7eb25-135">distributionMethod</span></span>  | <span data-ttu-id="7eb25-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="7eb25-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="7eb25-137">アプリの配布の方法です。</span><span class="sxs-lookup"><span data-stu-id="7eb25-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="7eb25-138">teamsAppDistributionMethod 値</span><span class="sxs-lookup"><span data-stu-id="7eb25-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="7eb25-139">メンバー</span><span class="sxs-lookup"><span data-stu-id="7eb25-139">Member</span></span>|<span data-ttu-id="7eb25-140">値</span><span class="sxs-lookup"><span data-stu-id="7eb25-140">Value</span></span>|<span data-ttu-id="7eb25-141">説明</span><span class="sxs-lookup"><span data-stu-id="7eb25-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7eb25-142">店</span><span class="sxs-lookup"><span data-stu-id="7eb25-142">store</span></span>|<span data-ttu-id="7eb25-143">0</span><span class="sxs-lookup"><span data-stu-id="7eb25-143">0</span></span>| <span data-ttu-id="7eb25-144">このアプリは、Microsoft Teamsアプリストアを通じてすべてのテナントに利用可能です。</span><span class="sxs-lookup"><span data-stu-id="7eb25-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="7eb25-145">組織</span><span class="sxs-lookup"><span data-stu-id="7eb25-145">organization</span></span>|<span data-ttu-id="7eb25-146">1</span><span class="sxs-lookup"><span data-stu-id="7eb25-146">1</span></span>|<span data-ttu-id="7eb25-147">アプリは、このテナントでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="7eb25-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="7eb25-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="7eb25-148">sideloaded</span></span>|<span data-ttu-id="7eb25-149">2</span><span class="sxs-lookup"><span data-stu-id="7eb25-149">2</span></span>|<span data-ttu-id="7eb25-150">アプリはそれがインストールされているユーザー/チームにのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="7eb25-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7eb25-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7eb25-151">Relationships</span></span>

| <span data-ttu-id="7eb25-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7eb25-152">Relationship</span></span> | <span data-ttu-id="7eb25-153">型</span><span class="sxs-lookup"><span data-stu-id="7eb25-153">Type</span></span>   | <span data-ttu-id="7eb25-154">説明</span><span class="sxs-lookup"><span data-stu-id="7eb25-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7eb25-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="7eb25-155">appDefinitions</span></span>|<span data-ttu-id="7eb25-156">[teamsAppDefinition](teamsappdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7eb25-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="7eb25-157">アプリの各バージョンの詳細。</span><span class="sxs-lookup"><span data-stu-id="7eb25-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7eb25-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7eb25-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="7eb25-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="7eb25-159">See also</span></span>

- [<span data-ttu-id="7eb25-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7eb25-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="7eb25-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="7eb25-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="7eb25-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7eb25-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


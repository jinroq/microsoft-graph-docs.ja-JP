---
title: teamsApp リソースの種類
description: Microsoft Teams アプリカタログの一つ。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2686bddad3c70e60c764647d5bef453fd7524462
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345769"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="26e39-103">teamsApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26e39-103">teamsApp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26e39-104">[Microsoft Teams](teams-api-overview.md)アプリカタログの一つ。</span><span class="sxs-lookup"><span data-stu-id="26e39-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="26e39-105">ユーザーはMicrosoft Teams Storeでこれらのアプリを見ることができ、これらのアプリを[Teams へのアプリを追加](../api/teamsappinstallation-add.md)方法を使用して[teams](team.md) にインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="26e39-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="26e39-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="26e39-106">Methods</span></span>

| <span data-ttu-id="26e39-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="26e39-107">Method</span></span>       | <span data-ttu-id="26e39-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="26e39-108">Return Type</span></span>  |<span data-ttu-id="26e39-109">説明</span><span class="sxs-lookup"><span data-stu-id="26e39-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26e39-110">公開アプリ をリストする</span><span class="sxs-lookup"><span data-stu-id="26e39-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="26e39-111">[teamsApp](teamsapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="26e39-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="26e39-112">Microsoft Teams アプリ カタログから公開されたアプリの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="26e39-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="26e39-113">アプリを発行します。</span><span class="sxs-lookup"><span data-stu-id="26e39-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="26e39-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="26e39-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="26e39-115">アプリを組織のアプリ カタログに発行します。</span><span class="sxs-lookup"><span data-stu-id="26e39-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="26e39-116">公開済みのアプリを更新します。</span><span class="sxs-lookup"><span data-stu-id="26e39-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="26e39-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="26e39-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="26e39-118">組織のアプリ カタログに発行したアプリを更新します。</span><span class="sxs-lookup"><span data-stu-id="26e39-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="26e39-119">公開済みのアプリを削除します。</span><span class="sxs-lookup"><span data-stu-id="26e39-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="26e39-120">なし</span><span class="sxs-lookup"><span data-stu-id="26e39-120">None</span></span> | <span data-ttu-id="26e39-121">組織のアプリ カタログに発行したアプリを削除します。</span><span class="sxs-lookup"><span data-stu-id="26e39-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="26e39-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26e39-122">Properties</span></span>

| <span data-ttu-id="26e39-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26e39-123">Property</span></span>            | <span data-ttu-id="26e39-124">型</span><span class="sxs-lookup"><span data-stu-id="26e39-124">Type</span></span>     | <span data-ttu-id="26e39-125">説明</span><span class="sxs-lookup"><span data-stu-id="26e39-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="26e39-126">id</span><span class="sxs-lookup"><span data-stu-id="26e39-126">id</span></span>                  | <span data-ttu-id="26e39-127">string</span><span class="sxs-lookup"><span data-stu-id="26e39-127">string</span></span>   | <span data-ttu-id="26e39-128">カタログアプリによって生成されたアプリID（[Microsoft Teams zipアプリパッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)内の開発者提供のIDとは異なります）。</span><span class="sxs-lookup"><span data-stu-id="26e39-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="26e39-129">外部ID</span><span class="sxs-lookup"><span data-stu-id="26e39-129">externalId</span></span>          | <span data-ttu-id="26e39-130">文字列</span><span class="sxs-lookup"><span data-stu-id="26e39-130">string</span></span>   | <span data-ttu-id="26e39-131">アプリ開発者が[Microsoft Teams zipアプリパッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)で提供しているカタログのID。</span><span class="sxs-lookup"><span data-stu-id="26e39-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="26e39-132">displayName</span><span class="sxs-lookup"><span data-stu-id="26e39-132">displayName</span></span>                | <span data-ttu-id="26e39-133">string</span><span class="sxs-lookup"><span data-stu-id="26e39-133">string</span></span>   | <span data-ttu-id="26e39-134">アプリ開発者が[Microsoft Teams zipアプリパッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)で提供しているカタログアプリの名前。</span><span class="sxs-lookup"><span data-stu-id="26e39-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="26e39-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="26e39-135">distributionMethod</span></span>  | <span data-ttu-id="26e39-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="26e39-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="26e39-137">アプリの配布の方法です。</span><span class="sxs-lookup"><span data-stu-id="26e39-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="26e39-138">teamsAppDistributionMethod 値</span><span class="sxs-lookup"><span data-stu-id="26e39-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="26e39-139">メンバー</span><span class="sxs-lookup"><span data-stu-id="26e39-139">Member</span></span>|<span data-ttu-id="26e39-140">値</span><span class="sxs-lookup"><span data-stu-id="26e39-140">Value</span></span>|<span data-ttu-id="26e39-141">説明</span><span class="sxs-lookup"><span data-stu-id="26e39-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e39-142">店</span><span class="sxs-lookup"><span data-stu-id="26e39-142">store</span></span>|<span data-ttu-id="26e39-143">0</span><span class="sxs-lookup"><span data-stu-id="26e39-143">0</span></span>| <span data-ttu-id="26e39-144">このアプリは、Microsoft Teamsアプリストアを通じてすべてのテナントに利用可能です。</span><span class="sxs-lookup"><span data-stu-id="26e39-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="26e39-145">組織</span><span class="sxs-lookup"><span data-stu-id="26e39-145">organization</span></span>|<span data-ttu-id="26e39-146">1</span><span class="sxs-lookup"><span data-stu-id="26e39-146">1</span></span>|<span data-ttu-id="26e39-147">アプリは、このテナントでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="26e39-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="26e39-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="26e39-148">sideloaded</span></span>|<span data-ttu-id="26e39-149">2</span><span class="sxs-lookup"><span data-stu-id="26e39-149">2</span></span>|<span data-ttu-id="26e39-150">アプリはそれがインストールされているユーザー/チームにのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="26e39-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26e39-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="26e39-151">Relationships</span></span>

| <span data-ttu-id="26e39-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="26e39-152">Relationship</span></span> | <span data-ttu-id="26e39-153">型</span><span class="sxs-lookup"><span data-stu-id="26e39-153">Type</span></span>   | <span data-ttu-id="26e39-154">説明</span><span class="sxs-lookup"><span data-stu-id="26e39-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="26e39-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="26e39-155">appDefinitions</span></span>|<span data-ttu-id="26e39-156">[teamsAppDefinition](teamsappdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="26e39-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="26e39-157">アプリの各バージョンの詳細。</span><span class="sxs-lookup"><span data-stu-id="26e39-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="26e39-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26e39-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="26e39-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="26e39-159">See also</span></span>

- [<span data-ttu-id="26e39-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="26e39-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="26e39-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="26e39-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="26e39-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="26e39-162">teamsTab</span></span>](../resources/teamstab.md)

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


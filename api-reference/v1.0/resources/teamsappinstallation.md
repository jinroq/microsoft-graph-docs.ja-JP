---
title: teamsAppInstallation リソースの種類
description: 'チームにインストールされている teamsapp。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c98f1b927c319eb1d81573fd9dc43e1baad86a39
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462355"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="df409-103">teamsAppInstallation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="df409-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df409-104">[チーム](team.md)にインストールされている[teamsapp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="df409-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="df409-105">アプリの一部である bot は、アプリが追加されるチームの一部になります。</span><span class="sxs-lookup"><span data-stu-id="df409-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="df409-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="df409-106">Methods</span></span>

| <span data-ttu-id="df409-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="df409-107">Method</span></span>       | <span data-ttu-id="df409-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="df409-108">Return Type</span></span>  |<span data-ttu-id="df409-109">説明</span><span class="sxs-lookup"><span data-stu-id="df409-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="df409-110">アプリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="df409-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="df409-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="df409-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="df409-112">チームにインストールされているアプリを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="df409-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="df409-113">アプリの追加</span><span class="sxs-lookup"><span data-stu-id="df409-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="df409-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="df409-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="df409-115">アプリをチームに追加 (インストール) します。</span><span class="sxs-lookup"><span data-stu-id="df409-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="df409-116">アプリの削除</span><span class="sxs-lookup"><span data-stu-id="df409-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="df409-117">なし</span><span class="sxs-lookup"><span data-stu-id="df409-117">None</span></span> | <span data-ttu-id="df409-118">チームからアプリを削除 (アンインストール) します。</span><span class="sxs-lookup"><span data-stu-id="df409-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="df409-119">アプリをアップグレードする</span><span class="sxs-lookup"><span data-stu-id="df409-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="df409-120">なし</span><span class="sxs-lookup"><span data-stu-id="df409-120">None</span></span> | <span data-ttu-id="df409-121">最新バージョンのアプリにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="df409-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="df409-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df409-122">Properties</span></span>

| <span data-ttu-id="df409-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df409-123">Property</span></span>            | <span data-ttu-id="df409-124">型</span><span class="sxs-lookup"><span data-stu-id="df409-124">Type</span></span>     | <span data-ttu-id="df409-125">説明</span><span class="sxs-lookup"><span data-stu-id="df409-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="df409-126">ID</span><span class="sxs-lookup"><span data-stu-id="df409-126">id</span></span>                  | <span data-ttu-id="df409-127">string</span><span class="sxs-lookup"><span data-stu-id="df409-127">string</span></span>   | <span data-ttu-id="df409-128">一意の id (teams appid ではない)。</span><span class="sxs-lookup"><span data-stu-id="df409-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="df409-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="df409-129">Relationships</span></span>

| <span data-ttu-id="df409-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="df409-130">Relationship</span></span>   | <span data-ttu-id="df409-131">型</span><span class="sxs-lookup"><span data-stu-id="df409-131">Type</span></span>    | <span data-ttu-id="df409-132">説明</span><span class="sxs-lookup"><span data-stu-id="df409-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="df409-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="df409-133">teamsApp</span></span>|[<span data-ttu-id="df409-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="df409-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="df409-135">インストールされているアプリ。</span><span class="sxs-lookup"><span data-stu-id="df409-135">The app that is installed.</span></span> |
|<span data-ttu-id="df409-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="df409-136">teamsAppDefinition</span></span>|[<span data-ttu-id="df409-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="df409-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="df409-138">このバージョンのアプリの詳細。</span><span class="sxs-lookup"><span data-stu-id="df409-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="df409-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="df409-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="df409-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="df409-140">See also</span></span>

- [<span data-ttu-id="df409-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="df409-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="df409-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="df409-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="df409-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="df409-143">teamsTab</span></span>](../resources/teamstab.md)


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
    "Error: /api-reference/beta/resources/teamsappinstallation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->


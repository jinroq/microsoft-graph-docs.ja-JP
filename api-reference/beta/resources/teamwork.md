---
title: teamwork リソースの種類
description: 組織で使用可能な Microsoft Teams の機能のコンテナー。
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7a72e34fc3d9d02a36e34295f7d4469536506df3
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908594"
---
# <a name="teamwork-resource-type"></a><span data-ttu-id="1fa73-103">teamwork リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1fa73-103">teamwork resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fa73-104">組織で使用可能な Microsoft Teams の機能の範囲のコンテナー。</span><span class="sxs-lookup"><span data-stu-id="1fa73-104">A container for the range of Microsoft Teams functionalities that are available for the organization.</span></span>

## <a name="properties"></a><span data-ttu-id="1fa73-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1fa73-105">Properties</span></span>

| <span data-ttu-id="1fa73-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1fa73-106">Property</span></span> | <span data-ttu-id="1fa73-107">型</span><span class="sxs-lookup"><span data-stu-id="1fa73-107">Type</span></span> | <span data-ttu-id="1fa73-108">説明</span><span class="sxs-lookup"><span data-stu-id="1fa73-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1fa73-109">id</span><span class="sxs-lookup"><span data-stu-id="1fa73-109">id</span></span>|<span data-ttu-id="1fa73-110">string</span><span class="sxs-lookup"><span data-stu-id="1fa73-110">string</span></span>| <span data-ttu-id="1fa73-111">一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1fa73-111">A globally unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1fa73-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1fa73-112">Relationships</span></span>

| <span data-ttu-id="1fa73-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1fa73-113">Relationship</span></span> | <span data-ttu-id="1fa73-114">型</span><span class="sxs-lookup"><span data-stu-id="1fa73-114">Type</span></span> | <span data-ttu-id="1fa73-115">説明</span><span class="sxs-lookup"><span data-stu-id="1fa73-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1fa73-116">installedApps</span><span class="sxs-lookup"><span data-stu-id="1fa73-116">installedApps</span></span>|<span data-ttu-id="1fa73-117">[teamsAppInstallation](teamsappinstallation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1fa73-117">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="1fa73-118">このユーザーのパーソナル スコープ内にインストールされているアプリ。</span><span class="sxs-lookup"><span data-stu-id="1fa73-118">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fa73-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1fa73-119">JSON representation</span></span>

<span data-ttu-id="1fa73-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1fa73-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="1fa73-121">関連項目</span><span class="sxs-lookup"><span data-stu-id="1fa73-121">See Also</span></span>

- [<span data-ttu-id="1fa73-122">userTeamwork リソース</span><span class="sxs-lookup"><span data-stu-id="1fa73-122">userTeamwork resource</span></span>](userteamwork.md)

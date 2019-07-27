---
title: userTeamwork リソースの種類
description: 'ユーザー 1 人あたりの使用可能な Microsoft Teams の機能のコンテナ―。 '
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d68ceff79856b23f2d86b2c57a6278b7c6ad7e9d
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908587"
---
# <a name="userteamwork-resource-type"></a><span data-ttu-id="fd780-103">userTeamwork リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd780-103">userTeamwork resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd780-104">テナント内のユーザー 1 人あたりの使用可能な Microsoft Teams の機能の範囲のコンテナー。</span><span class="sxs-lookup"><span data-stu-id="fd780-104">A container for the range of Microsoft Teams functionalities that are available per user in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="fd780-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd780-105">Properties</span></span>

| <span data-ttu-id="fd780-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd780-106">Property</span></span> | <span data-ttu-id="fd780-107">型</span><span class="sxs-lookup"><span data-stu-id="fd780-107">Type</span></span> | <span data-ttu-id="fd780-108">説明</span><span class="sxs-lookup"><span data-stu-id="fd780-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fd780-109">id</span><span class="sxs-lookup"><span data-stu-id="fd780-109">id</span></span>|<span data-ttu-id="fd780-110">string</span><span class="sxs-lookup"><span data-stu-id="fd780-110">string</span></span>| <span data-ttu-id="fd780-111">一意識別子。</span><span class="sxs-lookup"><span data-stu-id="fd780-111">A globally unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fd780-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fd780-112">Relationships</span></span>

| <span data-ttu-id="fd780-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fd780-113">Relationship</span></span> | <span data-ttu-id="fd780-114">型</span><span class="sxs-lookup"><span data-stu-id="fd780-114">Type</span></span> | <span data-ttu-id="fd780-115">説明</span><span class="sxs-lookup"><span data-stu-id="fd780-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fd780-116">installedApps</span><span class="sxs-lookup"><span data-stu-id="fd780-116">installedApps</span></span>|<span data-ttu-id="fd780-117">[teamsAppInstallation](teamsappinstallation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fd780-117">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="fd780-118">このユーザーのパーソナル スコープ内にインストールされているアプリ。</span><span class="sxs-lookup"><span data-stu-id="fd780-118">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd780-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd780-119">JSON representation</span></span>

<span data-ttu-id="fd780-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd780-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTeamwork",
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
  "description": "userteamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

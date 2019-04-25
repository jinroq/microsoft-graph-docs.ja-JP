---
title: teamguestsettings リソースの種類
description: ゲストがチームでチャネルを作成、更新、削除できるかどうかを構成する設定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: cb6e83093945a96784bfb91a76bc343a8c13d0ac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548454"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="98e58-103">teamguestsettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="98e58-103">teamGuestSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98e58-104">ゲストが[チーム](team.md)内でチャネルを作成、更新、または削除できるかどうかを構成するための設定。</span><span class="sxs-lookup"><span data-stu-id="98e58-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="98e58-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98e58-105">Properties</span></span>
| <span data-ttu-id="98e58-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98e58-106">Property</span></span>     | <span data-ttu-id="98e58-107">型</span><span class="sxs-lookup"><span data-stu-id="98e58-107">Type</span></span>   |<span data-ttu-id="98e58-108">説明</span><span class="sxs-lookup"><span data-stu-id="98e58-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98e58-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="98e58-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="98e58-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="98e58-110">Boolean</span></span>|<span data-ttu-id="98e58-111">true に設定すると、ゲストはチャネルを追加および更新できるようになります。</span><span class="sxs-lookup"><span data-stu-id="98e58-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="98e58-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="98e58-112">allowDeleteChannels</span></span>|<span data-ttu-id="98e58-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="98e58-113">Boolean</span></span>|<span data-ttu-id="98e58-114">true に設定されている場合、ゲストはチャネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="98e58-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98e58-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="98e58-115">JSON representation</span></span>

<span data-ttu-id="98e58-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="98e58-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamguestsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

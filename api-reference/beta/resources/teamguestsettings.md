---
title: teamGuestSettings リソースの種類
description: 来園者が作成、更新、またはチーム内のチャンネルを削除するかどうかを構成するのに設定します。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 4d76ffcbc5ec675ee670394854183c07721c0af9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522309"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="5cb15-103">teamGuestSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5cb15-103">teamGuestSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cb15-104">来園者が作成、更新、または[チーム](team.md)内のチャンネルを削除するかどうかを構成するのに設定します。</span><span class="sxs-lookup"><span data-stu-id="5cb15-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5cb15-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5cb15-105">Properties</span></span>
| <span data-ttu-id="5cb15-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5cb15-106">Property</span></span>     | <span data-ttu-id="5cb15-107">型</span><span class="sxs-lookup"><span data-stu-id="5cb15-107">Type</span></span>   |<span data-ttu-id="5cb15-108">説明</span><span class="sxs-lookup"><span data-stu-id="5cb15-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cb15-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="5cb15-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="5cb15-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="5cb15-110">Boolean</span></span>|<span data-ttu-id="5cb15-111">True の場合、来園者のセットを追加したりチャンネルを更新する場合。</span><span class="sxs-lookup"><span data-stu-id="5cb15-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="5cb15-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="5cb15-112">allowDeleteChannels</span></span>|<span data-ttu-id="5cb15-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="5cb15-113">Boolean</span></span>|<span data-ttu-id="5cb15-114">場合は true を指定すると、来園者に設定するには、チャンネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="5cb15-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5cb15-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5cb15-115">JSON representation</span></span>

<span data-ttu-id="5cb15-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5cb15-116">The following is a JSON representation of the resource.</span></span>

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

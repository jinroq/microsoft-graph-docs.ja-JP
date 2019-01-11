---
title: teamGuestSettings リソースの種類
description: 来園者が作成、更新、またはチーム内のチャンネルを削除するかどうかを構成するのに設定します。
localization_priority: Normal
ms.openlocfilehash: f0947101fc8de83d1a56ffa922d9b1e2d79d520f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844878"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="508d0-103">teamGuestSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="508d0-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="508d0-104">来園者が作成、更新、または[チーム](team.md)内のチャンネルを削除するかどうかを構成するのに設定します。</span><span class="sxs-lookup"><span data-stu-id="508d0-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="508d0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="508d0-105">Properties</span></span>
| <span data-ttu-id="508d0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="508d0-106">Property</span></span>     | <span data-ttu-id="508d0-107">種類</span><span class="sxs-lookup"><span data-stu-id="508d0-107">Type</span></span>   |<span data-ttu-id="508d0-108">説明</span><span class="sxs-lookup"><span data-stu-id="508d0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="508d0-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="508d0-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="508d0-110">ブール型</span><span class="sxs-lookup"><span data-stu-id="508d0-110">Boolean</span></span>|<span data-ttu-id="508d0-111">True の場合、来園者のセットを追加したりチャンネルを更新する場合。</span><span class="sxs-lookup"><span data-stu-id="508d0-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="508d0-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="508d0-112">allowDeleteChannels</span></span>|<span data-ttu-id="508d0-113">ブール型</span><span class="sxs-lookup"><span data-stu-id="508d0-113">Boolean</span></span>|<span data-ttu-id="508d0-114">場合は true を指定すると、来園者に設定するには、チャンネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="508d0-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="508d0-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="508d0-115">JSON representation</span></span>

<span data-ttu-id="508d0-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="508d0-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

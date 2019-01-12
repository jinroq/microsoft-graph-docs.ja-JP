---
title: teamGuestSettings リソースの種類
description: 来園者が作成、更新、またはチーム内のチャンネルを削除するかどうかを構成するのに設定します。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: cb6e83093945a96784bfb91a76bc343a8c13d0ac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924371"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="3beb4-103">teamGuestSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3beb4-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="3beb4-104">来園者が作成、更新、または[チーム](team.md)内のチャンネルを削除するかどうかを構成するのに設定します。</span><span class="sxs-lookup"><span data-stu-id="3beb4-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3beb4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3beb4-105">Properties</span></span>
| <span data-ttu-id="3beb4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3beb4-106">Property</span></span>     | <span data-ttu-id="3beb4-107">種類</span><span class="sxs-lookup"><span data-stu-id="3beb4-107">Type</span></span>   |<span data-ttu-id="3beb4-108">説明</span><span class="sxs-lookup"><span data-stu-id="3beb4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3beb4-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="3beb4-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="3beb4-110">ブール型</span><span class="sxs-lookup"><span data-stu-id="3beb4-110">Boolean</span></span>|<span data-ttu-id="3beb4-111">True の場合、来園者のセットを追加したりチャンネルを更新する場合。</span><span class="sxs-lookup"><span data-stu-id="3beb4-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="3beb4-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="3beb4-112">allowDeleteChannels</span></span>|<span data-ttu-id="3beb4-113">ブール型</span><span class="sxs-lookup"><span data-stu-id="3beb4-113">Boolean</span></span>|<span data-ttu-id="3beb4-114">場合は true を指定すると、来園者に設定するには、チャンネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="3beb4-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3beb4-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3beb4-115">JSON representation</span></span>

<span data-ttu-id="3beb4-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3beb4-116">The following is a JSON representation of the resource.</span></span>

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

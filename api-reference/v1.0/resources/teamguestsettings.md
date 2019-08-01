---
title: teamGuestSettings リソースの種類
description: ゲストがチームでチャネルを作成、更新、削除できるかどうかを構成する設定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7c5cc116567b0ee2db1b2dd5e28c4749d7c6772c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033867"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="57603-103">teamGuestSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="57603-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="57603-104">ゲストが[チーム](team.md)内でチャネルを作成、更新、または削除できるかどうかを構成するための設定。</span><span class="sxs-lookup"><span data-stu-id="57603-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="57603-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57603-105">Properties</span></span>
| <span data-ttu-id="57603-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57603-106">Property</span></span>     | <span data-ttu-id="57603-107">型</span><span class="sxs-lookup"><span data-stu-id="57603-107">Type</span></span>   |<span data-ttu-id="57603-108">説明</span><span class="sxs-lookup"><span data-stu-id="57603-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57603-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="57603-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="57603-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="57603-110">Boolean</span></span>|<span data-ttu-id="57603-111">True に設定すると、ゲストはチャネルを追加および更新できるようになります。</span><span class="sxs-lookup"><span data-stu-id="57603-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="57603-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="57603-112">allowDeleteChannels</span></span>|<span data-ttu-id="57603-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="57603-113">Boolean</span></span>|<span data-ttu-id="57603-114">True に設定されている場合、ゲストはチャネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="57603-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57603-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="57603-115">JSON representation</span></span>

<span data-ttu-id="57603-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="57603-116">The following is a JSON representation of the resource.</span></span>

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

---
title: teamMemberSettings リソースの種類
description: など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、チームにボットを追加します。
ms.openlocfilehash: 74d88e1d87c65745fe98da9b1ee21b26824dc4e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022960"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="410fc-103">teamMemberSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="410fc-103">teamMemberSettings resource type</span></span>



<span data-ttu-id="410fc-104">など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、[チーム](team.md)にボットを追加します。</span><span class="sxs-lookup"><span data-stu-id="410fc-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="410fc-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="410fc-105">Properties</span></span>
| <span data-ttu-id="410fc-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="410fc-106">Property</span></span>     | <span data-ttu-id="410fc-107">型</span><span class="sxs-lookup"><span data-stu-id="410fc-107">Type</span></span>   |<span data-ttu-id="410fc-108">説明</span><span class="sxs-lookup"><span data-stu-id="410fc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="410fc-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="410fc-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="410fc-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="410fc-110">Boolean</span></span>|<span data-ttu-id="410fc-111">True の場合、メンバー セットを追加したりチャンネルを更新する場合。</span><span class="sxs-lookup"><span data-stu-id="410fc-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="410fc-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="410fc-112">allowDeleteChannels</span></span>|<span data-ttu-id="410fc-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="410fc-113">Boolean</span></span>|<span data-ttu-id="410fc-114">場合は true の場合、メンバーに設定するには、チャンネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="410fc-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="410fc-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="410fc-115">allowAddRemoveApps</span></span>|<span data-ttu-id="410fc-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="410fc-116">Boolean</span></span>|<span data-ttu-id="410fc-117">場合は true の場合、メンバー セットは、追加し、アプリケーションを削除できます。</span><span class="sxs-lookup"><span data-stu-id="410fc-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="410fc-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="410fc-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="410fc-119">ブール値</span><span class="sxs-lookup"><span data-stu-id="410fc-119">Boolean</span></span>|<span data-ttu-id="410fc-120">場合は true の場合、メンバー セットを追加、更新、およびタブを削除します。</span><span class="sxs-lookup"><span data-stu-id="410fc-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="410fc-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="410fc-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="410fc-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="410fc-122">Boolean</span></span>|<span data-ttu-id="410fc-123">場合は true の場合、メンバー セットを追加、更新、およびコネクタを削除します。</span><span class="sxs-lookup"><span data-stu-id="410fc-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="410fc-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="410fc-124">JSON representation</span></span>

<span data-ttu-id="410fc-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="410fc-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

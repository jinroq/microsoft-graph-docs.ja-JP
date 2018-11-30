---
title: teamGuestSettings リソースの種類
description: 来園者が作成、更新、またはチーム内のチャンネルを削除するかどうかを構成するのに設定します。
ms.openlocfilehash: 744e19165121d101a720a86bec0242fc31137768
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070149"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="1cf68-103">teamGuestSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1cf68-103">teamGuestSettings resource type</span></span>

> <span data-ttu-id="1cf68-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1cf68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cf68-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1cf68-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1cf68-106">来園者が作成、更新、または[チーム](team.md)内のチャンネルを削除するかどうかを構成するのに設定します。</span><span class="sxs-lookup"><span data-stu-id="1cf68-106">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1cf68-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1cf68-107">Properties</span></span>
| <span data-ttu-id="1cf68-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1cf68-108">Property</span></span>     | <span data-ttu-id="1cf68-109">型</span><span class="sxs-lookup"><span data-stu-id="1cf68-109">Type</span></span>   |<span data-ttu-id="1cf68-110">説明</span><span class="sxs-lookup"><span data-stu-id="1cf68-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cf68-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="1cf68-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="1cf68-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="1cf68-112">Boolean</span></span>|<span data-ttu-id="1cf68-113">True の場合、来園者のセットを追加したりチャンネルを更新する場合。</span><span class="sxs-lookup"><span data-stu-id="1cf68-113">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="1cf68-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="1cf68-114">allowDeleteChannels</span></span>|<span data-ttu-id="1cf68-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="1cf68-115">Boolean</span></span>|<span data-ttu-id="1cf68-116">場合は true を指定すると、来園者に設定するには、チャンネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="1cf68-116">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1cf68-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1cf68-117">JSON representation</span></span>

<span data-ttu-id="1cf68-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1cf68-118">The following is a JSON representation of the resource.</span></span>

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

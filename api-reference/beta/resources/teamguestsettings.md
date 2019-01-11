---
title: teamGuestSettings リソースの種類
description: 来園者が作成、更新、またはチーム内のチャンネルを削除するかどうかを構成するのに設定します。
localization_priority: Normal
ms.openlocfilehash: 15644f3761329589a4d770e777ae5fd63751e6be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851542"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="ebd6e-103">teamGuestSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ebd6e-103">teamGuestSettings resource type</span></span>

> <span data-ttu-id="ebd6e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ebd6e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebd6e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebd6e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebd6e-106">来園者が作成、更新、または[チーム](team.md)内のチャンネルを削除するかどうかを構成するのに設定します。</span><span class="sxs-lookup"><span data-stu-id="ebd6e-106">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ebd6e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebd6e-107">Properties</span></span>
| <span data-ttu-id="ebd6e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebd6e-108">Property</span></span>     | <span data-ttu-id="ebd6e-109">種類</span><span class="sxs-lookup"><span data-stu-id="ebd6e-109">Type</span></span>   |<span data-ttu-id="ebd6e-110">説明</span><span class="sxs-lookup"><span data-stu-id="ebd6e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebd6e-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="ebd6e-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="ebd6e-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="ebd6e-112">Boolean</span></span>|<span data-ttu-id="ebd6e-113">True の場合、来園者のセットを追加したりチャンネルを更新する場合。</span><span class="sxs-lookup"><span data-stu-id="ebd6e-113">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="ebd6e-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="ebd6e-114">allowDeleteChannels</span></span>|<span data-ttu-id="ebd6e-115">ブール型</span><span class="sxs-lookup"><span data-stu-id="ebd6e-115">Boolean</span></span>|<span data-ttu-id="ebd6e-116">場合は true を指定すると、来園者に設定するには、チャンネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="ebd6e-116">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebd6e-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ebd6e-117">JSON representation</span></span>

<span data-ttu-id="ebd6e-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ebd6e-118">The following is a JSON representation of the resource.</span></span>

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

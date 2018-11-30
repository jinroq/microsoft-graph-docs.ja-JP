---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
ms.openlocfilehash: c9f06c7a4a6351b8a6554c944c0efe9af379e030
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070650"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="332ec-102">ShareAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="332ec-102">ShareAction resource type</span></span>

> <span data-ttu-id="332ec-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="332ec-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="332ec-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="332ec-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="332ec-105">**ShareAction** リソースは、アイテムを共有した[アクティビティ][activity]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="332ec-105">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="332ec-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="332ec-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="332ec-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="332ec-107">Properties</span></span>

| <span data-ttu-id="332ec-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="332ec-108">Property name</span></span> | <span data-ttu-id="332ec-109">型</span><span class="sxs-lookup"><span data-stu-id="332ec-109">Type</span></span>                       | <span data-ttu-id="332ec-110">説明</span><span class="sxs-lookup"><span data-stu-id="332ec-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="332ec-111">recipients</span><span class="sxs-lookup"><span data-stu-id="332ec-111">recipients</span></span>    | <span data-ttu-id="332ec-112">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="332ec-112">[identitySet][] collection</span></span> | <span data-ttu-id="332ec-113">このアクションでアイテムが共有された相手の ID。</span><span class="sxs-lookup"><span data-stu-id="332ec-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="332ec-115">備考</span><span class="sxs-lookup"><span data-stu-id="332ec-115">Remarks</span></span>

<span data-ttu-id="332ec-116">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="332ec-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction"
} -->
---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: b1570fc0ec0a6e28bab569dfae6992675d8b3537
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333661"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="c4833-102">id セットリソースの種類</span><span class="sxs-lookup"><span data-stu-id="c4833-102">identitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4833-103">identity **set**リソースは、 [id](identity.md)リソースのキー付きコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c4833-103">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>

<span data-ttu-id="c4833-104">_作成者_または_最終更新者_など、アイテムのさまざまなイベントに関連付けられている id のセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="c4833-104">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4833-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4833-105">JSON representation</span></span>

<span data-ttu-id="c4833-106">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c4833-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
    "conversation",
    "conversationIdentityType",
    "device",
    "encrypted",
    "guest",
    "phone",
    "user"
  ],
  "openType": true
} -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "microsoft.graph.identity"},
  "conversation": {"@odata.type": "microsoft.graph.identity"},
  "conversationIdentityType": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "encrypted": {"@odata.type": "microsoft.graph.identity"},
  "guest": {"@odata.type": "microsoft.graph.identity"},
  "phone": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="c4833-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4833-107">Properties</span></span>

| <span data-ttu-id="c4833-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4833-108">Property</span></span>    | <span data-ttu-id="c4833-109">型</span><span class="sxs-lookup"><span data-stu-id="c4833-109">Type</span></span>                    | <span data-ttu-id="c4833-110">説明</span><span class="sxs-lookup"><span data-stu-id="c4833-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="c4833-111">application</span><span class="sxs-lookup"><span data-stu-id="c4833-111">application</span></span> | [<span data-ttu-id="c4833-112">ID</span><span class="sxs-lookup"><span data-stu-id="c4833-112">Identity</span></span>](identity.md) | <span data-ttu-id="c4833-p101">省略可能。このアクションに関連付けられているアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="c4833-p101">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="c4833-115">conversation</span><span class="sxs-lookup"><span data-stu-id="c4833-115">conversation</span></span>| [<span data-ttu-id="c4833-116">Identity</span><span class="sxs-lookup"><span data-stu-id="c4833-116">Identity</span></span>](identity.md) | <span data-ttu-id="c4833-117">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c4833-117">Optional.</span></span> <span data-ttu-id="c4833-118">このアクションに関連付けられているチームまたはチャネル。</span><span class="sxs-lookup"><span data-stu-id="c4833-118">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="c4833-119">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="c4833-119">conversationIdentityType</span></span>| [<span data-ttu-id="c4833-120">Identity</span><span class="sxs-lookup"><span data-stu-id="c4833-120">Identity</span></span>](identity.md) | <span data-ttu-id="c4833-121">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c4833-121">Optional.</span></span> <span data-ttu-id="c4833-122">**会話**プロパティがチームまたはチャネルを識別するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c4833-122">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="c4833-123">デバイス</span><span class="sxs-lookup"><span data-stu-id="c4833-123">device</span></span>      | [<span data-ttu-id="c4833-124">ID</span><span class="sxs-lookup"><span data-stu-id="c4833-124">Identity</span></span>](identity.md) | <span data-ttu-id="c4833-p104">省略可能。このアクションに関連付けられているデバイス。</span><span class="sxs-lookup"><span data-stu-id="c4833-p104">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="c4833-127">phone</span><span class="sxs-lookup"><span data-stu-id="c4833-127">phone</span></span>       | [<span data-ttu-id="c4833-128">identity</span><span class="sxs-lookup"><span data-stu-id="c4833-128">identity</span></span>](identity.md) | <span data-ttu-id="c4833-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c4833-129">Optional.</span></span> <span data-ttu-id="c4833-130">このアクションに関連付けられている電話番号。</span><span class="sxs-lookup"><span data-stu-id="c4833-130">The phone number associated with this action.</span></span> |
| <span data-ttu-id="c4833-131">user</span><span class="sxs-lookup"><span data-stu-id="c4833-131">user</span></span>        | [<span data-ttu-id="c4833-132">Identity</span><span class="sxs-lookup"><span data-stu-id="c4833-132">Identity</span></span>](identity.md) | <span data-ttu-id="c4833-p106">省略可能。このアクションに関連付けられているユーザー。</span><span class="sxs-lookup"><span data-stu-id="c4833-p106">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="c4833-135">注釈</span><span class="sxs-lookup"><span data-stu-id="c4833-135">Remarks</span></span> 

<span data-ttu-id="c4833-136">「[呼び出し](call.md)を使用したリソースの**設定**」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4833-136">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->

---
author: JeremyKelley
description: Identity Set リソースは、id リソースのキー付きコレクションです。
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c43981c1f7e79567afe901217030a0b5abed6f53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006291"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="55456-103">id セットリソースの種類</span><span class="sxs-lookup"><span data-stu-id="55456-103">identitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55456-104">Identity **set**リソースは、 [id](identity.md)リソースのキー付きコレクションです。</span><span class="sxs-lookup"><span data-stu-id="55456-104">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>

<span data-ttu-id="55456-105">_作成者_または_最終更新者_など、アイテムのさまざまなイベントに関連付けられている id のセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="55456-105">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="55456-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55456-106">JSON representation</span></span>

<span data-ttu-id="55456-107">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="55456-107">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="55456-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55456-108">Properties</span></span>

| <span data-ttu-id="55456-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55456-109">Property</span></span>    | <span data-ttu-id="55456-110">型</span><span class="sxs-lookup"><span data-stu-id="55456-110">Type</span></span>                    | <span data-ttu-id="55456-111">説明</span><span class="sxs-lookup"><span data-stu-id="55456-111">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="55456-112">application</span><span class="sxs-lookup"><span data-stu-id="55456-112">application</span></span> | [<span data-ttu-id="55456-113">ID</span><span class="sxs-lookup"><span data-stu-id="55456-113">Identity</span></span>](identity.md) | <span data-ttu-id="55456-p101">省略可能。このアクションに関連付けられているアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="55456-p101">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="55456-116">conversation</span><span class="sxs-lookup"><span data-stu-id="55456-116">conversation</span></span>| [<span data-ttu-id="55456-117">Identity</span><span class="sxs-lookup"><span data-stu-id="55456-117">Identity</span></span>](identity.md) | <span data-ttu-id="55456-118">省略可能。</span><span class="sxs-lookup"><span data-stu-id="55456-118">Optional.</span></span> <span data-ttu-id="55456-119">このアクションに関連付けられているチームまたはチャネル。</span><span class="sxs-lookup"><span data-stu-id="55456-119">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="55456-120">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="55456-120">conversationIdentityType</span></span>| [<span data-ttu-id="55456-121">Identity</span><span class="sxs-lookup"><span data-stu-id="55456-121">Identity</span></span>](identity.md) | <span data-ttu-id="55456-122">省略可能。</span><span class="sxs-lookup"><span data-stu-id="55456-122">Optional.</span></span> <span data-ttu-id="55456-123">**会話**プロパティがチームまたはチャネルを識別するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="55456-123">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="55456-124">デバイス</span><span class="sxs-lookup"><span data-stu-id="55456-124">device</span></span>      | [<span data-ttu-id="55456-125">ID</span><span class="sxs-lookup"><span data-stu-id="55456-125">Identity</span></span>](identity.md) | <span data-ttu-id="55456-p104">省略可能。このアクションに関連付けられているデバイス。</span><span class="sxs-lookup"><span data-stu-id="55456-p104">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="55456-128">phone</span><span class="sxs-lookup"><span data-stu-id="55456-128">phone</span></span>       | [<span data-ttu-id="55456-129">identity</span><span class="sxs-lookup"><span data-stu-id="55456-129">identity</span></span>](identity.md) | <span data-ttu-id="55456-130">省略可能。</span><span class="sxs-lookup"><span data-stu-id="55456-130">Optional.</span></span> <span data-ttu-id="55456-131">このアクションに関連付けられている電話番号。</span><span class="sxs-lookup"><span data-stu-id="55456-131">The phone number associated with this action.</span></span> |
| <span data-ttu-id="55456-132">user</span><span class="sxs-lookup"><span data-stu-id="55456-132">user</span></span>        | [<span data-ttu-id="55456-133">Identity</span><span class="sxs-lookup"><span data-stu-id="55456-133">Identity</span></span>](identity.md) | <span data-ttu-id="55456-p106">省略可能。このアクションに関連付けられているユーザー。</span><span class="sxs-lookup"><span data-stu-id="55456-p106">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="55456-136">注釈</span><span class="sxs-lookup"><span data-stu-id="55456-136">Remarks</span></span> 

<span data-ttu-id="55456-137">「[呼び出し](call.md)を使用したリソースの**設定**」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55456-137">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->

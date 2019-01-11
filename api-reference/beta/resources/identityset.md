---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: 63178fc9add3d097b7e8aaf0c5c2a697a91eaeed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807022"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="b1728-102">identitySet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b1728-102">identitySet resource type</span></span>

<span data-ttu-id="b1728-p101">**IdentitySet** リソースは、[ID](identity.md) リソースのキー付きコレクションです。_作成者_または_最終更新者_など、アイテムのさまざまなイベントに関連付けられている ID のセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="b1728-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1728-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1728-105">JSON representation</span></span>

<span data-ttu-id="b1728-106">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b1728-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
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
  "application": {"@odata.type": "#microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "#microsoft.graph.identity"},
  "device": {"@odata.type": "#microsoft.graph.identity"},
  "encrypted": {"@odata.type": "#microsoft.graph.identity"},
  "guest": {"@odata.type": "#microsoft.graph.identity"},
  "phone": {"@odata.type": "#microsoft.graph.identity"},
  "user": {"@odata.type": "#microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="b1728-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1728-107">Properties</span></span>

| <span data-ttu-id="b1728-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1728-108">Property</span></span>    | <span data-ttu-id="b1728-109">型</span><span class="sxs-lookup"><span data-stu-id="b1728-109">Type</span></span>                    | <span data-ttu-id="b1728-110">説明</span><span class="sxs-lookup"><span data-stu-id="b1728-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="b1728-111">application</span><span class="sxs-lookup"><span data-stu-id="b1728-111">application</span></span> | [<span data-ttu-id="b1728-112">Identity</span><span class="sxs-lookup"><span data-stu-id="b1728-112">Identity</span></span>](identity.md) | <span data-ttu-id="b1728-p102">省略可能。このアクションに関連付けられているアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="b1728-p102">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="b1728-115">デバイス</span><span class="sxs-lookup"><span data-stu-id="b1728-115">device</span></span>      | [<span data-ttu-id="b1728-116">Identity</span><span class="sxs-lookup"><span data-stu-id="b1728-116">Identity</span></span>](identity.md) | <span data-ttu-id="b1728-p103">省略可能。このアクションに関連付けられているデバイス。</span><span class="sxs-lookup"><span data-stu-id="b1728-p103">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="b1728-119">phone</span><span class="sxs-lookup"><span data-stu-id="b1728-119">phone</span></span>       | [<span data-ttu-id="b1728-120">identity</span><span class="sxs-lookup"><span data-stu-id="b1728-120">identity</span></span>](identity.md) | <span data-ttu-id="b1728-121">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b1728-121">Optional.</span></span> <span data-ttu-id="b1728-122">このアクションに関連付けられている電話番号です。</span><span class="sxs-lookup"><span data-stu-id="b1728-122">The phone number associated with this action.</span></span> |
| <span data-ttu-id="b1728-123">user</span><span class="sxs-lookup"><span data-stu-id="b1728-123">user</span></span>        | [<span data-ttu-id="b1728-124">Identity</span><span class="sxs-lookup"><span data-stu-id="b1728-124">Identity</span></span>](identity.md) | <span data-ttu-id="b1728-p105">省略可能。このアクションに関連付けられているユーザー。</span><span class="sxs-lookup"><span data-stu-id="b1728-p105">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="b1728-127">注釈</span><span class="sxs-lookup"><span data-stu-id="b1728-127">Remarks</span></span> 

<span data-ttu-id="b1728-128">**IdentitySet**リソースの使用率の[呼び出し](call.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1728-128">See [Call](call.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->

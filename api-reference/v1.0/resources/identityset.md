---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
description: Identity Set リソースは、id リソースのキー付きコレクションです。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f1176f133f51432899a1fb6ddab964f04e658c69
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030220"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="8fff1-103">IdentitySet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8fff1-103">IdentitySet resource type</span></span>

<span data-ttu-id="8fff1-p101">**IdentitySet** リソースは、[ID](identity.md) リソースのキー付きコレクションです。_作成者_または_最終更新者_など、アイテムのさまざまなイベントに関連付けられている ID のセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="8fff1-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fff1-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8fff1-106">JSON representation</span></span>

<span data-ttu-id="8fff1-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8fff1-107">Here is a JSON representation of the resource.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identitySet",
       "optionalProperties": ["user", "application", "device"],
       "openType": true } -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="8fff1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fff1-108">Properties</span></span>

| <span data-ttu-id="8fff1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fff1-109">Property</span></span>    | <span data-ttu-id="8fff1-110">型</span><span class="sxs-lookup"><span data-stu-id="8fff1-110">Type</span></span>                    | <span data-ttu-id="8fff1-111">説明</span><span class="sxs-lookup"><span data-stu-id="8fff1-111">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="8fff1-112">application</span><span class="sxs-lookup"><span data-stu-id="8fff1-112">application</span></span> | [<span data-ttu-id="8fff1-113">ID</span><span class="sxs-lookup"><span data-stu-id="8fff1-113">Identity</span></span>](identity.md) | <span data-ttu-id="8fff1-p102">省略可能。このアクションに関連付けられているアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="8fff1-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="8fff1-116">デバイス</span><span class="sxs-lookup"><span data-stu-id="8fff1-116">device</span></span>      | [<span data-ttu-id="8fff1-117">ID</span><span class="sxs-lookup"><span data-stu-id="8fff1-117">Identity</span></span>](identity.md) | <span data-ttu-id="8fff1-p103">省略可能。このアクションに関連付けられているデバイス。</span><span class="sxs-lookup"><span data-stu-id="8fff1-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="8fff1-120">user</span><span class="sxs-lookup"><span data-stu-id="8fff1-120">user</span></span>        | [<span data-ttu-id="8fff1-121">Identity</span><span class="sxs-lookup"><span data-stu-id="8fff1-121">Identity</span></span>](identity.md) | <span data-ttu-id="8fff1-p104">省略可能。このアクションに関連付けられているユーザー。</span><span class="sxs-lookup"><span data-stu-id="8fff1-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="8fff1-124">注釈</span><span class="sxs-lookup"><span data-stu-id="8fff1-124">Remarks</span></span> 

<span data-ttu-id="8fff1-125">**IdentitySet** リソースの使用法については、[DriveItem](driveitem.md) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8fff1-125">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->

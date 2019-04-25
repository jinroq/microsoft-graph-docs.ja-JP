---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: 369068dd48b9173032542303e3fd9831d25e6e9e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567572"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="20692-102">IdentitySet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="20692-102">IdentitySet resource type</span></span>

<span data-ttu-id="20692-p101">**IdentitySet** リソースは、[ID](identity.md) リソースのキー付きコレクションです。_作成者_または_最終更新者_など、アイテムのさまざまなイベントに関連付けられている ID のセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="20692-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="20692-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="20692-105">JSON representation</span></span>

<span data-ttu-id="20692-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="20692-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="20692-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20692-107">Properties</span></span>

| <span data-ttu-id="20692-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20692-108">Property</span></span>    | <span data-ttu-id="20692-109">型</span><span class="sxs-lookup"><span data-stu-id="20692-109">Type</span></span>                    | <span data-ttu-id="20692-110">説明</span><span class="sxs-lookup"><span data-stu-id="20692-110">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="20692-111">application</span><span class="sxs-lookup"><span data-stu-id="20692-111">application</span></span> | [<span data-ttu-id="20692-112">ID</span><span class="sxs-lookup"><span data-stu-id="20692-112">Identity</span></span>](identity.md) | <span data-ttu-id="20692-p102">省略可能。このアクションに関連付けられているアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="20692-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="20692-115">デバイス</span><span class="sxs-lookup"><span data-stu-id="20692-115">device</span></span>      | [<span data-ttu-id="20692-116">ID</span><span class="sxs-lookup"><span data-stu-id="20692-116">Identity</span></span>](identity.md) | <span data-ttu-id="20692-p103">省略可能。このアクションに関連付けられているデバイス。</span><span class="sxs-lookup"><span data-stu-id="20692-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="20692-119">user</span><span class="sxs-lookup"><span data-stu-id="20692-119">user</span></span>        | [<span data-ttu-id="20692-120">Identity</span><span class="sxs-lookup"><span data-stu-id="20692-120">Identity</span></span>](identity.md) | <span data-ttu-id="20692-p104">省略可能。このアクションに関連付けられているユーザー。</span><span class="sxs-lookup"><span data-stu-id="20692-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="20692-123">注釈</span><span class="sxs-lookup"><span data-stu-id="20692-123">Remarks</span></span> 

<span data-ttu-id="20692-124">**IdentitySet** リソースの使用法については、[DriveItem](driveitem.md) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20692-124">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->

---
author: JeremyKelley
description: ID リソースは、アクター の ID を表します。
ms.date: 09/14/2017
title: ID
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: cb05aa4a8ddf9d4e641bcebdff3f5984ddd34d61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971824"
---
# <a name="identity-resource-type"></a><span data-ttu-id="23be6-103">id リソースの種類</span><span class="sxs-lookup"><span data-stu-id="23be6-103">identity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23be6-p101">**ID** リソースは、_アクター_ の ID を表します。たとえば、アクターは、ユーザー、デバイス、アプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="23be6-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23be6-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="23be6-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="23be6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23be6-107">Properties</span></span>

| <span data-ttu-id="23be6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23be6-108">Property</span></span>            | <span data-ttu-id="23be6-109">型</span><span class="sxs-lookup"><span data-stu-id="23be6-109">Type</span></span>   | <span data-ttu-id="23be6-110">説明</span><span class="sxs-lookup"><span data-stu-id="23be6-110">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="23be6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="23be6-111">displayName</span></span>         | <span data-ttu-id="23be6-112">String</span><span class="sxs-lookup"><span data-stu-id="23be6-112">String</span></span> | <span data-ttu-id="23be6-p102">ID の表示名。使用可能でない場合や、最新の状態ではない場合があることにご注意ください。たとえば、ユーザーが表示名を変更する場合、API は、将来の応答に新しい値を表示することがあります。しかし、ユーザーに関連付けられたアイテムについては、[delta](../api/driveitem-delta.md) の使用時に変更されたことは表示されません。</span><span class="sxs-lookup"><span data-stu-id="23be6-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="23be6-116">id</span><span class="sxs-lookup"><span data-stu-id="23be6-116">id</span></span>                  | <span data-ttu-id="23be6-117">文字列</span><span class="sxs-lookup"><span data-stu-id="23be6-117">String</span></span> | <span data-ttu-id="23be6-118">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="23be6-118">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="23be6-119">tenantId</span><span class="sxs-lookup"><span data-stu-id="23be6-119">tenantId</span></span>            | <span data-ttu-id="23be6-120">String</span><span class="sxs-lookup"><span data-stu-id="23be6-120">String</span></span> | <span data-ttu-id="23be6-121">テナントの一意の id (オプション)。</span><span class="sxs-lookup"><span data-stu-id="23be6-121">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="23be6-122">注釈</span><span class="sxs-lookup"><span data-stu-id="23be6-122">Remarks</span></span>

<span data-ttu-id="23be6-p103">状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。</span><span class="sxs-lookup"><span data-stu-id="23be6-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity",
  "suppressions": []
}
-->

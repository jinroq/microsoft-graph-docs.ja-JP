---
author: rgregg
ms.author: rgregg
ms.date: 09/14/2017
title: ID
ms.openlocfilehash: 66dcd979718665af650edbfc50a46ece7c2c4c06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068105"
---
# <a name="identity-resource-type"></a><span data-ttu-id="68d0a-102">id のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="68d0a-102">identity resource type</span></span>

> <span data-ttu-id="68d0a-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="68d0a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68d0a-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68d0a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="68d0a-p102">**ID** リソースは、_アクター_ の ID を表します。たとえば、アクターは、ユーザー、デバイス、アプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="68d0a-p102">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="68d0a-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68d0a-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="68d0a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68d0a-108">Properties</span></span>

| <span data-ttu-id="68d0a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68d0a-109">Property</span></span>            | <span data-ttu-id="68d0a-110">型</span><span class="sxs-lookup"><span data-stu-id="68d0a-110">Type</span></span>   | <span data-ttu-id="68d0a-111">説明</span><span class="sxs-lookup"><span data-stu-id="68d0a-111">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="68d0a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="68d0a-112">displayName</span></span>         | <span data-ttu-id="68d0a-113">String</span><span class="sxs-lookup"><span data-stu-id="68d0a-113">String</span></span> | <span data-ttu-id="68d0a-p103">ID の表示名。使用可能でない場合や、最新の状態ではない場合があることにご注意ください。たとえば、ユーザーが表示名を変更する場合、API は、将来の応答に新しい値を表示することがあります。しかし、ユーザーに関連付けられたアイテムについては、[delta](../api/driveitem-delta.md) の使用時に変更されたことは表示されません。</span><span class="sxs-lookup"><span data-stu-id="68d0a-p103">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="68d0a-117">id</span><span class="sxs-lookup"><span data-stu-id="68d0a-117">id</span></span>                  | <span data-ttu-id="68d0a-118">String</span><span class="sxs-lookup"><span data-stu-id="68d0a-118">String</span></span> | <span data-ttu-id="68d0a-119">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="68d0a-119">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="68d0a-120">tenantId</span><span class="sxs-lookup"><span data-stu-id="68d0a-120">tenantId</span></span>            | <span data-ttu-id="68d0a-121">String</span><span class="sxs-lookup"><span data-stu-id="68d0a-121">String</span></span> | <span data-ttu-id="68d0a-122">(省略可能) のテナントの一意の id。</span><span class="sxs-lookup"><span data-stu-id="68d0a-122">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="68d0a-123">注釈</span><span class="sxs-lookup"><span data-stu-id="68d0a-123">Remarks</span></span>

<span data-ttu-id="68d0a-p104">状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。</span><span class="sxs-lookup"><span data-stu-id="68d0a-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"
} -->
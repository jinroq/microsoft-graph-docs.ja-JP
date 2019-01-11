---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ID
localization_priority: Normal
ms.openlocfilehash: 0d4e7284da7353e7c6902d7ae1958d41f9eafd8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816017"
---
# <a name="identity-resource-type"></a><span data-ttu-id="37c21-102">ID リソースの種類</span><span class="sxs-lookup"><span data-stu-id="37c21-102">Identity resource type</span></span>

<span data-ttu-id="37c21-p101">**ID** リソースは、_アクター_ の ID を表します。たとえば、アクターは、ユーザー、デバイス、アプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="37c21-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="37c21-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="37c21-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity",
  "openType": true,
 "optionalProperties": ["displayName", "thumbnails"] } -->
```json
{
  "displayName": "string",
  "id": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="37c21-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37c21-106">Properties</span></span>

| <span data-ttu-id="37c21-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37c21-107">Property</span></span>    | <span data-ttu-id="37c21-108">型</span><span class="sxs-lookup"><span data-stu-id="37c21-108">Type</span></span>   | <span data-ttu-id="37c21-109">説明</span><span class="sxs-lookup"><span data-stu-id="37c21-109">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="37c21-110">displayName</span><span class="sxs-lookup"><span data-stu-id="37c21-110">displayName</span></span> | <span data-ttu-id="37c21-111">String</span><span class="sxs-lookup"><span data-stu-id="37c21-111">String</span></span> | <span data-ttu-id="37c21-p102">ID の表示名。使用可能でない場合や、最新の状態ではない場合があることにご注意ください。たとえば、ユーザーが表示名を変更する場合、API は、将来の応答に新しい値を表示することがあります。しかし、ユーザーに関連付けられたアイテムについては、[delta](../api/driveitem-delta.md) の使用時に変更されたことは表示されません。</span><span class="sxs-lookup"><span data-stu-id="37c21-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>     |
| <span data-ttu-id="37c21-115">id</span><span class="sxs-lookup"><span data-stu-id="37c21-115">id</span></span>          | <span data-ttu-id="37c21-116">String</span><span class="sxs-lookup"><span data-stu-id="37c21-116">String</span></span> | <span data-ttu-id="37c21-117">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="37c21-117">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |

## <a name="remarks"></a><span data-ttu-id="37c21-118">注釈</span><span class="sxs-lookup"><span data-stu-id="37c21-118">Remarks</span></span>

<span data-ttu-id="37c21-p103">状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。</span><span class="sxs-lookup"><span data-stu-id="37c21-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"

} -->

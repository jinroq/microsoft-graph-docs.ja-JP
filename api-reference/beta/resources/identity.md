---
author: rgregg
ms.author: rgregg
ms.date: 09/14/2017
title: ID
localization_priority: Normal
ms.openlocfilehash: 1ac2aea59ab0d6b09ae613b72fbfbf924240a4a0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518794"
---
# <a name="identity-resource-type"></a><span data-ttu-id="7c8b4-102">id のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="7c8b4-102">identity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c8b4-p101">**ID** リソースは、_アクター_ の ID を表します。たとえば、アクターは、ユーザー、デバイス、アプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="7c8b4-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c8b4-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7c8b4-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="7c8b4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c8b4-106">Properties</span></span>

| <span data-ttu-id="7c8b4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c8b4-107">Property</span></span>            | <span data-ttu-id="7c8b4-108">型</span><span class="sxs-lookup"><span data-stu-id="7c8b4-108">Type</span></span>   | <span data-ttu-id="7c8b4-109">説明</span><span class="sxs-lookup"><span data-stu-id="7c8b4-109">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7c8b4-110">displayName</span><span class="sxs-lookup"><span data-stu-id="7c8b4-110">displayName</span></span>         | <span data-ttu-id="7c8b4-111">String</span><span class="sxs-lookup"><span data-stu-id="7c8b4-111">String</span></span> | <span data-ttu-id="7c8b4-p102">ID の表示名。使用可能でない場合や、最新の状態ではない場合があることにご注意ください。たとえば、ユーザーが表示名を変更する場合、API は、将来の応答に新しい値を表示することがあります。しかし、ユーザーに関連付けられたアイテムについては、[delta](../api/driveitem-delta.md) の使用時に変更されたことは表示されません。</span><span class="sxs-lookup"><span data-stu-id="7c8b4-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="7c8b4-115">id</span><span class="sxs-lookup"><span data-stu-id="7c8b4-115">id</span></span>                  | <span data-ttu-id="7c8b4-116">String</span><span class="sxs-lookup"><span data-stu-id="7c8b4-116">String</span></span> | <span data-ttu-id="7c8b4-117">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7c8b4-117">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="7c8b4-118">tenantId</span><span class="sxs-lookup"><span data-stu-id="7c8b4-118">tenantId</span></span>            | <span data-ttu-id="7c8b4-119">String</span><span class="sxs-lookup"><span data-stu-id="7c8b4-119">String</span></span> | <span data-ttu-id="7c8b4-120">(省略可能) のテナントの一意の id。</span><span class="sxs-lookup"><span data-stu-id="7c8b4-120">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="7c8b4-121">注釈</span><span class="sxs-lookup"><span data-stu-id="7c8b4-121">Remarks</span></span>

<span data-ttu-id="7c8b4-p103">状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。</span><span class="sxs-lookup"><span data-stu-id="7c8b4-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity",
  "suppressions": [
    "Error: /api-reference/beta/resources/identity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

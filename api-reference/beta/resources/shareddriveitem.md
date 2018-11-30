---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
ms.openlocfilehash: 44d8a7c2bab9f19ff7b7680aea2e2a88fc2ef245
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066536"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="d51f1-102">SharedDriveItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d51f1-102">SharedDriveItem resource type</span></span>

> <span data-ttu-id="d51f1-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d51f1-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d51f1-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d51f1-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d51f1-105">**sharedDriveItem** リソースは、[Shares](../api/shares-get.md) API を使用して共有 [driveItem](driveitem.md) にアクセスする場合に返されます。</span><span class="sxs-lookup"><span data-stu-id="d51f1-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d51f1-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d51f1-106">JSON representation</span></span>

<span data-ttu-id="d51f1-107">以下は、**sharedDriveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d51f1-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="d51f1-108">**sharedDriveItem** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="d51f1-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItem",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "permission": { "@odata.type": "microsoft.graph.permission" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="d51f1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d51f1-109">Properties</span></span>

| <span data-ttu-id="d51f1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d51f1-110">Property</span></span> | <span data-ttu-id="d51f1-111">型</span><span class="sxs-lookup"><span data-stu-id="d51f1-111">Type</span></span>                          | <span data-ttu-id="d51f1-112">説明</span><span class="sxs-lookup"><span data-stu-id="d51f1-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="d51f1-113">id</span><span class="sxs-lookup"><span data-stu-id="d51f1-113">id</span></span>       | <span data-ttu-id="d51f1-114">String</span><span class="sxs-lookup"><span data-stu-id="d51f1-114">String</span></span>                        | <span data-ttu-id="d51f1-115">アクセスされている共有の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d51f1-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="d51f1-116">name</span><span class="sxs-lookup"><span data-stu-id="d51f1-116">name</span></span>     | <span data-ttu-id="d51f1-117">String</span><span class="sxs-lookup"><span data-stu-id="d51f1-117">String</span></span>                        | <span data-ttu-id="d51f1-118">共有項目の表示名。</span><span class="sxs-lookup"><span data-stu-id="d51f1-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="d51f1-119">owner</span><span class="sxs-lookup"><span data-stu-id="d51f1-119">owner</span></span>    | [<span data-ttu-id="d51f1-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="d51f1-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="d51f1-121">参照されている共有アイテムの所有者に関する情報。</span><span class="sxs-lookup"><span data-stu-id="d51f1-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d51f1-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d51f1-122">Relationships</span></span>

| <span data-ttu-id="d51f1-123">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="d51f1-123">Relationship name</span></span> | <span data-ttu-id="d51f1-124">種類</span><span class="sxs-lookup"><span data-stu-id="d51f1-124">Type</span></span>                | <span data-ttu-id="d51f1-125">説明</span><span class="sxs-lookup"><span data-stu-id="d51f1-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="d51f1-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="d51f1-126">**driveItem**</span></span>     | <span data-ttu-id="d51f1-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d51f1-127">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="d51f1-128">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="d51f1-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="d51f1-129">**list**</span><span class="sxs-lookup"><span data-stu-id="d51f1-129">**list**</span></span>          | <span data-ttu-id="d51f1-130">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="d51f1-130">[**list**][list]</span></span>           | <span data-ttu-id="d51f1-131">基になる **list** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="d51f1-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="d51f1-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="d51f1-132">**listItem**</span></span>      | <span data-ttu-id="d51f1-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="d51f1-133">[**listItem**][listItem]</span></span>   | <span data-ttu-id="d51f1-134">基になる **listItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="d51f1-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="d51f1-135">**permission**</span><span class="sxs-lookup"><span data-stu-id="d51f1-135">**permission**</span></span>    | <span data-ttu-id="d51f1-136">[**アクセス許可**][permission]</span><span class="sxs-lookup"><span data-stu-id="d51f1-136">[**permission**][permission]</span></span> | <span data-ttu-id="d51f1-137">基になっている共有リンクを表す**アクセス許可**にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="d51f1-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="d51f1-138">**site**</span><span class="sxs-lookup"><span data-stu-id="d51f1-138">**site**</span></span>          | <span data-ttu-id="d51f1-139">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="d51f1-139">[**site**][site]</span></span>           | <span data-ttu-id="d51f1-140">基になる **site** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="d51f1-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="d51f1-141">または、個人用の OneDrive アカウントから共有される **driveItem** には、次のリレーションシップも使用できます。</span><span class="sxs-lookup"><span data-stu-id="d51f1-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="d51f1-142">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="d51f1-142">Relationship name</span></span> | <span data-ttu-id="d51f1-143">種類</span><span class="sxs-lookup"><span data-stu-id="d51f1-143">Type</span></span>                         | <span data-ttu-id="d51f1-144">説明</span><span class="sxs-lookup"><span data-stu-id="d51f1-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="d51f1-145">**items**</span><span class="sxs-lookup"><span data-stu-id="d51f1-145">**items**</span></span>         | <span data-ttu-id="d51f1-146">[**driveItem**][driveItem] コレクション</span><span class="sxs-lookup"><span data-stu-id="d51f1-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="d51f1-147">共有ルートに含まれているすべての driveItem。</span><span class="sxs-lookup"><span data-stu-id="d51f1-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="d51f1-148">このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="d51f1-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="d51f1-149">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="d51f1-149">**driveItem**</span></span>     | <span data-ttu-id="d51f1-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d51f1-150">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="d51f1-151">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="d51f1-151">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="d51f1-152">メソッド</span><span class="sxs-lookup"><span data-stu-id="d51f1-152">Methods</span></span>

| <span data-ttu-id="d51f1-153">メソッド</span><span class="sxs-lookup"><span data-stu-id="d51f1-153">Method</span></span>                                  | <span data-ttu-id="d51f1-154">REST パス</span><span class="sxs-lookup"><span data-stu-id="d51f1-154">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="d51f1-155">共有アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="d51f1-155">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="d51f1-156">備考</span><span class="sxs-lookup"><span data-stu-id="d51f1-156">Remarks</span></span>

<span data-ttu-id="d51f1-157">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d51f1-157">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->

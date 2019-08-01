---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
description: sharedDriveItem リソースは、Shares API を使用して共有 driveItem にアクセスする場合に返されます。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1f6684e9c266a800f5a76a7085a8af22ea9518e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034336"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="506c1-103">SharedDriveItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="506c1-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="506c1-104">**sharedDriveItem** リソースは、[Shares](../api/shares-get.md) API を使用して共有 [driveItem](driveitem.md) にアクセスする場合に返されます。</span><span class="sxs-lookup"><span data-stu-id="506c1-104">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="506c1-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="506c1-105">JSON representation</span></span>

<span data-ttu-id="506c1-106">以下は、**sharedDriveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="506c1-106">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="506c1-107">**sharedDriveItem** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="506c1-107">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="506c1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="506c1-108">Properties</span></span>

| <span data-ttu-id="506c1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="506c1-109">Property</span></span> | <span data-ttu-id="506c1-110">型</span><span class="sxs-lookup"><span data-stu-id="506c1-110">Type</span></span>                          | <span data-ttu-id="506c1-111">説明</span><span class="sxs-lookup"><span data-stu-id="506c1-111">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="506c1-112">id</span><span class="sxs-lookup"><span data-stu-id="506c1-112">id</span></span>       | <span data-ttu-id="506c1-113">文字列</span><span class="sxs-lookup"><span data-stu-id="506c1-113">String</span></span>                        | <span data-ttu-id="506c1-114">アクセスされている共有の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="506c1-114">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="506c1-115">name</span><span class="sxs-lookup"><span data-stu-id="506c1-115">name</span></span>     | <span data-ttu-id="506c1-116">String</span><span class="sxs-lookup"><span data-stu-id="506c1-116">String</span></span>                        | <span data-ttu-id="506c1-117">共有項目の表示名。</span><span class="sxs-lookup"><span data-stu-id="506c1-117">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="506c1-118">owner</span><span class="sxs-lookup"><span data-stu-id="506c1-118">owner</span></span>    | [<span data-ttu-id="506c1-119">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="506c1-119">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="506c1-120">参照されている共有アイテムの所有者に関する情報。</span><span class="sxs-lookup"><span data-stu-id="506c1-120">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="506c1-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="506c1-121">Relationships</span></span>

| <span data-ttu-id="506c1-122">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="506c1-122">Relationship name</span></span> | <span data-ttu-id="506c1-123">種類</span><span class="sxs-lookup"><span data-stu-id="506c1-123">Type</span></span>                | <span data-ttu-id="506c1-124">説明</span><span class="sxs-lookup"><span data-stu-id="506c1-124">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="506c1-125">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="506c1-125">**driveItem**</span></span>     | <span data-ttu-id="506c1-126">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="506c1-126">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="506c1-127">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="506c1-127">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="506c1-128">**list**</span><span class="sxs-lookup"><span data-stu-id="506c1-128">**list**</span></span>          | <span data-ttu-id="506c1-129">[**一覧**][list]</span><span class="sxs-lookup"><span data-stu-id="506c1-129">[**list**][list]</span></span>        | <span data-ttu-id="506c1-130">基になる **list** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="506c1-130">Used to access the underlying **list**</span></span>
| <span data-ttu-id="506c1-131">**listItem**</span><span class="sxs-lookup"><span data-stu-id="506c1-131">**listItem**</span></span>      | <span data-ttu-id="506c1-132">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="506c1-132">[**listItem**][listItem]</span></span>    | <span data-ttu-id="506c1-133">基になる **listItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="506c1-133">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="506c1-134">**site**</span><span class="sxs-lookup"><span data-stu-id="506c1-134">**site**</span></span>          | <span data-ttu-id="506c1-135">[**サイト**][site]</span><span class="sxs-lookup"><span data-stu-id="506c1-135">[**site**][site]</span></span>        | <span data-ttu-id="506c1-136">基になる **site** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="506c1-136">Used to access the underlying **site**</span></span>

<span data-ttu-id="506c1-137">または、個人用の OneDrive アカウントから共有される **driveItem** には、次のリレーションシップも使用できます。</span><span class="sxs-lookup"><span data-stu-id="506c1-137">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="506c1-138">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="506c1-138">Relationship name</span></span> | <span data-ttu-id="506c1-139">種類</span><span class="sxs-lookup"><span data-stu-id="506c1-139">Type</span></span>                         | <span data-ttu-id="506c1-140">説明</span><span class="sxs-lookup"><span data-stu-id="506c1-140">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="506c1-141">**items**</span><span class="sxs-lookup"><span data-stu-id="506c1-141">**items**</span></span>         | <span data-ttu-id="506c1-142">[**Drive item**][driveItem]コレクション</span><span class="sxs-lookup"><span data-stu-id="506c1-142">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="506c1-143">共有ルートに含まれているすべての driveItem。</span><span class="sxs-lookup"><span data-stu-id="506c1-143">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="506c1-144">このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="506c1-144">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="506c1-145">**root**</span><span class="sxs-lookup"><span data-stu-id="506c1-145">**root**</span></span>          | <span data-ttu-id="506c1-146">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="506c1-146">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="506c1-147">基になる**ドライブ項目**へのアクセスに使用されます。</span><span class="sxs-lookup"><span data-stu-id="506c1-147">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="506c1-148">非推奨-- `driveItem`代わりに使用します。</span><span class="sxs-lookup"><span data-stu-id="506c1-148">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="506c1-149">メソッド</span><span class="sxs-lookup"><span data-stu-id="506c1-149">Methods</span></span>

| <span data-ttu-id="506c1-150">Method</span><span class="sxs-lookup"><span data-stu-id="506c1-150">Method</span></span>                                  | <span data-ttu-id="506c1-151">REST パス</span><span class="sxs-lookup"><span data-stu-id="506c1-151">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="506c1-152">共有アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="506c1-152">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="506c1-153">備考</span><span class="sxs-lookup"><span data-stu-id="506c1-153">Remarks</span></span>

<span data-ttu-id="506c1-154">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="506c1-154">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->

---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
ms.openlocfilehash: 3b4497c1a15704388dbb4bb4ba181d3985d65a69
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="f4f87-102">SharedDriveItem リソース型</span><span class="sxs-lookup"><span data-stu-id="f4f87-102">SharedDriveItem resource type</span></span>

<span data-ttu-id="f4f87-103">**sharedDriveItem** リソースは、[Shares](../api/shares_get.md) API を使用して共有 [driveItem](driveitem.md) にアクセスする場合に返されます。</span><span class="sxs-lookup"><span data-stu-id="f4f87-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares_get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4f87-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4f87-104">JSON representation</span></span>

<span data-ttu-id="f4f87-105">以下は、**sharedDriveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f4f87-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="f4f87-106">**sharedDriveItem** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="f4f87-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="f4f87-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4f87-107">Properties</span></span>

| <span data-ttu-id="f4f87-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4f87-108">Property</span></span> | <span data-ttu-id="f4f87-109">型</span><span class="sxs-lookup"><span data-stu-id="f4f87-109">Type</span></span>                          | <span data-ttu-id="f4f87-110">説明</span><span class="sxs-lookup"><span data-stu-id="f4f87-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="f4f87-111">id</span><span class="sxs-lookup"><span data-stu-id="f4f87-111">id</span></span>       | <span data-ttu-id="f4f87-112">String</span><span class="sxs-lookup"><span data-stu-id="f4f87-112">String</span></span>                        | <span data-ttu-id="f4f87-113">アクセスされている共有の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="f4f87-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="f4f87-114">name</span><span class="sxs-lookup"><span data-stu-id="f4f87-114">name</span></span>     | <span data-ttu-id="f4f87-115">String</span><span class="sxs-lookup"><span data-stu-id="f4f87-115">String</span></span>                        | <span data-ttu-id="f4f87-116">共有項目の表示名。</span><span class="sxs-lookup"><span data-stu-id="f4f87-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="f4f87-117">owner</span><span class="sxs-lookup"><span data-stu-id="f4f87-117">owner</span></span>    | [<span data-ttu-id="f4f87-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="f4f87-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="f4f87-119">参照されている共有アイテムの所有者に関する情報。</span><span class="sxs-lookup"><span data-stu-id="f4f87-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f4f87-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f4f87-120">Relationships</span></span>

| <span data-ttu-id="f4f87-121">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="f4f87-121">Relationship name</span></span> | <span data-ttu-id="f4f87-122">種類</span><span class="sxs-lookup"><span data-stu-id="f4f87-122">Type</span></span>                | <span data-ttu-id="f4f87-123">説明</span><span class="sxs-lookup"><span data-stu-id="f4f87-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="f4f87-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="f4f87-124">**DriveItem**</span></span>     | <span data-ttu-id="f4f87-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f4f87-125">DriveItem</span></span>   | <span data-ttu-id="f4f87-126">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="f4f87-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="f4f87-127">**list**</span><span class="sxs-lookup"><span data-stu-id="f4f87-127">**list**</span></span>          | <span data-ttu-id="f4f87-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="f4f87-128">List</span></span>        | <span data-ttu-id="f4f87-129">基になる **list** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="f4f87-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="f4f87-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="f4f87-130">**listItem**</span></span>      | <span data-ttu-id="f4f87-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="f4f87-131">**ListItem**</span></span>    | <span data-ttu-id="f4f87-132">基になる **listItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="f4f87-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="f4f87-133">**site**</span><span class="sxs-lookup"><span data-stu-id="f4f87-133">**site**</span></span>          | <span data-ttu-id="f4f87-134">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="f4f87-134">**site**</span></span>        | <span data-ttu-id="f4f87-135">基になる **site** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="f4f87-135">Used to access the underlying **site**</span></span>


<span data-ttu-id="f4f87-136">または、個人用の OneDrive アカウントから共有される **driveItem** には、次のリレーションシップも使用できます。</span><span class="sxs-lookup"><span data-stu-id="f4f87-136">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="f4f87-137">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="f4f87-137">Relationship name</span></span> | <span data-ttu-id="f4f87-138">種類</span><span class="sxs-lookup"><span data-stu-id="f4f87-138">Type</span></span>                         | <span data-ttu-id="f4f87-139">説明</span><span class="sxs-lookup"><span data-stu-id="f4f87-139">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="f4f87-140">**items**</span><span class="sxs-lookup"><span data-stu-id="f4f87-140">**items**</span></span>         | <span data-ttu-id="f4f87-141">[**driveItem**][driveItem] コレクション</span><span class="sxs-lookup"><span data-stu-id="f4f87-141">**driveItem** collection</span></span> | <span data-ttu-id="f4f87-142">共有ルートに含まれているすべての driveItem。</span><span class="sxs-lookup"><span data-stu-id="f4f87-142">All items contained in the sharing root.</span></span> <span data-ttu-id="f4f87-143">このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="f4f87-143">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="f4f87-144">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="f4f87-144">**DriveItem**</span></span>     | <span data-ttu-id="f4f87-145">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f4f87-145">DriveItem</span></span>            | <span data-ttu-id="f4f87-146">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="f4f87-146">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveItem.md
[list]: list.md
[listItem]: listItem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="f4f87-147">メソッド</span><span class="sxs-lookup"><span data-stu-id="f4f87-147">Methods</span></span>

| <span data-ttu-id="f4f87-148">Method</span><span class="sxs-lookup"><span data-stu-id="f4f87-148">Method</span></span>                                  | <span data-ttu-id="f4f87-149">REST パス</span><span class="sxs-lookup"><span data-stu-id="f4f87-149">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="f4f87-150">共有アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="f4f87-150">Get shared item</span></span>](../api/shares_get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="f4f87-151">備考</span><span class="sxs-lookup"><span data-stu-id="f4f87-151">Remarks</span></span>

<span data-ttu-id="f4f87-152">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4f87-152">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->

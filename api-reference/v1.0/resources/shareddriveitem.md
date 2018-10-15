---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
ms.openlocfilehash: abcf686be46e15a523a1a88170981cb318e71b00
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268201"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="a83d0-102">SharedDriveItem リソース型</span><span class="sxs-lookup"><span data-stu-id="a83d0-102">SharedDriveItem resource type</span></span>

<span data-ttu-id="a83d0-103">**sharedDriveItem** リソースは、[Shares](../api/shares_get.md) API を使用して共有 [driveItem](driveitem.md) にアクセスする場合に返されます。</span><span class="sxs-lookup"><span data-stu-id="a83d0-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares_get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a83d0-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a83d0-104">JSON representation</span></span>

<span data-ttu-id="a83d0-105">以下は、**sharedDriveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a83d0-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="a83d0-106">**sharedDriveItem** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="a83d0-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a83d0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a83d0-107">Properties</span></span>

| <span data-ttu-id="a83d0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a83d0-108">Property</span></span> | <span data-ttu-id="a83d0-109">タイプ</span><span class="sxs-lookup"><span data-stu-id="a83d0-109">Type</span></span>                          | <span data-ttu-id="a83d0-110">説明</span><span class="sxs-lookup"><span data-stu-id="a83d0-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="a83d0-111">id</span><span class="sxs-lookup"><span data-stu-id="a83d0-111">id</span></span>       | <span data-ttu-id="a83d0-112">文字列</span><span class="sxs-lookup"><span data-stu-id="a83d0-112">String</span></span>                        | <span data-ttu-id="a83d0-113">アクセスされている共有の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a83d0-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="a83d0-114">name</span><span class="sxs-lookup"><span data-stu-id="a83d0-114">name</span></span>     | <span data-ttu-id="a83d0-115">文字列</span><span class="sxs-lookup"><span data-stu-id="a83d0-115">String</span></span>                        | <span data-ttu-id="a83d0-116">共有項目の表示名。</span><span class="sxs-lookup"><span data-stu-id="a83d0-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="a83d0-117">owner</span><span class="sxs-lookup"><span data-stu-id="a83d0-117">owner</span></span>    | [<span data-ttu-id="a83d0-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="a83d0-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="a83d0-119">参照されている共有アイテムの所有者に関する情報。</span><span class="sxs-lookup"><span data-stu-id="a83d0-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a83d0-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a83d0-120">Relationships</span></span>

| <span data-ttu-id="a83d0-121">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="a83d0-121">Relationship name</span></span> | <span data-ttu-id="a83d0-122">種類</span><span class="sxs-lookup"><span data-stu-id="a83d0-122">Type</span></span>                | <span data-ttu-id="a83d0-123">説明</span><span class="sxs-lookup"><span data-stu-id="a83d0-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="a83d0-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="a83d0-124">**driveItem**</span></span>     | <span data-ttu-id="a83d0-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="a83d0-125">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="a83d0-126">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="a83d0-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="a83d0-127">**list**</span><span class="sxs-lookup"><span data-stu-id="a83d0-127">**list**</span></span>          | <span data-ttu-id="a83d0-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="a83d0-128">[**list**][list]</span></span>        | <span data-ttu-id="a83d0-129">基になる **list** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="a83d0-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="a83d0-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="a83d0-130">**listItem**</span></span>      | <span data-ttu-id="a83d0-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="a83d0-131">[**listItem**][listItem]</span></span>    | <span data-ttu-id="a83d0-132">基になる **listItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="a83d0-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="a83d0-133">**site**</span><span class="sxs-lookup"><span data-stu-id="a83d0-133">**site**</span></span>          | <span data-ttu-id="a83d0-134">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="a83d0-134">[**site**][site]</span></span>        | <span data-ttu-id="a83d0-135">基になる **site** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="a83d0-135">Used to access the underlying **site**</span></span>

<span data-ttu-id="a83d0-136">または、個人用の OneDrive アカウントから共有される **driveItem** には、次のリレーションシップも使用できます。</span><span class="sxs-lookup"><span data-stu-id="a83d0-136">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="a83d0-137">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="a83d0-137">Relationship name</span></span> | <span data-ttu-id="a83d0-138">種類</span><span class="sxs-lookup"><span data-stu-id="a83d0-138">Type</span></span>                         | <span data-ttu-id="a83d0-139">説明</span><span class="sxs-lookup"><span data-stu-id="a83d0-139">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="a83d0-140">**items**</span><span class="sxs-lookup"><span data-stu-id="a83d0-140">**items**</span></span>         | <span data-ttu-id="a83d0-141">[**driveItem**][driveItem] コレクション</span><span class="sxs-lookup"><span data-stu-id="a83d0-141">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="a83d0-142">共有ルートに含まれているすべての driveItem。</span><span class="sxs-lookup"><span data-stu-id="a83d0-142">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="a83d0-143">このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="a83d0-143">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="a83d0-144">**root**</span><span class="sxs-lookup"><span data-stu-id="a83d0-144">**root**</span></span>          | <span data-ttu-id="a83d0-145">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="a83d0-145">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="a83d0-146">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="a83d0-146">Used to access the underlying **driveItem**</span></span> <span data-ttu-id="a83d0-147">非推奨 -- 代わりに `driveItem` を使用してください。</span><span class="sxs-lookup"><span data-stu-id="a83d0-147">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveItem.md
[list]: list.md
[listItem]: listItem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="a83d0-148">メソッド</span><span class="sxs-lookup"><span data-stu-id="a83d0-148">Methods</span></span>

| <span data-ttu-id="a83d0-149">メソッド</span><span class="sxs-lookup"><span data-stu-id="a83d0-149">Method</span></span>                                  | <span data-ttu-id="a83d0-150">REST パス</span><span class="sxs-lookup"><span data-stu-id="a83d0-150">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="a83d0-151">共有アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="a83d0-151">Get shared item</span></span>](../api/shares_get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="a83d0-152">備考</span><span class="sxs-lookup"><span data-stu-id="a83d0-152">Remarks</span></span>

<span data-ttu-id="a83d0-153">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a83d0-153">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->

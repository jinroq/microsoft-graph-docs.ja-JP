---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: 3c0fa155088e39d69d52d4b14f33662d92666ed6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343200"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="3c418-102">SharedDriveItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3c418-102">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c418-103">**sharedDriveItem** リソースは、[Shares](../api/shares-get.md) API を使用して共有 [driveItem](driveitem.md) にアクセスする場合に返されます。</span><span class="sxs-lookup"><span data-stu-id="3c418-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c418-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3c418-104">JSON representation</span></span>

<span data-ttu-id="3c418-105">以下は、**sharedDriveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3c418-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="3c418-106">**sharedDriveItem** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="3c418-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3c418-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c418-107">Properties</span></span>

| <span data-ttu-id="3c418-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c418-108">Property</span></span> | <span data-ttu-id="3c418-109">型</span><span class="sxs-lookup"><span data-stu-id="3c418-109">Type</span></span>                          | <span data-ttu-id="3c418-110">説明</span><span class="sxs-lookup"><span data-stu-id="3c418-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="3c418-111">id</span><span class="sxs-lookup"><span data-stu-id="3c418-111">id</span></span>       | <span data-ttu-id="3c418-112">String</span><span class="sxs-lookup"><span data-stu-id="3c418-112">String</span></span>                        | <span data-ttu-id="3c418-113">アクセスされている共有の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="3c418-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="3c418-114">name</span><span class="sxs-lookup"><span data-stu-id="3c418-114">name</span></span>     | <span data-ttu-id="3c418-115">String</span><span class="sxs-lookup"><span data-stu-id="3c418-115">String</span></span>                        | <span data-ttu-id="3c418-116">共有項目の表示名。</span><span class="sxs-lookup"><span data-stu-id="3c418-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="3c418-117">owner</span><span class="sxs-lookup"><span data-stu-id="3c418-117">owner</span></span>    | [<span data-ttu-id="3c418-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="3c418-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="3c418-119">参照されている共有アイテムの所有者に関する情報。</span><span class="sxs-lookup"><span data-stu-id="3c418-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3c418-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3c418-120">Relationships</span></span>

| <span data-ttu-id="3c418-121">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="3c418-121">Relationship name</span></span> | <span data-ttu-id="3c418-122">種類</span><span class="sxs-lookup"><span data-stu-id="3c418-122">Type</span></span>                | <span data-ttu-id="3c418-123">説明</span><span class="sxs-lookup"><span data-stu-id="3c418-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="3c418-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="3c418-124">**driveItem**</span></span>     | <span data-ttu-id="3c418-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="3c418-125">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="3c418-126">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="3c418-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="3c418-127">**list**</span><span class="sxs-lookup"><span data-stu-id="3c418-127">**list**</span></span>          | <span data-ttu-id="3c418-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="3c418-128">[**list**][list]</span></span>           | <span data-ttu-id="3c418-129">基になる **list** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="3c418-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="3c418-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="3c418-130">**listItem**</span></span>      | <span data-ttu-id="3c418-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="3c418-131">[**listItem**][listItem]</span></span>   | <span data-ttu-id="3c418-132">基になる **listItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="3c418-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="3c418-133">**permission**</span><span class="sxs-lookup"><span data-stu-id="3c418-133">**permission**</span></span>    | <span data-ttu-id="3c418-134">[**権**][permission]</span><span class="sxs-lookup"><span data-stu-id="3c418-134">[**permission**][permission]</span></span> | <span data-ttu-id="3c418-135">基になる共有リンクを表す**アクセス許可**へのアクセスに使用されます。</span><span class="sxs-lookup"><span data-stu-id="3c418-135">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="3c418-136">**site**</span><span class="sxs-lookup"><span data-stu-id="3c418-136">**site**</span></span>          | <span data-ttu-id="3c418-137">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="3c418-137">[**site**][site]</span></span>           | <span data-ttu-id="3c418-138">基になる **site** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="3c418-138">Used to access the underlying **site**</span></span>

<span data-ttu-id="3c418-139">または、個人用の OneDrive アカウントから共有される **driveItem** には、次のリレーションシップも使用できます。</span><span class="sxs-lookup"><span data-stu-id="3c418-139">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="3c418-140">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="3c418-140">Relationship name</span></span> | <span data-ttu-id="3c418-141">種類</span><span class="sxs-lookup"><span data-stu-id="3c418-141">Type</span></span>                         | <span data-ttu-id="3c418-142">説明</span><span class="sxs-lookup"><span data-stu-id="3c418-142">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="3c418-143">**items**</span><span class="sxs-lookup"><span data-stu-id="3c418-143">**items**</span></span>         | <span data-ttu-id="3c418-144">[**driveItem**][driveItem] コレクション</span><span class="sxs-lookup"><span data-stu-id="3c418-144">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="3c418-145">共有ルートに含まれているすべての driveItem。</span><span class="sxs-lookup"><span data-stu-id="3c418-145">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="3c418-146">このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="3c418-146">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="3c418-147">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="3c418-147">**driveItem**</span></span>     | <span data-ttu-id="3c418-148">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="3c418-148">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="3c418-149">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="3c418-149">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="3c418-150">メソッド</span><span class="sxs-lookup"><span data-stu-id="3c418-150">Methods</span></span>

| <span data-ttu-id="3c418-151">Method</span><span class="sxs-lookup"><span data-stu-id="3c418-151">Method</span></span>                                  | <span data-ttu-id="3c418-152">REST パス</span><span class="sxs-lookup"><span data-stu-id="3c418-152">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="3c418-153">共有アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="3c418-153">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="3c418-154">備考</span><span class="sxs-lookup"><span data-stu-id="3c418-154">Remarks</span></span>

<span data-ttu-id="3c418-155">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c418-155">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share",
  "suppressions": []
}
-->

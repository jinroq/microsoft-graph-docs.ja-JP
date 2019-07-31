---
author: JeremyKelley
description: sharedDriveItem リソースは、Shares API を使用して共有 driveItem にアクセスする場合に返されます。
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7d5af60c4ba5c67046909f6998d298444fa06d51
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965160"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="90844-103">SharedDriveItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90844-103">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90844-104">**sharedDriveItem** リソースは、[Shares](../api/shares-get.md) API を使用して共有 [driveItem](driveitem.md) にアクセスする場合に返されます。</span><span class="sxs-lookup"><span data-stu-id="90844-104">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="90844-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="90844-105">JSON representation</span></span>

<span data-ttu-id="90844-106">以下は、**sharedDriveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="90844-106">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="90844-107">**sharedDriveItem** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="90844-107">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="90844-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90844-108">Properties</span></span>

| <span data-ttu-id="90844-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90844-109">Property</span></span> | <span data-ttu-id="90844-110">型</span><span class="sxs-lookup"><span data-stu-id="90844-110">Type</span></span>                          | <span data-ttu-id="90844-111">説明</span><span class="sxs-lookup"><span data-stu-id="90844-111">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="90844-112">id</span><span class="sxs-lookup"><span data-stu-id="90844-112">id</span></span>       | <span data-ttu-id="90844-113">文字列</span><span class="sxs-lookup"><span data-stu-id="90844-113">String</span></span>                        | <span data-ttu-id="90844-114">アクセスされている共有の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="90844-114">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="90844-115">name</span><span class="sxs-lookup"><span data-stu-id="90844-115">name</span></span>     | <span data-ttu-id="90844-116">String</span><span class="sxs-lookup"><span data-stu-id="90844-116">String</span></span>                        | <span data-ttu-id="90844-117">共有項目の表示名。</span><span class="sxs-lookup"><span data-stu-id="90844-117">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="90844-118">owner</span><span class="sxs-lookup"><span data-stu-id="90844-118">owner</span></span>    | [<span data-ttu-id="90844-119">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="90844-119">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="90844-120">参照されている共有アイテムの所有者に関する情報。</span><span class="sxs-lookup"><span data-stu-id="90844-120">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="90844-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="90844-121">Relationships</span></span>

| <span data-ttu-id="90844-122">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="90844-122">Relationship name</span></span> | <span data-ttu-id="90844-123">種類</span><span class="sxs-lookup"><span data-stu-id="90844-123">Type</span></span>                | <span data-ttu-id="90844-124">説明</span><span class="sxs-lookup"><span data-stu-id="90844-124">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="90844-125">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="90844-125">**driveItem**</span></span>     | <span data-ttu-id="90844-126">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="90844-126">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="90844-127">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="90844-127">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="90844-128">**list**</span><span class="sxs-lookup"><span data-stu-id="90844-128">**list**</span></span>          | <span data-ttu-id="90844-129">[**一覧**][list]</span><span class="sxs-lookup"><span data-stu-id="90844-129">[**list**][list]</span></span>           | <span data-ttu-id="90844-130">基になる **list** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="90844-130">Used to access the underlying **list**</span></span>
| <span data-ttu-id="90844-131">**listItem**</span><span class="sxs-lookup"><span data-stu-id="90844-131">**listItem**</span></span>      | <span data-ttu-id="90844-132">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="90844-132">[**listItem**][listItem]</span></span>   | <span data-ttu-id="90844-133">基になる **listItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="90844-133">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="90844-134">**permission**</span><span class="sxs-lookup"><span data-stu-id="90844-134">**permission**</span></span>    | <span data-ttu-id="90844-135">[**権**][permission]</span><span class="sxs-lookup"><span data-stu-id="90844-135">[**permission**][permission]</span></span> | <span data-ttu-id="90844-136">基になる共有リンクを表す**アクセス許可**へのアクセスに使用されます。</span><span class="sxs-lookup"><span data-stu-id="90844-136">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="90844-137">**リスト**</span><span class="sxs-lookup"><span data-stu-id="90844-137">**site**</span></span>          | <span data-ttu-id="90844-138">[**サイト**][site]</span><span class="sxs-lookup"><span data-stu-id="90844-138">[**site**][site]</span></span>           | <span data-ttu-id="90844-139">基になる **site** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="90844-139">Used to access the underlying **site**</span></span>

<span data-ttu-id="90844-140">または、個人用の OneDrive アカウントから共有される **driveItem** には、次のリレーションシップも使用できます。</span><span class="sxs-lookup"><span data-stu-id="90844-140">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="90844-141">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="90844-141">Relationship name</span></span> | <span data-ttu-id="90844-142">種類</span><span class="sxs-lookup"><span data-stu-id="90844-142">Type</span></span>                         | <span data-ttu-id="90844-143">説明</span><span class="sxs-lookup"><span data-stu-id="90844-143">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="90844-144">**items**</span><span class="sxs-lookup"><span data-stu-id="90844-144">**items**</span></span>         | <span data-ttu-id="90844-145">[**Drive item**][driveItem]コレクション</span><span class="sxs-lookup"><span data-stu-id="90844-145">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="90844-146">共有ルートに含まれているすべての driveItem。</span><span class="sxs-lookup"><span data-stu-id="90844-146">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="90844-147">このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="90844-147">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="90844-148">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="90844-148">**driveItem**</span></span>     | <span data-ttu-id="90844-149">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="90844-149">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="90844-150">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="90844-150">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="90844-151">メソッド</span><span class="sxs-lookup"><span data-stu-id="90844-151">Methods</span></span>

| <span data-ttu-id="90844-152">Method</span><span class="sxs-lookup"><span data-stu-id="90844-152">Method</span></span>                                  | <span data-ttu-id="90844-153">REST パス</span><span class="sxs-lookup"><span data-stu-id="90844-153">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="90844-154">共有アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="90844-154">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="90844-155">備考</span><span class="sxs-lookup"><span data-stu-id="90844-155">Remarks</span></span>

<span data-ttu-id="90844-156">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90844-156">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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

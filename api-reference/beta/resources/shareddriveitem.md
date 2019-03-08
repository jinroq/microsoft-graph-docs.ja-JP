---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: b146fdf0f7ee2e2037fcb1d36511d0afa503005b
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480629"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="26ece-102">SharedDriveItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26ece-102">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26ece-103">**sharedDriveItem** リソースは、[Shares](../api/shares-get.md) API を使用して共有 [driveItem](driveitem.md) にアクセスする場合に返されます。</span><span class="sxs-lookup"><span data-stu-id="26ece-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="26ece-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26ece-104">JSON representation</span></span>

<span data-ttu-id="26ece-105">以下は、**sharedDriveItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="26ece-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="26ece-106">**sharedDriveItem** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="26ece-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="26ece-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26ece-107">Properties</span></span>

| <span data-ttu-id="26ece-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26ece-108">Property</span></span> | <span data-ttu-id="26ece-109">種類</span><span class="sxs-lookup"><span data-stu-id="26ece-109">Type</span></span>                          | <span data-ttu-id="26ece-110">説明</span><span class="sxs-lookup"><span data-stu-id="26ece-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="26ece-111">id</span><span class="sxs-lookup"><span data-stu-id="26ece-111">id</span></span>       | <span data-ttu-id="26ece-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="26ece-112">String</span></span>                        | <span data-ttu-id="26ece-113">アクセスされている共有の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="26ece-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="26ece-114">name</span><span class="sxs-lookup"><span data-stu-id="26ece-114">name</span></span>     | <span data-ttu-id="26ece-115">String</span><span class="sxs-lookup"><span data-stu-id="26ece-115">String</span></span>                        | <span data-ttu-id="26ece-116">共有項目の表示名。</span><span class="sxs-lookup"><span data-stu-id="26ece-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="26ece-117">owner</span><span class="sxs-lookup"><span data-stu-id="26ece-117">owner</span></span>    | [<span data-ttu-id="26ece-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="26ece-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="26ece-119">参照されている共有アイテムの所有者に関する情報。</span><span class="sxs-lookup"><span data-stu-id="26ece-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="26ece-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="26ece-120">Relationships</span></span>

| <span data-ttu-id="26ece-121">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="26ece-121">Relationship name</span></span> | <span data-ttu-id="26ece-122">種類</span><span class="sxs-lookup"><span data-stu-id="26ece-122">Type</span></span>                | <span data-ttu-id="26ece-123">説明</span><span class="sxs-lookup"><span data-stu-id="26ece-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="26ece-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="26ece-124">**driveItem**</span></span>     | <span data-ttu-id="26ece-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="26ece-125">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="26ece-126">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="26ece-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="26ece-127">**list**</span><span class="sxs-lookup"><span data-stu-id="26ece-127">**list**</span></span>          | <span data-ttu-id="26ece-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="26ece-128">[**list**][list]</span></span>           | <span data-ttu-id="26ece-129">基になる **list** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="26ece-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="26ece-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="26ece-130">**listItem**</span></span>      | <span data-ttu-id="26ece-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="26ece-131">[**listItem**][listItem]</span></span>   | <span data-ttu-id="26ece-132">基になる **listItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="26ece-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="26ece-133">**permission**</span><span class="sxs-lookup"><span data-stu-id="26ece-133">**permission**</span></span>    | <span data-ttu-id="26ece-134">[**権**][permission]</span><span class="sxs-lookup"><span data-stu-id="26ece-134">[**permission**][permission]</span></span> | <span data-ttu-id="26ece-135">基になる共有リンクを表す**アクセス許可**へのアクセスに使用されます。</span><span class="sxs-lookup"><span data-stu-id="26ece-135">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="26ece-136">**site**</span><span class="sxs-lookup"><span data-stu-id="26ece-136">**site**</span></span>          | <span data-ttu-id="26ece-137">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="26ece-137">[**site**][site]</span></span>           | <span data-ttu-id="26ece-138">基になる **site** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="26ece-138">Used to access the underlying **site**</span></span>

<span data-ttu-id="26ece-139">または、個人用の OneDrive アカウントから共有される **driveItem** には、次のリレーションシップも使用できます。</span><span class="sxs-lookup"><span data-stu-id="26ece-139">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="26ece-140">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="26ece-140">Relationship name</span></span> | <span data-ttu-id="26ece-141">種類</span><span class="sxs-lookup"><span data-stu-id="26ece-141">Type</span></span>                         | <span data-ttu-id="26ece-142">説明</span><span class="sxs-lookup"><span data-stu-id="26ece-142">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="26ece-143">**items**</span><span class="sxs-lookup"><span data-stu-id="26ece-143">**items**</span></span>         | <span data-ttu-id="26ece-144">[**driveItem**][driveItem] コレクション</span><span class="sxs-lookup"><span data-stu-id="26ece-144">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="26ece-145">共有ルートに含まれているすべての driveItem。</span><span class="sxs-lookup"><span data-stu-id="26ece-145">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="26ece-146">このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="26ece-146">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="26ece-147">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="26ece-147">**driveItem**</span></span>     | <span data-ttu-id="26ece-148">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="26ece-148">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="26ece-149">基になる **driveItem** にアクセスするために使用</span><span class="sxs-lookup"><span data-stu-id="26ece-149">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="26ece-150">メソッド</span><span class="sxs-lookup"><span data-stu-id="26ece-150">Methods</span></span>

| <span data-ttu-id="26ece-151">メソッド</span><span class="sxs-lookup"><span data-stu-id="26ece-151">Method</span></span>                                  | <span data-ttu-id="26ece-152">REST パス</span><span class="sxs-lookup"><span data-stu-id="26ece-152">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="26ece-153">共有アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="26ece-153">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="26ece-154">備考</span><span class="sxs-lookup"><span data-stu-id="26ece-154">Remarks</span></span>

<span data-ttu-id="26ece-155">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26ece-155">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share",
  "suppressions": [
    "Error: /api-reference/beta/resources/shareddriveitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

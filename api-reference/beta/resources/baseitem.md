---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
ms.openlocfilehash: 6c37ecc2ab0f838f4957a5aff1d88c4c6b75b382
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339119"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="0e856-102">BaseItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e856-102">BaseItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e856-p101">**baseItem** リソースは、他のいくつかのリソースの種類間で共有されるプロパティの共通セットを含む抽象リソースです。**baseItem** から派生するリソースには以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="0e856-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="0e856-105">drive</span><span class="sxs-lookup"><span data-stu-id="0e856-105">drive</span></span>](drive.md)
* [<span data-ttu-id="0e856-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="0e856-106">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="0e856-107">site</span><span class="sxs-lookup"><span data-stu-id="0e856-107">site</span></span>](site.md)
* [<span data-ttu-id="0e856-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="0e856-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="0e856-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e856-109">JSON representation</span></span>

<span data-ttu-id="0e856-110">以下は、**baseItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0e856-110">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItem",
  "abstract": true
}-->

```json
{
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="0e856-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e856-111">Properties</span></span>

| <span data-ttu-id="0e856-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e856-112">Property</span></span>             | <span data-ttu-id="0e856-113">型</span><span class="sxs-lookup"><span data-stu-id="0e856-113">Type</span></span>              | <span data-ttu-id="0e856-114">説明</span><span class="sxs-lookup"><span data-stu-id="0e856-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="0e856-115">id</span><span class="sxs-lookup"><span data-stu-id="0e856-115">id</span></span>                   | <span data-ttu-id="0e856-116">string</span><span class="sxs-lookup"><span data-stu-id="0e856-116">string</span></span>            | <span data-ttu-id="0e856-p102">ドライブの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0e856-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="0e856-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="0e856-119">createdBy</span></span>            | <span data-ttu-id="0e856-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0e856-120">[identitySet][]</span></span>   | <span data-ttu-id="0e856-p103">アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e856-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="0e856-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e856-123">createdDateTime</span></span>      | <span data-ttu-id="0e856-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e856-124">dateTimeOffset</span></span>    | <span data-ttu-id="0e856-p104">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e856-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="0e856-127">eTag</span><span class="sxs-lookup"><span data-stu-id="0e856-127">eTag</span></span>                 | <span data-ttu-id="0e856-128">string</span><span class="sxs-lookup"><span data-stu-id="0e856-128">string</span></span>            | <span data-ttu-id="0e856-p105">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e856-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="0e856-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0e856-131">lastModifiedBy</span></span>       | <span data-ttu-id="0e856-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0e856-132">[identitySet][]</span></span>   | <span data-ttu-id="0e856-p106">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e856-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="0e856-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e856-135">lastModifiedDateTime</span></span> | <span data-ttu-id="0e856-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e856-136">dateTimeOffset</span></span>    | <span data-ttu-id="0e856-p107">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e856-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="0e856-139">name</span><span class="sxs-lookup"><span data-stu-id="0e856-139">name</span></span>                 | <span data-ttu-id="0e856-140">string</span><span class="sxs-lookup"><span data-stu-id="0e856-140">string</span></span>            | <span data-ttu-id="0e856-p108">アイテムの名前。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="0e856-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="0e856-143">parentReference</span><span class="sxs-lookup"><span data-stu-id="0e856-143">parentReference</span></span>      | <span data-ttu-id="0e856-144">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="0e856-144">[itemReference][]</span></span> | <span data-ttu-id="0e856-p109">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="0e856-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="0e856-147">webUrl</span><span class="sxs-lookup"><span data-stu-id="0e856-147">webUrl</span></span>               | <span data-ttu-id="0e856-148">string (URL)</span><span class="sxs-lookup"><span data-stu-id="0e856-148">string (url)</span></span>      | <span data-ttu-id="0e856-p110">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e856-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="0e856-153">備考</span><span class="sxs-lookup"><span data-stu-id="0e856-153">Remarks</span></span>

<span data-ttu-id="0e856-154">`baseItem` の種類は直接使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e856-154">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem",
  "suppressions": []
}
-->

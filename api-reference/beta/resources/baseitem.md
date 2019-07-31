---
author: JeremyKelley
description: BaseItem リソースは、他のいくつかのリソースの種類で共有される共通のプロパティセットが含まれる抽象リソースです。
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 38e697e4a991871bd592cc891dcd131e845572fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013144"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="5a1a3-103">BaseItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a1a3-103">BaseItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a1a3-p101">**baseItem** リソースは、他のいくつかのリソースの種類間で共有されるプロパティの共通セットを含む抽象リソースです。**baseItem** から派生するリソースには以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5a1a3-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="5a1a3-106">drive</span><span class="sxs-lookup"><span data-stu-id="5a1a3-106">drive</span></span>](drive.md)
* [<span data-ttu-id="5a1a3-107">driveItem</span><span class="sxs-lookup"><span data-stu-id="5a1a3-107">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="5a1a3-108">site</span><span class="sxs-lookup"><span data-stu-id="5a1a3-108">site</span></span>](site.md)
* [<span data-ttu-id="5a1a3-109">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="5a1a3-109">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="5a1a3-110">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a1a3-110">JSON representation</span></span>

<span data-ttu-id="5a1a3-111">以下は、**baseItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a1a3-111">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5a1a3-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a1a3-112">Properties</span></span>

| <span data-ttu-id="5a1a3-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a1a3-113">Property</span></span>             | <span data-ttu-id="5a1a3-114">型</span><span class="sxs-lookup"><span data-stu-id="5a1a3-114">Type</span></span>              | <span data-ttu-id="5a1a3-115">説明</span><span class="sxs-lookup"><span data-stu-id="5a1a3-115">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="5a1a3-116">id</span><span class="sxs-lookup"><span data-stu-id="5a1a3-116">id</span></span>                   | <span data-ttu-id="5a1a3-117">string</span><span class="sxs-lookup"><span data-stu-id="5a1a3-117">string</span></span>            | <span data-ttu-id="5a1a3-p102">ドライブの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="5a1a3-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="5a1a3-120">createdBy</span><span class="sxs-lookup"><span data-stu-id="5a1a3-120">createdBy</span></span>            | <span data-ttu-id="5a1a3-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5a1a3-121">[identitySet][]</span></span>   | <span data-ttu-id="5a1a3-p103">アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5a1a3-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="5a1a3-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a1a3-124">createdDateTime</span></span>      | <span data-ttu-id="5a1a3-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a1a3-125">dateTimeOffset</span></span>    | <span data-ttu-id="5a1a3-p104">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5a1a3-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="5a1a3-128">eTag</span><span class="sxs-lookup"><span data-stu-id="5a1a3-128">eTag</span></span>                 | <span data-ttu-id="5a1a3-129">string</span><span class="sxs-lookup"><span data-stu-id="5a1a3-129">string</span></span>            | <span data-ttu-id="5a1a3-p105">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5a1a3-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="5a1a3-132">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5a1a3-132">lastModifiedBy</span></span>       | <span data-ttu-id="5a1a3-133">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5a1a3-133">[identitySet][]</span></span>   | <span data-ttu-id="5a1a3-p106">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5a1a3-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="5a1a3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a1a3-136">lastModifiedDateTime</span></span> | <span data-ttu-id="5a1a3-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a1a3-137">dateTimeOffset</span></span>    | <span data-ttu-id="5a1a3-p107">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5a1a3-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="5a1a3-140">name</span><span class="sxs-lookup"><span data-stu-id="5a1a3-140">name</span></span>                 | <span data-ttu-id="5a1a3-141">string</span><span class="sxs-lookup"><span data-stu-id="5a1a3-141">string</span></span>            | <span data-ttu-id="5a1a3-p108">アイテムの名前。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="5a1a3-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="5a1a3-144">parentReference</span><span class="sxs-lookup"><span data-stu-id="5a1a3-144">parentReference</span></span>      | <span data-ttu-id="5a1a3-145">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="5a1a3-145">[itemReference][]</span></span> | <span data-ttu-id="5a1a3-p109">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="5a1a3-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="5a1a3-148">webUrl</span><span class="sxs-lookup"><span data-stu-id="5a1a3-148">webUrl</span></span>               | <span data-ttu-id="5a1a3-149">string (URL)</span><span class="sxs-lookup"><span data-stu-id="5a1a3-149">string (url)</span></span>      | <span data-ttu-id="5a1a3-p110">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5a1a3-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="5a1a3-154">備考</span><span class="sxs-lookup"><span data-stu-id="5a1a3-154">Remarks</span></span>

<span data-ttu-id="5a1a3-155">`baseItem` の種類は直接使用できません。</span><span class="sxs-lookup"><span data-stu-id="5a1a3-155">The `baseItem` type is not expected to be used directly.</span></span>

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

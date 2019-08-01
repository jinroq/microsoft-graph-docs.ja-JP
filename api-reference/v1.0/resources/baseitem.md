---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
description: BaseItem リソースは、他のいくつかのリソースの種類で共有される共通のプロパティセットが含まれる抽象リソースです。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2bde386a736805d52758f6d80e629c585f82d87e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029982"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="21ee5-103">BaseItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21ee5-103">BaseItem resource type</span></span>

<span data-ttu-id="21ee5-p101">**baseItem** リソースは、他のいくつかのリソースの種類間で共有されるプロパティの共通セットを含む抽象リソースです。**baseItem** から派生するリソースには以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="21ee5-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="21ee5-106">drive</span><span class="sxs-lookup"><span data-stu-id="21ee5-106">drive</span></span>](drive.md)
* [<span data-ttu-id="21ee5-107">driveItem</span><span class="sxs-lookup"><span data-stu-id="21ee5-107">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="21ee5-108">site</span><span class="sxs-lookup"><span data-stu-id="21ee5-108">site</span></span>](site.md)
* [<span data-ttu-id="21ee5-109">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="21ee5-109">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="21ee5-110">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21ee5-110">JSON representation</span></span>

<span data-ttu-id="21ee5-111">以下は、**baseItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21ee5-111">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItem"
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

## <a name="properties"></a><span data-ttu-id="21ee5-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21ee5-112">Properties</span></span>

| <span data-ttu-id="21ee5-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21ee5-113">Property</span></span>             | <span data-ttu-id="21ee5-114">型</span><span class="sxs-lookup"><span data-stu-id="21ee5-114">Type</span></span>              | <span data-ttu-id="21ee5-115">説明</span><span class="sxs-lookup"><span data-stu-id="21ee5-115">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="21ee5-116">id</span><span class="sxs-lookup"><span data-stu-id="21ee5-116">id</span></span>                   | <span data-ttu-id="21ee5-117">文字列</span><span class="sxs-lookup"><span data-stu-id="21ee5-117">string</span></span>            | <span data-ttu-id="21ee5-p102">ドライブの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="21ee5-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="21ee5-120">createdBy</span><span class="sxs-lookup"><span data-stu-id="21ee5-120">createdBy</span></span>            | <span data-ttu-id="21ee5-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="21ee5-121">[identitySet][]</span></span>   | <span data-ttu-id="21ee5-p103">アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21ee5-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="21ee5-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21ee5-124">createdDateTime</span></span>      | <span data-ttu-id="21ee5-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21ee5-125">dateTimeOffset</span></span>    | <span data-ttu-id="21ee5-p104">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21ee5-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="21ee5-128">説明</span><span class="sxs-lookup"><span data-stu-id="21ee5-128">description</span></span>          | <span data-ttu-id="21ee5-129">String</span><span class="sxs-lookup"><span data-stu-id="21ee5-129">String</span></span>            | <span data-ttu-id="21ee5-130">ユーザーに表示されるアイテムの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="21ee5-130">Provides a user-visible description of the item.</span></span> <span data-ttu-id="21ee5-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="21ee5-131">Optional.</span></span>                             |
| <span data-ttu-id="21ee5-132">eTag</span><span class="sxs-lookup"><span data-stu-id="21ee5-132">eTag</span></span>                 | <span data-ttu-id="21ee5-133">string</span><span class="sxs-lookup"><span data-stu-id="21ee5-133">string</span></span>            | <span data-ttu-id="21ee5-p106">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21ee5-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="21ee5-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="21ee5-136">lastModifiedBy</span></span>       | <span data-ttu-id="21ee5-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="21ee5-137">[identitySet][]</span></span>   | <span data-ttu-id="21ee5-p107">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21ee5-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="21ee5-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21ee5-140">lastModifiedDateTime</span></span> | <span data-ttu-id="21ee5-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21ee5-141">dateTimeOffset</span></span>    | <span data-ttu-id="21ee5-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21ee5-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="21ee5-144">name</span><span class="sxs-lookup"><span data-stu-id="21ee5-144">name</span></span>                 | <span data-ttu-id="21ee5-145">string</span><span class="sxs-lookup"><span data-stu-id="21ee5-145">string</span></span>            | <span data-ttu-id="21ee5-p109">アイテムの名前。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="21ee5-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="21ee5-148">parentReference</span><span class="sxs-lookup"><span data-stu-id="21ee5-148">parentReference</span></span>      | <span data-ttu-id="21ee5-149">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="21ee5-149">[itemReference][]</span></span> | <span data-ttu-id="21ee5-p110">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="21ee5-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="21ee5-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="21ee5-152">webUrl</span></span>               | <span data-ttu-id="21ee5-153">string (URL)</span><span class="sxs-lookup"><span data-stu-id="21ee5-153">string (url)</span></span>      | <span data-ttu-id="21ee5-p111">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21ee5-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="21ee5-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21ee5-156">Relationships</span></span>

| <span data-ttu-id="21ee5-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21ee5-157">Relationship</span></span>       | <span data-ttu-id="21ee5-158">型</span><span class="sxs-lookup"><span data-stu-id="21ee5-158">Type</span></span>     | <span data-ttu-id="21ee5-159">説明</span><span class="sxs-lookup"><span data-stu-id="21ee5-159">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="21ee5-160">createdByUser</span><span class="sxs-lookup"><span data-stu-id="21ee5-160">createdByUser</span></span>      | <span data-ttu-id="21ee5-161">[user][]</span><span class="sxs-lookup"><span data-stu-id="21ee5-161">[user][]</span></span> | <span data-ttu-id="21ee5-162">アイテムを作成したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="21ee5-162">Identity of the user who created the item.</span></span> <span data-ttu-id="21ee5-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21ee5-163">Read-only.</span></span>
| <span data-ttu-id="21ee5-164">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="21ee5-164">lastModifiedByUser</span></span> | <span data-ttu-id="21ee5-165">[user][]</span><span class="sxs-lookup"><span data-stu-id="21ee5-165">[user][]</span></span> | <span data-ttu-id="21ee5-166">アイテムを最後に変更したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="21ee5-166">Identity of the user who last modified the item.</span></span> <span data-ttu-id="21ee5-167">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21ee5-167">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[ユーザー]: user.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="21ee5-171">備考</span><span class="sxs-lookup"><span data-stu-id="21ee5-171">Remarks</span></span>

<span data-ttu-id="21ee5-172">`baseItem` の種類は直接使用できません。</span><span class="sxs-lookup"><span data-stu-id="21ee5-172">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->

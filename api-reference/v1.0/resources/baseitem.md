---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
ms.openlocfilehash: ae22b0a36acb46c2a9d872f224c0a6d4c567782c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481133"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="ce14a-102">BaseItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce14a-102">BaseItem resource type</span></span>

<span data-ttu-id="ce14a-p101">**baseItem** リソースは、他のいくつかのリソースの種類間で共有されるプロパティの共通セットを含む抽象リソースです。**baseItem** から派生するリソースには以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="ce14a-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="ce14a-105">drive</span><span class="sxs-lookup"><span data-stu-id="ce14a-105">drive</span></span>](drive.md)
* [<span data-ttu-id="ce14a-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="ce14a-106">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="ce14a-107">site</span><span class="sxs-lookup"><span data-stu-id="ce14a-107">site</span></span>](site.md)
* [<span data-ttu-id="ce14a-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="ce14a-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="ce14a-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce14a-109">JSON representation</span></span>

<span data-ttu-id="ce14a-110">以下は、**baseItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ce14a-110">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ce14a-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce14a-111">Properties</span></span>

| <span data-ttu-id="ce14a-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce14a-112">Property</span></span>             | <span data-ttu-id="ce14a-113">種類</span><span class="sxs-lookup"><span data-stu-id="ce14a-113">Type</span></span>              | <span data-ttu-id="ce14a-114">説明</span><span class="sxs-lookup"><span data-stu-id="ce14a-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="ce14a-115">id</span><span class="sxs-lookup"><span data-stu-id="ce14a-115">id</span></span>                   | <span data-ttu-id="ce14a-116">文字列</span><span class="sxs-lookup"><span data-stu-id="ce14a-116">string</span></span>            | <span data-ttu-id="ce14a-p102">ドライブの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ce14a-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="ce14a-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="ce14a-119">createdBy</span></span>            | <span data-ttu-id="ce14a-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ce14a-120">[identitySet][]</span></span>   | <span data-ttu-id="ce14a-p103">アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ce14a-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="ce14a-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce14a-123">createdDateTime</span></span>      | <span data-ttu-id="ce14a-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce14a-124">dateTimeOffset</span></span>    | <span data-ttu-id="ce14a-p104">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ce14a-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="ce14a-127">説明</span><span class="sxs-lookup"><span data-stu-id="ce14a-127">description</span></span>          | <span data-ttu-id="ce14a-128">String</span><span class="sxs-lookup"><span data-stu-id="ce14a-128">String</span></span>            | <span data-ttu-id="ce14a-129">ユーザーに表示されるアイテムの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="ce14a-129">Provides a user-visible description of the item.</span></span> <span data-ttu-id="ce14a-130">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ce14a-130">Optional.</span></span>                             |
| <span data-ttu-id="ce14a-131">eTag</span><span class="sxs-lookup"><span data-stu-id="ce14a-131">eTag</span></span>                 | <span data-ttu-id="ce14a-132">string</span><span class="sxs-lookup"><span data-stu-id="ce14a-132">string</span></span>            | <span data-ttu-id="ce14a-p106">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ce14a-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="ce14a-135">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ce14a-135">lastModifiedBy</span></span>       | <span data-ttu-id="ce14a-136">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ce14a-136">[identitySet][]</span></span>   | <span data-ttu-id="ce14a-p107">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ce14a-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="ce14a-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce14a-139">lastModifiedDateTime</span></span> | <span data-ttu-id="ce14a-140">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce14a-140">dateTimeOffset</span></span>    | <span data-ttu-id="ce14a-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ce14a-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="ce14a-143">name</span><span class="sxs-lookup"><span data-stu-id="ce14a-143">name</span></span>                 | <span data-ttu-id="ce14a-144">string</span><span class="sxs-lookup"><span data-stu-id="ce14a-144">string</span></span>            | <span data-ttu-id="ce14a-p109">アイテムの名前。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="ce14a-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="ce14a-147">parentReference</span><span class="sxs-lookup"><span data-stu-id="ce14a-147">parentReference</span></span>      | <span data-ttu-id="ce14a-148">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="ce14a-148">[itemReference][]</span></span> | <span data-ttu-id="ce14a-p110">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="ce14a-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="ce14a-151">webUrl</span><span class="sxs-lookup"><span data-stu-id="ce14a-151">webUrl</span></span>               | <span data-ttu-id="ce14a-152">string (URL)</span><span class="sxs-lookup"><span data-stu-id="ce14a-152">string (url)</span></span>      | <span data-ttu-id="ce14a-p111">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ce14a-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="ce14a-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce14a-155">Relationships</span></span>

| <span data-ttu-id="ce14a-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce14a-156">Relationship</span></span>       | <span data-ttu-id="ce14a-157">種類</span><span class="sxs-lookup"><span data-stu-id="ce14a-157">Type</span></span>     | <span data-ttu-id="ce14a-158">説明</span><span class="sxs-lookup"><span data-stu-id="ce14a-158">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="ce14a-159">createdByUser</span><span class="sxs-lookup"><span data-stu-id="ce14a-159">createdByUser</span></span>      | <span data-ttu-id="ce14a-160">[ユーザー][]</span><span class="sxs-lookup"><span data-stu-id="ce14a-160">[user][]</span></span> | <span data-ttu-id="ce14a-161">アイテムを作成したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="ce14a-161">Identity of the user who created the item.</span></span> <span data-ttu-id="ce14a-162">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ce14a-162">Read-only.</span></span>
| <span data-ttu-id="ce14a-163">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="ce14a-163">lastModifiedByUser</span></span> | <span data-ttu-id="ce14a-164">[user][]</span><span class="sxs-lookup"><span data-stu-id="ce14a-164">[user][]</span></span> | <span data-ttu-id="ce14a-165">アイテムを最後に変更したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="ce14a-165">Identity of the user who last modified the item.</span></span> <span data-ttu-id="ce14a-166">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ce14a-166">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[ユーザー]: user.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="ce14a-170">備考</span><span class="sxs-lookup"><span data-stu-id="ce14a-170">Remarks</span></span>

<span data-ttu-id="ce14a-171">`baseItem` の種類は直接使用できません。</span><span class="sxs-lookup"><span data-stu-id="ce14a-171">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->

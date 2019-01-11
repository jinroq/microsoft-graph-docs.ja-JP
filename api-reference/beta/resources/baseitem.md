---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
ms.openlocfilehash: ac119ab0b63aecba384d34014f3d0d18111b05ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866249"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="cfa28-102">BaseItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cfa28-102">BaseItem resource type</span></span>

> <span data-ttu-id="cfa28-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cfa28-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfa28-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfa28-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cfa28-p102">**baseItem** リソースは、他のいくつかのリソースの種類間で共有されるプロパティの共通セットを含む抽象リソースです。**baseItem** から派生するリソースには以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cfa28-p102">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="cfa28-107">drive</span><span class="sxs-lookup"><span data-stu-id="cfa28-107">drive</span></span>](drive.md)
* [<span data-ttu-id="cfa28-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="cfa28-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="cfa28-109">site</span><span class="sxs-lookup"><span data-stu-id="cfa28-109">site</span></span>](site.md)
* [<span data-ttu-id="cfa28-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="cfa28-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="cfa28-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cfa28-111">JSON representation</span></span>

<span data-ttu-id="cfa28-112">以下は、**baseItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cfa28-112">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
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

## <a name="properties"></a><span data-ttu-id="cfa28-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfa28-113">Properties</span></span>

| <span data-ttu-id="cfa28-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfa28-114">Property</span></span>             | <span data-ttu-id="cfa28-115">種類</span><span class="sxs-lookup"><span data-stu-id="cfa28-115">Type</span></span>              | <span data-ttu-id="cfa28-116">説明</span><span class="sxs-lookup"><span data-stu-id="cfa28-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="cfa28-117">ID</span><span class="sxs-lookup"><span data-stu-id="cfa28-117">id</span></span>                   | <span data-ttu-id="cfa28-118">文字列</span><span class="sxs-lookup"><span data-stu-id="cfa28-118">string</span></span>            | <span data-ttu-id="cfa28-p103">ドライブの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfa28-p103">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="cfa28-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="cfa28-121">createdBy</span></span>            | <span data-ttu-id="cfa28-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="cfa28-122">[identitySet][]</span></span>   | <span data-ttu-id="cfa28-p104">アイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfa28-p104">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="cfa28-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfa28-125">createdDateTime</span></span>      | <span data-ttu-id="cfa28-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfa28-126">dateTimeOffset</span></span>    | <span data-ttu-id="cfa28-p105">アイテム作成の日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfa28-p105">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="cfa28-129">eTag</span><span class="sxs-lookup"><span data-stu-id="cfa28-129">eTag</span></span>                 | <span data-ttu-id="cfa28-130">文字列</span><span class="sxs-lookup"><span data-stu-id="cfa28-130">string</span></span>            | <span data-ttu-id="cfa28-p106">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfa28-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="cfa28-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="cfa28-133">lastModifiedBy</span></span>       | <span data-ttu-id="cfa28-134">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="cfa28-134">[identitySet][]</span></span>   | <span data-ttu-id="cfa28-p107">アイテムを最終更新したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfa28-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="cfa28-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfa28-137">lastModifiedDateTime</span></span> | <span data-ttu-id="cfa28-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfa28-138">dateTimeOffset</span></span>    | <span data-ttu-id="cfa28-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfa28-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="cfa28-141">name</span><span class="sxs-lookup"><span data-stu-id="cfa28-141">name</span></span>                 | <span data-ttu-id="cfa28-142">文字列</span><span class="sxs-lookup"><span data-stu-id="cfa28-142">string</span></span>            | <span data-ttu-id="cfa28-p109">アイテムの名前。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="cfa28-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="cfa28-145">parentReference</span><span class="sxs-lookup"><span data-stu-id="cfa28-145">parentReference</span></span>      | <span data-ttu-id="cfa28-146">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="cfa28-146">[itemReference][]</span></span> | <span data-ttu-id="cfa28-p110">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="cfa28-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="cfa28-149">webUrl</span><span class="sxs-lookup"><span data-stu-id="cfa28-149">webUrl</span></span>               | <span data-ttu-id="cfa28-150">string (URL)</span><span class="sxs-lookup"><span data-stu-id="cfa28-150">string (url)</span></span>      | <span data-ttu-id="cfa28-p111">ブラウザーでリソースを表示するための URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cfa28-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="cfa28-155">備考</span><span class="sxs-lookup"><span data-stu-id="cfa28-155">Remarks</span></span>

<span data-ttu-id="cfa28-156">`baseItem` の種類は直接使用できません。</span><span class="sxs-lookup"><span data-stu-id="cfa28-156">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->

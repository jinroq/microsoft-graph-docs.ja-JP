---
title: itemAttachment リソースの種類
description: '別のイベント、メッセージ、または投稿に添付された連絡先、イベント、またはメッセージです。  '
localization_priority: Priority
ms.openlocfilehash: df996175e545b78f4ca9a1b6271b9cb012ffffce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584818"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="4008b-103">itemAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4008b-103">itemAttachment resource type</span></span>

<span data-ttu-id="4008b-104">別のイベント、メッセージ、または投稿に添付された連絡先、イベント、またはメッセージです。</span><span class="sxs-lookup"><span data-stu-id="4008b-104">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="4008b-105">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="4008b-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4008b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4008b-106">Methods</span></span>

| <span data-ttu-id="4008b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4008b-107">Method</span></span>       | <span data-ttu-id="4008b-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4008b-108">Return Type</span></span>  |<span data-ttu-id="4008b-109">説明</span><span class="sxs-lookup"><span data-stu-id="4008b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4008b-110">取得</span><span class="sxs-lookup"><span data-stu-id="4008b-110">Get</span></span>](../api/attachment-get.md) | <span data-ttu-id="4008b-111">[itemAttachment](itemattachment.md)</span><span class="sxs-lookup"><span data-stu-id="4008b-111">[itemAttachment](itemattachment.md),</span></span> |<span data-ttu-id="4008b-112">itemAttachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4008b-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="4008b-113">Delete</span><span class="sxs-lookup"><span data-stu-id="4008b-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="4008b-114">なし</span><span class="sxs-lookup"><span data-stu-id="4008b-114">None</span></span> |<span data-ttu-id="4008b-115">itemAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="4008b-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4008b-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4008b-116">Properties</span></span>
| <span data-ttu-id="4008b-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4008b-117">Property</span></span>     | <span data-ttu-id="4008b-118">型</span><span class="sxs-lookup"><span data-stu-id="4008b-118">Type</span></span>   |<span data-ttu-id="4008b-119">説明</span><span class="sxs-lookup"><span data-stu-id="4008b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4008b-120">contentType</span><span class="sxs-lookup"><span data-stu-id="4008b-120">contentType</span></span>|<span data-ttu-id="4008b-121">String</span><span class="sxs-lookup"><span data-stu-id="4008b-121">String</span></span>|<span data-ttu-id="4008b-122">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="4008b-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="4008b-123">id</span><span class="sxs-lookup"><span data-stu-id="4008b-123">id</span></span>|<span data-ttu-id="4008b-124">String</span><span class="sxs-lookup"><span data-stu-id="4008b-124">String</span></span>| <span data-ttu-id="4008b-125">添付ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="4008b-125">The attachment ID.</span></span>|
|<span data-ttu-id="4008b-126">isInline</span><span class="sxs-lookup"><span data-stu-id="4008b-126">isInline</span></span>|<span data-ttu-id="4008b-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="4008b-127">Boolean</span></span>|<span data-ttu-id="4008b-128">添付ファイルがインライン (アイテムの本文に埋め込まれた画像など) の場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="4008b-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="4008b-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4008b-129">lastModifiedDateTime</span></span>|<span data-ttu-id="4008b-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4008b-130">DateTimeOffset</span></span>|<span data-ttu-id="4008b-131">添付ファイルが変更された最後の日時です。</span><span class="sxs-lookup"><span data-stu-id="4008b-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="4008b-132">name</span><span class="sxs-lookup"><span data-stu-id="4008b-132">name</span></span>|<span data-ttu-id="4008b-133">String</span><span class="sxs-lookup"><span data-stu-id="4008b-133">String</span></span>|<span data-ttu-id="4008b-134">添付ファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="4008b-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="4008b-135">size</span><span class="sxs-lookup"><span data-stu-id="4008b-135">size</span></span>|<span data-ttu-id="4008b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4008b-136">Int32</span></span>|<span data-ttu-id="4008b-137">添付ファイルのバイト単位のサイズ。</span><span class="sxs-lookup"><span data-stu-id="4008b-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4008b-138">関係</span><span class="sxs-lookup"><span data-stu-id="4008b-138">Relationships</span></span>
| <span data-ttu-id="4008b-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4008b-139">Relationship</span></span> | <span data-ttu-id="4008b-140">型</span><span class="sxs-lookup"><span data-stu-id="4008b-140">Type</span></span>   |<span data-ttu-id="4008b-141">説明</span><span class="sxs-lookup"><span data-stu-id="4008b-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4008b-142">item</span><span class="sxs-lookup"><span data-stu-id="4008b-142">item</span></span>|[<span data-ttu-id="4008b-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="4008b-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="4008b-p101">添付されたメッセージまたはイベントです。ナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="4008b-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4008b-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4008b-146">JSON representation</span></span>

<span data-ttu-id="4008b-147">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4008b-147">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

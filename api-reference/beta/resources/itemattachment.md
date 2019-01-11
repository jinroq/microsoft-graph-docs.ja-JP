---
title: itemAttachment リソースの種類
description: 連絡先、イベント、または別のイベントに関連付けられているメッセージ
localization_priority: Normal
ms.openlocfilehash: f7372db19a545bd7d6ae39121fd14be4c9f4436b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825005"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="fad2f-103">itemAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fad2f-103">itemAttachment resource type</span></span>

> <span data-ttu-id="fad2f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fad2f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fad2f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fad2f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fad2f-106">連絡先、イベント、または他の[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または[投稿](../resources/post.md)に添付されているメッセージです。</span><span class="sxs-lookup"><span data-stu-id="fad2f-106">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="fad2f-107">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="fad2f-107">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fad2f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fad2f-108">Methods</span></span>

| <span data-ttu-id="fad2f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="fad2f-109">Method</span></span>       | <span data-ttu-id="fad2f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fad2f-110">Return Type</span></span>  |<span data-ttu-id="fad2f-111">説明</span><span class="sxs-lookup"><span data-stu-id="fad2f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fad2f-112">Get</span><span class="sxs-lookup"><span data-stu-id="fad2f-112">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="fad2f-113">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="fad2f-113">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="fad2f-114">itemAttachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fad2f-114">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="fad2f-115">Delete</span><span class="sxs-lookup"><span data-stu-id="fad2f-115">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="fad2f-116">なし</span><span class="sxs-lookup"><span data-stu-id="fad2f-116">None</span></span> |<span data-ttu-id="fad2f-117">itemAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="fad2f-117">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fad2f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fad2f-118">Properties</span></span>
| <span data-ttu-id="fad2f-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fad2f-119">Property</span></span>     | <span data-ttu-id="fad2f-120">種類</span><span class="sxs-lookup"><span data-stu-id="fad2f-120">Type</span></span>   |<span data-ttu-id="fad2f-121">説明</span><span class="sxs-lookup"><span data-stu-id="fad2f-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fad2f-122">contentType</span><span class="sxs-lookup"><span data-stu-id="fad2f-122">contentType</span></span>|<span data-ttu-id="fad2f-123">String</span><span class="sxs-lookup"><span data-stu-id="fad2f-123">String</span></span>|<span data-ttu-id="fad2f-124">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="fad2f-124">The content type of the attachment.</span></span>|
|<span data-ttu-id="fad2f-125">id</span><span class="sxs-lookup"><span data-stu-id="fad2f-125">id</span></span>|<span data-ttu-id="fad2f-126">String</span><span class="sxs-lookup"><span data-stu-id="fad2f-126">String</span></span>| <span data-ttu-id="fad2f-127">添付ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="fad2f-127">The attachment ID.</span></span>|
|<span data-ttu-id="fad2f-128">isInline</span><span class="sxs-lookup"><span data-stu-id="fad2f-128">isInline</span></span>|<span data-ttu-id="fad2f-129">ブール値</span><span class="sxs-lookup"><span data-stu-id="fad2f-129">Boolean</span></span>|<span data-ttu-id="fad2f-130">添付ファイルがインライン (アイテムの本文に埋め込まれた画像など) の場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="fad2f-130">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="fad2f-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fad2f-131">lastModifiedDateTime</span></span>|<span data-ttu-id="fad2f-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fad2f-132">DateTimeOffset</span></span>|<span data-ttu-id="fad2f-133">添付ファイルが変更された最後の日時です。</span><span class="sxs-lookup"><span data-stu-id="fad2f-133">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="fad2f-134">name</span><span class="sxs-lookup"><span data-stu-id="fad2f-134">name</span></span>|<span data-ttu-id="fad2f-135">String</span><span class="sxs-lookup"><span data-stu-id="fad2f-135">String</span></span>|<span data-ttu-id="fad2f-136">添付ファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="fad2f-136">The display name of the attachment.</span></span>|
|<span data-ttu-id="fad2f-137">size</span><span class="sxs-lookup"><span data-stu-id="fad2f-137">size</span></span>|<span data-ttu-id="fad2f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="fad2f-138">Int32</span></span>|<span data-ttu-id="fad2f-139">添付ファイルのバイト単位のサイズ。</span><span class="sxs-lookup"><span data-stu-id="fad2f-139">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fad2f-140">関係</span><span class="sxs-lookup"><span data-stu-id="fad2f-140">Relationships</span></span>
| <span data-ttu-id="fad2f-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fad2f-141">Relationship</span></span> | <span data-ttu-id="fad2f-142">型</span><span class="sxs-lookup"><span data-stu-id="fad2f-142">Type</span></span>   |<span data-ttu-id="fad2f-143">説明</span><span class="sxs-lookup"><span data-stu-id="fad2f-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fad2f-144">item</span><span class="sxs-lookup"><span data-stu-id="fad2f-144">item</span></span>|[<span data-ttu-id="fad2f-145">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="fad2f-145">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="fad2f-146">添付されている連絡先、メッセージまたはイベントです。</span><span class="sxs-lookup"><span data-stu-id="fad2f-146">The attached contact, message or event.</span></span> <span data-ttu-id="fad2f-147">ナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="fad2f-147">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fad2f-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fad2f-148">JSON representation</span></span>

<span data-ttu-id="fad2f-149">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="fad2f-149">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "@odata.type": "microsoft.graph.itemAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
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

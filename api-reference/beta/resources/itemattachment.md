---
title: itemAttachment リソースの種類
description: 別のイベントに添付されている連絡先、イベント、またはメッセージ
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 31fd3e74e7fc35589abc57a891678e9a129c2a2e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010085"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="2c3c2-103">itemAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c3c2-103">itemAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c3c2-104">別の[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook タスク](../resources/outlooktask.md)、または[投稿](../resources/post.md)に添付されている連絡先、イベント、またはメッセージ。</span><span class="sxs-lookup"><span data-stu-id="2c3c2-104">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="2c3c2-105">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="2c3c2-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2c3c2-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2c3c2-106">Methods</span></span>

| <span data-ttu-id="2c3c2-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2c3c2-107">Method</span></span>       | <span data-ttu-id="2c3c2-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2c3c2-108">Return Type</span></span>  |<span data-ttu-id="2c3c2-109">説明</span><span class="sxs-lookup"><span data-stu-id="2c3c2-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c3c2-110">取得</span><span class="sxs-lookup"><span data-stu-id="2c3c2-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="2c3c2-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="2c3c2-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="2c3c2-112">itemAttachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2c3c2-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="2c3c2-113">Delete</span><span class="sxs-lookup"><span data-stu-id="2c3c2-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="2c3c2-114">なし</span><span class="sxs-lookup"><span data-stu-id="2c3c2-114">None</span></span> |<span data-ttu-id="2c3c2-115">itemAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="2c3c2-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2c3c2-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c3c2-116">Properties</span></span>
| <span data-ttu-id="2c3c2-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c3c2-117">Property</span></span>     | <span data-ttu-id="2c3c2-118">型</span><span class="sxs-lookup"><span data-stu-id="2c3c2-118">Type</span></span>   |<span data-ttu-id="2c3c2-119">説明</span><span class="sxs-lookup"><span data-stu-id="2c3c2-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c3c2-120">contentType</span><span class="sxs-lookup"><span data-stu-id="2c3c2-120">contentType</span></span>|<span data-ttu-id="2c3c2-121">String</span><span class="sxs-lookup"><span data-stu-id="2c3c2-121">String</span></span>|<span data-ttu-id="2c3c2-122">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="2c3c2-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="2c3c2-123">id</span><span class="sxs-lookup"><span data-stu-id="2c3c2-123">id</span></span>|<span data-ttu-id="2c3c2-124">String</span><span class="sxs-lookup"><span data-stu-id="2c3c2-124">String</span></span>| <span data-ttu-id="2c3c2-125">添付ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="2c3c2-125">The attachment ID.</span></span>|
|<span data-ttu-id="2c3c2-126">isInline</span><span class="sxs-lookup"><span data-stu-id="2c3c2-126">isInline</span></span>|<span data-ttu-id="2c3c2-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c3c2-127">Boolean</span></span>|<span data-ttu-id="2c3c2-128">添付ファイルがインライン (アイテムの本文に埋め込まれた画像など) の場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="2c3c2-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="2c3c2-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c3c2-129">lastModifiedDateTime</span></span>|<span data-ttu-id="2c3c2-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c3c2-130">DateTimeOffset</span></span>|<span data-ttu-id="2c3c2-131">添付ファイルが変更された最後の日時です。</span><span class="sxs-lookup"><span data-stu-id="2c3c2-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="2c3c2-132">name</span><span class="sxs-lookup"><span data-stu-id="2c3c2-132">name</span></span>|<span data-ttu-id="2c3c2-133">String</span><span class="sxs-lookup"><span data-stu-id="2c3c2-133">String</span></span>|<span data-ttu-id="2c3c2-134">添付ファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="2c3c2-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="2c3c2-135">size</span><span class="sxs-lookup"><span data-stu-id="2c3c2-135">size</span></span>|<span data-ttu-id="2c3c2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2c3c2-136">Int32</span></span>|<span data-ttu-id="2c3c2-137">添付ファイルのバイト単位のサイズ。</span><span class="sxs-lookup"><span data-stu-id="2c3c2-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c3c2-138">関係</span><span class="sxs-lookup"><span data-stu-id="2c3c2-138">Relationships</span></span>
| <span data-ttu-id="2c3c2-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2c3c2-139">Relationship</span></span> | <span data-ttu-id="2c3c2-140">型</span><span class="sxs-lookup"><span data-stu-id="2c3c2-140">Type</span></span>   |<span data-ttu-id="2c3c2-141">説明</span><span class="sxs-lookup"><span data-stu-id="2c3c2-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c3c2-142">item</span><span class="sxs-lookup"><span data-stu-id="2c3c2-142">item</span></span>|[<span data-ttu-id="2c3c2-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="2c3c2-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="2c3c2-144">添付された連絡先、メッセージ、またはイベント。</span><span class="sxs-lookup"><span data-stu-id="2c3c2-144">The attached contact, message or event.</span></span> <span data-ttu-id="2c3c2-145">ナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="2c3c2-145">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c3c2-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c3c2-146">JSON representation</span></span>

<span data-ttu-id="2c3c2-147">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2c3c2-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
<!--
{
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

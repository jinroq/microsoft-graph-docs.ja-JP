---
title: itemAttachment リソースの種類
description: 連絡先、イベント、または別のイベントに関連付けられているメッセージ
localization_priority: Normal
ms.openlocfilehash: cce33cb7597f04435daff723a0125305968eea99
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520110"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="552c1-103">itemAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="552c1-103">itemAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="552c1-104">連絡先、イベント、または他の[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または[投稿](../resources/post.md)に添付されているメッセージです。</span><span class="sxs-lookup"><span data-stu-id="552c1-104">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="552c1-105">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="552c1-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="552c1-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="552c1-106">Methods</span></span>

| <span data-ttu-id="552c1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="552c1-107">Method</span></span>       | <span data-ttu-id="552c1-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="552c1-108">Return Type</span></span>  |<span data-ttu-id="552c1-109">説明</span><span class="sxs-lookup"><span data-stu-id="552c1-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="552c1-110">Get</span><span class="sxs-lookup"><span data-stu-id="552c1-110">Get</span></span>](../api/attachment-get.md) | <span data-ttu-id="552c1-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="552c1-111">[itemAttachment](itemattachment.md)</span></span> |<span data-ttu-id="552c1-112">itemAttachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="552c1-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="552c1-113">Delete</span><span class="sxs-lookup"><span data-stu-id="552c1-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="552c1-114">なし</span><span class="sxs-lookup"><span data-stu-id="552c1-114">None</span></span> |<span data-ttu-id="552c1-115">itemAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="552c1-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="552c1-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="552c1-116">Properties</span></span>
| <span data-ttu-id="552c1-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="552c1-117">Property</span></span>     | <span data-ttu-id="552c1-118">型</span><span class="sxs-lookup"><span data-stu-id="552c1-118">Type</span></span>   |<span data-ttu-id="552c1-119">説明</span><span class="sxs-lookup"><span data-stu-id="552c1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="552c1-120">contentType</span><span class="sxs-lookup"><span data-stu-id="552c1-120">contentType</span></span>|<span data-ttu-id="552c1-121">String</span><span class="sxs-lookup"><span data-stu-id="552c1-121">String</span></span>|<span data-ttu-id="552c1-122">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="552c1-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="552c1-123">id</span><span class="sxs-lookup"><span data-stu-id="552c1-123">id</span></span>|<span data-ttu-id="552c1-124">String</span><span class="sxs-lookup"><span data-stu-id="552c1-124">String</span></span>| <span data-ttu-id="552c1-125">添付ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="552c1-125">The attachment ID.</span></span>|
|<span data-ttu-id="552c1-126">isInline</span><span class="sxs-lookup"><span data-stu-id="552c1-126">isInline</span></span>|<span data-ttu-id="552c1-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="552c1-127">Boolean</span></span>|<span data-ttu-id="552c1-128">添付ファイルがインライン (アイテムの本文に埋め込まれた画像など) の場合に、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="552c1-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="552c1-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="552c1-129">lastModifiedDateTime</span></span>|<span data-ttu-id="552c1-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="552c1-130">DateTimeOffset</span></span>|<span data-ttu-id="552c1-131">添付ファイルが変更された最後の日時です。</span><span class="sxs-lookup"><span data-stu-id="552c1-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="552c1-132">name</span><span class="sxs-lookup"><span data-stu-id="552c1-132">name</span></span>|<span data-ttu-id="552c1-133">String</span><span class="sxs-lookup"><span data-stu-id="552c1-133">String</span></span>|<span data-ttu-id="552c1-134">添付ファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="552c1-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="552c1-135">size</span><span class="sxs-lookup"><span data-stu-id="552c1-135">size</span></span>|<span data-ttu-id="552c1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="552c1-136">Int32</span></span>|<span data-ttu-id="552c1-137">添付ファイルのバイト単位のサイズ。</span><span class="sxs-lookup"><span data-stu-id="552c1-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="552c1-138">関係</span><span class="sxs-lookup"><span data-stu-id="552c1-138">Relationships</span></span>
| <span data-ttu-id="552c1-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="552c1-139">Relationship</span></span> | <span data-ttu-id="552c1-140">型</span><span class="sxs-lookup"><span data-stu-id="552c1-140">Type</span></span>   |<span data-ttu-id="552c1-141">説明</span><span class="sxs-lookup"><span data-stu-id="552c1-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="552c1-142">item</span><span class="sxs-lookup"><span data-stu-id="552c1-142">item</span></span>|<span data-ttu-id="552c1-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="552c1-143">[OutlookItem](outlookitem.md)</span></span>|<span data-ttu-id="552c1-144">添付されている連絡先、メッセージまたはイベントです。</span><span class="sxs-lookup"><span data-stu-id="552c1-144">The attached contact, message or event.</span></span> <span data-ttu-id="552c1-145">ナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="552c1-145">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="552c1-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="552c1-146">JSON representation</span></span>

<span data-ttu-id="552c1-147">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="552c1-147">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: 添付ファイル リソースの種類
description: 関連コンテンツをイベントに追加できます。
localization_priority: Priority
ms.openlocfilehash: 284895871a0c6a80140ff248045b89d2de104c20
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569383"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="b582a-103">添付ファイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b582a-103">attachment resource type</span></span>

<span data-ttu-id="b582a-104">関連コンテンツを添付ファイルの形式で[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、または[投稿](../resources/post.md)に追加できます。</span><span class="sxs-lookup"><span data-stu-id="b582a-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="b582a-105">**attachment** は、次の派生型の添付ファイルの基本リソースです。</span><span class="sxs-lookup"><span data-stu-id="b582a-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="b582a-106">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)</span><span class="sxs-lookup"><span data-stu-id="b582a-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="b582a-107">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、またはメッセージ)</span><span class="sxs-lookup"><span data-stu-id="b582a-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="b582a-108">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)</span><span class="sxs-lookup"><span data-stu-id="b582a-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>


## <a name="methods"></a><span data-ttu-id="b582a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b582a-109">Methods</span></span>

<span data-ttu-id="b582a-110">次のメソッドは、派生型の添付ファイル (**fileAttachment**、**itemAttachment**、または **referenceAttachment**) のすべてに適用されます。</span><span class="sxs-lookup"><span data-stu-id="b582a-110">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="b582a-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="b582a-111">Method</span></span>       | <span data-ttu-id="b582a-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b582a-112">Return Type</span></span>  |<span data-ttu-id="b582a-113">説明</span><span class="sxs-lookup"><span data-stu-id="b582a-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b582a-114">添付ファイルを取得する</span><span class="sxs-lookup"><span data-stu-id="b582a-114">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="b582a-115">attachment</span><span class="sxs-lookup"><span data-stu-id="b582a-115">attachment</span></span>](attachment.md) |<span data-ttu-id="b582a-116">イベント、メッセージ、または投稿に添付されている添付ファイルのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b582a-116">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="b582a-117">イベントに添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="b582a-117">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="b582a-118">attachment</span><span class="sxs-lookup"><span data-stu-id="b582a-118">attachment</span></span>](attachment.md) |<span data-ttu-id="b582a-119">ファイル、アイテム、またはリンクの添付ファイルをイベントに追加します。</span><span class="sxs-lookup"><span data-stu-id="b582a-119">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="b582a-120">メッセージに添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="b582a-120">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="b582a-121">attachment</span><span class="sxs-lookup"><span data-stu-id="b582a-121">attachment</span></span>](attachment.md) |<span data-ttu-id="b582a-122">ファイル、アイテム、またはリンクの添付ファイルをメッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="b582a-122">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="b582a-123">投稿に添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="b582a-123">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="b582a-124">attachment</span><span class="sxs-lookup"><span data-stu-id="b582a-124">attachment</span></span>](attachment.md) |<span data-ttu-id="b582a-125">ファイル、アイテム、またはリンクの添付ファイルを投稿に追加します。</span><span class="sxs-lookup"><span data-stu-id="b582a-125">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="b582a-126">イベントの添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b582a-126">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="b582a-127">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b582a-127">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="b582a-128">イベントの添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b582a-128">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="b582a-129">メッセージの添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b582a-129">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="b582a-130">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b582a-130">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="b582a-131">メッセージの添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b582a-131">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="b582a-132">投稿の添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b582a-132">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="b582a-133">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b582a-133">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="b582a-134">投稿の添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b582a-134">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="b582a-135">削除</span><span class="sxs-lookup"><span data-stu-id="b582a-135">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="b582a-136">None</span><span class="sxs-lookup"><span data-stu-id="b582a-136">None</span></span> |<span data-ttu-id="b582a-137">イベント、メッセージ、または投稿の添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="b582a-137">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="b582a-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b582a-138">Properties</span></span>

<span data-ttu-id="b582a-p101">次に、添付ファイル リソースの基本プロパティを示します。他のプロパティについては、特定の種類の添付ファイル ([fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md)、または [referenceAttachment](../resources/referenceattachment.md)) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b582a-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="b582a-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b582a-141">Property</span></span>     | <span data-ttu-id="b582a-142">型</span><span class="sxs-lookup"><span data-stu-id="b582a-142">Type</span></span>   |<span data-ttu-id="b582a-143">説明</span><span class="sxs-lookup"><span data-stu-id="b582a-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b582a-144">contentType</span><span class="sxs-lookup"><span data-stu-id="b582a-144">contentType</span></span>|<span data-ttu-id="b582a-145">String</span><span class="sxs-lookup"><span data-stu-id="b582a-145">String</span></span>|<span data-ttu-id="b582a-146">MIME タイプ。</span><span class="sxs-lookup"><span data-stu-id="b582a-146">The MIME type.</span></span>|
|<span data-ttu-id="b582a-147">id</span><span class="sxs-lookup"><span data-stu-id="b582a-147">id</span></span>|<span data-ttu-id="b582a-148">String</span><span class="sxs-lookup"><span data-stu-id="b582a-148">String</span></span>| <span data-ttu-id="b582a-149">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b582a-149">Read-only.</span></span>|
|<span data-ttu-id="b582a-150">isInline</span><span class="sxs-lookup"><span data-stu-id="b582a-150">isInline</span></span>|<span data-ttu-id="b582a-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="b582a-151">Boolean</span></span>|<span data-ttu-id="b582a-152">添付ファイルがインライン添付ファイルの場合は `true`、それ以外の場合は `false`。</span><span class="sxs-lookup"><span data-stu-id="b582a-152">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="b582a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b582a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b582a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b582a-154">DateTimeOffset</span></span>|<span data-ttu-id="b582a-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b582a-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b582a-157">name</span><span class="sxs-lookup"><span data-stu-id="b582a-157">name</span></span>|<span data-ttu-id="b582a-158">String</span><span class="sxs-lookup"><span data-stu-id="b582a-158">String</span></span>|<span data-ttu-id="b582a-159">添付ファイルのファイル名。</span><span class="sxs-lookup"><span data-stu-id="b582a-159">The attachment's file name.</span></span>|
|<span data-ttu-id="b582a-160">size</span><span class="sxs-lookup"><span data-stu-id="b582a-160">size</span></span>|<span data-ttu-id="b582a-161">Int32</span><span class="sxs-lookup"><span data-stu-id="b582a-161">Int32</span></span>|<span data-ttu-id="b582a-162">添付ファイルの長さ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="b582a-162">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b582a-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b582a-163">Relationships</span></span>
<span data-ttu-id="b582a-164">なし</span><span class="sxs-lookup"><span data-stu-id="b582a-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b582a-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b582a-165">JSON representation</span></span>

<span data-ttu-id="b582a-166">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b582a-166">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
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
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

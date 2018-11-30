---
title: 添付ファイル リソースの種類
description: イベントに関連するコンテンツを追加します。
ms.openlocfilehash: f0bb9ec37d2fe3d034dce9532ad316d371c4937e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073811"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="a3707-103">添付ファイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a3707-103">attachment resource type</span></span>

> <span data-ttu-id="a3707-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a3707-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3707-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3707-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3707-106">[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または添付ファイルの形式での[投稿](../resources/post.md)に関連するコンテンツを追加できます。</span><span class="sxs-lookup"><span data-stu-id="a3707-106">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="a3707-107">**attachment** は、次の派生型の添付ファイルの基本リソースです。</span><span class="sxs-lookup"><span data-stu-id="a3707-107">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="a3707-108">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)</span><span class="sxs-lookup"><span data-stu-id="a3707-108">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="a3707-109">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、またはメッセージ)</span><span class="sxs-lookup"><span data-stu-id="a3707-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="a3707-110">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)</span><span class="sxs-lookup"><span data-stu-id="a3707-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="a3707-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="a3707-111">Methods</span></span>

<span data-ttu-id="a3707-112">次のメソッドは、派生型の添付ファイル (**fileAttachment**、**itemAttachment**、または **referenceAttachment**) のすべてに適用されます。</span><span class="sxs-lookup"><span data-stu-id="a3707-112">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="a3707-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="a3707-113">Method</span></span>       | <span data-ttu-id="a3707-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a3707-114">Return Type</span></span>  |<span data-ttu-id="a3707-115">説明</span><span class="sxs-lookup"><span data-stu-id="a3707-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a3707-116">添付ファイルを取得する</span><span class="sxs-lookup"><span data-stu-id="a3707-116">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="a3707-117">attachment</span><span class="sxs-lookup"><span data-stu-id="a3707-117">attachment</span></span>](attachment.md) |<span data-ttu-id="a3707-118">プロパティとイベント、メッセージ、Outlook のタスク、または投稿に添付された添付ファイルの関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3707-118">Read the properties and relationships of an attachment, attached to an event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="a3707-119">イベントに添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="a3707-119">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="a3707-120">attachment</span><span class="sxs-lookup"><span data-stu-id="a3707-120">attachment</span></span>](attachment.md) |<span data-ttu-id="a3707-121">ファイル、アイテム、またはリンクの添付ファイルをイベントに追加します。</span><span class="sxs-lookup"><span data-stu-id="a3707-121">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="a3707-122">メッセージに添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="a3707-122">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="a3707-123">attachment</span><span class="sxs-lookup"><span data-stu-id="a3707-123">attachment</span></span>](attachment.md) |<span data-ttu-id="a3707-124">ファイル、アイテム、またはリンクの添付ファイルをメッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="a3707-124">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="a3707-125">Outlook のタスクに添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="a3707-125">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="a3707-126">attachment</span><span class="sxs-lookup"><span data-stu-id="a3707-126">attachment</span></span>](attachment.md) |<span data-ttu-id="a3707-127">ファイル、アイテム、またはリンクの添付ファイルを Outlook のタスクを追加します。</span><span class="sxs-lookup"><span data-stu-id="a3707-127">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="a3707-128">投稿に添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="a3707-128">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="a3707-129">attachment</span><span class="sxs-lookup"><span data-stu-id="a3707-129">attachment</span></span>](attachment.md) |<span data-ttu-id="a3707-130">ファイル、アイテム、またはリンクの添付ファイルを投稿に追加します。</span><span class="sxs-lookup"><span data-stu-id="a3707-130">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="a3707-131">イベントの添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a3707-131">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="a3707-132">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a3707-132">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="a3707-133">イベントの添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3707-133">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="a3707-134">メッセージの添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a3707-134">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="a3707-135">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a3707-135">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="a3707-136">メッセージの添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3707-136">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="a3707-137">Outlook の仕事リストの添付ファイル</span><span class="sxs-lookup"><span data-stu-id="a3707-137">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="a3707-138">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a3707-138">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="a3707-139">Outlook のタスクの添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3707-139">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="a3707-140">投稿の添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a3707-140">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="a3707-141">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a3707-141">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="a3707-142">投稿の添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3707-142">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="a3707-143">削除</span><span class="sxs-lookup"><span data-stu-id="a3707-143">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="a3707-144">なし</span><span class="sxs-lookup"><span data-stu-id="a3707-144">None</span></span> |<span data-ttu-id="a3707-145">イベント、メッセージ、Outlook のタスク、または投稿の添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="a3707-145">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="a3707-146">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3707-146">Properties</span></span>

<span data-ttu-id="a3707-p102">次に、添付ファイル リソースの基本プロパティを示します。他のプロパティについては、特定の種類の添付ファイル ([fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md)、または [referenceAttachment](../resources/referenceattachment.md)) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3707-p102">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="a3707-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3707-149">Property</span></span>     | <span data-ttu-id="a3707-150">型</span><span class="sxs-lookup"><span data-stu-id="a3707-150">Type</span></span>   |<span data-ttu-id="a3707-151">説明</span><span class="sxs-lookup"><span data-stu-id="a3707-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3707-152">contentType</span><span class="sxs-lookup"><span data-stu-id="a3707-152">contentType</span></span>|<span data-ttu-id="a3707-153">String</span><span class="sxs-lookup"><span data-stu-id="a3707-153">String</span></span>|<span data-ttu-id="a3707-154">MIME タイプ。</span><span class="sxs-lookup"><span data-stu-id="a3707-154">The MIME type.</span></span>|
|<span data-ttu-id="a3707-155">id</span><span class="sxs-lookup"><span data-stu-id="a3707-155">id</span></span>|<span data-ttu-id="a3707-156">String</span><span class="sxs-lookup"><span data-stu-id="a3707-156">String</span></span>| <span data-ttu-id="a3707-157">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a3707-157">Read-only.</span></span>|
|<span data-ttu-id="a3707-158">isInline</span><span class="sxs-lookup"><span data-stu-id="a3707-158">isInline</span></span>|<span data-ttu-id="a3707-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3707-159">Boolean</span></span>|<span data-ttu-id="a3707-160">添付ファイルがインライン添付ファイルの場合は `true`、それ以外の場合は `false`。</span><span class="sxs-lookup"><span data-stu-id="a3707-160">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="a3707-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3707-161">lastModifiedDateTime</span></span>|<span data-ttu-id="a3707-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3707-162">DateTimeOffset</span></span>|<span data-ttu-id="a3707-p103">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a3707-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a3707-165">name</span><span class="sxs-lookup"><span data-stu-id="a3707-165">name</span></span>|<span data-ttu-id="a3707-166">String</span><span class="sxs-lookup"><span data-stu-id="a3707-166">String</span></span>|<span data-ttu-id="a3707-p104">添付ファイルの表示名。実際のファイル名である必要はありません。</span><span class="sxs-lookup"><span data-stu-id="a3707-p104">The display name of the attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="a3707-169">size</span><span class="sxs-lookup"><span data-stu-id="a3707-169">size</span></span>|<span data-ttu-id="a3707-170">Int32</span><span class="sxs-lookup"><span data-stu-id="a3707-170">Int32</span></span>|<span data-ttu-id="a3707-171">添付ファイルの長さ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="a3707-171">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3707-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a3707-172">Relationships</span></span>
<span data-ttu-id="a3707-173">なし</span><span class="sxs-lookup"><span data-stu-id="a3707-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3707-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a3707-174">JSON representation</span></span>

<span data-ttu-id="a3707-175">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a3707-175">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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

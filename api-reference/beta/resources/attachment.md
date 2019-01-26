---
title: 添付ファイル リソースの種類
description: イベントに関連するコンテンツを追加します。
localization_priority: Normal
ms.openlocfilehash: 8f7a6f9392d376995a53d9a4c06083780b0437b9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573425"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="dbdbf-103">添付ファイル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dbdbf-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbdbf-104">[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または添付ファイルの形式での[投稿](../resources/post.md)に関連するコンテンツを追加できます。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="dbdbf-105">**attachment** は、次の派生型の添付ファイルの基本リソースです。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="dbdbf-106">ファイル ([fileAttachment](../resources/fileattachment.md) リソース)</span><span class="sxs-lookup"><span data-stu-id="dbdbf-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="dbdbf-107">項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、またはメッセージ)</span><span class="sxs-lookup"><span data-stu-id="dbdbf-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="dbdbf-108">ファイルへのリンク ([referenceAttachment](../resources/referenceattachment.md) リソース)</span><span class="sxs-lookup"><span data-stu-id="dbdbf-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="dbdbf-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="dbdbf-109">Methods</span></span>

<span data-ttu-id="dbdbf-110">次のメソッドは、派生型の添付ファイル (**fileAttachment**、**itemAttachment**、または **referenceAttachment**) のすべてに適用されます。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-110">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="dbdbf-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="dbdbf-111">Method</span></span>       | <span data-ttu-id="dbdbf-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dbdbf-112">Return Type</span></span>  |<span data-ttu-id="dbdbf-113">説明</span><span class="sxs-lookup"><span data-stu-id="dbdbf-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dbdbf-114">添付ファイルを取得する</span><span class="sxs-lookup"><span data-stu-id="dbdbf-114">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="dbdbf-115">attachment</span><span class="sxs-lookup"><span data-stu-id="dbdbf-115">attachment</span></span>](attachment.md) |<span data-ttu-id="dbdbf-116">プロパティとイベント、メッセージ、Outlook のタスク、または投稿に添付された添付ファイルの関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-116">Read the properties and relationships of an attachment, attached to an event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="dbdbf-117">イベントに添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="dbdbf-117">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="dbdbf-118">attachment</span><span class="sxs-lookup"><span data-stu-id="dbdbf-118">attachment</span></span>](attachment.md) |<span data-ttu-id="dbdbf-119">ファイル、アイテム、またはリンクの添付ファイルをイベントに追加します。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-119">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="dbdbf-120">メッセージに添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="dbdbf-120">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="dbdbf-121">attachment</span><span class="sxs-lookup"><span data-stu-id="dbdbf-121">attachment</span></span>](attachment.md) |<span data-ttu-id="dbdbf-122">ファイル、アイテム、またはリンクの添付ファイルをメッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-122">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="dbdbf-123">Outlook のタスクに添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-123">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="dbdbf-124">attachment</span><span class="sxs-lookup"><span data-stu-id="dbdbf-124">attachment</span></span>](attachment.md) |<span data-ttu-id="dbdbf-125">ファイル、アイテム、またはリンクの添付ファイルを Outlook のタスクを追加します。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-125">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="dbdbf-126">投稿に添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="dbdbf-126">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="dbdbf-127">attachment</span><span class="sxs-lookup"><span data-stu-id="dbdbf-127">attachment</span></span>](attachment.md) |<span data-ttu-id="dbdbf-128">ファイル、アイテム、またはリンクの添付ファイルを投稿に追加します。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-128">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="dbdbf-129">イベントの添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="dbdbf-129">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="dbdbf-130">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dbdbf-130">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="dbdbf-131">イベントの添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-131">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="dbdbf-132">メッセージの添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="dbdbf-132">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="dbdbf-133">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dbdbf-133">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="dbdbf-134">メッセージの添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-134">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="dbdbf-135">Outlook の仕事リストの添付ファイル</span><span class="sxs-lookup"><span data-stu-id="dbdbf-135">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="dbdbf-136">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dbdbf-136">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="dbdbf-137">Outlook のタスクの添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-137">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="dbdbf-138">投稿の添付ファイルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="dbdbf-138">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="dbdbf-139">[attachment](attachment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dbdbf-139">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="dbdbf-140">投稿の添付ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-140">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="dbdbf-141">削除</span><span class="sxs-lookup"><span data-stu-id="dbdbf-141">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="dbdbf-142">なし</span><span class="sxs-lookup"><span data-stu-id="dbdbf-142">None</span></span> |<span data-ttu-id="dbdbf-143">イベント、メッセージ、Outlook のタスク、または投稿の添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-143">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="dbdbf-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dbdbf-144">Properties</span></span>

<span data-ttu-id="dbdbf-p101">次に、添付ファイル リソースの基本プロパティを示します。他のプロパティについては、特定の種類の添付ファイル ([fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md)、または [referenceAttachment](../resources/referenceattachment.md)) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="dbdbf-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dbdbf-147">Property</span></span>     | <span data-ttu-id="dbdbf-148">型</span><span class="sxs-lookup"><span data-stu-id="dbdbf-148">Type</span></span>   |<span data-ttu-id="dbdbf-149">説明</span><span class="sxs-lookup"><span data-stu-id="dbdbf-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbdbf-150">contentType</span><span class="sxs-lookup"><span data-stu-id="dbdbf-150">contentType</span></span>|<span data-ttu-id="dbdbf-151">String</span><span class="sxs-lookup"><span data-stu-id="dbdbf-151">String</span></span>|<span data-ttu-id="dbdbf-152">MIME タイプ。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-152">The MIME type.</span></span>|
|<span data-ttu-id="dbdbf-153">id</span><span class="sxs-lookup"><span data-stu-id="dbdbf-153">id</span></span>|<span data-ttu-id="dbdbf-154">String</span><span class="sxs-lookup"><span data-stu-id="dbdbf-154">String</span></span>| <span data-ttu-id="dbdbf-155">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-155">Read-only.</span></span>|
|<span data-ttu-id="dbdbf-156">isInline</span><span class="sxs-lookup"><span data-stu-id="dbdbf-156">isInline</span></span>|<span data-ttu-id="dbdbf-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbdbf-157">Boolean</span></span>|<span data-ttu-id="dbdbf-158">添付ファイルがインライン添付ファイルの場合は `true`、それ以外の場合は `false`。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-158">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="dbdbf-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbdbf-159">lastModifiedDateTime</span></span>|<span data-ttu-id="dbdbf-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbdbf-160">DateTimeOffset</span></span>|<span data-ttu-id="dbdbf-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="dbdbf-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="dbdbf-163">name</span><span class="sxs-lookup"><span data-stu-id="dbdbf-163">name</span></span>|<span data-ttu-id="dbdbf-164">String</span><span class="sxs-lookup"><span data-stu-id="dbdbf-164">String</span></span>|<span data-ttu-id="dbdbf-p103">添付ファイルの表示名。実際のファイル名である必要はありません。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-p103">The display name of the attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="dbdbf-167">size</span><span class="sxs-lookup"><span data-stu-id="dbdbf-167">size</span></span>|<span data-ttu-id="dbdbf-168">Int32</span><span class="sxs-lookup"><span data-stu-id="dbdbf-168">Int32</span></span>|<span data-ttu-id="dbdbf-169">添付ファイルの長さ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="dbdbf-169">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbdbf-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dbdbf-170">Relationships</span></span>
<span data-ttu-id="dbdbf-171">なし</span><span class="sxs-lookup"><span data-stu-id="dbdbf-171">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbdbf-172">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dbdbf-172">JSON representation</span></span>

<span data-ttu-id="dbdbf-173">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="dbdbf-173">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

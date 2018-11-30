---
title: fileAttachment リソースの種類
description: イベントに関連付けられているテキスト ファイルまたは Word 文書) などのファイル
ms.openlocfilehash: 2a43ebbc78d831e907bfd19d647e4b7e398abe90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070673"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="77244-103">fileAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="77244-103">fileAttachment resource type</span></span>

> <span data-ttu-id="77244-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="77244-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77244-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77244-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77244-106">(テキスト ファイルなどの Word 文書)、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または[投稿](../resources/post.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="77244-106">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="77244-107">**ContentBytes**プロパティには、base64 でエンコードされたファイルの内容が含まれています。</span><span class="sxs-lookup"><span data-stu-id="77244-107">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="77244-108">添付ファイルを作成する場合は、要求本文に以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="77244-108">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="77244-109">必要なプロパティ **name** と **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="77244-109">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="77244-110">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="77244-110">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="77244-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="77244-111">Methods</span></span>

| <span data-ttu-id="77244-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="77244-112">Method</span></span>       | <span data-ttu-id="77244-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="77244-113">Return Type</span></span>  |<span data-ttu-id="77244-114">説明</span><span class="sxs-lookup"><span data-stu-id="77244-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77244-115">取得</span><span class="sxs-lookup"><span data-stu-id="77244-115">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="77244-116">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="77244-116">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="77244-117">fileattachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="77244-117">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="77244-118">Delete</span><span class="sxs-lookup"><span data-stu-id="77244-118">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="77244-119">なし</span><span class="sxs-lookup"><span data-stu-id="77244-119">None</span></span> |<span data-ttu-id="77244-120">fileAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="77244-120">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="77244-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77244-121">Properties</span></span>
| <span data-ttu-id="77244-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77244-122">Property</span></span>     | <span data-ttu-id="77244-123">型</span><span class="sxs-lookup"><span data-stu-id="77244-123">Type</span></span>   |<span data-ttu-id="77244-124">説明</span><span class="sxs-lookup"><span data-stu-id="77244-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77244-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="77244-125">contentBytes</span></span>|<span data-ttu-id="77244-126">Binary</span><span class="sxs-lookup"><span data-stu-id="77244-126">Binary</span></span>|<span data-ttu-id="77244-127">base64 でエンコードされたファイルの内容。</span><span class="sxs-lookup"><span data-stu-id="77244-127">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="77244-128">contentId</span><span class="sxs-lookup"><span data-stu-id="77244-128">contentId</span></span>|<span data-ttu-id="77244-129">String</span><span class="sxs-lookup"><span data-stu-id="77244-129">String</span></span>|<span data-ttu-id="77244-130">Exchange ストア内の添付ファイルの ID。</span><span class="sxs-lookup"><span data-stu-id="77244-130">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="77244-131">contentLocation</span><span class="sxs-lookup"><span data-stu-id="77244-131">contentLocation</span></span>|<span data-ttu-id="77244-132">String</span><span class="sxs-lookup"><span data-stu-id="77244-132">String</span></span>|<span data-ttu-id="77244-133">添付ファイルのコンテンツの場所に対応する Uniform Resource Identifier (URI)。</span><span class="sxs-lookup"><span data-stu-id="77244-133">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="77244-134">contentType</span><span class="sxs-lookup"><span data-stu-id="77244-134">contentType</span></span>|<span data-ttu-id="77244-135">String</span><span class="sxs-lookup"><span data-stu-id="77244-135">String</span></span>|<span data-ttu-id="77244-136">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="77244-136">The content type of the attachment.</span></span>|
|<span data-ttu-id="77244-137">id</span><span class="sxs-lookup"><span data-stu-id="77244-137">id</span></span>|<span data-ttu-id="77244-138">String</span><span class="sxs-lookup"><span data-stu-id="77244-138">String</span></span>|<span data-ttu-id="77244-139">添付ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="77244-139">The attachment ID.</span></span>|
|<span data-ttu-id="77244-140">isInline</span><span class="sxs-lookup"><span data-stu-id="77244-140">isInline</span></span>|<span data-ttu-id="77244-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="77244-141">Boolean</span></span>|<span data-ttu-id="77244-142">インライン添付ファイルの場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="77244-142">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="77244-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77244-143">lastModifiedDateTime</span></span>|<span data-ttu-id="77244-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77244-144">DateTimeOffset</span></span>|<span data-ttu-id="77244-145">添付ファイルが最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="77244-145">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="77244-146">name</span><span class="sxs-lookup"><span data-stu-id="77244-146">name</span></span>|<span data-ttu-id="77244-147">String</span><span class="sxs-lookup"><span data-stu-id="77244-147">String</span></span>|<span data-ttu-id="77244-148">埋め込み添付ファイルを表すアイコンの下に表示されるテキストを表す名前。これは、実際のファイル名にする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="77244-148">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="77244-149">size</span><span class="sxs-lookup"><span data-stu-id="77244-149">size</span></span>|<span data-ttu-id="77244-150">Int32</span><span class="sxs-lookup"><span data-stu-id="77244-150">Int32</span></span>|<span data-ttu-id="77244-151">添付ファイルのバイト単位のサイズ。</span><span class="sxs-lookup"><span data-stu-id="77244-151">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77244-152">関係</span><span class="sxs-lookup"><span data-stu-id="77244-152">Relationships</span></span>
<span data-ttu-id="77244-153">なし</span><span class="sxs-lookup"><span data-stu-id="77244-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="77244-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77244-154">JSON representation</span></span>

<span data-ttu-id="77244-155">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="77244-155">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "binary",
  "contentId": "string",
  "contentLocation": "string",
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
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

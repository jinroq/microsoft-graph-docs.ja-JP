---
title: fileAttachment リソースの種類
description: イベントに関連付けられているテキスト ファイルまたは Word 文書) などのファイル
localization_priority: Normal
ms.openlocfilehash: 5f7be9bca3114fc7e74be711dc606a278e0025ff
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572802"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="dc0ba-103">fileAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc0ba-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc0ba-104">(テキスト ファイルなどの Word 文書)、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または[投稿](../resources/post.md)の添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-104">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="dc0ba-105">**ContentBytes**プロパティには、base64 でエンコードされたファイルの内容が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="dc0ba-106">添付ファイルを作成する場合は、要求本文に以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="dc0ba-107">必要なプロパティ **name** と **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="dc0ba-108">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dc0ba-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="dc0ba-109">Methods</span></span>

| <span data-ttu-id="dc0ba-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="dc0ba-110">Method</span></span>       | <span data-ttu-id="dc0ba-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dc0ba-111">Return Type</span></span>  |<span data-ttu-id="dc0ba-112">説明</span><span class="sxs-lookup"><span data-stu-id="dc0ba-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dc0ba-113">取得</span><span class="sxs-lookup"><span data-stu-id="dc0ba-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="dc0ba-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="dc0ba-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="dc0ba-115">fileattachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-115">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="dc0ba-116">Delete</span><span class="sxs-lookup"><span data-stu-id="dc0ba-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="dc0ba-117">なし</span><span class="sxs-lookup"><span data-stu-id="dc0ba-117">None</span></span> |<span data-ttu-id="dc0ba-118">fileAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dc0ba-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc0ba-119">Properties</span></span>
| <span data-ttu-id="dc0ba-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc0ba-120">Property</span></span>     | <span data-ttu-id="dc0ba-121">型</span><span class="sxs-lookup"><span data-stu-id="dc0ba-121">Type</span></span>   |<span data-ttu-id="dc0ba-122">説明</span><span class="sxs-lookup"><span data-stu-id="dc0ba-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc0ba-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="dc0ba-123">contentBytes</span></span>|<span data-ttu-id="dc0ba-124">String</span><span class="sxs-lookup"><span data-stu-id="dc0ba-124">String</span></span>|<span data-ttu-id="dc0ba-125">base64 でエンコードされたファイルの内容。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="dc0ba-126">contentId</span><span class="sxs-lookup"><span data-stu-id="dc0ba-126">contentId</span></span>|<span data-ttu-id="dc0ba-127">String</span><span class="sxs-lookup"><span data-stu-id="dc0ba-127">String</span></span>|<span data-ttu-id="dc0ba-128">Exchange ストア内の添付ファイルの ID。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="dc0ba-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="dc0ba-129">contentLocation</span></span>|<span data-ttu-id="dc0ba-130">String</span><span class="sxs-lookup"><span data-stu-id="dc0ba-130">String</span></span>|<span data-ttu-id="dc0ba-131">サポートされていないと、このプロパティは使用しません。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-131">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="dc0ba-132">contentType</span><span class="sxs-lookup"><span data-stu-id="dc0ba-132">contentType</span></span>|<span data-ttu-id="dc0ba-133">String</span><span class="sxs-lookup"><span data-stu-id="dc0ba-133">String</span></span>|<span data-ttu-id="dc0ba-134">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="dc0ba-135">id</span><span class="sxs-lookup"><span data-stu-id="dc0ba-135">id</span></span>|<span data-ttu-id="dc0ba-136">String</span><span class="sxs-lookup"><span data-stu-id="dc0ba-136">String</span></span>|<span data-ttu-id="dc0ba-137">添付ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-137">The attachment ID.</span></span>|
|<span data-ttu-id="dc0ba-138">isInline</span><span class="sxs-lookup"><span data-stu-id="dc0ba-138">isInline</span></span>|<span data-ttu-id="dc0ba-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="dc0ba-139">Boolean</span></span>|<span data-ttu-id="dc0ba-140">インライン添付ファイルの場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="dc0ba-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc0ba-141">lastModifiedDateTime</span></span>|<span data-ttu-id="dc0ba-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc0ba-142">DateTimeOffset</span></span>|<span data-ttu-id="dc0ba-143">添付ファイルが最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="dc0ba-144">name</span><span class="sxs-lookup"><span data-stu-id="dc0ba-144">name</span></span>|<span data-ttu-id="dc0ba-145">String</span><span class="sxs-lookup"><span data-stu-id="dc0ba-145">String</span></span>|<span data-ttu-id="dc0ba-146">埋め込み添付ファイルを表すアイコンの下に表示されるテキストを表す名前。これは、実際のファイル名にする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="dc0ba-147">size</span><span class="sxs-lookup"><span data-stu-id="dc0ba-147">size</span></span>|<span data-ttu-id="dc0ba-148">Int32</span><span class="sxs-lookup"><span data-stu-id="dc0ba-148">Int32</span></span>|<span data-ttu-id="dc0ba-149">添付ファイルのバイト単位のサイズ。</span><span class="sxs-lookup"><span data-stu-id="dc0ba-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc0ba-150">関係</span><span class="sxs-lookup"><span data-stu-id="dc0ba-150">Relationships</span></span>
<span data-ttu-id="dc0ba-151">なし</span><span class="sxs-lookup"><span data-stu-id="dc0ba-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dc0ba-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc0ba-152">JSON representation</span></span>

<span data-ttu-id="dc0ba-153">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="dc0ba-153">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "String",
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
<!--
{
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/fileattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

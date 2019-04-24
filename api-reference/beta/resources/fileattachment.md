---
title: fileAttachment リソースの種類
description: イベントに添付されたファイル (テキストファイルや Word 文書など)
localization_priority: Normal
ms.openlocfilehash: 7d9f92565e38aaf418691480b7f8f3187c57647c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506369"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="6849a-103">fileAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6849a-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6849a-104">[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook タスク](../resources/outlooktask.md)、または[投稿](../resources/post.md)に添付されたファイル (テキストファイルや Word 文書など)。</span><span class="sxs-lookup"><span data-stu-id="6849a-104">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="6849a-105">**contentbytes**プロパティには、ファイルの base64 でエンコードされたコンテンツが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6849a-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="6849a-106">添付ファイルを作成する場合は、要求本文に以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="6849a-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="6849a-107">必要なプロパティ **name** と **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="6849a-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="6849a-108">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="6849a-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6849a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6849a-109">Methods</span></span>

| <span data-ttu-id="6849a-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="6849a-110">Method</span></span>       | <span data-ttu-id="6849a-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6849a-111">Return Type</span></span>  |<span data-ttu-id="6849a-112">説明</span><span class="sxs-lookup"><span data-stu-id="6849a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6849a-113">取得</span><span class="sxs-lookup"><span data-stu-id="6849a-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="6849a-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="6849a-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="6849a-115">fileattachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6849a-115">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="6849a-116">削除する</span><span class="sxs-lookup"><span data-stu-id="6849a-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="6849a-117">なし</span><span class="sxs-lookup"><span data-stu-id="6849a-117">None</span></span> |<span data-ttu-id="6849a-118">fileAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="6849a-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6849a-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6849a-119">Properties</span></span>
| <span data-ttu-id="6849a-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6849a-120">Property</span></span>     | <span data-ttu-id="6849a-121">型</span><span class="sxs-lookup"><span data-stu-id="6849a-121">Type</span></span>   |<span data-ttu-id="6849a-122">説明</span><span class="sxs-lookup"><span data-stu-id="6849a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6849a-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="6849a-123">contentBytes</span></span>|<span data-ttu-id="6849a-124">Binary</span><span class="sxs-lookup"><span data-stu-id="6849a-124">Binary</span></span>|<span data-ttu-id="6849a-125">base64 でエンコードされたファイルの内容。</span><span class="sxs-lookup"><span data-stu-id="6849a-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="6849a-126">contentId</span><span class="sxs-lookup"><span data-stu-id="6849a-126">contentId</span></span>|<span data-ttu-id="6849a-127">String</span><span class="sxs-lookup"><span data-stu-id="6849a-127">String</span></span>|<span data-ttu-id="6849a-128">Exchange ストア内の添付ファイルの ID。</span><span class="sxs-lookup"><span data-stu-id="6849a-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="6849a-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="6849a-129">contentLocation</span></span>|<span data-ttu-id="6849a-130">String</span><span class="sxs-lookup"><span data-stu-id="6849a-130">String</span></span>|<span data-ttu-id="6849a-131">このプロパティは、サポートされていないため、使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="6849a-131">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="6849a-132">contentType</span><span class="sxs-lookup"><span data-stu-id="6849a-132">contentType</span></span>|<span data-ttu-id="6849a-133">String</span><span class="sxs-lookup"><span data-stu-id="6849a-133">String</span></span>|<span data-ttu-id="6849a-134">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="6849a-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="6849a-135">id</span><span class="sxs-lookup"><span data-stu-id="6849a-135">id</span></span>|<span data-ttu-id="6849a-136">String</span><span class="sxs-lookup"><span data-stu-id="6849a-136">String</span></span>|<span data-ttu-id="6849a-137">添付ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="6849a-137">The attachment ID.</span></span>|
|<span data-ttu-id="6849a-138">isInline</span><span class="sxs-lookup"><span data-stu-id="6849a-138">isInline</span></span>|<span data-ttu-id="6849a-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="6849a-139">Boolean</span></span>|<span data-ttu-id="6849a-140">インライン添付ファイルの場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="6849a-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="6849a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6849a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="6849a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6849a-142">DateTimeOffset</span></span>|<span data-ttu-id="6849a-143">添付ファイルが最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="6849a-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="6849a-144">name</span><span class="sxs-lookup"><span data-stu-id="6849a-144">name</span></span>|<span data-ttu-id="6849a-145">String</span><span class="sxs-lookup"><span data-stu-id="6849a-145">String</span></span>|<span data-ttu-id="6849a-146">埋め込み添付ファイルを表すアイコンの下に表示されるテキストを表す名前。これは、実際のファイル名にする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="6849a-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="6849a-147">size</span><span class="sxs-lookup"><span data-stu-id="6849a-147">size</span></span>|<span data-ttu-id="6849a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6849a-148">Int32</span></span>|<span data-ttu-id="6849a-149">添付ファイルのバイト単位のサイズ。</span><span class="sxs-lookup"><span data-stu-id="6849a-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6849a-150">関係</span><span class="sxs-lookup"><span data-stu-id="6849a-150">Relationships</span></span>
<span data-ttu-id="6849a-151">なし</span><span class="sxs-lookup"><span data-stu-id="6849a-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6849a-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6849a-152">JSON representation</span></span>

<span data-ttu-id="6849a-153">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6849a-153">Here is a JSON representation of the resource</span></span>

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

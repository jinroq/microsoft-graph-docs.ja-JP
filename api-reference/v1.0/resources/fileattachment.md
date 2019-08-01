---
title: fileAttachment リソースの種類
description: 'イベント、メッセージまたは投稿に添付されたファイル (テキスト ファイルや Word 文書など) です。**contentBytes** '
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7e80a4599d79d17829f2bb07bb61d4adf60df607
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032509"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="bef00-104">fileAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bef00-104">fileAttachment resource type</span></span>

<span data-ttu-id="bef00-p102">イベント、メッセージまたは投稿に添付されたファイル (テキスト ファイルや Word 文書など) です。**contentBytes** プロパティには、base64 でエンコードされたファイルの内容が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bef00-p102">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="bef00-107">添付ファイルを作成する場合は、要求本文に以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="bef00-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="bef00-108">必要なプロパティ **name** と **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="bef00-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="bef00-109">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="bef00-109">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bef00-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="bef00-110">Methods</span></span>

| <span data-ttu-id="bef00-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="bef00-111">Method</span></span>       | <span data-ttu-id="bef00-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bef00-112">Return Type</span></span>  |<span data-ttu-id="bef00-113">説明</span><span class="sxs-lookup"><span data-stu-id="bef00-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bef00-114">取得</span><span class="sxs-lookup"><span data-stu-id="bef00-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="bef00-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="bef00-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="bef00-116">fileattachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bef00-116">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="bef00-117">Delete</span><span class="sxs-lookup"><span data-stu-id="bef00-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="bef00-118">なし</span><span class="sxs-lookup"><span data-stu-id="bef00-118">None</span></span> |<span data-ttu-id="bef00-119">fileAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="bef00-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bef00-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bef00-120">Properties</span></span>
| <span data-ttu-id="bef00-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bef00-121">Property</span></span>     | <span data-ttu-id="bef00-122">型</span><span class="sxs-lookup"><span data-stu-id="bef00-122">Type</span></span>   |<span data-ttu-id="bef00-123">説明</span><span class="sxs-lookup"><span data-stu-id="bef00-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bef00-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="bef00-124">contentBytes</span></span>|<span data-ttu-id="bef00-125">Binary</span><span class="sxs-lookup"><span data-stu-id="bef00-125">Binary</span></span>|<span data-ttu-id="bef00-126">base64 でエンコードされたファイルの内容。</span><span class="sxs-lookup"><span data-stu-id="bef00-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="bef00-127">contentId</span><span class="sxs-lookup"><span data-stu-id="bef00-127">contentId</span></span>|<span data-ttu-id="bef00-128">String</span><span class="sxs-lookup"><span data-stu-id="bef00-128">String</span></span>|<span data-ttu-id="bef00-129">Exchange ストア内の添付ファイルの ID。</span><span class="sxs-lookup"><span data-stu-id="bef00-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="bef00-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="bef00-130">contentLocation</span></span>|<span data-ttu-id="bef00-131">String</span><span class="sxs-lookup"><span data-stu-id="bef00-131">String</span></span>|<span data-ttu-id="bef00-132">このプロパティは、サポートされていないため、使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="bef00-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="bef00-133">contentType</span><span class="sxs-lookup"><span data-stu-id="bef00-133">contentType</span></span>|<span data-ttu-id="bef00-134">String</span><span class="sxs-lookup"><span data-stu-id="bef00-134">String</span></span>|<span data-ttu-id="bef00-135">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="bef00-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="bef00-136">id</span><span class="sxs-lookup"><span data-stu-id="bef00-136">id</span></span>|<span data-ttu-id="bef00-137">String</span><span class="sxs-lookup"><span data-stu-id="bef00-137">String</span></span>|<span data-ttu-id="bef00-138">添付ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="bef00-138">The attachment ID.</span></span>|
|<span data-ttu-id="bef00-139">isInline</span><span class="sxs-lookup"><span data-stu-id="bef00-139">isInline</span></span>|<span data-ttu-id="bef00-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef00-140">Boolean</span></span>|<span data-ttu-id="bef00-141">インライン添付ファイルの場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="bef00-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="bef00-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bef00-142">lastModifiedDateTime</span></span>|<span data-ttu-id="bef00-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bef00-143">DateTimeOffset</span></span>|<span data-ttu-id="bef00-144">添付ファイルが最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="bef00-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="bef00-145">name</span><span class="sxs-lookup"><span data-stu-id="bef00-145">name</span></span>|<span data-ttu-id="bef00-146">String</span><span class="sxs-lookup"><span data-stu-id="bef00-146">String</span></span>|<span data-ttu-id="bef00-147">埋め込み添付ファイルを表すアイコンの下に表示されるテキストを表す名前。これは、実際のファイル名にする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="bef00-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="bef00-148">size</span><span class="sxs-lookup"><span data-stu-id="bef00-148">size</span></span>|<span data-ttu-id="bef00-149">Int32</span><span class="sxs-lookup"><span data-stu-id="bef00-149">Int32</span></span>|<span data-ttu-id="bef00-150">添付ファイルのバイト単位のサイズ。</span><span class="sxs-lookup"><span data-stu-id="bef00-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bef00-151">関係</span><span class="sxs-lookup"><span data-stu-id="bef00-151">Relationships</span></span>
<span data-ttu-id="bef00-152">なし</span><span class="sxs-lookup"><span data-stu-id="bef00-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bef00-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bef00-153">JSON representation</span></span>

<span data-ttu-id="bef00-154">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="bef00-154">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
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

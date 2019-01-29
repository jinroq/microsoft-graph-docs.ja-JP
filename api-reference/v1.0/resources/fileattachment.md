---
title: fileAttachment リソースの種類
description: 'イベント、メッセージまたは投稿に添付されたファイル (テキスト ファイルや Word 文書など) です。**contentBytes** '
localization_priority: Priority
ms.openlocfilehash: 07dcdac0497caa106eac38d1248661218a7fcc5e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574818"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="69a98-104">fileAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="69a98-104">fileAttachment resource type</span></span>

<span data-ttu-id="69a98-p102">イベント、メッセージまたは投稿に添付されたファイル (テキスト ファイルや Word 文書など) です。**contentBytes** プロパティには、base64 でエンコードされたファイルの内容が含まれています。</span><span class="sxs-lookup"><span data-stu-id="69a98-p102">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="69a98-107">添付ファイルを作成する場合は、要求本文に以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="69a98-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="69a98-108">必要なプロパティ **name** と **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="69a98-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="69a98-109">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="69a98-109">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="69a98-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="69a98-110">Methods</span></span>

| <span data-ttu-id="69a98-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="69a98-111">Method</span></span>       | <span data-ttu-id="69a98-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="69a98-112">Return Type</span></span>  |<span data-ttu-id="69a98-113">説明</span><span class="sxs-lookup"><span data-stu-id="69a98-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69a98-114">取得</span><span class="sxs-lookup"><span data-stu-id="69a98-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="69a98-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="69a98-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="69a98-116">fileattachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="69a98-116">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="69a98-117">Delete</span><span class="sxs-lookup"><span data-stu-id="69a98-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="69a98-118">なし</span><span class="sxs-lookup"><span data-stu-id="69a98-118">None</span></span> |<span data-ttu-id="69a98-119">fileAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="69a98-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="69a98-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69a98-120">Properties</span></span>
| <span data-ttu-id="69a98-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69a98-121">Property</span></span>     | <span data-ttu-id="69a98-122">型</span><span class="sxs-lookup"><span data-stu-id="69a98-122">Type</span></span>   |<span data-ttu-id="69a98-123">説明</span><span class="sxs-lookup"><span data-stu-id="69a98-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69a98-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="69a98-124">contentBytes</span></span>|<span data-ttu-id="69a98-125">Binary</span><span class="sxs-lookup"><span data-stu-id="69a98-125">Binary</span></span>|<span data-ttu-id="69a98-126">base64 でエンコードされたファイルの内容。</span><span class="sxs-lookup"><span data-stu-id="69a98-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="69a98-127">contentId</span><span class="sxs-lookup"><span data-stu-id="69a98-127">contentId</span></span>|<span data-ttu-id="69a98-128">String</span><span class="sxs-lookup"><span data-stu-id="69a98-128">String</span></span>|<span data-ttu-id="69a98-129">Exchange ストア内の添付ファイルの ID。</span><span class="sxs-lookup"><span data-stu-id="69a98-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="69a98-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="69a98-130">contentLocation</span></span>|<span data-ttu-id="69a98-131">String</span><span class="sxs-lookup"><span data-stu-id="69a98-131">String</span></span>|<span data-ttu-id="69a98-132">このプロパティは、サポートされていないため、使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="69a98-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="69a98-133">contentType</span><span class="sxs-lookup"><span data-stu-id="69a98-133">contentType</span></span>|<span data-ttu-id="69a98-134">String</span><span class="sxs-lookup"><span data-stu-id="69a98-134">String</span></span>|<span data-ttu-id="69a98-135">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="69a98-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="69a98-136">id</span><span class="sxs-lookup"><span data-stu-id="69a98-136">id</span></span>|<span data-ttu-id="69a98-137">String</span><span class="sxs-lookup"><span data-stu-id="69a98-137">String</span></span>|<span data-ttu-id="69a98-138">添付ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="69a98-138">The attachment ID.</span></span>|
|<span data-ttu-id="69a98-139">isInline</span><span class="sxs-lookup"><span data-stu-id="69a98-139">isInline</span></span>|<span data-ttu-id="69a98-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="69a98-140">Boolean</span></span>|<span data-ttu-id="69a98-141">インライン添付ファイルの場合、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="69a98-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="69a98-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69a98-142">lastModifiedDateTime</span></span>|<span data-ttu-id="69a98-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69a98-143">DateTimeOffset</span></span>|<span data-ttu-id="69a98-144">添付ファイルが最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="69a98-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="69a98-145">name</span><span class="sxs-lookup"><span data-stu-id="69a98-145">name</span></span>|<span data-ttu-id="69a98-146">String</span><span class="sxs-lookup"><span data-stu-id="69a98-146">String</span></span>|<span data-ttu-id="69a98-147">埋め込み添付ファイルを表すアイコンの下に表示されるテキストを表す名前。これは、実際のファイル名にする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="69a98-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="69a98-148">size</span><span class="sxs-lookup"><span data-stu-id="69a98-148">size</span></span>|<span data-ttu-id="69a98-149">Int32</span><span class="sxs-lookup"><span data-stu-id="69a98-149">Int32</span></span>|<span data-ttu-id="69a98-150">添付ファイルのバイト単位のサイズ。</span><span class="sxs-lookup"><span data-stu-id="69a98-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69a98-151">関係</span><span class="sxs-lookup"><span data-stu-id="69a98-151">Relationships</span></span>
<span data-ttu-id="69a98-152">なし</span><span class="sxs-lookup"><span data-stu-id="69a98-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="69a98-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="69a98-153">JSON representation</span></span>

<span data-ttu-id="69a98-154">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="69a98-154">Here is a JSON representation of the resource</span></span>

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

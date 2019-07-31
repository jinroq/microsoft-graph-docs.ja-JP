---
title: referenceAttachment リソースの種類
description: 'OneDrive for Business のクラウドドライブ上のフォルダーまたはファイル (テキストファイルや Word 文書など) またはその他のサポートされているストレージの場所へのリンクは、 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ef3e2dd5292ee018c0b72c29c8bd6c33fed00f11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008713"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="09468-103">referenceAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09468-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09468-104">OneDrive for Business クラウドドライブ上のフォルダーまたはファイル (テキストファイルや Word 文書など) またはその他のサポートされているストレージの場所を、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook のタスク](../resources/outlooktask.md)、または[投稿](../resources/post.md)に添付したリンク。</span><span class="sxs-lookup"><span data-stu-id="09468-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="09468-105">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="09468-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="09468-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="09468-106">Methods</span></span>

| <span data-ttu-id="09468-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="09468-107">Method</span></span>       | <span data-ttu-id="09468-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="09468-108">Return Type</span></span>  |<span data-ttu-id="09468-109">説明</span><span class="sxs-lookup"><span data-stu-id="09468-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="09468-110">Get</span><span class="sxs-lookup"><span data-stu-id="09468-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="09468-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="09468-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="09468-112">referenceAttachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="09468-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="09468-113">Delete</span><span class="sxs-lookup"><span data-stu-id="09468-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="09468-114">None</span><span class="sxs-lookup"><span data-stu-id="09468-114">None</span></span> |<span data-ttu-id="09468-115">referenceAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="09468-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="09468-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09468-116">Properties</span></span>
| <span data-ttu-id="09468-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09468-117">Property</span></span>     | <span data-ttu-id="09468-118">型</span><span class="sxs-lookup"><span data-stu-id="09468-118">Type</span></span>   |<span data-ttu-id="09468-119">説明</span><span class="sxs-lookup"><span data-stu-id="09468-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09468-120">contentType</span><span class="sxs-lookup"><span data-stu-id="09468-120">contentType</span></span>|<span data-ttu-id="09468-121">String</span><span class="sxs-lookup"><span data-stu-id="09468-121">String</span></span>|<span data-ttu-id="09468-122">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="09468-122">The content type of the attachment.</span></span> <span data-ttu-id="09468-123">省略可能。</span><span class="sxs-lookup"><span data-stu-id="09468-123">Optional.</span></span>|
|<span data-ttu-id="09468-124">id</span><span class="sxs-lookup"><span data-stu-id="09468-124">id</span></span>|<span data-ttu-id="09468-125">文字列</span><span class="sxs-lookup"><span data-stu-id="09468-125">String</span></span>|<span data-ttu-id="09468-p102">添付ファイル ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="09468-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="09468-128">isFolder</span><span class="sxs-lookup"><span data-stu-id="09468-128">isFolder</span></span>|<span data-ttu-id="09468-129">ブール型</span><span class="sxs-lookup"><span data-stu-id="09468-129">Boolean</span></span>|<span data-ttu-id="09468-130">添付ファイルがフォルダーへのリンクであるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="09468-130">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="09468-131">**Sourceurl**がフォルダーへのリンクの場合は、true に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="09468-131">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="09468-132">省略可能。</span><span class="sxs-lookup"><span data-stu-id="09468-132">Optional.</span></span>|
|<span data-ttu-id="09468-133">isInline</span><span class="sxs-lookup"><span data-stu-id="09468-133">isInline</span></span>|<span data-ttu-id="09468-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="09468-134">Boolean</span></span>|<span data-ttu-id="09468-135">添付ファイルを埋め込みオブジェクトの本文にインラインで表示する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="09468-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="09468-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="09468-136">Optional.</span></span>|
|<span data-ttu-id="09468-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09468-137">lastModifiedDateTime</span></span>|<span data-ttu-id="09468-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09468-138">DateTimeOffset</span></span>|<span data-ttu-id="09468-139">添付ファイルが最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="09468-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="09468-140">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="09468-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="09468-141">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="09468-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="09468-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="09468-142">Optional.</span></span>|
|<span data-ttu-id="09468-143">name</span><span class="sxs-lookup"><span data-stu-id="09468-143">name</span></span>|<span data-ttu-id="09468-144">String</span><span class="sxs-lookup"><span data-stu-id="09468-144">String</span></span>|<span data-ttu-id="09468-145">埋め込まれた添付ファイルを表すアイコンの下に表示されるテキスト。</span><span class="sxs-lookup"><span data-stu-id="09468-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="09468-146">実際のファイル名である必要はありません。</span><span class="sxs-lookup"><span data-stu-id="09468-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="09468-147">必須。</span><span class="sxs-lookup"><span data-stu-id="09468-147">Required.</span></span>|
|<span data-ttu-id="09468-148">権</span><span class="sxs-lookup"><span data-stu-id="09468-148">permission</span></span>|<span data-ttu-id="09468-149">Referenceattachmentpermission が</span><span class="sxs-lookup"><span data-stu-id="09468-149">referenceAttachmentPermission</span></span>|<span data-ttu-id="09468-150">**Providertype**のプロバイダーの種類によって添付ファイルに付与されるアクセス許可を指定します。</span><span class="sxs-lookup"><span data-stu-id="09468-150">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="09468-151">可能な値は、`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView`、`organizationEdit` です。</span><span class="sxs-lookup"><span data-stu-id="09468-151">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="09468-152">省略可能。</span><span class="sxs-lookup"><span data-stu-id="09468-152">Optional.</span></span>|
|<span data-ttu-id="09468-153">previewUrl</span><span class="sxs-lookup"><span data-stu-id="09468-153">previewUrl</span></span>|<span data-ttu-id="09468-154">String</span><span class="sxs-lookup"><span data-stu-id="09468-154">String</span></span>|<span data-ttu-id="09468-155">イメージ URL の参照添付ファイルにのみ適用され、プレビューイメージを取得します。</span><span class="sxs-lookup"><span data-stu-id="09468-155">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="09468-156">**ThumbnailUrl**および**プレビュー Url**は、 **sourceurl**が画像ファイルを識別する場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="09468-156">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="09468-157">省略可能。</span><span class="sxs-lookup"><span data-stu-id="09468-157">Optional.</span></span>|
|<span data-ttu-id="09468-158">providerType</span><span class="sxs-lookup"><span data-stu-id="09468-158">providerType</span></span>|<span data-ttu-id="09468-159">referenceAttachmentProvider</span><span class="sxs-lookup"><span data-stu-id="09468-159">referenceAttachmentProvider</span></span>|<span data-ttu-id="09468-160">この contentType の添付ファイルをサポートするプロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="09468-160">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="09468-161">可能な値は、`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox` です。</span><span class="sxs-lookup"><span data-stu-id="09468-161">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="09468-162">省略可能。</span><span class="sxs-lookup"><span data-stu-id="09468-162">Optional.</span></span>|
|<span data-ttu-id="09468-163">size</span><span class="sxs-lookup"><span data-stu-id="09468-163">size</span></span>|<span data-ttu-id="09468-164">Int32</span><span class="sxs-lookup"><span data-stu-id="09468-164">Int32</span></span>|<span data-ttu-id="09468-165">参照添付ファイルのメッセージに格納されているメタデータのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="09468-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="09468-166">この値は実際のファイルのサイズを示すものではありません。</span><span class="sxs-lookup"><span data-stu-id="09468-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="09468-167">省略可能。</span><span class="sxs-lookup"><span data-stu-id="09468-167">Optional.</span></span>|
|<span data-ttu-id="09468-168">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="09468-168">sourceUrl</span></span>|<span data-ttu-id="09468-169">文字列</span><span class="sxs-lookup"><span data-stu-id="09468-169">String</span></span>|<span data-ttu-id="09468-170">添付ファイルの内容を取得するための URL。</span><span class="sxs-lookup"><span data-stu-id="09468-170">URL to get the attachment content.</span></span> <span data-ttu-id="09468-171">これがフォルダーへの URL である場合、Outlook または web 上の Outlook でフォルダーが正しく表示されるようにするには、 **Isfolder**を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="09468-171">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="09468-172">必須です。</span><span class="sxs-lookup"><span data-stu-id="09468-172">Required.</span></span>|
|<span data-ttu-id="09468-173">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="09468-173">thumbnailUrl</span></span>|<span data-ttu-id="09468-174">String</span><span class="sxs-lookup"><span data-stu-id="09468-174">String</span></span>|<span data-ttu-id="09468-175">サムネイルイメージを取得するために、イメージ URL の参照添付ファイルにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="09468-175">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="09468-176">**ThumbnailUrl**および**プレビュー Url**は、 **sourceurl**が画像ファイルを識別する場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="09468-176">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="09468-177">省略可能。</span><span class="sxs-lookup"><span data-stu-id="09468-177">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09468-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09468-178">Relationships</span></span>
<span data-ttu-id="09468-179">なし</span><span class="sxs-lookup"><span data-stu-id="09468-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="09468-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09468-180">JSON representation</span></span>

<span data-ttu-id="09468-181">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="09468-181">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isFolder": true,
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "permission": "string",
  "previewUrl": "string",
  "providerType": "string",
  "size": 1024,
  "sourceUrl": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

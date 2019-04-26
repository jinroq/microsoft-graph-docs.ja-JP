---
title: referenceAttachment リソースの種類
description: 'OneDrive for business のクラウドドライブ上のフォルダーまたはファイル (テキストファイルや Word 文書など) またはその他のサポートされているストレージの場所へのリンクは、 '
localization_priority: Normal
ms.openlocfilehash: 59ebb0af10a64195643cb7073d1206790ae6a875
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563097"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="a32e3-103">referenceAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a32e3-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a32e3-104">OneDrive for business クラウドドライブ上のフォルダーまたはファイル (テキストファイルや Word 文書など) またはその他のサポートされているストレージの場所を、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook のタスク](../resources/outlooktask.md)、または[投稿](../resources/post.md)に添付したリンク。</span><span class="sxs-lookup"><span data-stu-id="a32e3-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="a32e3-105">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="a32e3-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a32e3-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a32e3-106">Methods</span></span>

| <span data-ttu-id="a32e3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a32e3-107">Method</span></span>       | <span data-ttu-id="a32e3-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a32e3-108">Return Type</span></span>  |<span data-ttu-id="a32e3-109">説明</span><span class="sxs-lookup"><span data-stu-id="a32e3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a32e3-110">取得</span><span class="sxs-lookup"><span data-stu-id="a32e3-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="a32e3-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="a32e3-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="a32e3-112">referenceAttachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a32e3-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="a32e3-113">削除</span><span class="sxs-lookup"><span data-stu-id="a32e3-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="a32e3-114">なし</span><span class="sxs-lookup"><span data-stu-id="a32e3-114">None</span></span> |<span data-ttu-id="a32e3-115">referenceAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a32e3-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a32e3-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a32e3-116">Properties</span></span>
| <span data-ttu-id="a32e3-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a32e3-117">Property</span></span>     | <span data-ttu-id="a32e3-118">型</span><span class="sxs-lookup"><span data-stu-id="a32e3-118">Type</span></span>   |<span data-ttu-id="a32e3-119">説明</span><span class="sxs-lookup"><span data-stu-id="a32e3-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a32e3-120">contentType</span><span class="sxs-lookup"><span data-stu-id="a32e3-120">contentType</span></span>|<span data-ttu-id="a32e3-121">String</span><span class="sxs-lookup"><span data-stu-id="a32e3-121">String</span></span>|<span data-ttu-id="a32e3-122">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="a32e3-122">The content type of the attachment.</span></span> <span data-ttu-id="a32e3-123">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a32e3-123">Optional.</span></span>|
|<span data-ttu-id="a32e3-124">id</span><span class="sxs-lookup"><span data-stu-id="a32e3-124">id</span></span>|<span data-ttu-id="a32e3-125">String</span><span class="sxs-lookup"><span data-stu-id="a32e3-125">String</span></span>|<span data-ttu-id="a32e3-p102">添付ファイル ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a32e3-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="a32e3-128">isFolder</span><span class="sxs-lookup"><span data-stu-id="a32e3-128">isFolder</span></span>|<span data-ttu-id="a32e3-129">ブール型</span><span class="sxs-lookup"><span data-stu-id="a32e3-129">Boolean</span></span>|<span data-ttu-id="a32e3-130">添付ファイルがフォルダーへのリンクであるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a32e3-130">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="a32e3-131">**sourceurl**がフォルダーへのリンクの場合は、true に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a32e3-131">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="a32e3-132">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a32e3-132">Optional.</span></span>|
|<span data-ttu-id="a32e3-133">isInline</span><span class="sxs-lookup"><span data-stu-id="a32e3-133">isInline</span></span>|<span data-ttu-id="a32e3-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="a32e3-134">Boolean</span></span>|<span data-ttu-id="a32e3-135">添付ファイルを埋め込みオブジェクトの本文にインラインで表示する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="a32e3-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="a32e3-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a32e3-136">Optional.</span></span>|
|<span data-ttu-id="a32e3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a32e3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a32e3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a32e3-138">DateTimeOffset</span></span>|<span data-ttu-id="a32e3-139">添付ファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="a32e3-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="a32e3-140">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="a32e3-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a32e3-141">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a32e3-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a32e3-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a32e3-142">Optional.</span></span>|
|<span data-ttu-id="a32e3-143">name</span><span class="sxs-lookup"><span data-stu-id="a32e3-143">name</span></span>|<span data-ttu-id="a32e3-144">String</span><span class="sxs-lookup"><span data-stu-id="a32e3-144">String</span></span>|<span data-ttu-id="a32e3-145">埋め込まれた添付ファイルを表すアイコンの下に表示されるテキスト。</span><span class="sxs-lookup"><span data-stu-id="a32e3-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="a32e3-146">実際のファイル名である必要はありません。</span><span class="sxs-lookup"><span data-stu-id="a32e3-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="a32e3-147">必須。</span><span class="sxs-lookup"><span data-stu-id="a32e3-147">Required.</span></span>|
|<span data-ttu-id="a32e3-148">権</span><span class="sxs-lookup"><span data-stu-id="a32e3-148">permission</span></span>|<span data-ttu-id="a32e3-149">ReferenceAttachmentPermissions</span><span class="sxs-lookup"><span data-stu-id="a32e3-149">ReferenceAttachmentPermissions</span></span>|<span data-ttu-id="a32e3-150">**providertype**のプロバイダーの種類によって添付ファイルに付与されるアクセス許可を指定します。</span><span class="sxs-lookup"><span data-stu-id="a32e3-150">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="a32e3-151">可能な値は、`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView`、`organizationEdit` です。</span><span class="sxs-lookup"><span data-stu-id="a32e3-151">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="a32e3-152">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a32e3-152">Optional.</span></span>|
|<span data-ttu-id="a32e3-153">previewUrl</span><span class="sxs-lookup"><span data-stu-id="a32e3-153">previewUrl</span></span>|<span data-ttu-id="a32e3-154">String</span><span class="sxs-lookup"><span data-stu-id="a32e3-154">String</span></span>|<span data-ttu-id="a32e3-155">イメージ URL の参照添付ファイルにのみ適用され、プレビューイメージを取得します。</span><span class="sxs-lookup"><span data-stu-id="a32e3-155">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="a32e3-156">**thumbnailUrl**および**プレビュー url**は、 **sourceurl**が画像ファイルを識別する場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="a32e3-156">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="a32e3-157">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a32e3-157">Optional.</span></span>|
|<span data-ttu-id="a32e3-158">providerType</span><span class="sxs-lookup"><span data-stu-id="a32e3-158">providerType</span></span>|<span data-ttu-id="a32e3-159">ReferenceAttachmentProviders</span><span class="sxs-lookup"><span data-stu-id="a32e3-159">ReferenceAttachmentProviders</span></span>|<span data-ttu-id="a32e3-160">この contentType の添付ファイルをサポートするプロバイダーの種類。</span><span class="sxs-lookup"><span data-stu-id="a32e3-160">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="a32e3-161">可能な値は、`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox` です。</span><span class="sxs-lookup"><span data-stu-id="a32e3-161">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="a32e3-162">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a32e3-162">Optional.</span></span>|
|<span data-ttu-id="a32e3-163">size</span><span class="sxs-lookup"><span data-stu-id="a32e3-163">size</span></span>|<span data-ttu-id="a32e3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a32e3-164">Int32</span></span>|<span data-ttu-id="a32e3-165">参照添付ファイルのメッセージに格納されているメタデータのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="a32e3-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="a32e3-166">この値は実際のファイルのサイズを示すものではありません。</span><span class="sxs-lookup"><span data-stu-id="a32e3-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="a32e3-167">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a32e3-167">Optional.</span></span>|
|<span data-ttu-id="a32e3-168">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="a32e3-168">sourceUrl</span></span>|<span data-ttu-id="a32e3-169">文字列</span><span class="sxs-lookup"><span data-stu-id="a32e3-169">String</span></span>|<span data-ttu-id="a32e3-170">添付ファイルの内容を取得するための URL。</span><span class="sxs-lookup"><span data-stu-id="a32e3-170">URL to get the attachment content.</span></span> <span data-ttu-id="a32e3-171">これがフォルダーへの URL である場合、outlook または web 上の outlook でフォルダーが正しく表示されるようにするには、 **isfolder**を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="a32e3-171">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="a32e3-172">必須です。</span><span class="sxs-lookup"><span data-stu-id="a32e3-172">Required.</span></span>|
|<span data-ttu-id="a32e3-173">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="a32e3-173">thumbnailUrl</span></span>|<span data-ttu-id="a32e3-174">String</span><span class="sxs-lookup"><span data-stu-id="a32e3-174">String</span></span>|<span data-ttu-id="a32e3-175">サムネイルイメージを取得するために、イメージ URL の参照添付ファイルにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="a32e3-175">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="a32e3-176">**thumbnailUrl**および**プレビュー url**は、 **sourceurl**が画像ファイルを識別する場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="a32e3-176">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="a32e3-177">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a32e3-177">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a32e3-178">関係</span><span class="sxs-lookup"><span data-stu-id="a32e3-178">Relationships</span></span>
<span data-ttu-id="a32e3-179">なし</span><span class="sxs-lookup"><span data-stu-id="a32e3-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="a32e3-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a32e3-180">JSON representation</span></span>

<span data-ttu-id="a32e3-181">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a32e3-181">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/referenceattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: referenceAttachment リソースの種類
description: '接続されているフォルダーや、OneDrive ビジネス クラウド ドライブ、またはその他のサポートされているストレージの場所にテキスト ファイルまたは Word 文書) などのファイルへのリンク '
localization_priority: Normal
ms.openlocfilehash: adf078f7ba678a4fe90a51972c5e4be4788c9c0c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574559"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="7afb1-103">referenceAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7afb1-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7afb1-104">フォルダーまたはビジネス クラウド ドライブ、またはその他の OneDrive のテキスト ファイル、または Word 文書) などのファイルへのリンクには、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または[ポスト](../resources/post.md)に接続されているストレージの場所がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="7afb1-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="7afb1-105">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="7afb1-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7afb1-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7afb1-106">Methods</span></span>

| <span data-ttu-id="7afb1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7afb1-107">Method</span></span>       | <span data-ttu-id="7afb1-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7afb1-108">Return Type</span></span>  |<span data-ttu-id="7afb1-109">説明</span><span class="sxs-lookup"><span data-stu-id="7afb1-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7afb1-110">取得</span><span class="sxs-lookup"><span data-stu-id="7afb1-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="7afb1-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="7afb1-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="7afb1-112">referenceAttachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7afb1-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="7afb1-113">Delete</span><span class="sxs-lookup"><span data-stu-id="7afb1-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="7afb1-114">なし</span><span class="sxs-lookup"><span data-stu-id="7afb1-114">None</span></span> |<span data-ttu-id="7afb1-115">referenceAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="7afb1-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7afb1-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7afb1-116">Properties</span></span>
| <span data-ttu-id="7afb1-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7afb1-117">Property</span></span>     | <span data-ttu-id="7afb1-118">型</span><span class="sxs-lookup"><span data-stu-id="7afb1-118">Type</span></span>   |<span data-ttu-id="7afb1-119">説明</span><span class="sxs-lookup"><span data-stu-id="7afb1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7afb1-120">contentType</span><span class="sxs-lookup"><span data-stu-id="7afb1-120">contentType</span></span>|<span data-ttu-id="7afb1-121">String</span><span class="sxs-lookup"><span data-stu-id="7afb1-121">String</span></span>|<span data-ttu-id="7afb1-122">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="7afb1-122">The content type of the attachment.</span></span> <span data-ttu-id="7afb1-123">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7afb1-123">Optional.</span></span>|
|<span data-ttu-id="7afb1-124">id</span><span class="sxs-lookup"><span data-stu-id="7afb1-124">id</span></span>|<span data-ttu-id="7afb1-125">String</span><span class="sxs-lookup"><span data-stu-id="7afb1-125">String</span></span>|<span data-ttu-id="7afb1-p102">添付ファイル ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7afb1-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="7afb1-128">isFolder</span><span class="sxs-lookup"><span data-stu-id="7afb1-128">isFolder</span></span>|<span data-ttu-id="7afb1-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="7afb1-129">Boolean</span></span>|<span data-ttu-id="7afb1-130">添付ファイルがフォルダーへのリンクであるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7afb1-130">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="7afb1-131">True を設定**し直すこと**は、フォルダーへのリンクを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7afb1-131">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="7afb1-132">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7afb1-132">Optional.</span></span>|
|<span data-ttu-id="7afb1-133">isInline</span><span class="sxs-lookup"><span data-stu-id="7afb1-133">isInline</span></span>|<span data-ttu-id="7afb1-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="7afb1-134">Boolean</span></span>|<span data-ttu-id="7afb1-135">添付ファイルを埋め込みオブジェクトの本文にインラインで表示する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="7afb1-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="7afb1-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7afb1-136">Optional.</span></span>|
|<span data-ttu-id="7afb1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7afb1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7afb1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7afb1-138">DateTimeOffset</span></span>|<span data-ttu-id="7afb1-139">添付ファイルが最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="7afb1-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="7afb1-140">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="7afb1-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7afb1-141">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="7afb1-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7afb1-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7afb1-142">Optional.</span></span>|
|<span data-ttu-id="7afb1-143">name</span><span class="sxs-lookup"><span data-stu-id="7afb1-143">name</span></span>|<span data-ttu-id="7afb1-144">String</span><span class="sxs-lookup"><span data-stu-id="7afb1-144">String</span></span>|<span data-ttu-id="7afb1-145">埋め込まれた添付ファイルを表すアイコンの下に表示されるテキストです。</span><span class="sxs-lookup"><span data-stu-id="7afb1-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="7afb1-146">これは、実際のファイル名を指定するのには必要ありません。</span><span class="sxs-lookup"><span data-stu-id="7afb1-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="7afb1-147">必須です。</span><span class="sxs-lookup"><span data-stu-id="7afb1-147">Required.</span></span>|
|<span data-ttu-id="7afb1-148">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7afb1-148">permission</span></span>|<span data-ttu-id="7afb1-149">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="7afb1-149">referenceAttachmentPermission</span></span>|<span data-ttu-id="7afb1-150">**プロバイダーの種類**のプロバイダーの種類によって、添付ファイルに付与するアクセス許可を指定します。</span><span class="sxs-lookup"><span data-stu-id="7afb1-150">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="7afb1-151">可能な値は、`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView`、`organizationEdit` です。</span><span class="sxs-lookup"><span data-stu-id="7afb1-151">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="7afb1-152">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7afb1-152">Optional.</span></span>|
|<span data-ttu-id="7afb1-153">previewUrl</span><span class="sxs-lookup"><span data-stu-id="7afb1-153">previewUrl</span></span>|<span data-ttu-id="7afb1-154">String</span><span class="sxs-lookup"><span data-stu-id="7afb1-154">String</span></span>|<span data-ttu-id="7afb1-155">イメージのプレビュー イメージを取得する URL の参照添付ファイルのみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="7afb1-155">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="7afb1-156">**直すこと**は、イメージ ファイルを指定するときにのみ、 **thumbnailUrl**および**previewUrl**を使用します。</span><span class="sxs-lookup"><span data-stu-id="7afb1-156">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="7afb1-157">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7afb1-157">Optional.</span></span>|
|<span data-ttu-id="7afb1-158">プロバイダーの種類</span><span class="sxs-lookup"><span data-stu-id="7afb1-158">providerType</span></span>| <span data-ttu-id="7afb1-159">referenceAttachmentProvider</span><span class="sxs-lookup"><span data-stu-id="7afb1-159">referenceAttachmentProvider</span></span> |<span data-ttu-id="7afb1-160">このコンテンツ タイプの添付ファイルをサポートするプロバイダーの型。</span><span class="sxs-lookup"><span data-stu-id="7afb1-160">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="7afb1-161">可能な値は、`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox` です。</span><span class="sxs-lookup"><span data-stu-id="7afb1-161">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="7afb1-162">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7afb1-162">Optional.</span></span>|
|<span data-ttu-id="7afb1-163">size</span><span class="sxs-lookup"><span data-stu-id="7afb1-163">size</span></span>|<span data-ttu-id="7afb1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7afb1-164">Int32</span></span>|<span data-ttu-id="7afb1-165">バイト内の参照の添付ファイルをメッセージに格納されているメタデータのサイズです。</span><span class="sxs-lookup"><span data-stu-id="7afb1-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="7afb1-166">この値は実際のファイルのサイズを示すものではありません。</span><span class="sxs-lookup"><span data-stu-id="7afb1-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="7afb1-167">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7afb1-167">Optional.</span></span>|
|<span data-ttu-id="7afb1-168">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="7afb1-168">sourceUrl</span></span>|<span data-ttu-id="7afb1-169">String</span><span class="sxs-lookup"><span data-stu-id="7afb1-169">String</span></span>|<span data-ttu-id="7afb1-170">添付ファイルのコンテンツを取得する URL です。</span><span class="sxs-lookup"><span data-stu-id="7afb1-170">URL to get the attachment content.</span></span> <span data-ttu-id="7afb1-171">フォルダーへの URL の場合は、し、Outlook または Outlook web 上で正しく表示されるフォルダーの**isFolder** true に設定します。</span><span class="sxs-lookup"><span data-stu-id="7afb1-171">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="7afb1-172">必須です。</span><span class="sxs-lookup"><span data-stu-id="7afb1-172">Required.</span></span>|
|<span data-ttu-id="7afb1-173">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="7afb1-173">thumbnailUrl</span></span>|<span data-ttu-id="7afb1-174">String</span><span class="sxs-lookup"><span data-stu-id="7afb1-174">String</span></span>|<span data-ttu-id="7afb1-175">イメージのサムネイル イメージを取得する URL の参照添付ファイルのみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="7afb1-175">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="7afb1-176">**直すこと**は、イメージ ファイルを指定するときにのみ、 **thumbnailUrl**および**previewUrl**を使用します。</span><span class="sxs-lookup"><span data-stu-id="7afb1-176">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="7afb1-177">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7afb1-177">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7afb1-178">関係</span><span class="sxs-lookup"><span data-stu-id="7afb1-178">Relationships</span></span>
<span data-ttu-id="7afb1-179">なし</span><span class="sxs-lookup"><span data-stu-id="7afb1-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="7afb1-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7afb1-180">JSON representation</span></span>

<span data-ttu-id="7afb1-181">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7afb1-181">Here is a JSON representation of the resource</span></span>

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
  "permission": "referenceAttachmentPermission",
  "previewUrl": "string",
  "providerType": "referenceAttachmentProvider",
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

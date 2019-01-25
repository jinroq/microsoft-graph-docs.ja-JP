---
title: referenceAttachment リソースの種類
description: '接続されているフォルダーや、OneDrive ビジネス クラウド ドライブ、またはその他のサポートされているストレージの場所にテキスト ファイルまたは Word 文書) などのファイルへのリンク '
localization_priority: Normal
ms.openlocfilehash: 59ebb0af10a64195643cb7073d1206790ae6a875
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512711"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="1673a-103">referenceAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1673a-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1673a-104">フォルダーまたはビジネス クラウド ドライブ、またはその他の OneDrive のテキスト ファイル、または Word 文書) などのファイルへのリンクには、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または[ポスト](../resources/post.md)に接続されているストレージの場所がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="1673a-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="1673a-105">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="1673a-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1673a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1673a-106">Methods</span></span>

| <span data-ttu-id="1673a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1673a-107">Method</span></span>       | <span data-ttu-id="1673a-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1673a-108">Return Type</span></span>  |<span data-ttu-id="1673a-109">説明</span><span class="sxs-lookup"><span data-stu-id="1673a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1673a-110">取得</span><span class="sxs-lookup"><span data-stu-id="1673a-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="1673a-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="1673a-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="1673a-112">referenceAttachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1673a-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="1673a-113">Delete</span><span class="sxs-lookup"><span data-stu-id="1673a-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="1673a-114">なし</span><span class="sxs-lookup"><span data-stu-id="1673a-114">None</span></span> |<span data-ttu-id="1673a-115">referenceAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="1673a-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1673a-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1673a-116">Properties</span></span>
| <span data-ttu-id="1673a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1673a-117">Property</span></span>     | <span data-ttu-id="1673a-118">型</span><span class="sxs-lookup"><span data-stu-id="1673a-118">Type</span></span>   |<span data-ttu-id="1673a-119">説明</span><span class="sxs-lookup"><span data-stu-id="1673a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1673a-120">contentType</span><span class="sxs-lookup"><span data-stu-id="1673a-120">contentType</span></span>|<span data-ttu-id="1673a-121">String</span><span class="sxs-lookup"><span data-stu-id="1673a-121">String</span></span>|<span data-ttu-id="1673a-122">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="1673a-122">The content type of the attachment.</span></span> <span data-ttu-id="1673a-123">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1673a-123">Optional.</span></span>|
|<span data-ttu-id="1673a-124">id</span><span class="sxs-lookup"><span data-stu-id="1673a-124">id</span></span>|<span data-ttu-id="1673a-125">String</span><span class="sxs-lookup"><span data-stu-id="1673a-125">String</span></span>|<span data-ttu-id="1673a-p102">添付ファイル ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1673a-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="1673a-128">IsFolder</span><span class="sxs-lookup"><span data-stu-id="1673a-128">isFolder</span></span>|<span data-ttu-id="1673a-129">ブール値</span><span class="sxs-lookup"><span data-stu-id="1673a-129">Boolean</span></span>|<span data-ttu-id="1673a-p103">添付ファイルがフォルダーへのリンクであるかどうかを指定します。**SourceUrl** がフォルダーへのリンクの場合、true に設定する必要があります。省略可能。</span><span class="sxs-lookup"><span data-stu-id="1673a-p103">Specifies whether the attachment is a link to a folder. Must set this to true if **sourceUrl** is a link to a folder. Optional.</span></span>|
|<span data-ttu-id="1673a-133">isInline</span><span class="sxs-lookup"><span data-stu-id="1673a-133">isInline</span></span>|<span data-ttu-id="1673a-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="1673a-134">Boolean</span></span>|<span data-ttu-id="1673a-135">添付ファイルを埋め込みオブジェクトの本文にインラインで表示する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="1673a-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="1673a-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1673a-136">Optional.</span></span>|
|<span data-ttu-id="1673a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1673a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1673a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1673a-138">DateTimeOffset</span></span>|<span data-ttu-id="1673a-139">添付ファイルが最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="1673a-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="1673a-140">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="1673a-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1673a-141">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="1673a-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="1673a-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1673a-142">Optional.</span></span>|
|<span data-ttu-id="1673a-143">name</span><span class="sxs-lookup"><span data-stu-id="1673a-143">name</span></span>|<span data-ttu-id="1673a-144">String</span><span class="sxs-lookup"><span data-stu-id="1673a-144">String</span></span>|<span data-ttu-id="1673a-145">埋め込まれた添付ファイルを表すアイコンの下に表示されるテキストです。</span><span class="sxs-lookup"><span data-stu-id="1673a-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="1673a-146">これは、実際のファイル名を指定するのには必要ありません。</span><span class="sxs-lookup"><span data-stu-id="1673a-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="1673a-147">必須です。</span><span class="sxs-lookup"><span data-stu-id="1673a-147">Required.</span></span>|
|<span data-ttu-id="1673a-148">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1673a-148">permission</span></span>|<span data-ttu-id="1673a-149">ReferenceAttachmentPermissions</span><span class="sxs-lookup"><span data-stu-id="1673a-149">ReferenceAttachmentPermissions</span></span>|<span data-ttu-id="1673a-p107">**ProviderType** のプロバイダーの種類によって、添付ファイルに付与されるアクセス許可を指定します。可能な値は、`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView`、`organizationEdit` です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="1673a-p107">Specifies the permissions granted for the attachment by the type of provider in **providerType**. Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`. Optional.</span></span>|
|<span data-ttu-id="1673a-153">PreviewUrl</span><span class="sxs-lookup"><span data-stu-id="1673a-153">previewUrl</span></span>|<span data-ttu-id="1673a-154">String</span><span class="sxs-lookup"><span data-stu-id="1673a-154">String</span></span>|<span data-ttu-id="1673a-p108">プレビュー イメージを取得するための、イメージの URL の参照添付ファイルのみに適用されます。**SourceUrl** によってイメージ ファイルが識別される場合にのみ、**ThumbnailUrl** と **PreviewUrl** を使用します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="1673a-p108">Applies to only a reference attachment of an image - URL to get a preview image. Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file. Optional.</span></span>|
|<span data-ttu-id="1673a-158">ProviderType</span><span class="sxs-lookup"><span data-stu-id="1673a-158">providerType</span></span>|<span data-ttu-id="1673a-159">ReferenceAttachmentProviders</span><span class="sxs-lookup"><span data-stu-id="1673a-159">ReferenceAttachmentProviders</span></span>|<span data-ttu-id="1673a-p109">この `other` の添付ファイルをサポートするプロバイダーの種類。可能な値は、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox`、 です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="1673a-p109">The type of provider that supports an attachment of this contentType. Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`. Optional.</span></span>|
|<span data-ttu-id="1673a-163">size</span><span class="sxs-lookup"><span data-stu-id="1673a-163">size</span></span>|<span data-ttu-id="1673a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1673a-164">Int32</span></span>|<span data-ttu-id="1673a-165">バイト内の参照の添付ファイルをメッセージに格納されているメタデータのサイズです。</span><span class="sxs-lookup"><span data-stu-id="1673a-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="1673a-166">この値は実際のファイルのサイズを示すものではありません。</span><span class="sxs-lookup"><span data-stu-id="1673a-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="1673a-167">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1673a-167">Optional.</span></span>|
|<span data-ttu-id="1673a-168">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="1673a-168">sourceUrl</span></span>|<span data-ttu-id="1673a-169">String</span><span class="sxs-lookup"><span data-stu-id="1673a-169">String</span></span>|<span data-ttu-id="1673a-p111">添付ファイルの内容を取得するための URL。フォルダーへの URL の場合、Outlook または Outlook on the web 上でフォルダーが正しく表示されるには、**IsFolder** を true に設定します。必須。</span><span class="sxs-lookup"><span data-stu-id="1673a-p111">URL to get the attachment content. If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true. Required.</span></span>|
|<span data-ttu-id="1673a-173">ThumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="1673a-173">thumbnailUrl</span></span>|<span data-ttu-id="1673a-174">String</span><span class="sxs-lookup"><span data-stu-id="1673a-174">String</span></span>|<span data-ttu-id="1673a-p112">サムネイル イメージを取得するための、イメージの URL の参照添付ファイルのみに適用されます。**SourceUrl** によってイメージ ファイルが識別される場合にのみ、**ThumbnailUrl** と **PreviewUrl** を使用します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="1673a-p112">Applies to only a reference attachment of an image - URL to get a thumbnail image. Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file. Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1673a-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1673a-178">Relationships</span></span>
<span data-ttu-id="1673a-179">なし</span><span class="sxs-lookup"><span data-stu-id="1673a-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="1673a-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1673a-180">JSON representation</span></span>

<span data-ttu-id="1673a-181">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1673a-181">Here is a JSON representation of the resource</span></span>

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

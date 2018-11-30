---
title: referenceAttachment リソースの種類
description: '接続されているフォルダーや、OneDrive ビジネス クラウド ドライブ、またはその他のサポートされているストレージの場所にテキスト ファイルまたは Word 文書) などのファイルへのリンク '
ms.openlocfilehash: e9885c3a0e5c7f723303d7d6461f4c07dbed6bf6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072252"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="ca6d8-103">referenceAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ca6d8-103">referenceAttachment resource type</span></span>

> <span data-ttu-id="ca6d8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca6d8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca6d8-106">フォルダーまたはビジネス クラウド ドライブ、またはその他の OneDrive のテキスト ファイル、または Word 文書) などのファイルへのリンクには、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、 [Outlook の仕事](../resources/outlooktask.md)、または[ポスト](../resources/post.md)に接続されているストレージの場所がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-106">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="ca6d8-107">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-107">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ca6d8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ca6d8-108">Methods</span></span>

| <span data-ttu-id="ca6d8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ca6d8-109">Method</span></span>       | <span data-ttu-id="ca6d8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ca6d8-110">Return Type</span></span>  |<span data-ttu-id="ca6d8-111">説明</span><span class="sxs-lookup"><span data-stu-id="ca6d8-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ca6d8-112">取得</span><span class="sxs-lookup"><span data-stu-id="ca6d8-112">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="ca6d8-113">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="ca6d8-113">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="ca6d8-114">referenceAttachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-114">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="ca6d8-115">Delete</span><span class="sxs-lookup"><span data-stu-id="ca6d8-115">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="ca6d8-116">なし</span><span class="sxs-lookup"><span data-stu-id="ca6d8-116">None</span></span> |<span data-ttu-id="ca6d8-117">referenceAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-117">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ca6d8-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca6d8-118">Properties</span></span>
| <span data-ttu-id="ca6d8-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca6d8-119">Property</span></span>     | <span data-ttu-id="ca6d8-120">型</span><span class="sxs-lookup"><span data-stu-id="ca6d8-120">Type</span></span>   |<span data-ttu-id="ca6d8-121">説明</span><span class="sxs-lookup"><span data-stu-id="ca6d8-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca6d8-122">contentType</span><span class="sxs-lookup"><span data-stu-id="ca6d8-122">contentType</span></span>|<span data-ttu-id="ca6d8-123">String</span><span class="sxs-lookup"><span data-stu-id="ca6d8-123">String</span></span>|<span data-ttu-id="ca6d8-124">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-124">The content type of the attachment.</span></span> <span data-ttu-id="ca6d8-125">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-125">Optional.</span></span>|
|<span data-ttu-id="ca6d8-126">id</span><span class="sxs-lookup"><span data-stu-id="ca6d8-126">id</span></span>|<span data-ttu-id="ca6d8-127">String</span><span class="sxs-lookup"><span data-stu-id="ca6d8-127">String</span></span>|<span data-ttu-id="ca6d8-p103">添付ファイル ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-p103">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="ca6d8-130">isFolder</span><span class="sxs-lookup"><span data-stu-id="ca6d8-130">isFolder</span></span>|<span data-ttu-id="ca6d8-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="ca6d8-131">Boolean</span></span>|<span data-ttu-id="ca6d8-132">添付ファイルがフォルダーへのリンクであるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-132">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="ca6d8-133">True を設定**し直すこと**は、フォルダーへのリンクを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-133">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="ca6d8-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-134">Optional.</span></span>|
|<span data-ttu-id="ca6d8-135">isInline</span><span class="sxs-lookup"><span data-stu-id="ca6d8-135">isInline</span></span>|<span data-ttu-id="ca6d8-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="ca6d8-136">Boolean</span></span>|<span data-ttu-id="ca6d8-137">添付ファイルを埋め込みオブジェクトの本文にインラインで表示する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-137">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="ca6d8-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-138">Optional.</span></span>|
|<span data-ttu-id="ca6d8-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca6d8-139">lastModifiedDateTime</span></span>|<span data-ttu-id="ca6d8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca6d8-140">DateTimeOffset</span></span>|<span data-ttu-id="ca6d8-141">添付ファイルが最後に変更された日時です。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-141">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="ca6d8-142">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ca6d8-143">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ca6d8-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ca6d8-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-144">Optional.</span></span>|
|<span data-ttu-id="ca6d8-145">名前</span><span class="sxs-lookup"><span data-stu-id="ca6d8-145">name</span></span>|<span data-ttu-id="ca6d8-146">String</span><span class="sxs-lookup"><span data-stu-id="ca6d8-146">String</span></span>|<span data-ttu-id="ca6d8-147">埋め込まれた添付ファイルを表すアイコンの下に表示されるテキストです。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-147">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="ca6d8-148">これは、実際のファイル名を指定するのには必要ありません。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-148">This does not need to be the actual file name.</span></span> <span data-ttu-id="ca6d8-149">必須。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-149">Required.</span></span>|
|<span data-ttu-id="ca6d8-150">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ca6d8-150">permission</span></span>|<span data-ttu-id="ca6d8-151">ReferenceAttachmentPermissions</span><span class="sxs-lookup"><span data-stu-id="ca6d8-151">ReferenceAttachmentPermissions</span></span>|<span data-ttu-id="ca6d8-152">**プロバイダーの種類**のプロバイダーの種類によって、添付ファイルに付与するアクセス許可を指定します。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-152">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="ca6d8-153">可能な値は、`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView`、`organizationEdit` です。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-153">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="ca6d8-154">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-154">Optional.</span></span>|
|<span data-ttu-id="ca6d8-155">previewUrl</span><span class="sxs-lookup"><span data-stu-id="ca6d8-155">previewUrl</span></span>|<span data-ttu-id="ca6d8-156">String</span><span class="sxs-lookup"><span data-stu-id="ca6d8-156">String</span></span>|<span data-ttu-id="ca6d8-157">イメージのプレビュー イメージを取得する URL の参照添付ファイルのみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-157">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="ca6d8-158">**直すこと**は、イメージ ファイルを指定するときにのみ、 **thumbnailUrl**および**previewUrl**を使用します。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-158">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="ca6d8-159">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-159">Optional.</span></span>|
|<span data-ttu-id="ca6d8-160">プロバイダーの種類</span><span class="sxs-lookup"><span data-stu-id="ca6d8-160">providerType</span></span>|<span data-ttu-id="ca6d8-161">ReferenceAttachmentProviders</span><span class="sxs-lookup"><span data-stu-id="ca6d8-161">ReferenceAttachmentProviders</span></span>|<span data-ttu-id="ca6d8-162">このコンテンツ タイプの添付ファイルをサポートするプロバイダーの型。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-162">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="ca6d8-163">可能な値は、`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox` です。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-163">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="ca6d8-164">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-164">Optional.</span></span>|
|<span data-ttu-id="ca6d8-165">size</span><span class="sxs-lookup"><span data-stu-id="ca6d8-165">size</span></span>|<span data-ttu-id="ca6d8-166">Int32</span><span class="sxs-lookup"><span data-stu-id="ca6d8-166">Int32</span></span>|<span data-ttu-id="ca6d8-167">バイト内の参照の添付ファイルをメッセージに格納されているメタデータのサイズです。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-167">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="ca6d8-168">この値は実際のファイルのサイズを示すものではありません。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-168">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="ca6d8-169">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-169">Optional.</span></span>|
|<span data-ttu-id="ca6d8-170">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="ca6d8-170">sourceUrl</span></span>|<span data-ttu-id="ca6d8-171">String</span><span class="sxs-lookup"><span data-stu-id="ca6d8-171">String</span></span>|<span data-ttu-id="ca6d8-172">添付ファイルのコンテンツを取得する URL です。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-172">URL to get the attachment content.</span></span> <span data-ttu-id="ca6d8-173">フォルダーへの URL の場合は、し、Outlook または Outlook web 上で正しく表示されるフォルダーの**isFolder** true に設定します。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-173">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="ca6d8-174">必須。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-174">Required.</span></span>|
|<span data-ttu-id="ca6d8-175">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="ca6d8-175">thumbnailUrl</span></span>|<span data-ttu-id="ca6d8-176">String</span><span class="sxs-lookup"><span data-stu-id="ca6d8-176">String</span></span>|<span data-ttu-id="ca6d8-177">イメージのサムネイル イメージを取得する URL の参照添付ファイルのみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-177">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="ca6d8-178">**直すこと**は、イメージ ファイルを指定するときにのみ、 **thumbnailUrl**および**previewUrl**を使用します。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-178">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="ca6d8-179">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ca6d8-179">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca6d8-180">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ca6d8-180">Relationships</span></span>
<span data-ttu-id="ca6d8-181">なし</span><span class="sxs-lookup"><span data-stu-id="ca6d8-181">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="ca6d8-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ca6d8-182">JSON representation</span></span>

<span data-ttu-id="ca6d8-183">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="ca6d8-183">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

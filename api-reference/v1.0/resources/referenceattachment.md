---
title: referenceAttachment リソースの種類
description: OneDrive for Business のクラウド ドライブまたは他のサポートされている保存場所にあり、イベント、メッセージ、または投稿にアタッチされているファイル (テキスト ファイルまたは Word 文書など) へのリンク。
localization_priority: Normal
ms.openlocfilehash: 0696ac4b0f93ed4982ec576a15afe071486f9c88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579416"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="4d19e-103">referenceAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d19e-103">referenceAttachment resource type</span></span>

<span data-ttu-id="4d19e-104">OneDrive for Business のクラウド ドライブまたは他のサポートされている保存場所にあり、イベント、メッセージ、または投稿にアタッチされているファイル (テキスト ファイルまたは Word 文書など) へのリンク。</span><span class="sxs-lookup"><span data-stu-id="4d19e-104">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="4d19e-105">[添付ファイル](attachment.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="4d19e-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4d19e-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4d19e-106">Methods</span></span>

| <span data-ttu-id="4d19e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4d19e-107">Method</span></span>       | <span data-ttu-id="4d19e-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4d19e-108">Return Type</span></span>  |<span data-ttu-id="4d19e-109">説明</span><span class="sxs-lookup"><span data-stu-id="4d19e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4d19e-110">取得</span><span class="sxs-lookup"><span data-stu-id="4d19e-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="4d19e-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="4d19e-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="4d19e-112">referenceAttachment オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4d19e-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="4d19e-113">削除</span><span class="sxs-lookup"><span data-stu-id="4d19e-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="4d19e-114">なし</span><span class="sxs-lookup"><span data-stu-id="4d19e-114">None</span></span> |<span data-ttu-id="4d19e-115">referenceAttachment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="4d19e-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4d19e-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d19e-116">Properties</span></span>
| <span data-ttu-id="4d19e-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d19e-117">Property</span></span>     | <span data-ttu-id="4d19e-118">型</span><span class="sxs-lookup"><span data-stu-id="4d19e-118">Type</span></span>   |<span data-ttu-id="4d19e-119">説明</span><span class="sxs-lookup"><span data-stu-id="4d19e-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d19e-120">contentType</span><span class="sxs-lookup"><span data-stu-id="4d19e-120">contentType</span></span>|<span data-ttu-id="4d19e-121">String</span><span class="sxs-lookup"><span data-stu-id="4d19e-121">String</span></span>|<span data-ttu-id="4d19e-122">添付ファイルのコンテンツ タイプ。</span><span class="sxs-lookup"><span data-stu-id="4d19e-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="4d19e-123">id</span><span class="sxs-lookup"><span data-stu-id="4d19e-123">id</span></span>|<span data-ttu-id="4d19e-124">String</span><span class="sxs-lookup"><span data-stu-id="4d19e-124">String</span></span>|<span data-ttu-id="4d19e-p101">添付ファイル ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d19e-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="4d19e-127">isInline</span><span class="sxs-lookup"><span data-stu-id="4d19e-127">isInline</span></span>|<span data-ttu-id="4d19e-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="4d19e-128">Boolean</span></span>|<span data-ttu-id="4d19e-129">添付ファイルを埋め込みオブジェクトの本文にインラインで表示する場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="4d19e-129">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="4d19e-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d19e-130">lastModifiedDateTime</span></span>|<span data-ttu-id="4d19e-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d19e-131">DateTimeOffset</span></span>|<span data-ttu-id="4d19e-p102">添付ファイルが最後に変更された日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4d19e-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4d19e-135">name</span><span class="sxs-lookup"><span data-stu-id="4d19e-135">name</span></span>|<span data-ttu-id="4d19e-136">String</span><span class="sxs-lookup"><span data-stu-id="4d19e-136">String</span></span>|<span data-ttu-id="4d19e-p103">埋め込まれた添付ファイルを表すアイコンの下に表示されるテキスト。実際のファイル名である必要はありません。</span><span class="sxs-lookup"><span data-stu-id="4d19e-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="4d19e-139">size</span><span class="sxs-lookup"><span data-stu-id="4d19e-139">size</span></span>|<span data-ttu-id="4d19e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4d19e-140">Int32</span></span>|<span data-ttu-id="4d19e-141">添付ファイルのメッセージに格納されているメタデータのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="4d19e-141">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="4d19e-142">この値は実際のファイルのサイズを示すものではありません。</span><span class="sxs-lookup"><span data-stu-id="4d19e-142">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d19e-143">関係</span><span class="sxs-lookup"><span data-stu-id="4d19e-143">Relationships</span></span>
<span data-ttu-id="4d19e-144">なし</span><span class="sxs-lookup"><span data-stu-id="4d19e-144">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="4d19e-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4d19e-145">JSON representation</span></span>

<span data-ttu-id="4d19e-146">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4d19e-146">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.attachment",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
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
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

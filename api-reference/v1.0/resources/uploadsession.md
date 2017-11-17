---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
ms.openlocfilehash: d84b588c28791ab8f1cf6cef1be6af767fa18e47
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="uploadsession-resource"></a><span data-ttu-id="69d39-102">UploadSession リソース</span><span class="sxs-lookup"><span data-stu-id="69d39-102">UploadSession resource</span></span>

<span data-ttu-id="69d39-103">**UploadSession** リソースは、OneDrive、OneDrive for Business、または SharePoint のドキュメント ライブラリに、大容量ファイルをアップロードする方法に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="69d39-103">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69d39-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="69d39-104">JSON representation</span></span>

<span data-ttu-id="69d39-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="69d39-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="properties"></a><span data-ttu-id="69d39-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69d39-106">Properties</span></span>


| <span data-ttu-id="69d39-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69d39-107">Property</span></span>       | <span data-ttu-id="69d39-108">型</span><span class="sxs-lookup"><span data-stu-id="69d39-108">Type</span></span>              |<span data-ttu-id="69d39-109">説明</span><span class="sxs-lookup"><span data-stu-id="69d39-109">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="69d39-110">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="69d39-110">expirationDateTime</span></span> | <span data-ttu-id="69d39-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69d39-111">DateTimeOffset</span></span>    | <span data-ttu-id="69d39-p101">アップロード セッションの有効期限が切れる日時の UTC 表示。この有効期限に達する前に、完全なファイルをアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="69d39-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="69d39-114">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="69d39-114">nextExpectedRanges</span></span> | <span data-ttu-id="69d39-115">String collection</span><span class="sxs-lookup"><span data-stu-id="69d39-115">String collection</span></span> | <span data-ttu-id="69d39-p102">サーバーのファイルに足りないバイト範囲のコレクションです。これらの範囲は 0 インデックスが作成されており、「開始-終了」形式のものです (例、「0-26」でファイルの最初の 27 バイトを示す)。</span><span class="sxs-lookup"><span data-stu-id="69d39-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="69d39-118">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="69d39-118">uploadUrl</span></span>          | <span data-ttu-id="69d39-119">String</span><span class="sxs-lookup"><span data-stu-id="69d39-119">String</span></span>            | <span data-ttu-id="69d39-120">ファイルのバイト範囲の PUT 要求を受け付ける URL エンドポイントです。</span><span class="sxs-lookup"><span data-stu-id="69d39-120">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="69d39-121">その他の技術情報</span><span class="sxs-lookup"><span data-stu-id="69d39-121">Additional Resources</span></span>

<span data-ttu-id="69d39-122">アップロード セッションを使用してファイルをアップロードする方法の詳細は、「[アップロード セッションを使ってサイズの大きなファイルをアップロードする](../api/driveitem_createuploadsession.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69d39-122">See [Upload large files with an upload session](../api/driveitem_createuploadsession.md) for details on how to upload files using an upload session.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->

---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: UploadSession リソースは、OneDrive、OneDrive for Business、または SharePoint のドキュメント ライブラリに、大容量ファイルをアップロードする方法に関する情報を提供します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 49453d730e1195c68b1c6245496e9c5530aba720
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033545"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="c1d38-103">UploadSession リソース</span><span class="sxs-lookup"><span data-stu-id="c1d38-103">UploadSession resource</span></span>

<span data-ttu-id="c1d38-104">**UploadSession** リソースは、OneDrive、OneDrive for Business、または SharePoint のドキュメント ライブラリに、大容量ファイルをアップロードする方法に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c1d38-104">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1d38-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1d38-105">JSON representation</span></span>

<span data-ttu-id="c1d38-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c1d38-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="c1d38-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1d38-107">Properties</span></span>


| <span data-ttu-id="c1d38-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1d38-108">Property</span></span>       | <span data-ttu-id="c1d38-109">型</span><span class="sxs-lookup"><span data-stu-id="c1d38-109">Type</span></span>              |<span data-ttu-id="c1d38-110">説明</span><span class="sxs-lookup"><span data-stu-id="c1d38-110">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="c1d38-111">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c1d38-111">expirationDateTime</span></span> | <span data-ttu-id="c1d38-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1d38-112">DateTimeOffset</span></span>    | <span data-ttu-id="c1d38-p101">アップロード セッションの有効期限が切れる日時の UTC 表示。この有効期限に達する前に、完全なファイルをアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c1d38-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="c1d38-115">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="c1d38-115">nextExpectedRanges</span></span> | <span data-ttu-id="c1d38-116">String collection</span><span class="sxs-lookup"><span data-stu-id="c1d38-116">String collection</span></span> | <span data-ttu-id="c1d38-p102">サーバーのファイルに足りないバイト範囲のコレクションです。これらの範囲は 0 インデックスが作成されており、「開始-終了」形式のものです (例、「0-26」でファイルの最初の 27 バイトを示す)。</span><span class="sxs-lookup"><span data-stu-id="c1d38-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="c1d38-119">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="c1d38-119">uploadUrl</span></span>          | <span data-ttu-id="c1d38-120">String</span><span class="sxs-lookup"><span data-stu-id="c1d38-120">String</span></span>            | <span data-ttu-id="c1d38-121">ファイルのバイト範囲の PUT 要求を受け付ける URL エンドポイントです。</span><span class="sxs-lookup"><span data-stu-id="c1d38-121">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="c1d38-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="c1d38-122">See also</span></span>

- [<span data-ttu-id="c1d38-123">アップロード セッションを使ってサイズが大きいファイルをアップロードする</span><span class="sxs-lookup"><span data-stu-id="c1d38-123">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->

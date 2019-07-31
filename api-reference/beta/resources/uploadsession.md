---
author: JeremyKelley
description: <descrption>
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6b047c8eed22647083da07f2e7722269fb872783
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964229"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="00d22-102">UploadSession リソース</span><span class="sxs-lookup"><span data-stu-id="00d22-102">UploadSession resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00d22-103">**UploadSession** リソースは、OneDrive、OneDrive for Business、または SharePoint のドキュメント ライブラリに、大容量ファイルをアップロードする方法に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="00d22-103">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="00d22-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="00d22-104">JSON representation</span></span>

<span data-ttu-id="00d22-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="00d22-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="00d22-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00d22-106">Properties</span></span>


| <span data-ttu-id="00d22-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00d22-107">Property</span></span>       | <span data-ttu-id="00d22-108">型</span><span class="sxs-lookup"><span data-stu-id="00d22-108">Type</span></span>              |<span data-ttu-id="00d22-109">説明</span><span class="sxs-lookup"><span data-stu-id="00d22-109">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="00d22-110">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="00d22-110">expirationDateTime</span></span> | <span data-ttu-id="00d22-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00d22-111">DateTimeOffset</span></span>    | <span data-ttu-id="00d22-p101">アップロード セッションの有効期限が切れる日時の UTC 表示。この有効期限に達する前に、完全なファイルをアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="00d22-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="00d22-114">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="00d22-114">nextExpectedRanges</span></span> | <span data-ttu-id="00d22-115">String collection</span><span class="sxs-lookup"><span data-stu-id="00d22-115">String collection</span></span> | <span data-ttu-id="00d22-p102">サーバーのファイルに足りないバイト範囲のコレクションです。これらの範囲は 0 インデックスが作成されており、「開始-終了」形式のものです (例、「0-26」でファイルの最初の 27 バイトを示す)。</span><span class="sxs-lookup"><span data-stu-id="00d22-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="00d22-118">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="00d22-118">uploadUrl</span></span>          | <span data-ttu-id="00d22-119">String</span><span class="sxs-lookup"><span data-stu-id="00d22-119">String</span></span>            | <span data-ttu-id="00d22-120">ファイルのバイト範囲の PUT 要求を受け付ける URL エンドポイントです。</span><span class="sxs-lookup"><span data-stu-id="00d22-120">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="00d22-121">関連項目</span><span class="sxs-lookup"><span data-stu-id="00d22-121">See also</span></span>

- [<span data-ttu-id="00d22-122">アップロード セッションを使ってサイズが大きいファイルをアップロードする</span><span class="sxs-lookup"><span data-stu-id="00d22-122">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession",
  "suppressions": []
}
-->

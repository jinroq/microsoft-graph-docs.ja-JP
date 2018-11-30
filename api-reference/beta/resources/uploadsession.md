---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
ms.openlocfilehash: 27e3b448b54df0a5d35e2992391a554b73fd2c42
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074409"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="e43dc-102">UploadSession リソース</span><span class="sxs-lookup"><span data-stu-id="e43dc-102">UploadSession resource</span></span>

> <span data-ttu-id="e43dc-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e43dc-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e43dc-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e43dc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e43dc-105">**UploadSession** リソースは、OneDrive、OneDrive for Business、または SharePoint のドキュメント ライブラリに、大容量ファイルをアップロードする方法に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="e43dc-105">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e43dc-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e43dc-106">JSON representation</span></span>

<span data-ttu-id="e43dc-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e43dc-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e43dc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e43dc-108">Properties</span></span>


| <span data-ttu-id="e43dc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e43dc-109">Property</span></span>       | <span data-ttu-id="e43dc-110">型</span><span class="sxs-lookup"><span data-stu-id="e43dc-110">Type</span></span>              |<span data-ttu-id="e43dc-111">説明</span><span class="sxs-lookup"><span data-stu-id="e43dc-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="e43dc-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e43dc-112">expirationDateTime</span></span> | <span data-ttu-id="e43dc-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e43dc-113">DateTimeOffset</span></span>    | <span data-ttu-id="e43dc-p102">アップロード セッションの有効期限が切れる日時の UTC 表示。この有効期限に達する前に、完全なファイルをアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="e43dc-p102">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="e43dc-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="e43dc-116">nextExpectedRanges</span></span> | <span data-ttu-id="e43dc-117">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e43dc-117">String collection</span></span> | <span data-ttu-id="e43dc-p103">サーバーのファイルに足りないバイト範囲のコレクションです。これらの範囲は 0 インデックスが作成されており、「開始-終了」形式のものです (例、「0-26」でファイルの最初の 27 バイトを示す)。</span><span class="sxs-lookup"><span data-stu-id="e43dc-p103">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="e43dc-120">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="e43dc-120">uploadUrl</span></span>          | <span data-ttu-id="e43dc-121">String</span><span class="sxs-lookup"><span data-stu-id="e43dc-121">String</span></span>            | <span data-ttu-id="e43dc-122">ファイルのバイト範囲の PUT 要求を受け付ける URL エンドポイントです。</span><span class="sxs-lookup"><span data-stu-id="e43dc-122">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="e43dc-123">関連項目</span><span class="sxs-lookup"><span data-stu-id="e43dc-123">See also</span></span>

- [<span data-ttu-id="e43dc-124">アップロード セッションを使ってサイズの大きなファイルをアップロードする</span><span class="sxs-lookup"><span data-stu-id="e43dc-124">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->

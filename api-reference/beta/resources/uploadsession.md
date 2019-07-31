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
# <a name="uploadsession-resource"></a>UploadSession リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**UploadSession** リソースは、OneDrive、OneDrive for Business、または SharePoint のドキュメント ライブラリに、大容量ファイルをアップロードする方法に関する情報を提供します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

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

## <a name="properties"></a>プロパティ


| プロパティ       | 型              |説明
|:-------------------|:------------------|:------------------------------------
| expirationDateTime | DateTimeOffset    | アップロード セッションの有効期限が切れる日時の UTC 表示。この有効期限に達する前に、完全なファイルをアップロードする必要があります。
| nextExpectedRanges | String collection | サーバーのファイルに足りないバイト範囲のコレクションです。これらの範囲は 0 インデックスが作成されており、「開始-終了」形式のものです (例、「0-26」でファイルの最初の 27 バイトを示す)。
| uploadUrl          | String            | ファイルのバイト範囲の PUT 要求を受け付ける URL エンドポイントです。

## <a name="see-also"></a>関連項目

- [アップロード セッションを使ってサイズが大きいファイルをアップロードする](../api/driveitem-createuploadsession.md)

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

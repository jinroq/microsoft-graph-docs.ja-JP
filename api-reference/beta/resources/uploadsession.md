---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
ms.openlocfilehash: 85e26779d7c7df72a3176290654511ebd0f9493b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576116"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/uploadsession.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

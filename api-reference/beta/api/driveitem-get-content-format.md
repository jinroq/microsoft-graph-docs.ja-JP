---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 他の形式に変換する
localization_priority: Normal
ms.openlocfilehash: d27420153a295eac9d3f880910d63bd701525427
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887438"
---
# <a name="download-a-file-in-another-format"></a>別の形式でファイルをダウンロードする

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

この API を使用して、アイテムのコンテンツを特定の形式で取得します。
すべてのファイルがすべての形式に変換できるわけではありません。

元の形式でアイテムをダウンロードするには、[アイテムの内容をダウンロードする](driveitem-get-content.md)を参照してください。

## <a name="prerequisites"></a>前提条件

この API を呼び出すには、ユーザーがアプリケーションに対して、アプリが変換するファイルへの読み取りアクセス権を付与している必要があります。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a>クエリ パラメーター

| Parameter      | Type  | 説明                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| _format_  | 文字列 | アイテムのコンテンツをダウンロードする形式を指定します。 |


次の値は、 **format**パラメーターに有効です。

| 値 | 説明                        | サポートされているソースの拡張子
|:------|:-----------------------------------|---------------------------------
| glb   | GLB の形式にアイテムを変換します。  | クール、fbx、obj、プライ、stl、3mf
| html  | 項目を HTML 形式に変換します。 | eml, md, メッセージ
| jpg   | アイテムを JPG 形式に変換します。  | 3 g 2、3 gp、3gp2、3 gpp、3mf、ai、arw、asf、avi、bas、bash、bat、bmp、c、cbl、cmd、冷却、cpp、cr2、crw、cs、css、csv、cur、dcm、dcm30、dic、dicm、dicom、dng、doc、docx、dwg、eml、epi、eps、epsf、epsi、epub 形式、erf、fbx、fppx、gif、glb、h、hcp、heic、heif、htm、html、ico、アイコン、java、欠落、jpeg、jpg、js、json、キー、ログ、m2ts、m4a、m4v、値下げ、md、mef、mov、ビデオ、mp3、mp4、mp4v、mrw、msg、mts、nef、nrw、番号、obj、odp、密接に関連、ogg、orf、ページ、pano、pdf、pef、php、pict、pl、プライ、png、ポット、potm、potx、pps、ppsx、ppsxm、ppt、pptm、pptx、ps、ps1、psb、psd、py、生の、rb、rtf 形式、rw1、rw2、sh では、スケッチ、sql、sr2、stl、tif、tiff、ts、txt、vb、webm、wma、wmv、xaml、xbm、xcf、xd、xml、xpm、yaml、yml
| pdf   | 項目を PDF 形式に変換します。  | doc、docx、epub 形式、eml、htm、html、md、メッセージ、odp、ods、密接に関連、pps、ppsx、ppt、pptx、rtf 形式、tif、tiff、xls、xlsm、xlsx

## <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前            | 値   | 説明                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | String  | この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。 |

## <a name="example"></a>例

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a>応答

変換されたファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。

変換されたファイルをダウンロードするには、アプリが応答の `Location` ヘッダーに従う必要があります。

事前認証された URL は、短期間 (数分) のみ有効で、アクセスのために `Authorization` ヘッダーを必要としません。

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a>エラー応答

エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->

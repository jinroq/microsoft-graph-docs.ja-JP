---
author: JeremyKelley
description: この API を使用して、アイテムのコンテンツを特定の形式で取得します。
ms.date: 09/10/2017
title: 他の形式に変換する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 914f6b5d847c6b8af5439c4b5e83f3d9f281aa65
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719382"
---
# <a name="download-a-file-in-another-format"></a>別の形式でファイルをダウンロードする

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

この API を使用して、アイテムのコンテンツを特定の形式で取得します。
すべてのファイルがすべての形式に変換できるわけではありません。

アイテムを元の形式でダウンロードするには、「[アイテムのコンテンツをダウンロードする](driveitem-get-content.md)」を参照してください。

## <a name="prerequisites"></a>前提条件

この API を呼び出すには、ユーザーがアプリケーションに対して、アプリが変換するファイルへの読み取りアクセス権を付与している必要があります。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a>クエリ パラメーター

| パラメーター      | 型  | 説明                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| _format_  | string | アイテムのコンテンツをダウンロードする形式を指定します。 |


**format** パラメーターには次の値を指定できます。

| 値 | 説明                        | サポートされているソースの拡張子
|:------|:-----------------------------------|---------------------------------
| glb   | アイテムを GLB 形式に変換します。  | クール、fbx、obj、プライ、stl、3mf
| Html  | アイテムを HTML 形式に変換します。 | eml、md、msg
| .jpg   | 項目を JPG 形式に変換します。  | 3g2、3gp、3g2、3gpp、3mf、ai、arw、asf、avi、bas、bash、bat、bmp、c、cbl、cmd、クール、cpp、cr2、crw、cs、css、csv、dcm30、dcm、、.dic、dicm、dicom、dng、doc、.docx、dwg、eml、epi、.eps、epsf、epsi、epub、glb、h、および、heic、heic、htm、html、.ico、icon、java、jfif、jpeg、jpg、js、json、key、log、m2ts、m4a、m4v、markdown、md、mef、mov、movie、、mp4、mp4v、mrw、msg、mts、nef、nrw、ogg、obj、、、、pef、、、pict、、、php、pict、pl、プライ、png、.pot、potm、potx、pps、ppsx、ppsxm、ppt、pptm、.pptx、ps、ps1、psb、psd、py、raw、、rtf、rw1、rw2、sh、sketch、sql、sr2、、、、ts、txt、vb、webm、wma、wmv、xaml、xbm、xcf、xd、xml、xpm、yaml、yml
| pdf   | アイテムを PDF 形式に変換します。  | doc、.docx、epub、eml、htm、html、md、msg、odp、ods、odt、pps、ppsx、ppt、.pptx、rtf、tif、tiff、xls、.xlsm、.xlsx

## <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前            | 値   | 説明                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | String  | この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。 |

## <a name="example"></a>例


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /drive/items/{item-id}/content?format={format}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

<!--
{
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": [
  ]
}
-->

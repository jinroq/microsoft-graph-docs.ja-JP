---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: b0c6eab7d2111870192a4ed6c30c1cbd72e4163e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022974"
---
# <a name="personorgroupcolumn-resource-type"></a>PersonOrGroupColumn リソースの種類

[columnDefinition](columndefinition.md) リソースの **PersonOrGroupColumn** は、列の値がディレクトリから選択した個人またはグループを表すことを示しています。

## <a name="json-representation"></a>JSON 表記

以下は、**personOrGroupColumn** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名              | 種類    | 説明
|:---------------------------|:--------|:--------------------------------------
| **allowMultipleSelection** | boolean | ソースから複数の値を選択できるかどうかを示します。
| **displayAs**              | string  | 選択された個人またはグループについての情報を表示する方法。 以下を参照してください。
| **chooseFromType**         | string  | 個人のみ選択、または個人とグループの選択が可能かどうか。 `peopleAndGroups` または `peopleOnly` のいずれかでなければなりません。

## <a name="displayas-options"></a>DisplayAs オプション

| DisplayAs 値               | 説明
|:------------------------------|:-----------------------
| **account**                   | 個人またはグループの、未加工の SharePoint エンコードの要求文字列 (たとえば  i:0#.f|membership|jane@contoso.com)。
| **department**                | 個人またはグループの部門。
| **firstName**                 | 個人の名。
| **id**                        | ディレクトリ内の個人またはグループの ID。
| **lastName**                  | 個人の姓。
| **mobilePhone**               | 個人の携帯電話番号。
| **name**                      | 個人の名前。
| **nameWithPictureAndDetails** | 個人の名前、画像、その他の詳細。
| **nameWithPresence**          | 既定値。 個人の名前とプレゼンス インジケーターのアイコン (連絡可能/通話中/その他)
| **office**                    | 個人の会社の電話番号。
| **pictureOnly36x36**          | 36 x 36 ピクセルの正方形で囲まれた個人の画像。
| **pictureOnly48x48**          | 48 x 48 ピクセルの正方形で囲まれた個人の画像。
| **pictureOnly72x72**          | 72 x 72 ピクセルの正方形で囲まれた個人の画像。
| **sipAddress**                | 個人の SIP アドレス。
| **title**                     | 個人の組織内での役職。
| **userName**                  | 個人またはグループのユーザー名。
| **workEmail**                 | 個人またはグループのメール アドレス。
| **workPhone**                 | 個人の勤務先電話番号。

注: その他の DisplayAs の種類が返される可能性があります。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(peopleAndGroups,peopleOnly) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(account,contentType,created,department,...) are in resource, but () are in table"
  ],
  "tocPath": "Resources/PersonOrGroupColumn"
} -->

---
title: 契約のリソースの種類
description: テナントのカスタマイズ可能な使用許諾契約書が作成され、Azure Active Directory (AD の Azure) を使用して管理する条件を表します。 機能を管理、Azure Active Directory の使用条件に従って、シナリオを作成し、次のメソッドを使用できます。
localization_priority: Normal
ms.openlocfilehash: 8c082ed6229b44cc3a3d4cba6dd8645feee5d07c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845347"
---
# <a name="agreement-resource-type"></a>契約のリソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

テナントのカスタマイズ可能な使用許諾契約書が作成され、Azure Active Directory (AD の Azure) を使用して管理する条件を表します。 作成し、シナリオに基づく[Azure Active Directory の使用条件の機能](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou)を管理するのには、次のメソッドを使用できます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [契約書を作成します。](../api/agreement-post-agreements.md) | [契約](agreement.md) | 契約コレクションへの投稿には、新しい契約を作成します。 |
| [リスト契約](../api/agreement-list.md) | [契約](agreement.md)コレクション | 契約オブジェクト コレクションを取得します。 |
| [契約を取得します。](../api/agreement-get.md) | [契約](agreement.md) | 契約オブジェクトのプロパティと関係を参照してください。 |
| [契約を更新します。](../api/agreement-update.md) | [契約](agreement.md) | 契約オブジェクトを更新します。 |
| [契約を削除します。](../api/agreement-delete.md) | なし | 契約オブジェクトを削除します。 |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>プロパティ
| プロパティ     | 種類        | 説明 |
|:-------------|:------------|:------------|
|displayName|String|契約書の名前を表示します。|
|id|String| 読み取り専用です。|
|isViewingBeforeAcceptanceRequired|ブール型|ユーザーを展開し、受け入れる前に契約書を表示するかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|files|[agreementFile](agreementfile.md)コレクション|読み取り専用です。 Pdf は、本契約にリンクされています。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isViewingBeforeAcceptanceRequired": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

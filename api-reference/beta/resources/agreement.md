---
title: 契約のリソースの種類
description: テナントのカスタマイズ可能な使用許諾契約書が作成され、Azure Active Directory (AD の Azure) を使用して管理する条件を表します。 機能を管理、Azure Active Directory の使用条件に従って、シナリオを作成し、次のメソッドを使用できます。
ms.openlocfilehash: 2e5c9087cd809f9c067150654d420fda533ca61b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068805"
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
| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|displayName|String|契約書の名前を表示します。|
|id|String| 読み取り専用。|
|isViewingBeforeAcceptanceRequired|ブール値|ユーザーを展開し、受け入れる前に契約書を表示するかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|files|[agreementFile](agreementfile.md)コレクション|読み取り専用。 Pdf は、本契約にリンクされています。|

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

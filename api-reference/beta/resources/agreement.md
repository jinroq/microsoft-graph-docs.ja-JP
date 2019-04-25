---
title: アグリーメントリソースの種類
description: azure Active Directory (azure AD) で作成および管理されるテナントのカスタマイズ可能な利用規約を表します。 次のメソッドを使用すると、シナリオに従って、Azure Active Directory の使用条件の作成と管理を行うことができます。
localization_priority: Normal
ms.openlocfilehash: b253877f1bf82e4fbc61cebaef3c1bce208d9cca
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535749"
---
# <a name="agreement-resource-type"></a>アグリーメントリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

azure Active Directory (azure AD) で作成および管理されるテナントのカスタマイズ可能な利用規約を表します。 次のメソッドを使用すると、シナリオに従って、 [Azure Active Directory の使用条件の](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou)作成と管理を行うことができます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [契約の作成](../api/agreement-post-agreements.md) | [保証](agreement.md) | アグリーメントコレクションに投稿して、新しい契約を作成します。 |
| [契約を一覧表示する](../api/agreement-list.md) | [アグリーメント](agreement.md)コレクション | アグリーメントオブジェクトのコレクションを取得します。 |
| [契約を取得する](../api/agreement-get.md) | [保証](agreement.md) | アグリーメントオブジェクトのプロパティとリレーションシップを読み取ります。 |
| [契約を更新する](../api/agreement-update.md) | [保証](agreement.md) | アグリーメントオブジェクトを更新します。 |
| [契約を削除する](../api/agreement-delete.md) | なし | アグリーメントオブジェクトを削除します。 |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>プロパティ
| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|displayName|String|アグリーメントの表示名。|
|id|String| 読み取り専用です。|
|isViewingBeforeAcceptanceRequired|ブール値|ユーザーが同意する前に、契約を展開して表示する必要があるかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|files|[agreementFile](agreementfile.md)コレクション|読み取り専用。 このアグリーメントにリンクされている pdf。|

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
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreement.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

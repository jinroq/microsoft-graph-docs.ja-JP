---
title: privilegedOperationEvent リソースの種類
description: 管理者が特権のある役割を管理する、ユーザーが自分の役割をアクティブにし、ユーザーがその役割を非アクティブ化するなどの役割操作について特権 id 管理によって生成される監査イベントを表します。
localization_priority: Normal
ms.openlocfilehash: 2ad8f7e5db956dfbb2fa0d74f441b01f2b5d68aa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563679"
---
# <a name="privilegedoperationevent-resource-type"></a>privilegedOperationEvent リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

管理者が特権のある役割を管理する、ユーザーが自分の役割をアクティブにし、ユーザーがその役割を非アクティブ化するなどの役割操作について特権 id 管理によって生成される監査イベントを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リスト privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md)コレクション。 |privilegedOperationEvent オブジェクトのコレクションを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|additionalinformation|string|イベントに関する人の詳細な読み取り情報。|
|日付/時刻 (datetime)|dateTimeOffset|イベントが作成された時刻を示します。|
|expirationDateTime|dateTimeOffset|これは、requestType が "Activate" の場合にのみ使用され、役割のアクティブ化の有効期限を示します。|
|id|string|privilegedOperationEvent の一意識別子。 読み取り専用。|
|referencekey|string|ロールライセンス認証時のインシデント/要求チケット番号。 この値は、ロールのライセンス認証時にチケット番号が提供されている場合にのみ表示されます。|
|referenceSystem|string|tole アクティブ化の間に提供されたインシデント/要求のチケットのシステム。 この値は、チケットシステムが役割のライセンス認証時に提供された場合にのみ表示されます。|
|requestType|string|要求操作の種類。 requestType の値は、( ```Assign```役割の割り当て)、 ```Activate``` ```Unassign``` (役割のアクティブ化)、(役割の割り当て```Deactivate```の削除)、( ```ScanAlersNow```役割の非アクティブ化) ```DismissAlert``` 、(スキャンセキュリティの警告```FixAlertItem``` )、(セキュリティの警告を無視する) の各値にすることができます (セキュリティを修正します)。アラートの問題) ```AccessReview_Review``` 、(アクセスレビューを確認する```AccessReview_Create``` )、(アクセスレビューを更新```AccessReview_Update```する)、(アクセスレビューを削除```AccessReview_Delete```する) を参照してください。|
|requestorId|string|操作を開始するリクエスターのユーザー id。|
|requestorName|string|操作を開始するリクエスターのユーザー名。|
|roleId|string|操作に関連付けられているロールの id。|
|roleName|string|ロールの名前。|
|tenantId|string|テナント (組織) id。|
|userId|string|操作に関連付けられているユーザーの id。|
|usermail|string|ユーザーの電子メール。|
|userName|string|ユーザーの表示名。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedOperationEvent"
}-->

```json
{
  "additionalInformation": "string",
  "creationDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "requestType": "string",
  "requestorId": "string",
  "requestorName": "string",
  "roleId": "string",
  "roleName": "string",
  "tenantId": "string",
  "userId": "string",
  "userMail": "string",
  "userName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedOperationEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedoperationevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: governanceRoleSetting の更新
description: governanceRoleSetting のプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: f9c851f95df340693626ff82c960243eb2f85b54
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789621"
---
# <a name="update-governancerolesetting"></a>governanceRoleSetting の更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[governanceRoleSetting](../resources/governancerolesetting.md)のプロパティを更新します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

>**注:** また、この API では、リクエスターがリソースに`Active`対して少なくと`owner`も`user access administrator`1 つの管理者ロールの割り当て (または) を持っている必要があります。

|アクセス許可の種類      | アクセス許可              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess AzureResources  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | PrivilegedAccess AzureResources |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | Bearer {code}|
| Content-type  | application/json|


## <a name="request-body"></a>要求本文
要求本文で、更新する必要がある[governanceRuleSettings](../resources/governancerulesetting.md)の値を指定します。 

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)コレクション|管理者が対象となる役割の割り当てを追加しようとしたときに評価されるルールの設定。|
|adminmembersettings|[governanceRuleSetting](../resources/governancerulesetting.md)コレクション|管理者が直接メンバーの役割の割り当てを追加しようとしたときに評価されるルールの設定。|
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)コレクション|ユーザーが対象となる役割の割り当てを追加しようとしたときに評価されるルールの設定。 これは、現在の`pimforazurerbac`シナリオではサポートされておらず、今後のシナリオで利用できる場合があります。|
|usermembersettings|[governanceRuleSetting](../resources/governancerulesetting.md)コレクション|ユーザーが役割の割り当てをアクティブ化しようとしたときに評価されるルールの設定。|

## <a name="response"></a>応答
成功した場合、このメソッドは `204 NoContent` 応答コードを返します。応答本文には何も返されません。 

### <a name="error-codes"></a>エラー コード
この API は、標準の HTTP エラーコードを返します。 さらに、次のカスタムエラーコードが返されます。

|エラー コード     | エラー メッセージ         | 詳細             |
|:--------------| :---------------------|:--------------------|
| 400 badrequest| RoleSettingNotFound   | [governanceRoleSetting](../resources/governancerolesetting.md)は、システムに存在しません。
| 400 badrequest| invalidrolesetting    | 要求本文で指定された[governanceRuleSettings](../resources/governancerulesetting.md)値が無効です。

## <a name="example"></a>例 
この例では、サブスクリプションの Wingtip Toys-製品のカスタムロール3のロール設定を更新します。
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
  "adminEligibleSettings":[{"ruleIdentifier":"ExpirationRule","setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"}]
}
```
##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

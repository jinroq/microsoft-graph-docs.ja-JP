---
title: GovernanceRoleSetting を更新します。
description: GovernanceRoleSetting のプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: e76d7955576d9d514a70b52b31f4d034362aac1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874908"
---
# <a name="update-governancerolesetting"></a>GovernanceRoleSetting を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[GovernanceRoleSetting](../resources/governancerolesetting.md)のプロパティを更新します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

>**注:** この API では、依頼者の少なくとも 1 つある必要があります`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。

|アクセス許可の種類      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess.ReadWrite.AzureResources  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | PrivilegedAccess.ReadWrite.AzureResources |

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
要求の本体を更新する必要がある[governanceRuleSettings](../resources/governancerulesetting.md)の値を指定します。 

| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|管理者対象のロール割り当てを追加しようとするときに評価されるルールの設定。|
|adminMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|直接的なメンバーの役割の割り当てを追加する際に管理者に評価されるルールの設定。|
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|ユーザーが対象のロール割り当てを追加するときに評価されるルールの設定。 サポートされていない`pimforazurerbac`ここでは、シナリオと、将来のシナリオで使用可能な場合があります。|
|userMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|ユーザーが彼の役割の割り当てを有効にしようとした場合に評価されるルールの設定。|

## <a name="response"></a>応答
成功した場合、このメソッドは `204 NoContent` 応答コードを返します。応答本文には何も返されません。 

### <a name="error-codes"></a>エラー コード
この API では、標準の HTTP エラー コードを返します。 さらに、次のカスタム エラー コードを返します。

|エラー コード     | エラー メッセージ         | 詳細             |
|:--------------| :---------------------|:--------------------|
| 400 BadRequest| RoleSettingNotFound   | [GovernanceRoleSetting](../resources/governancerolesetting.md)は、システムに存在しません。
| 400 BadRequest| InvalidRoleSetting    | 要求の本文に記載されている[governanceRuleSettings](../resources/governancerulesetting.md)の値が有効ではありません。

## <a name="example"></a>例 
この例では、サブスクリプション Wingtip toys 社の商品にカスタム ロール 3 のロール設定を更新します。
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
<!-- {
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

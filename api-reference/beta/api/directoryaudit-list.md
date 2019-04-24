---
title: directoryAudits を一覧表示する
description: Azure Active Directory によって生成された監査ログの一覧を示します。 ユーザー、アプリ、デバイス、グループの管理、特権 ID 管理、アクセス レビュー、使用条件、ID 保護、パスワードの管理 (SSPR および管理者パスワードのリセット)、セルフサービス グループ管理など、Azure Active Directory 内のさまざまなサービスによって生成された監査ログが含まれています。
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: df6a737696c855cd60e396c6571169f8c46b3952
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455108"
---
# <a name="list-directoryaudits"></a>directoryAudits を一覧表示する

Azure Active Directory によって生成された監査ログの一覧を示します。 ユーザー、アプリ、デバイス、グループの管理、特権 ID 管理、アクセス レビュー、使用条件、ID 保護、パスワードの管理 (SSPR および管理者パスワードのリセット)、セルフサービス グループ管理など、Azure Active Directory 内のさまざまなサービスによって生成された監査ログが含まれています。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | AuditLog.Read.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません   |
|アプリケーション | AuditLog.Read.All | 

また、アプリは Azure AD に[正しく登録されている](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)必要があります。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための以下の OData クエリ パラメーターをサポートします。 [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)でこれらのパラメーターを使用する方法について確認してください。

|名前     |説明                            |例|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](/graph/query-parameters#filter-parameter)|結果 (行) をフィルターします。 |/`auditLogs/directoryAudits?&$filter=createdDateTime le 2018-01-24`
|[$top](/graph/query-parameters#top-parameter)|結果のページ サイズを設定します。|`/auditLogs/directoryAudits?$top=1`|
|[$skiptoken](/graph/query-parameters#skiptoken-parameter)|複数ページにわたる結果セットから、結果の次のページを取得します。|`auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a>$Filter パラメーターにサポートされる属性の一覧
|属性名 |サポートされる演算子|
|:----------------|:------|
|activityDisplayName| eq、startswith|
|activityDateTime| eq、ge、le|
|loggedByService|eq|
|initiatedBy/user/id|eq|
|initiatedBy/user/displayName| eq|
|initiatedBy/user/userPrincipalName| eq、startswith|
|initiatedBy/app/appId| eq|
|initiatedBy/app/appDisplayName| eq|
|targetResources/any(t: t/id)| eq|
|targetResources/any(t:t/displayName)| eq、startswith|
## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。
## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryAudit](../resources/directoryaudit.md) オブジェクトのコレクションを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_directoryaudits"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits
```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 271
```
```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryAudits
  "value": [{
        "id": "id",
        "category": "UserManagement",
        "correlationId": "da159bfb-54fa-4092-8a38-6e1fa7870e30",
        "result": "success",
        "resultReason": "Successfully added member to group",
        "activityDisplayName": "Add member to group",
        "activityDateTime": "2018-01-09T21:20:02.7215374Z",
        "loggedByService": "Core Directory",
        "initiatedBy": {
            "user": {
                "id": "7283X9ae-1a37-4937-9aex-e35d964db09b",
                "displayName": "Jamie Doe",
                "userPrincipalName": "jdoe@wingtiptoysonline.com",
                "ipAddress": "127.0.0.1"
            },
            "app": null
        },
        "targetResources": [{
            "@odata.type": "#microsoft.graph.TargetResourceGroup",
            "id": "ef7x527d-6x92-42x4-8x6d-cfxfdfx57f95",
            "displayName": "Lynda.com",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync"
            }],
            "groupType": "unifiedGroups"
        }, {
            "@odata.type": "#microsoft.graph.targetResourceUser",
            "id": "1f0ex8f5-3x61-4x6b-9x50-d4xx572f2bb7",
            "displayName": null,
            "modifiedProperties": [],
            "userPrincipalName": "jdoe@contoso.com"
        }],
        "additionalDetails": [{
            "key": "Additional Detail Name",
            "value": "Additional Detail Value"
        }]
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryAudits",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

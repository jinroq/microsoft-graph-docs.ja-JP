---
title: Azure AD 同期 API の概要
description: ) を使用すると、削除、管理、およびクラウドでの id の作成、保守、および削除 (たとえば、サービスとしてのソフトウェア、または SaaS) アプリケーション (Dropbox、Salesforce、ServiceNow など) を自動化できます。 Microsoft Graph の同期 Api を使用して、次のようなプログラムによって id 同期を管理できます。
localization_priority: Normal
doc_type: conceptualPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 818f5060db1fe4f6c05f0473e438095877ead119
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007866"
---
# <a name="azure-ad-synchronization-api-overview"></a>Azure AD 同期 API の概要

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) id 同期 ("プロビジョニング" とも呼ばれます) により、(サービスとしてのソフトウェア、または SaaS) アプリケーションとしての、クラウドでの id の作成、保守、削除を自動化できます (Dropbox、Salesforce、ServiceNow、その他。 Microsoft Graph の同期 Api を使用して、次のようなプログラムによって id 同期を管理できます。

- 同期ジョブの作成、開始、停止
- ジョブの同期スキーマに変更を加える
- 現在の同期の状態を確認する 

Azure AD での同期の詳細については、以下を参照してください。

* [Azure Active Directory を使用した SaaS アプリケーションへのユーザープロビジョニングとプロビジョニング解除を自動化する](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [Azure portal でエンタープライズアプリのユーザーアカウントプロビジョニングを管理する](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

サンプルテナントまたは独自のテナントで、 [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API を試すこともできます。

## <a name="synchronization-job"></a>同期ジョブ

同期ジョブは、バックグラウンドで定期的に実行して同期を実行し、1つのディレクトリに加えられた変更をポーリングして、別のディレクトリにプッシュします。 同期ジョブは、テナント内のアプリケーションの特定のインスタンスに対して常に固有です。 同期ジョブの設定の一部として、ターゲットディレクトリのオブジェクトの読み取りおよび書き込みの承認を付与し、ジョブの同期スキーマをカスタマイズする必要があります。

詳細については、「[同期ジョブ](synchronization-synchronizationjob.md)」を参照してください。

## <a name="synchronization-schema"></a>同期スキーマ

同期スキーマは、どのオブジェクトが同期されるか、またどのように同期されるかを定義します。 同期スキーマには、特定の同期ジョブの設定情報の大部分が含まれています。 通常、[属性マッピング](synchronization-attributemapping.md)の一部をカスタマイズするか、特定の条件を満たすオブジェクトのみを同期する[スコープフィルター](synchronization-filter.md)を追加します。

同期スキーマには、次のコンポーネントが含まれています。

- ディレクトリ定義
- 同期ルール
- オブジェクトマッピング

詳細については、「[同期スキーマ](synchronization-synchronizationschema.md)」を参照してください。

## <a name="synchronization-template"></a>同期テンプレート

同期テンプレートは、特定のアプリケーションに事前に構成された同期設定を提供します。 これらの設定 (最も重要なのは[同期スキーマ](synchronization-synchronizationschema.md)) は、テンプレートに基づくすべての[同期ジョブ](synchronization-synchronizationjob.md)に対して既定で使用されます。 テンプレートは、アプリケーション開発者によって指定されます。

詳細については、「[同期テンプレート](synchronization-synchronizationtemplate.md)」を参照してください。

## <a name="working-with-the-synchronization-api"></a>同期 API を使用する

同期 API の処理では、主に同期[ジョブ](synchronization-synchronizationjob.md)と同期[スキーマ](synchronization-synchronizationschema.md)リソースにアクセスします。 同期[ジョブ](synchronization-synchronizationjob.md)リソースを見つけるには、同期ジョブが属するサービスプリンシパルオブジェクトの ID を知る必要があります。 次の例は、**同期ジョブ**と**同期スキーマ**リソースを操作する方法を示しています。

### <a name="authorization"></a>Authorization

Azure AD 同期 API は、認証に OAuth 2.0 を使用します。 API に対して要求を行う前に、アクセストークンを取得する必要があります。 詳細については、「 [Microsoft Graph を呼び出すためのアクセストークンの取得](https://developer.microsoft.com/graph/docs/concepts/auth_overview)」を参照してください。 同期リソースにアクセスするには、アプリケーションにディレクトリの ReadWrite というアクセス許可が必要です。 詳細については、「[ディレクトリのアクセス許可](/graph/permissions-reference#directory-permissions)」を参照してください。

### <a name="find-the-service-principal-object-by-display-name"></a>表示名でサービスプリンシパルオブジェクトを検索する

次の例は、表示名でサービスプリンシパルオブジェクトを検索する方法を示しています。

**要求** 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

**応答**

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
    {
        "id": "bc0dc311-87df-48ac-91b1-259bd2c3a31c",
        "appId": "f7808c5e-cb57-4e37-8094-406d302c0f8d",
        "displayName": "Salesforce"
    },
    {
        "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
        "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
        "displayName": "salesforce 3"
    }
    ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a>サービスプリンシパルオブジェクトをアプリ ID で検索する

次の例は、サービスプリンシパルオブジェクトをアプリ ID で検索する方法を示しています。

**タキ** 
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

**応答**
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
            "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
            "displayName": "salesforce 3"
        }
    ]
}
```

### <a name="list-existing-synchronization-jobs"></a>既存の同期ジョブを一覧表示する

次の例は、既存の同期ジョブを一覧表示する方法を示しています。

**要求**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

**応答**
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {
                "expiration": null,
                "interval": "PT20M",
                "state": "Active"
            },
            "status": {}
        }
    ]
}
```

### <a name="get-synchronization-job-status"></a>同期ジョブの状態を取得する
次の例は、同期ジョブの状態を取得する方法を示しています。

**要求**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

**応答**
<!-- { "blockType": "ignored" } -->
```http
    HTTP/1.1 200 OK
    {
        "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
        "templateId": "SfSandboxOutDelta",
        "schedule": {
            "expiration": null,
            "interval": "PT20M",
            "state": "Active"
        },
        "status": {}
    }
```

### <a name="get-synchronization-schema"></a>同期スキーマを取得する
次の例は、同期スキーマを取得する方法を示しています。

**要求**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

**応答**
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a>関連項目

* [ディレクトリ拡張属性を使用して同期を構成する](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [カスタムターゲット属性を使用して同期を構成する](../resources/synchronization-configure-with-custom-target-attributes.md)




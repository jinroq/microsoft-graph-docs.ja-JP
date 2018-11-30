---
title: Azure AD 同期 API の概要
description: )、作成を自動化することにより、保守、および id の削除クラウド (ソフトウェア、サービス、または saas のどちらとして) アプリケーションをドロップ ボックス、セールス、ServiceNow などです。 使用できます同期 Api Graph でプログラムを使用して、id の同期を管理するのになど。
ms.openlocfilehash: ff3acb00801c9b04b8257345b06100297e11710c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073126"
---
# <a name="azure-ad-synchronization-api-overview"></a>Azure AD 同期 API の概要

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

(「プロビジョニング」とも呼ばれます)、azure Active Directory (AD の Azure) id の同期を使用すると、作成、保守、およびクラウド (SaaS サービスとしてのソフトウェア) の id の削除を自動化するアプリケーションをドロップ ボックス セールス ServiceNow、など。 使用できます同期 Api Graph でプログラムを使用して、id の同期を管理するのになど。

- 作成、起動、および同期ジョブを停止します。
- ジョブの同期スキーマに変更を加える
- 現在の同期状態を確認します。 

Azure AD での同期の詳細についてを参照してください。

* [ユーザー プロビジョニングと Azure Active Directory を使用して、SaaS アプリケーションをプロビジョニング解除の自動化します。](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [Azure ポータル エンタープライズ アプリケーションのプロビジョニングのユーザー アカウントを管理します。](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

サンプルのテナントや、独自のテナントでの[グラフのエクスプ ローラー](https://developer.microsoft.com/graph/graph-explorer)の API を試みることができます。

## <a name="synchronization-job"></a>同期ジョブ

同期ジョブは、バック グラウンドで定期的に実行している、1 つのディレクトリと別のディレクトリにプッシュすることで変更をポーリングして同期を実行します。 同期ジョブは、テナントにアプリケーションの特定のインスタンスに固有では常にします。 同期ジョブの設定の一部として、ターゲット ディレクトリにオブジェクトを読み書きするための承認を与えると、ジョブの同期スキーマをカスタマイズする必要があります。

詳細については、[同期ジョブ](synchronization-synchronizationjob.md)を参照してください。

## <a name="synchronization-schema"></a>同期スキーマ

同期スキーマで定義されるオブジェクトの同期し、同期する方法です。 同期スキーマには、特定の同期ジョブのセットアップ情報のほとんどが含まれています。 通常、[属性マッピング](synchronization-attributemapping.md)の一部をカスタマイズまたはを特定の条件を満たすオブジェクトのみを同期する[スコープのフィルター](synchronization-filter.md)が追加されます。

同期スキーマには、次のコンポーネントが含まれています。

- ディレクトリの定義
- 同期ルール
- オブジェクトのマッピング

詳細については、[同期スキーマ](synchronization-synchronizationschema.md)を参照してください。

## <a name="synchronization-template"></a>同期テンプレート

同期テンプレートは、特定のアプリケーションの構成済みの同期設定を提供します。 (最も重要なは、[同期スキーマ](synchronization-synchronizationschema.md)) は、これらの設定は、テンプレートに基づくすべての[同期ジョブ](synchronization-synchronizationjob.md)の既定で使用されます。 テンプレートは、アプリケーション開発者によって指定されます。

詳細については、[同期のテンプレート](synchronization-synchronizationtemplate.md)を参照してください。

## <a name="working-with-the-synchronization-api"></a>同期 API を使用します。

同期を使用する API の主要部分は[synchronizationJob](synchronization-synchronizationjob.md)と[synchronizationSchema](synchronization-synchronizationschema.md)のリソースにアクセスします。 [SynchronizationJob](synchronization-synchronizationjob.md)リソースを検索するには、同期ジョブが属するサービスのプリンシパル オブジェクトの ID を確認する必要があります。 次の例では、 **synchronizationJob**と**synchronizationSchema**のリソースを操作する方法を示します。

### <a name="authorization"></a>Authorization

Azure AD 同期 API では、OAuth 2.0 を使用して、承認のため。 API へのすべての要求を行う前に、アクセス トークンを取得する必要があります。 詳細については、 [Microsoft Graph を呼び出すための Get アクセス トークン](https://developer.microsoft.com/graph/docs/concepts/auth_overview)を参照してください。 同期リソースにアクセスするには、アプリケーションには、Directory.ReadWrite.All のアクセス許可が必要があります。 詳細については、[ディレクトリのアクセス許可](/graph/permissions-reference#directory-permissions)を参照してください。

### <a name="find-the-service-principal-object-by-display-name"></a>サービスのプリンシパル オブジェクトを表示名で検索します。

次の例では、表示名でサービスのプリンシパル オブジェクトを検索する方法を示します。

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

### <a name="find-the-service-principal-object-by-app-id"></a>アプリケーション id サービスのプリンシパル オブジェクトを検索します。

次の使用例は、アプリケーション id サービスのプリンシパル オブジェクトを検索する方法を示しています。

**要求** 
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

### <a name="list-existing-synchronization-jobs"></a>既存の同期ジョブを一覧表示します。

次の使用例は、既存の同期ジョブを一覧表示する方法を示しています。

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

### <a name="get-synchronization-job-status"></a>同期ジョブのステータスを取得します。
次の例では、同期ジョブのステータスを取得する方法を示します。

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

### <a name="get-synchronization-schema"></a>同期スキーマを取得します
次の例では、同期スキーマを取得する方法を示します。

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

* [ディレクトリの拡張属性を使用して同期を構成します。](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [カスタム ターゲットの属性を使用して同期を構成します。](../resources/synchronization-configure-with-custom-target-attributes.md)




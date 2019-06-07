---
title: アプリケーションのアクセス許可を Exchange Online の特定のメールボックスにスコーピングする
description: アプリのアプリケーション アクセス許可を Exchange Online の特定のメールボックスにスコープ設定するには、アプリケーション アクセス ポリシーを作成する必要があります。
author: svpsiva
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42e08989f462def2d1956c7e6fee2ad635f23e5a
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2019
ms.locfileid: "34692767"
---
# <a name="scoping-application-permissions-to-specific-exchange-online-mailboxes"></a>アプリケーションのアクセス許可を Exchange Online の特定のメールボックスにスコーピングする 

一部のアプリは、ユーザーの代理としてではなく、独自の ID を使用して Microsoft Graph を呼び出します。 通常、これに該当するものは、サーバーで実行される、サインインしているユーザーが存在しないバックグラウンド サービスやデーモン アプリです。 こうしたアプリは、認証のために [OAuth 2.0 クライアント資格情報付与フロー](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)を使用し、アプリケーションのアクセス許可によって構成されています。これにより、そうしたアプリは Exchange Online の組織内のすべてのメールボックスにアクセスできるようになります。 たとえば、アプリケーションのアクセス許可 Mail.Read により、サインインしているユーザーなしで、すべてのメールボックスのメールをアプリで読み取れるようになります。 

管理者は、アプリのアクセスを特定のメールボックスのセットに制限するために、PowerShell コマンドレット **New-ApplicationAccessPolicy** を使用してアクセス制御を構成できます。 この記事では、アプリケーション アクセス ポリシーの基本的な構成手順について説明します。

この手順は Exchange Online のリソースに固有のものであり、その他の Microsoft Graph のワークロードには適用できません。 

## <a name="configure-applicationaccesspolicy"></a>アプリケーション アクセス ポリシーの構成

アプリケーション アクセス ポリシーを構成して、アプリケーションのアクセス許可のスコープを制限するには、次の操作を実行します。
1.  Exchange Online PowerShell に接続します。 詳細については、「[Exchange Online PowerShell への接続](https://docs.microsoft.com/ja-JP/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)」を参照してください。

2.  アプリのクライアント ID とメールが有効なセキュリティ グループを特定して、アプリのアクセス対象を制限します。

    - [Azure のアプリの登録ポータル](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)で、アプリのアプリケーション (クライアント) ID を特定します。
    - メールが有効な新しいセキュリティ グループを作成するか既存のグループを使用して、そのグループの電子メール アドレスを特定します。 

3.  アプリケーション アクセス ポリシーを作成します。 

    次のコマンドを実行します。ただし、引数の **AppId**、**PolicyScopeGroupId**、および **Description** は置き換えてください。
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  新しく作成したアプリケーション アクセス ポリシーをテストします。

    次のコマンドを実行します。ただし、引数の **AppId** および **Identity** は置き換えてください。
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    このコマンドの出力には、アプリが User1 のメールボックスにアクセスできるかどうかが示されます。

注: アプリケーション アクセス ポリシーの変更が Microsoft Graph REST API の呼び出しに反映されるまでに、最長で 30 分かかることがあります。

## <a name="supported-permissions-and-additional-resources"></a>サポートされるアクセス許可と追加のリソース
管理者は、ApplicationAccessPolicy コマンドレットを使用して、次のいずれかのアプリケーションのアクセス許可が付与されているアプリのメールボックス アクセスを制御できます。 
- Mail.Read
- Mail.ReadWrite
- Mail.Send
- MailboxSettings.Read  
- MailboxSettings.ReadWrite
- Calendars.Read
- Calendars.ReadWrite
- Contacts.Read
- Contacts.ReadWrite

アプリケーション アクセス ポリシーの構成の詳細については、[PowerShell コマンドレット リファレンスの New-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/exchange/organization/new-applicationaccesspolicy)の項目を参照してください。 

## <a name="handling-api-errors"></a>API エラーの処理
構成済みのアプリケーション アクセス ポリシーによって API 呼び出しのアクセスが拒否されると、次のエラーが発生することがあります。 
```json
{
    "error": {
        "code": "ErrorAccessDenied",
        "message": "Access to OData is disabled.",
        "innerError": {
            "request-id": "2f038156-cf40-403d-8e46-831fe42a8229",
            "date": "2019-05-24T10:16:21"
        }
    }
}
```
このエラーがアプリからの Microsoft Graph API 呼び出しで返された場合は、組織の Exchange Online 管理者と協力して、メールボックス リソースにアクセスするためのアクセス許可をアプリに付与してください。



## <a name="see-also"></a>関連項目

- [アクセス許可リファレンス](permissions-reference.md)
- [New-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/exchange/organization/new-applicationaccesspolicy)
- [Get-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/exchange/organization/get-applicationaccesspolicy)
- [Remove-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/exchange/organization/remove-applicationaccesspolicy)
- [Set-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/exchange/organization/set-applicationaccesspolicy)
- [Test-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/exchange/organization/test-applicationaccesspolicy)

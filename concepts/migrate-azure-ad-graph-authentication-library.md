---
title: アプリ認証ライブラリの変更を確認する
description: Azure Active Directory (Azure AD) API アプリから Microsoft Graph API にアプリを移行するために、認証ライブラリの使用を更新する方法について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 77604945064565f1387553b22a26a0fa871c998d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630266"
---
# <a name="review-app-authentication-library-changes"></a>アプリ認証ライブラリの変更を確認する

この記事は、「*手順 3:* アプリ[を移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の詳細を確認する」に含まれています。

ほとんどのアプリは、認証ライブラリを使用して、Microsoft Graph を呼び出すためのアクセストークンを要求して管理します。  Microsoft では、2つの認証ライブラリを提供しています。

- [Azure Active Directory 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)ADAL
- [Microsoft 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)MSAL

## <a name="updating-adal"></a>ADAL の更新

アプリで現在 ADAL を使用している場合は、2段階の移行アプローチを使用します。

1. アプリを更新して、Microsoft Graph のアクセストークンを取得します。 この手順では、引き続き ADAL を使用します。 リソース web API を表す URI を保持する**Resourceurl**を次のように更新します。

    `https://graph.windows.net`  

    宛先：  

    `https://graph.microsoft.com`

    この変更後、新しく取得したトークンのスコープは同じですが、アクセストークンの対象ユーザーは Microsoft Graph になりました。  

    **Resourceurl**および検証された機能を更新したら、暫定的な更新をリリースしてユーザーを runnning します。

1.  次に、MSAL を使用するようにアプリを移行する作業を開始します。これは、移動を使用するためにサポートされているライブラリです。

## <a name="migrating-to-msal"></a>MSAL への移行

MSAL は、追加の同意、豊富なシングルサインオンエクスペリエンス、個人の Microsoft アカウントのサポート、標準ベースのプロトコルの使用などを含む、ADAL に対して複数の利点を提供します。  

アプリを MSAL に切り替えるときには、次のようにいくつかの変更を行う必要があります。これには、トークン acquistion 要求の**範囲**パラメーターの設定などが含まれます。

``` csharp
var scopes = new string[] { "https://graph.microsoft.com/.default" };
```

上記の式では、アクセス許可スコープ要求が、Azure Portal のアプリケーション登録時に構成されたものに制限され、既存のユーザーがアプリに再び同意する必要がなくなります。

一般的なエラーに関するトラブルシューティングやヘルプを含む、プロセスに関する直接の広範なヘルプについては、「 [ADAL を MSAL に移行する](https://aka.ms/adal-net-to-msal-net)」を参照してください。

MSAL に移行した後は、追加のスコープを動的に要求することができます。ユーザーは、次回アプリを使用するときに、増分の同意を提供するように求められます。

## <a name="next-steps"></a>次のステップ

- Azure AD Graph と Microsoft Graph の間の[.net クライアントライブラリ](migrate-azure-ad-graph-client-libraries.md)の違いについて説明します。
- MSAL への移行に関する詳細なヘルプについては、「 [ADAL を MSAL に移行する](https://aka.ms/adal-net-to-msal-net)」を参照してください。
- [Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。
- [Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。

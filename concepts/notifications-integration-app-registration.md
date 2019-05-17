---
title: Microsoft Graph 通知のためのアプリの登録と API アクセス許可を管理する
description: Microsoft Graph 経由で送信される通知を受信するためには、最初に、Microsoft Azure portal でアプリケーションを登録する必要があります。
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: 93ee4d83afac73b7d7ae90abe8e2876ffe688b68
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063376"
---
# <a name="manage-app-registration-and-api-permission-for-microsoft-graph-notifications"></a>Microsoft Graph 通知のためのアプリの登録と API アクセス許可を管理する

Microsoft Graph 通知と統合するアプリケーション サービスのためには、Microsoft アカウントあるいは職場や学校のアカウントをサポートする Microsoft ID プラットフォームでアプリを登録する必要があり、必要な API アクセス許可を宣言する必要があります。

## <a name="register-your-app-to-support-microsoft-accounts-or-work-or-school-accounts"></a>Microsoft アカウントあるいは職場や学校のアカウントをサポートするアプリを登録します。

[Microsoft Azure portal](https://portal.azure.com/#home) で、Microsoft アカウントあるいは職場や学校のアカウントをサポートするアプリを登録します。 [Microsoft アプリケーション ポータル](https://apps.dev.microsoft.com/)で、以前アプリケーションを登録したことがある場合、新機能と改善された機能の Azure portal エクスペリエンスに既存のアプリが表示されます。

アプリの登録の方法については、[Microsoft ID プラットフォームへのアプリケーションの登録](auth-register-app-v2.md)に関するページを参照してください。 


> [!NOTE]
> Microsoft アカウントを持っていないが使用したい場合には、 [Microsoft アカウント](https://account.microsoft.com/account) ページを参照してください。 職場または学校のアカウントで、認証と ID フレームワークとして Azure AD v1.0 使用する必要があるアプリを作成する場合は、 [Azure Active Directory 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)を参照してください。 新しく収束された Microsoft ID プラットフォーム (バージョン 2.0) について学んだり利用に関心がある場合は、 [Microsoft アイデンティティ プラットフォームのエンドポイントと Azure AD v1.0 エンドポイントを比較する](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/azure-ad-endpoint-comparison)を参照してください。

アプリを登録すると、アプリケーション ID/ クライアント ID がいろいろと便利になります。 [Microsoft パートナー センター](https://partner.microsoft.com/)でさまざまなデバイスの操作でのアプリケーションを登録するときに、この ID が後で必要になります。 

## <a name="app-certificates-and-secrets"></a>アプリ証明書とシークレット

アプリケーションを識別し、認証トークンを取得するときに認証を有効にするには、独自の証明書をアップロードしたり、Azure portal の**証明書とシークレット**に移動して新しいクライアント シークレットを作成することもできます。
    
![Azure portal 内のアプリ証明書とシークレットのスクリーン ショット](images/notifications-app-secrets.png)
    
> [!NOTE]
> 新しいクライアント シークレットの生成を選択する場合は、必ずをコピーして、安全な場所に保管してください。 ポータルから脱退したら、もう一度アクセスすることはできません。

## <a name="api-permissions"></a>API アクセス許可

Microsoft Graph の通知を使用するために追加の許可を追加する必要があります。 [**アクセス許可を追加**]を選択し、Microsoft Api で [**Microsoft Graph**]を選択してから、[**アクセス許可を委任**] を選択します。
    
![Azure portal の API アクセス許可の要求ページのスクリーンショット](images/notifications-api-permissions.png)
    
以下のアクセス許可を追加します。

  - User.Read - ユーザーにサインインするアプリケーションを許可する

  - Device.Read - デバイスのユーザーの一覧の ID を許可する

  - Device.Command - ユーザーのデバイスとの通信を許可する

  - UserActivity.ReadWrite.CreatedByApp - 通知を取得するためのアプリのサブスクリプションを許可する

  - Notifications.ReadWrite.CreatedByApp - アクセスと配信の通知を許可する

  - wns.connect - windows の通知サービスへの接続を許可する

  ![Azure portal で通知を行うのための代理アクセス権を示すスクリーン ショット](images/notifications-api-permissions-list.png)

## <a name="next-steps"></a>次の手順


  [アクセス許可と同意](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/v2-permissions-and-consent)に関する詳細を確認する、または「Microsoft Graph [アクセス許可のリファレンス](https://docs.microsoft.com/ja-JP/graph/permissions-reference)」を参照します。

これで、アプリの登録が完了しました。デバイス間の操作性のためのアプリケーションをセットアップし、Microsoft Graph 経由で送信される通知を行うためと、対応するアプリ プラットフォームを対象にするために[パートナー センター](https://partner.microsoft.com/)に移動します。 詳細については、[クロスデバイス エクスペリエンスに参加する](notifications-integration-cross-device-experiences-onboarding.md)を参照してください。 

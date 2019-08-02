---
title: Microsoft Graph での Azure Active Directory リソースの使用
description: Azure Active Directory (Azure AD) 用の Microsoft Graph には、組織、リソース、アセットの管理に役立つ REST API が備わっています。
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 83c9f8b9c1d95139ed2b170dd3df4964add15b1b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013165"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Microsoft Graph での Azure Active Directory リソースの使用

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph を使用すると、[Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis) リソースにアクセスして、管理者 (ディレクトリ) ロールの管理や外部ユーザーの組織への招待、[クラウド ソリューション プロバイダー (CSP)](https://partner.microsoft.com/cloud-solution-provider) の場合は顧客のデータの管理などのシナリオを有効にできます。 Microsoft Graph には、たとえばグループやロールにおけるユーザーの推移的なメンバーシップに関する情報を検出するメソッドなど、アプリで使用できるメソッドも用意されています。 

> **注**: Azure AD リソースの一部については、API リファレンスの他のセクションに記載されています。 詳細については、「[ユーザー](users.md)」と「[グループ](group.md)」を参照してください。


## <a name="authorization"></a>承認
 
Azure AD リソースに Microsoft Graph API を呼び出すには、アプリに適切なアクセス許可が必要です。 Azure AD リソース上で公開されている API の多くには、[_ディレクトリ_ アクセス許可](/graph/permissions-reference#directory-permissions)が必要です。 ディレクトリ アクセス許可は高い権限が与えられており、常に管理者の同意を必要とします。 

アプリがユーザーを代行している場合 (委任されたアクセス許可)、Azure AD API のうちの多くを正常に呼び出すには、ユーザーがそのアプリの適切な[管理者ロール](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles) メンバーである必要があります。

アクセス許可 (委任されたアクセス許可とアプリケーションのアクセス許可を含む) の詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。 

## <a name="common-use-cases"></a>一般的なユース ケース 

次の表に、Azure AD リソースの一般的なユース ケースを示します。

| **ユース ケース**        | **REST リソース** | **関連項目** |
|:-----------------|:--------|:----------|
| **ディレクトリ オブジェクトおよびメソッド** | | |
| `directoryObject` は、ユーザーやグループなどの多数のディレクトリ リソースの継承元となる基底クラスです。 Microsoft Graph では、ユーザーやグループなどのディレクトリ オブジェクトに関する情報の検出に使用できる複数のメソッドを公開しています。 たとえば、グループのリストに推移的なメンバーシップが含まれていないか確認すること、ディレクトリ オブジェクトが推移的なメンバーとなっているすべての所属先グループとディレクトリ ロールを返すこと、汎用リソース ID のリストから指定された種類のリソース (ユーザーまたはグループなど) をすべて返すことができます。 | [directoryObject](../resources/directoryobject.md) | 該当なし |
| **ディレクトリ (管理者) ロール、管理単位、ディレクトリ設定、ポリシーの管理** | | |
| Azure AD テナント内のディレクトリ ロールをアクティブにし、ディレクトリ ロール内のユーザー メンバーシップを管理します。 ディレクトリ ロールは、管理者ロールとも呼ばれます。 | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) |[Azure Active Directory での管理者ロールの割り当て](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)|
| 管理単位を管理します。 ディレクトリ ロールは、メンバーにテナント全体の権限を委任します。 管理者は、管理単位を作成および管理して、詳細に範囲を指定した管理権限をユーザーに委任できます。 | [administrativeUnit](../resources/administrativeunit.md) | [Azure AD の管理単位の管理](https://docs.microsoft.com/azure/active-directory/active-directory-administrative-units-management) |
| テナント全体または個々のリソースのインスタンスに、定義済みのディレクトリ設定を適用します。 現在サポートされているのは、Office 365 グループの設定のみです。 ディレクトリ設定は、グループ表示名でブロックする単語の一覧や、ゲスト ユーザーがグループの所有者になることを許可するか、といった動作を制御します。 | [directorySetting](../resources/directorysetting.md) <br/>[directorySettingTemplate](../resources/directorysettingtemplate.md)| [グループ設定を構成するための Azure Active Directory コマンドレット](https://docs.microsoft.com/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| Azure AD ポリシーを、アプリケーション、サービス プリンシパル、グループ、または組織全体に適用します。 現在サポートされているのは、トークンの有効期間およびホーム領域検出に関するポリシーです。  | [ポリシー](../resources/policy.md) | 該当なし |
| **Azure AD に対する特権アクセスをセキュリティで保護する** | | |
| Privileged Identity Management (PIM) を使用して管理者および IT プロフェッショナルのディレクトリと Azure リソースに対する期限付きの特権アクセスを管理および監視します。 | [Privileged Identity Management API](../resources/privilegedidentitymanagement-root.md) | [Azure AD Privileged Identity Management とは](https://docs.microsoft.com/azure/active-directory/active-directory-privileged-identity-management-configure)|
| マルウェアに感染したデバイスまたは未知の場所からのユーザーのサインインなど、ID リスク イベントを監視します。 | [Identity Protection Service API](../resources/identityprotection-root.md) | [Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/active-directory-identityprotection)<br/><br/>
  [Azure Active Directory リスク イベント](https://docs.microsoft.com/ja-JP/azure/active-directory/active-directory-reporting-risk-events) |
| **デバイスの管理** | | |
| 組織に登録されているデバイスを管理します。 デバイスはユーザーに登録されており、ノート PC、デスクトップ、タブレット、携帯電話などのアイテムを含みます。 デバイスは通常、Device Registration Service を使用するか、Microsoft Intune によって、クラウドで作成されます。 これは、多要素認証の条件付きアクセス ポリシーで使用されます。 | [デバイス](../resources/device.md) | [Azure Active Directory デバイス登録の使用](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview)<br/><br/>[InTune とは](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[Intune における管理用にデバイスを登録する](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **アプリの管理** | | |
| 開発テナントのアプリ構成を管理します。 | [アプリケーション](../resources/application.md) | [Azure Active Directory のアプリケーション オブジェクトとサービス プリンシパル オブジェクト](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| テナントにインストールされているアプリを管理します。 | [servicePrinicpal](../resources/serviceprincipal.md) | [Azure Active Directory のアプリケーション オブジェクトとサービス プリンシパル オブジェクト](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| テナントにインストールされているアプリにおける、ユーザーと管理者が同意したアクセス許可を管理します。 | [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) | 該当なし |
| テナントにインストールされている、ユーザー、グループ、サービス プリンシパル ロールのメンバーシップを管理します。 | [appRoleAssignment](../resources/approleassignment.md) | 該当なし |
| **パートナー テナント管理** | | |
| 顧客テナントとのパートナーシップに関する情報を取得します。 <br/><br/>**注:** これはパートナー テナントにのみ適用されます。 パートナー テナントとは、[Microsoft クラウド ソリューション プロバイダー](https://partnercenter.microsoft.com/partner/programs)、Office 365 Syndication、Microsoft Advisor パートナー プログラムのいずれかに含まれている、Microsoft パートナーに所属する Azure AD テナントです。| [コントラクト](../resources/contract.md) | [クラウド ソリューション プロバイダーのアプリケーションからの Microsoft Graph の呼び出し](/graph/auth-cloudsolutionprovider) |
| テナントに関連付けられているドメインを管理します。 ドメイン操作によって Office 365 などのサービスのドメインの関連付けを自動化するレジストラーを有効にします。 | [domain](../resources/domain.md) | [Azure Active Directory へのカスタム ドメイン名の追加](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal) |
| **テナント管理** | | |
| 会社住所、技術部連絡先、通知連絡先、サブスクライブ先のサービス プラン、関連付けられているドメインなど、組織に関する情報を取得します。 | [organization](../resources/organization.md) | N/A |
| 会社のサブスクライブ先のサービス SKU に関する情報を取得します。 | [subscribedSku](../resources/subscribedsku.md) | N/A |
| 組織に外部 (ゲスト) ユーザーを招待します。 | [invitation](../resources/invitation.md) | [Azure AD B2B コラボレーションとは](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)|
| **アクセス レビュー** | | |
| グループのメンバーシップとアプリケーションのアクセス権がアクセス レビューで適切であることを確認します。 | [アクセス レビュー API](../resources/accessreviews-root.md) |
  [Azure AD アクセス レビュー](https://docs.microsoft.com/ja-JP/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) |
## <a name="next-steps"></a>次のステップ
ディレクトリ リソースと API によって、ユーザーとの連携や、ユーザーの Microsoft Graph のエクスペリエンスを管理する新しい方法が見つかります。 詳細情報 

- 特定のシナリオに役立つ、メソッドとリソースのプロパティを詳しく調べます。
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。

さらに情報が必要な場合「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。


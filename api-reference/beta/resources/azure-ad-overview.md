---
title: Microsoft Graph での Azure Active Directory リソースの使用
description: Azure Active Directory (AD の Azure) のグラフは、組織、リソース、および資産を管理するための REST Api を提供します。
ms.openlocfilehash: 85f44df36057220e4ea26eb8d9342e9fd1df5bb6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305384"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Microsoft Graph での Azure Active Directory リソースの使用

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Microsoft Graph を使用してリソースにアクセスできます[Azure Active Directory (AD の Azure)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis) (ディレクトリ) の管理者の役割を管理するようなシナリオを有効にするのには、組織の外部ユーザーを招待し、[クラウド ・ ソリューション ・ プロバイダー (CSP)](https://partner.microsoft.com/cloud-solution-provider)を使用する場合お客様のデータを管理します。 Graph では、メソッドのアプリケーション使用できます、たとえば、ユーザーの推移的なグループおよびロール メンバーシップに関する情報を検索も用意されています。 

> **注**:Azure AD リソースの一部については、API リファレンスの他のセクションに記載されています。詳細については、「[ユーザー](users.md)」と「[グループ](group.md)」を参照してください。


## <a name="authorization"></a>Authorization
 
Azure AD リソースに Microsoft Graph API を呼び出すには、アプリに適切なアクセス許可が必要です。Azure AD リソース上で公開されている API の多くには、[_ディレクトリ_ アクセス許可](/graph/permissions-reference#directory-permissions)が必要です。ディレクトリ アクセス許可は高い権限が与えられており、常に管理者の同意を必要とします。 

アプリがユーザーを代行している場合 (委任されたアクセス許可)、Azure AD API のうちの多くを正常に呼び出すには、ユーザーがそのアプリの適切な[管理者ロール](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles) メンバーである必要があります。

アクセス許可 (委任されたアクセス許可とアプリケーションのアクセス許可を含む) の詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。 

## <a name="common-use-cases"></a>一般的なユース ケース 

次の表に、Azure AD リソースの一般的なユース ケースを示します。

| **ユース ケース**        | **REST リソース** | **関連項目** |
|:-----------------|:--------|:----------|
| **ディレクトリ オブジェクトおよびメソッド** | | |
| `directoryObject` は、ユーザーやグループなどの多数のディレクトリ リソースの継承元となる基底クラスです。Microsoft Graph では、ユーザーやグループなどのディレクトリ オブジェクトに関する情報の検出に使用できる複数のメソッドを公開しています。たとえば、グループのリストに推移的なメンバーシップが含まれていないか確認すること、ディレクトリ オブジェクトが推移的なメンバーとなっているすべての所属先グループとディレクトリ ロールを返すこと、汎用リソース ID のリストから指定された種類のリソース (ユーザーまたはグループなど) をすべて返すことができます。 | [directoryObject](../resources/directoryobject.md) | N/A |
| **ディレクトリ (管理者) の役割、管理単位、ディレクトリの設定、およびポリシーを管理します。** | | |
| Azure AD テナント内のディレクトリ ロールをアクティブにし、ディレクトリ ロール内のユーザー メンバーシップを管理します。ディレクトリ ロールは、管理者ロールとも呼ばれます。 | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) |[Azure Active Directory での管理者ロールの割り当て](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)|
| 管理単位を管理します。 ディレクトリの役割では、そのメンバーにテナントの権限を委任します。 管理者は、作成し、ユーザーに管理権限をより細かくスコープを委任する管理の単位を管理できます。 | [administrativeUnit](../resources/administrativeunit.md) | [Azure AD での管理単位の管理](https://docs.microsoft.com/azure/active-directory/active-directory-administrative-units-management) |
| テナント全体または個々 のリソースのインスタンスには、定義済みのディレクトリの設定を適用します。 現時点では、Office 365 のグループの設定のみがサポートされています。 ディレクトリの設定のコントロールの動作は、グループの所有者、およびその他のことをゲストが許可されているかどうかに阻止される単語のリストのグループの表示名をします。 | [directorySetting](../resources/directorysetting.md) <br/>[directorySettingTemplate](../resources/directorysettingtemplate.md)| [グループ設定を構成するための Azure Active Directory コマンドレット](https://docs.microsoft.com/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| Azure AD ポリシーは、アプリケーション、サービス ・ プリンシパル、グループ、または組織全体に適用されます。 現時点では、トークンの有効期間およびホーム領域の検出のポリシーはサポートされています。  | [ポリシー](../resources/policy.md) | N/A |
| **Azure AD にアクセス権限をセキュリティで保護されました。** | | |
| 管理し、管理者および IT プロフェッショナルに特権を持つユーザー情報管理 (PIM) の期限付きディレクトリと Azure のリソースへのアクセス権限を監視します。 | [特権 Id の管理 API](../resources/privilegedidentitymanagement-root.md) | [Azure AD 管理者の Id 管理とは何ですか。](https://docs.microsoft.com/azure/active-directory/active-directory-privileged-identity-management-configure)|
| アイデンティティ リスク イベントの監視などのユーザーがマルウェアに感染したデバイスまたは不明な場所からサインインします。 | [アイデンティティ保護サービス API](../resources/identityprotection-root.md) | [Azure Active Directory Id の保護](https://docs.microsoft.com/azure/active-directory/active-directory-identityprotection)<br/><br/>[Azure Active Directory のリスク イベント](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events) |
| **デバイスを管理する** | | |
| 組織に登録されているデバイスを管理します。デバイスはユーザーに登録されており、ノート PC、デスクトップ、タブレット、携帯電話などのアイテムを含みます。デバイスは通常、Device Registration Service を使用するか、Microsoft Intune によって、クラウドで作成されます。これは、多要素認証の条件付きアクセス ポリシーで使用されます。 | [device](../resources/device.md) | [Azure Active Directory のデバイスの登録の概要](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview)<br/><br/>[InTune とは](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[Intune における管理用にデバイスを登録する](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **アプリケーションの管理** | | |
| 開発者のテナントにアプリケーションの構成を管理します。 | [application](../resources/application.md) | [アプリケーションと Azure Active Directory 内のサービス プリンシパル オブジェクト](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| テナントにインストールされているアプリケーションを管理します。 | [servicePrinicpal](../resources/serviceprincipal.md) | [アプリケーションと Azure Active Directory 内のサービス プリンシパル オブジェクト](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| アクセス許可を管理するユーザーとテナントにインストールされているアプリケーションの管理者が同意しました。 | [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) | N/A |
| ユーザー、グループ、およびテナントにインストールされているアプリケーションのサービス プリンシパル ロールのメンバーシップを管理します。 | [appRoleAssignment](../resources/approleassignment.md) | N/A |
| **パートナー テナント管理** | | |
| 顧客テナントとのパートナーシップに関する情報を取得します。 <br/><br/>**注:** これはパートナー テナントにのみ適用されます。パートナー テナントとは、[Microsoft クラウド ソリューション プロバイダー](https://partnercenter.microsoft.com/partner/programs)、Office 365 Syndication、Microsoft Advisor パートナー プログラムのいずれかに含まれている、Microsoft パートナーに所属する Azure AD テナントです。| [contract](../resources/contract.md) | [クラウド ソリューション プロバイダーのアプリケーションからの Microsoft Graph の呼び出し](/graph/auth-cloudsolutionprovider) |
| テナントに関連付けられているドメインを管理します。ドメイン操作によって Office 365 などのサービスのドメインの関連付けを自動化するレジストラーを有効にします。 | [domain](../resources/domain.md) | [Azure Active Directory へのカスタム ドメイン名の追加](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal) |
| **テナント管理** | | |
| 会社住所、技術部連絡先、通知連絡先、サブスクライブ先のサービス プラン、関連付けられているドメインなど、組織に関する情報を取得します。 | [organization](../resources/organization.md) | N/A |
| 会社のサブスクライブ先のサービス SKU に関する情報を取得します。 | [subscribedSku](../resources/subscribedsku.md) | N/A |
| 組織に外部 (ゲスト) ユーザーを招待します。 | [invitation](../resources/invitation.md) | [Azure AD B2B コラボレーションとは](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)|
| **アクセス レビュー** | | |
| グループ メンバーシップと、アプリケーションのアクセス権限は、アクセスのレビューでは、正しいことを確認 | [アクセス API を確認します。](../resources/accessreviews-root.md) |[Azure AD アクセスを確認します。](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) |
## <a name="next-steps"></a>次の手順
ディレクトリ リソースと API によって、ユーザーとの連携や、ユーザーの Microsoft Graph のエクスペリエンスを管理する新しい方法が見つかります。詳細情報 

- 特定のシナリオに役立つ、メソッドとリソースのプロパティを詳しく調べます。
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。

さらに情報が必要な場合「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。


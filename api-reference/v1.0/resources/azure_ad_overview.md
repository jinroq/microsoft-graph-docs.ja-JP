# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Microsoft Graph での Azure Active Directory リソースの使用

Microsoft Graph を使用すると、[Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis) リソースにアクセスして、管理者 (ディレクトリ) ロールの管理や外部ユーザーの組織への招待、[クラウド ソリューション プロバイダー (CSP)](https://partner.microsoft.com/cloud-solution-provider) の場合は顧客のデータの管理などのシナリオを有効にできます。Microsoft Graph には、たとえばグループやロールにおけるユーザーの推移的なメンバーシップに関する情報を検出するメソッドなど、アプリで使用できるメソッドも用意されています。 

> **注**:Azure AD リソースの一部については、API リファレンスの他のセクションに記載されています。詳細については、「[ユーザー](users.md)」と「[グループ](group.md)」を参照してください。


## <a name="authorization"></a>Authorization
 
Azure AD リソースに Microsoft Graph API を呼び出すには、アプリに適切なアクセス許可が必要です。Azure AD リソース上で公開されている API の多くには、[_ディレクトリ_ アクセス許可](../../../concepts/permissions_reference.md#directory-permissions)が必要です。ディレクトリ アクセス許可は高い権限が与えられており、常に管理者の同意を必要とします。 

アプリがユーザーを代行している場合 (委任されたアクセス許可)、Azure AD API のうちの多くを正常に呼び出すには、ユーザーがそのアプリの適切な[管理者ロール](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles) メンバーである必要があります。

アクセス許可 (委任されたアクセス許可とアプリケーションのアクセス許可を含む) の詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。 

## <a name="common-use-cases"></a>一般的なユース ケース 

次の表に、Azure AD リソースの一般的なユース ケースを示します。

| **ユース ケース**        | **REST リソース** | **関連項目** |
|:---------------|:--------|:----------|
| **ディレクトリ オブジェクトおよびメソッド** | | |
| `directoryObject` は、ユーザーやグループなどの多数のディレクトリ リソースの継承元となる基底クラスです。Microsoft Graph では、ユーザーやグループなどのディレクトリ オブジェクトに関する情報の検出に使用できる複数のメソッドを公開しています。たとえば、グループのリストに推移的なメンバーシップが含まれていないか確認すること、ディレクトリ オブジェクトが推移的なメンバーとなっているすべての所属先グループとディレクトリ ロールを返すこと、汎用リソース ID のリストから指定された種類のリソース (ユーザーまたはグループなど) をすべて返すことができます。 | [directoryObject](../resources/directoryobject.md) | N/A |
| **ディレクトリ (管理者) ロールを管理する** | | |
| Azure AD テナント内のディレクトリ ロールをアクティブにし、ディレクトリ ロール内のユーザー メンバーシップを管理します。ディレクトリ ロールは、管理者ロールとも呼ばれます。 | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) | [Azure Active Directory での管理者ロールの割り当て](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles) |
| テナント全体または個々のリソースのインスタンスに、定義済みのグループ設定を適用します。グループ設定は、グループ表示名でブロックする単語の一覧や、ゲスト ユーザーがグループの所有者になることを許可するか、といった動作を制御します。 | [groupSetting](../resources/groupsetting.md) <br/>[groupSettingTemplate](../resources/groupsettingtemplate.md)| [グループ設定を構成するための Azure Active Directory コマンドレット](https://docs.microsoft.com/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| **デバイスを管理する** | | |
| 組織に登録されているデバイスを管理します。デバイスはユーザーに登録されており、ノート PC、デスクトップ、タブレット、携帯電話などのアイテムを含みます。デバイスは通常、Device Registration Service を使用するか、Microsoft Intune によって、クラウドで作成されます。これは、多要素認証の条件付きアクセス ポリシーで使用されます。 | [device](../resources/device.md) | [Azure Active Directory デバイス登録の使用](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview)。<br/><br/>[InTune とは](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[Intune における管理用にデバイスを登録する](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **パートナー テナント管理** | | |
| 顧客テナントとのパートナーシップに関する情報を取得します。<br/><br/>**注:**これはパートナー テナントにのみ適用されます。パートナー テナントとは、[Microsoft クラウド ソリューション プロバイダー](https://partnercenter.microsoft.com/partner/programs)、Office 365 Syndication、Microsoft Advisor パートナー プログラムのいずれかに含まれている、Microsoft パートナーに所属する Azure AD テナントです。 | [contract](../resources/contract.md) | [クラウド ソリューション プロバイダーのアプリケーションからの Microsoft Graph の呼び出し](../../../concepts/auth_cloudsolutionprovider.md) |
| テナントに関連付けられているドメインを管理します。ドメイン操作によって Office 365 などのサービスのドメインの関連付けを自動化するレジストラーを有効にします。 | [domain](../resources/domain.md) | [Azure Active Directory へのカスタム ドメイン名の追加](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal) |
| **テナント管理** | | |
| 会社住所、技術部連絡先、通知連絡先、サブスクライブ先のサービス プラン、関連付けられているドメインなど、組織に関する情報を取得します。 | [organization](../resources/organization.md) | N/A |
| 会社のサブスクライブ先のサービス SKU に関する情報を取得します。 | [subscribedSku](../resources/subscribedsku.md) | N/A |
| 組織に外部 (ゲスト) ユーザーを招待します。 | [invitation](../resources/invitation.md) | [Azure AD B2B コラボレーションとは](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b) |

## <a name="next-steps"></a>次の手順
ディレクトリ リソースと API によって、ユーザーとの連携や、ユーザーの Microsoft Graph のエクスペリエンスを管理する新しい方法が見つかります。詳細情報 

- 特定のシナリオに役立つ、メソッドとリソースのプロパティを詳しく調べます。
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。

さらに情報が必要な場合「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。



# <a name="shared-resources-in-microsoft-intune"></a>Microsoft Intune 内の共有リソース

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

これらのエンドポイントは、Intune ワークフローの複数の Microsoft Graph API で使用されます。  所与のリソースを使用する意図、目的、必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。  さらに、特定のワークフローに対してのみサポートされているメソッド、プロパティ、アクションもあります。

次の Graph リソースは、Intune ワークフロー間で共有されます。

- [すべてのデバイスの割り当て先](intune_shared_alldevicesassignmenttarget.md)
- [すべてのライセンス ユーザーの割り当て先](intune_shared_alllicensedusersassignmenttarget.md)
- [コンプライアンスの状況](intune_shared_compliancestatus.md)
- [デバイスおよびアプリ管理の割り当て先](intune_shared_deviceandappmanagementassignmenttarget.md)
- [デバイス アプリの管理](intune_shared_deviceappmanagement.md)
- [デバイス カテゴリ](intune_shared_devicecategory.md)
- [デバイス登録の種類](intune_shared_deviceenrollmenttype.md)
- [デバイスの管理](intune_shared_devicemanagement.md)
- [除外グループの割り当て先](intune_shared_exclusiongroupassignmenttarget.md)
- [グループの割り当て先](intune_shared_groupassignmenttarget.md)
- [目的をインストールします](intune_shared_installintent.md)
- [MIME コンテンツ](intune_shared_mimecontent.md)
- [UI 状態の生成オプションを保存しました](intune_shared_saveduistategenerationoptions.md)
- [URI](intune_shared_uri.md)
- [ユーザー](intune_shared_user.md)
- [VPP トークン アカウントの種類](intune_shared_vpptokenaccounttype.md)

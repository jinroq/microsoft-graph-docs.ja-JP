# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイスの Exchange のアクセス状態の理由です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|なし|0|Exchange から検出されたアクセス状態の理由なし|
|不明|1|不明なアクセス状態の理由|
|exchangeGlobalRule|2|Exchange のグローバル規則により確認されたアクセス状態|
|exchangeIndividualRule|3|Exchange の個別規則により確認されたアクセス状態|
|exchangeDeviceRule|4|Exchange デバイスの規則によって確認されたアクセス状態|
|exchangeUpgrade|5|Exchange のアップグレードによるアクセス状態|
|exchangeMailboxPolicy|6|Exchange メールボックス ポリシーにより確認されたアクセス状態|
|その他|7|Exchange によって確認されたアクセス状態|
|準拠|8|コンプライアンスの課題により付与されたアクセス状態|
|notCompliant|9|コンプライアンスの課題によって取り消されたアクセス状態|
|notEnrolled|10|管理の課題によって取り消されたアクセス状態|
|unknownLocation|12|不明の場所によるアクセス状態|
|mfaRequired|13|MFA の課題によるアクセス状態|
|azureADBlockDueToAccessPolicy|14|AAD アクセス ポリシーによって取り消されるアクセス状態|
|compromisedPassword|15|危険にさらされたパスワードによって取り消されたアクセス状態|
|deviceNotKnownWithManagedApp|16|マネージ アプリケーションの課題によって取り消されたアクセス状態|




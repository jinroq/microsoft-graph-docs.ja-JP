# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

マルウェアの脅威を検出するための Defender の既定のアクションです。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|更新の定義に基づいてアクションを適用します。|
|clean|1|検出された脅威をクリーンアップします。|
|quarantine|2|検出された脅威を隔離します。|
|remove|3|検出された脅威を削除します。|
|allow|4|検出された脅威を許可します。|
|UserDefined|5|検出された脅威に対して実行するアクションをユーザーが決定することを許可します。|
|block|6|検出された脅威をブロックします。|




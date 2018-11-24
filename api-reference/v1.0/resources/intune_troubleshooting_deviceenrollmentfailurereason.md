# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

登録の最上位レベルの障害のカテゴリ。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|既定値、失敗の理由は不明です。|
|認証|1|認証に失敗しました|
|承認|2|呼び出しが認証されると、ですが、登録する権限がありませんでした。|
|accountValidation|3|登録用のアカウントを検証できませんでした。 (アカウントがブロックされている登録が有効になっていません)|
|userValidation|4|ユーザーを検証できませんでした。 (ユーザーが存在しない場合は、不足しているライセンス)|
|deviceNotSupported|5|モバイル デバイスの管理には、デバイスはサポートされていません。|
|inMaintenance|6|アカウントがメンテナンスします。|
|badRequest|7|サービスで認識されるサポートではない要求をクライアントに送信されます。|
|featureNotSupported|8|このアカウントには、この登録で使用される機能はサポートされていません。|
|enrollmentRestrictionsEnforced|9|管理者によって構成されている登録の制限には、この登録がブロックされています。|
|clientDisconnected|10|クライアントがタイムアウトするか、登録は、エンド ・ ユーザーによって中止されました。|
|userAbandonment|11|登録は、エンド ・ ユーザーによって中断されました。 (エンド ・ ユーザーは、契約時の開始が、時間内に完了できませんでした)|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->

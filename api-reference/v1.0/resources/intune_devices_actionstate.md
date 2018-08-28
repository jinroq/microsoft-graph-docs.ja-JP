# <a name="actionstate-enum-type"></a>actionState 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス上の操作の状態
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|有効な動作状態ではありません。|
|pending|1|操作が保留中です。|
|canceled|2|操作がキャンセルされました。|
|"class="inGlossary">" 操作がキャンセルされました。|3|操作はアクティブではありません。|
|done|4|操作がエラーなく完了しました。|
|failed|5|操作が失敗しました。|
|notSupported|6|操作はサポートされていません。|




# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理するモバイル デバイスを追加するための方法です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|登録型の既定値は収集されませんでした。|
|userEnrollment|1|BYOD チャネルを通じてユーザー駆動の登録を行います。|
|deviceEnrollmentManager|2|デバイス登録の管理者アカウントでユーザーを登録します。|
|appleBulkWithUser|3|アップル一括登録はユーザーのチャレンジ (DEP、Apple Configurator)。|
|appleBulkWithoutUser|4|ユーザーの課題 (DEP では、Apple の構成ウィザードは、モバイルの設定) にアップル一括登録します。|
|windowsAzureADJoin|5|Windows 10 で Azure AD を参加させます。|
|windowsBulkUserless|6|証明書を使って ICD から Windows 10 の一括登録を行います。|
|windowsAutoEnrollment|7|Windows 10 自動登録です。 (勤務先のアカウントを追加)|
|windowsBulkAzureDomainJoin|8|Windows 10 で Azure AD を一括参加させます。|
|windowsCoManagement|9|Windows 10 共同管理が AutoPilot またはグループ ポリシーによって起動します。|




---
title: Microsoft Graph データ接続と Privileged Access Management の統合
description: Microsoft Graph データ接続は、Office 365 管理者がデータ移動の要求を承認できるようにするために、Privileged Access Management に依存しています。
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 439a5e50779888ff1ae7ccfb11311d8b3f6b8a14
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645269"
---
# <a name="microsoft-graph-data-connect-integration-with-privileged-access-management"></a>Microsoft Graph データ接続と Privileged Access Management の統合

Microsoft Graph データ接続は、Office 365 管理者がデータ移動の要求を承認できるようにするために、Privileged Access Management (PAM) に依存しています。 データ接続のパイプラインは有効化中に、Office 365 管理者から指定されたデータ アクセス要求の承認者のメンバーによって承認される必要があります。 承認者グループを設定するには、「[はじめに](data-connect-get-started.md)」を参照してください。

コピー アクティビティが Office 365 データを抽出するためのアクセスを要求したときに、承認要求メールが承認者グループの各メンバーに送信されます。 承認者は、これらの要求を承認または拒否したり、抽出されたデータから削除する必要があるユーザー グループを指定したりすることができます。また、以前に承認した要求を取り消すこともできます。 承認は 6 か月間有効となり、Azure Data Factory のパイプラインでのコピー アクティビティごとに 1 つの承認が必要となります。 

すべての要求には、データセットと、データの抽出先のユーザーに関する以下の詳細が常に含まれます。

* **要求者**: パイプラインを要求したユーザー。
* **期間**: 承認された場合の有効期間。 基本的に 4320 時間 (6 か月)。
* **理由**: 要求の理由。「組織用にインストールされたアプリに、Office 365 データへのアクセスの承認が必要」が通常の理由となります。
* **要求日時**: 要求の DateTime。
* **要求 ID**: 承認の目的で使用される要求の ID。
* **DataTable**: 抽出されるデータ セット (例: 送信済みアイテムなど)。
* **列**: データ テーブルから抽出される列のリスト (例: SentDateTime など)。
* **AllowedGroups**: パイプラインによるデータ抽出の対象となるユーザーのグループ。 グループのリストが空の場合、パイプラインはテナント内の全ユーザーのデータへのアクセスを要求します。
* **ユーザー スコープ クエリ**: ユーザーをフィルターで除外する場合に使用する述語。 要求がテナント内のすべてのユーザーに対するものである場合にのみ適用されます。 これが空の場合は、フィルターは適用されません。 
* **OutputUri**: 抽出されたデータが格納される出力パス。
* **SourceTenantId**: データの抽出元のテナント ID。
* **InstallerIdentity**: アプリのインストーラーの ID。

要求内の次のフィールドは、限られた場合にのみ使用可能となります。

* アプリケーション名と Marketplace URI (Azure Marketplace からインストールされたアプリケーションに対してのみ使用可能)。
* アプリケーションのプライバシー ポリシーとサービス利用規約へのリンク (アプリケーションから提供されている場合にのみ使用可能)。
* 出力の保管場所での保存データの暗号化など、アプリケーションが実施するコンプライアンス ポリシー (コンプライアンス ポリシーがアプリケーションから提供され、アプリケーションが Azure Marketplace からインストールされている場合にのみ使用可能)。
* 拒否リスト - 抽出されたデータから削除できるユーザー グループ。 このフィールドは、抽出されたデータのプライバシーに関するスクラブをサポートする要求の一環として、空となります。 要求を承認する承認者グループのメンバーが、承認の際にこのフィールドを設定できます。 

## <a name="approving-requests"></a>要求の承認

データ接続のパイプラインは、データ アクセス要求の承認者グループのメンバーによって承認される必要があります。 承認者は、Exchange Online PowerShell モジュールまたは PAM ユーザー エクスペリエンスを使用して、パイプラインの承認、拒否、あるいは取り消しを行うことができます。

### <a name="approving-denying-and-revoking-requests-by-using-powershell"></a>PowerShell を使用した要求の承認、拒否、取り消し

Exchange Online PowerShell モジュールを使用して要求を処理するには、次の手順を実行します。

1. Exchange Online PowerShell モジュールをインストールします。 インストール方法の詳細については、「[多要素認証を使用して Exchange Online PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps)」を参照してください。

2. 多要素認証 (MFA) を使用して Exchange Online PowerShell に接続します。 詳細については、「[多要素認証を使用して Exchange Online PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps)」を参照してください。
    >**注**: Exchange Online PowerShell への接続中でなくても、組織で多要素認証を有効にしてこれらの手順を実行することができます。 MFA と接続すると、要求への署名のために PAM によって使用される OAuth トークンが作成されます。

3. 自分のアカウントでサインインします。 要求の承認、拒否、または取り消しを行うには、構成済みのデータ アクセスの承認者グループのメンバーである必要があります。 ゲスト ユーザーは承認者グループであっても要求を承認することができません。 

   ```powershell
   Connect-EXOPSSession
   ```

4. 保留中の要求を確認します。
   >**注:** 要求を識別して承認または拒否するには、**ID** プロパティの値を使用します。 この値をメモして、-RequestId パラメーターで使用してください。 

   ```powershell
   Get-ElevatedAccessRequest | ?{$_.RequestStatus -eq 'Pending'}
   ```

4. 関心のある要求の**コンテキスト** フィールドの詳細を確認します。 
   >**注:** データ アクセスの要求のコンテキスト フィールドには、コピー アクティビティのパラメーターとプロパティが記述されます。

   ```powershell
   (Get-ElevatedAccessRequest -RequestId $requestId).Context | ConvertFrom-Json
   ```

   次のような応答を受け取ります。

   ```powershell
   Key                          Value
   ---                          -----
   ApplicationName
   ComplianceStatus             [{"Timestamp":"2018-05-02T18:29:21.5705664Z","RequirementName":"adlsEncryption","PolicyComplianceState":"Compliant","Violations":0},{"Timestamp":"2018-05-02T...
   ApplicationMarketPlaceUri
   OutputUri                    adl://myadlserumvrroyspmq.azuredatalakestore.net/targetFolder/Event
   ApplicationPrivacyPolicyUri  http://www.wkw.com/privacy
   ApplicationTermsOfServiceUri http://www.wkw.com/tos
   InstallerIdentity            a89885c3-4b0e-499e-86ed-14d7ed9147c2@942229f8-4656-4fb0-828b-e938dad4019a
   SourceTenantId               942229f8-4656-4fb0-828b-e938dad4019a
   UserScopeQuery               tenant in (942229f8-4656-4fb0-828b-e938dad4019a)
   ApplicationId
   DataTable                    Calendar Events
   DestinationTenantId          942229f8-4656-4fb0-828b-e938dad4019a
   Columns                      Subject:string, HasAttachments:bool, End:DateTime, Start:DateTime, ResponseStatus:string, Organizer:Object, Attendees:string, Importance:string, Sensitivity:...
   ```

5. -RequestId パラメーターに **ID** の値を使用して、要求の承認または拒否を行います。

   ```powershell
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!"
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

特定のユーザーからのデータが含まれないように、拒否リストを使用して要求を承認することもできます。 これを行うには、要求のコンテキストを変更して、除外するグループの `object Id` を追加してから要求を承認する必要があります。 

   ```powershell
   $request = Get-ElevatedAccessRequest -RequestId
   $hash = $request.Context
   $hash["DenyList"] = <Object ID of denied user group>;
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!" -RequestContext $hash
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```
以前に承認した要求を取り消すこともできます。 要求の承認と同様に、**ID** の値は -RequestId パラメーターに必要となります。 

   ```powershell 
   Revoke-ElevatedAccessAuthorization -Comment "Revoking this request!" -RequestId $requestId
   ```
   次のような応答を受信します。
   
   ```powershell
   AuthorizedBy          : user@tenant.onmicrosoft.com
   Type                  : Task
   AuthorizedAccess      : Data Access Request
   StartTimeUtc          : 7/24/2018 6:02:42 PM
   EndTimeUtc            : 10/22/2018 6:02:42 PM
   Revoked               : True
   RevocationDateTimeUtc : 7/24/2018 9:12:55 PM
   RevokedBy             : NAMPR00A001.prod.outlook.com/Microsoft Exchange Hosted  Organizations/tenant.onmicrosoft.com/user
   RevocationComment     : Revoking this request!
   Identity              : bda75607-0d87-43cb-bdf1-284b18446b34
   DateCreatedUtc        : 1/1/0001 12:00:00 AM
   DateUpdatedUtc        : 7/24/2018 9:12:55 PM
   ```

### <a name="approving-denying-and-revoking-requests-by-using-the-pam-user-experience"></a>PAM ユーザー エクスペリエンスを使用した要求の承認、拒否、取り消し

PAM Web エクスペリエンスを使用して要求を処理するには、次の手順を実行します。

1. 管理者の資格情報を使用して Office 365 管理ポータルにサインインし、[Privileged Access Management の承認ユーザー エクスペリエンス](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess)のページに移動します。 ページに移動すると、すべてのアクセス要求 (保留中/承認済み/期限切れ/拒否) が表示されます。

表示されたページで、関心のある要求を選択します。 プライバシーに関するスクラブの拒否リストを選択するには、**[DenyList]** ドロップダウンをクリックし、スクラブを行うグループを選択して、**[承認]** を選択します。

以前に承認した要求を取り消すには、取り消す必要がある承認済みの要求を選択し、**[取り消し]** を選択します。 この操作以降、取り消した承認でデータを移動することはできなくなります。 

### <a name="approval-behavior"></a>承認の動作

データ接続の承認要求をする際には、以下の点に注意することが重要です。

- 承認要求は Azure Data Factory、パイプライン、コピー アクティビティの名前に基づきます。 コピー アクティビティを実行するたびに、Office 365 管理者が Office データへのアクセスに関するコピー アクティビティの要求を承認したかどうかが確認されます。また、承認のパラメーターに対するコピー アクティビティの重要なパラメーターが実行されているかどうかの検証も行われます。
- 特定の条件においては、新しい承認要求が自動的にトリガーされます。 コピー アクティビティが Office 365 データにアクセスするには、データ接続の承認者が新しい要求を承認する必要があります。
- コピー アクティビティ実行のパラメーターが変更されると、新しい承認要求がトリガーされます。
- Data Factory、パイプライン、コピー アクティビティの名前のパラメーターが変更されると、新しい承認要求がトリガーされます。
- たとえば、コピー アクティビティがアクセスしているデータ テーブルまたは列のセットが変更された場合は、新しい承認が必要になります。
- コピー アクティビティは 6 か月に 1 回承認される必要があります。 元の承認が 6 か月前に承認された場合は、新しい承認要求が自動的にトリガーされます。
- Office 365 データへのアクセス承認者が承認要求を拒否したり、以前に承認した要求を取り消したりした場合、コピー アクティビティの実行ができなくなります。 承認者と協力して、拒否または取り消しの理由を確認し、必要に応じてコピー アクティビティのパラメーターを修正する必要があります。 新しい承認要求をトリガーするためには、新しいコピー アクティビティを展開するか、既存のコピー アクティビティの名前を変更する必要があります。
- Office 365 データへのアクセス承認者が要求を処理しない限り、承認要求は 24 時間で期限切れになります。 新しい承認要求は 24 時間ごとに 1 回送信されます。 コピー アクティビティが承認待ち (同意が保留中の段階) の場合は、Office 365 データへのアクセス承認者と協力して要求を承認する必要があります。

## <a name="privacy-scrubbing"></a>プライバシーに関するスクラブ 
要求を承認する承認者グループのメンバーは、抽出されたデータからデータを削除する 1 つのユーザー グループの名前を指定することができます。 拒否されたグループのメンバーのメール アドレスを含む行は、抽出されたデータから削除されます。 拒否されたグループ内に入れ子になっているグループは展開され、ユーザーだけが削除されます。PowerShell または PAM UX を使用して承認中に拒否リストを適用する方法の詳細については、このトピックの「要求の承認」セクションを参照してください。 

次の表は、データセットの名前と、プライバシーに関するスクラブ用にコンテンツの確認が行われる列を示しています。

| データセット名                     | 拒否リストに基づいたスクラブに使用される列                                                  |
|---------------------------------------------------------------------|----------------------------------------------------------|
| **BasicDataSet_v0.Message_v0**<br>**BasicDataSet_v0.Message_v1**   | Sender、From、ToRecipients、CcRecipients、BccRecipients    |                                                                               
| **BasicDataSet_v0.SentItem_v0**<br>**BasicDataSet_v0.SentItem_v1**  | Sender、From、ToRecipients、CcRecipients、BccRecipients  |
| **BasicDataSet_v0.Event_v0**<br>**BasicDataSet_v0.Event_v1**     | Organizer、Attendees                                        |
| **BasicDataSet_v0.Contact_v0**<br>**BasicDataSet_v0.Contact_v1**  | EmailAddresses                                            |
| **BasicDataSet_v0.CalendarView_v0**                                | Organizer、Attendees                                      |

## <a name="next-steps"></a>次の手順

「[はじめに](data-connect-get-started.md)」の手順をすべて実行して、Microsoft Graph データが使用できるように Privileged Access Management が組織内で正しく構成されていることを確認します。

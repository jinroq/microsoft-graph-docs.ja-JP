---
title: Create windows10GeneralConfiguration
description: 新しい windows10GeneralConfiguration オブジェクトを作成します。
ms.openlocfilehash: 4f725e95190995cdfa2a920cd2906ff7ff805319
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072389"
---
# <a name="create-windows10generalconfiguration"></a>Create windows10GeneralConfiguration

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

新しい [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) オブジェクトを作成します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementConfiguration.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求本文で、windows10GeneralConfiguration オブジェクトの JSON 表記を指定します。

次の表に、windows10GeneralConfiguration の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール値|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは値の取得のみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|windows10AppsForceUpdateSchedule|[windows10AppsForceUpdateSchedule](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|Windows 10 アプリの更新スケジュールを強制します。|
|enableAutomaticRedeployment|ブール値|すべてのユーザー データとデバイスに自動的に再を構成および管理を取得するために、デバイスのロック画面で ctrl キー + 勝利 + R を使用する設定を削除するのには管理者権限を持つユーザーを許可します。|
|assignedAccessSingleModeUserName|String|このポリシー設定は、アプリケーション キオスク モードの 1 つがロックアウトされているユーザー アカウントを定義することです。|
|assignedAccessSingleModeAppUserModelId|String|このポリシー設定は、1 つのアプリケーション キオスク モードに、アプリケーション ユーザー モデル ID (AUMID) がロックされることを定義します。|
|microsoftAccountSignInAssistantSettings|[signInAssistantOptions](../resources/intune-deviceconfig-signinassistantoptions.md)|Microsoft アカウントでサインイン アシスタント (wlidsvc) の NT サービスを制御します。 使用可能な値は、`notConfigured`、`disabled` です。|
|authenticationAllowSecondaryDevice|ブール値|Windows で動作する第 2 の認証デバイスを使用できます。|
|authenticationAllowFIDODevice|ブール値|デバイス (FIDO を使用して認証を許可するかどうかを示しますhttps://fidoalliance.org/)|
|cryptographyAllowFipsAlgorithmPolicy|ブール値|連邦情報処理規格 (FIPS) ポリシーを有効または無効にするかどうかを指定します。|
|displayAppListWithGdiDPIScalingTurnedOn|String コレクション|GDI DPI スケールをオンになっているレガシ アプリケーションの一覧です。|
|displayAppListWithGdiDPIScalingTurnedOff|String コレクション|GDI の DPI スケーリングを無効になっているレガシ アプリケーションの一覧です。|
|enterpriseCloudPrintDiscoveryEndPoint|String|クラウド プリンターを検出するエンドポイント。|
|enterpriseCloudPrintOAuthAuthority|String|OAuth トークンを取得するための認証エンドポイント。|
|enterpriseCloudPrintOAuthClientIdentifier|String|OAuth 認証機関から OAuth トークンを取得することを承認されているクライアント アプリケーションの GUID。|
|enterpriseCloudPrintResourceIdentifier|String|Azure Portal で構成されている印刷サービスの OAuth リソース URI。|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|検出エンドポイントからクエリを実行する必要があるプリンターの最大数。 これはモバイルのみでの設定です。 有効な値は 1 から 65535 までです|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|String|Azure Portal で構成されているプリンター検出サービスの OAuth リソース URI。|
|messagingBlockSync|ブール値|テキスト メッセージをブロックをバックアップおよび復元するかどうか、すべてのメッセージを示します。|
|messagingBlockMMS|ブール値|ブロックするかどうかを示します、MMS の送信/受信デバイスで機能します。|
|messagingBlockRichCommunicationServices|ブール値|ブロックするかどうかを示します、RCS は、デバイスの機能を送信/受信します。|
|printerNames|String コレクション|名前 (ホストのネットワーク名) に基づいてプリンターを自動的に準備します。|
|printerDefaultName|String|インストール済みのプリンターの名前 (ネットワーク ・ ホスト名) が。|
|printerBlockAddition|ブール値|プリンターの設定からの他のプリンターのインストールをユーザーを防止します。|
|searchBlockDiacritics|Boolean|検索で分音記号を使用できるかどうかを指定します。|
|searchDisableAutoLanguageDetection|Boolean|コンテンツとプロパティのインデックスを作成するときに、自動言語検出を使用するかどうかを指定します。|
|searchDisableIndexingEncryptedItems|Boolean|Cortana またはエクスプローラーの検索結果に表示されないようにするため、WIP で保護されているアイテムのインデックス作成を禁止するかどうかを示します。|
|searchEnableRemoteQueries|Boolean|このコンピューターのインデックスに対するリモート クエリをブロックするかどうかを示します。|
|searchDisableUseLocation|ブール値|場所情報検索を使用してかどうかを指定します。|
|searchDisableLocation|ブール値|場所情報検索を使用してかどうかを指定します。|
|searchDisableIndexerBackoff|Boolean|インデクサー バックオフの検索機能を無効にするかどうかを示します。|
|searchDisableIndexingRemovableDrive|Boolean|リムーバブル ドライブ上の場所をライブラリに追加してインデックスを作成することをユーザーに許可するかどうかを示します。|
|searchEnableAutomaticIndexSizeManangement|Boolean|インデックスの場所と同じドライブ上のハード ドライブ領域の最小値を指定して、その最小値を下回ったらインデックス作成を停止するかどうかを示します。|
|searchBlockWebResults|ブール値|Web 検索をブロックするかどうかを示します。|
|securityBlockAzureADJoinedDevicesAutoEncryption|ブール値|デバイスが Azure の AD が参加している (デスクトップのみ) の場合は、OOBE 中にデバイスの自動暗号化を許可するかどうかを指定します。|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|診断データと利用統計情報データ (Watson など) の送信をデバイスに許可する値を取得または設定します。 可能な値は、`userDefined`、`none`、`basic`、`enhanced`、`full` です。|
|oneDriveDisableFileSync|Boolean|アプリや機能から OneDrive 上のファイルを操作することを IT 管理者が禁止できるかどうかを示す値を取得または設定します。|
|systemTelemetryProxyServer|String|取得または完全修飾ドメイン名 (FQDN) または接続されているユーザーの経験および遠隔測定の要求を転送するようにプロキシ サーバーの IP アドレスを設定します。|
|inkWorkspaceAccess|[inkAccessSetting](../resources/intune-deviceconfig-inkaccesssetting.md)|デスクトップで、画面のロックの上から、インクのワークスペースにユーザー アクセスを制御します。 可能な値は、`notConfigured`、`enabled`、`disabled` です。|
|inkWorkspaceAccessState|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|デスクトップで、画面のロックの上から、インクのワークスペースにユーザー アクセスを制御します。 可能な値は、`notConfigured`、`blocked`、`allowed` です。|
|inkWorkspaceBlockSuggestedApps|ブール値|インクのワークスペースでアプリケーションの推奨される修正候補を表示するかどうかを指定します。|
|smartScreenEnableAppInstallControl|Boolean|ユーザーがストア以外の場所からアプリをインストールできるかどうかを IT 管理者が制御することを許可します。|
|personalizationDesktopImageUrl|String|ダウンロードしてデスクトップ画像として使用する必要がある jpg、jpeg、png 画像の http または https URL、あるいはデスクトップ画像として使用する必要があるファイル システム上のローカル画像のファイル URL。|
|personalizationLockScreenImageUrl|String|ダウンロードしてロック画面画像として使用する必要がある jpg、jpeg、png 画像の http または https URL、あるいはロック画面画像として使用する必要があるファイル システム上のローカル画像のファイル URL。|
|bluetoothAllowedServices|String コレクション|許可されている Bluetooth サービスおよびプロファイルの一覧を 16 進形式の文字列として指定します。|
|bluetoothBlockAdvertising|Boolean|ユーザーが Bluetooth 広告を使用することを禁止するかどうか。|
|bluetoothBlockDiscoverableMode|Boolean|ユーザーが Bluetooth の発見可能モードを使用することを禁止するかどうか。|
|bluetoothBlockPrePairing|Boolean|バンドルされた特定のいくつかの Bluetooth 周辺機器を自動的にホスト デバイスとペアにすることを禁止するかどうか。|
|edgeBlockAutofill|Boolean|自動入力を禁止するかどうかを示します。|
|edgeBlocked|Boolean|ユーザーが Edge ブラウザーを使用することを禁止するかどうかを示します。|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune-deviceconfig-edgecookiepolicy.md)|Edge ブラウザーでどの Cookie を禁止するかを示します。 可能な値は、`userDefined`、`allow`、`blockThirdParty`、`blockAll` です。|
|edgeBlockDeveloperTools|Boolean|Edge ブラウザー内の開発者ツールを禁止するかどうかを示します。|
|edgeBlockSendingDoNotTrackHeader|Boolean|ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。|
|edgeBlockExtensions|Boolean|Edge ブラウザーの拡張機能を禁止するかどうかを示します。|
|edgeBlockInPrivateBrowsing|Boolean|Edge ブラウザーで会社のネットワークの InPrivate ブラウズを禁止するかどうかを示します。|
|edgeBlockJavaScript|Boolean|ユーザーが JavaScript を使用することを禁止するかどうかを示します。|
|edgeBlockPasswordManager|Boolean|パスワード マネージャーを禁止するかどうかを示します。|
|edgeBlockAddressBarDropdown|Boolean|Microsoft Edge のアドレス バー ドロップダウン機能を禁止します。 Microsoft Edge から Microsoft サービスへのネットワーク接続を最小限に抑えるには、この設定を無効にします。|
|edgeBlockCompatibilityList|Boolean|Microsoft Edge での Microsoft 互換性リストを禁止します。 Microsoft ではこのリストを利用して、既知の互換性の問題があるサイトを Edge で正しく表示できるようにします。|
|edgeClearBrowsingDataOnExit|Boolean|Microsoft Edge の終了時にブラウズ データを消去します。|
|edgeAllowStartPagesModification|Boolean|Edge のスタート ページをユーザーが変更することを許可します。 ユーザーが Edge を開いたときに既定で表示されるスタート ページを指定するには、EdgeHomepageUrls を使用します。|
|edgeDisableFirstRunPage|Boolean|Microsoft Edge の初回使用時に表示される Microsoft の Web ページを禁止します。 このポリシーでは、ゼロ エミッション構成に登録している企業などが、このページの表示を禁止できます。|
|edgeBlockLiveTileDataCollection|Boolean|ユーザーが Microsoft Edge からスタートにサイトをピン留めしたときに、ライブ タイルを作成するために Microsoft が情報を収集することを禁止します。|
|edgeSyncFavoritesWithInternetExplorer|Boolean|Internet Explorer と Microsoft Edge の間でお気に入りの同期を有効にします。 お気に入りの追加、削除、変更、順序変更が、ブラウザー間で共有されます。|
|edgeFavoritesListLocation|String|お気に入りの一覧を提供する場所です。 ローカル ファイル、ローカル ネットワーク、http の場所が該当します。|
|edgeBlockEditFavorites|ブール値|[お気に入り] に変更を加えてからユーザーをブロックするかどうかを示します。|
|cellularBlockDataWhenRoaming|Boolean|ローミング中に携帯電話上でユーザーがデータを使用することを禁止するかどうか。|
|cellularBlockVpn|Boolean|携帯電話上でユーザーが VPN を使用することを禁止するかどうか。|
|cellularBlockVpnWhenRoaming|Boolean|ローミング時に携帯電話上でユーザーが VPN を使用することを禁止するかどうか。|
|cellularData|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|デバイスの携帯電話のデータ チャネルを許可するかどうかを指定します。 できない場合は、構成、携帯電話のデータ チャネルを許可し、ユーザーがオフにできます。 可能な値は、`blocked`、`required`、`allowed` です。|
|defenderBlockEndUserAccess|Boolean|エンド ユーザーが Defender にアクセスすることを禁止するかどうか。|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|検疫済みのマルウェアを削除するまでの日数。 有効な値は 0 から 90 までです|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|検出されたマルウェアに対する Defender のアクションを脅威レベルごとに取得または設定します。|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune-deviceconfig-weeklyschedule.md)|Defender がシステムをスキャンする曜日。 可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。|
|defenderFilesAndFoldersToExclude|String コレクション|スキャンとリアルタイム保護から除外するファイルとフォルダー。|
|defenderFileExtensionsToExclude|String コレクション|スキャンとリアルタイム保護から除外するファイル拡張子。|
|defenderScanMaxCpu|Int32|スキャン中の最大 CPU 使用率。 有効な値は 0 から 100 までです|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|ファイル アクティビティを監視する値。 可能な値は、`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly` です。|
|defenderPotentiallyUnwantedAppAction|[defenderPotentiallyUnwantedAppAction](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|取得または設定の Defender の動作の可能性のある不要なアプリケーション (PUA)、広告挿入、支払やサブスクリプションなどのソフトウェアのバンドル化、永続的な要請のビヘイビアーを使用してソフトウェアが含まれています。Defender 警告ユーザーと私用のダウンロード自体をインストールしようとしています。 デスクトップの Windows 10 に追加されます。 可能な値は、`deviceDefault`、`block`、`audit` です。|
|defenderPotentiallyUnwantedAppActionSetting|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|取得または設定の Defender の動作の可能性のある不要なアプリケーション (PUA)、広告挿入、支払やサブスクリプションなどのソフトウェアのバンドル化、永続的な要請のビヘイビアーを使用してソフトウェアが含まれています。Defender 警告ユーザーと私用のダウンロード自体をインストールしようとしています。 デスクトップの Windows 10 に追加されます。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderProcessesToExclude|String コレクション|スキャンとリアルタイム保護から除外するプロセス。|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|ユーザーにサンプルの送信を要求する方法の構成。 可能な値は、`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting` です。|
|defenderRequireBehaviorMonitoring|Boolean|動作の監視が必要かどうかを示します。|
|defenderRequireCloudProtection|Boolean|クラウドの保護が必要かどうかを示します。|
|defenderRequireNetworkInspectionSystem|Boolean|ネットワーク検査システムが必要かどうかを示します。|
|defenderRequireRealTimeMonitoring|Boolean|リアルタイムの監視が必要かどうかを示します。|
|defenderScanArchiveFiles|Boolean|アーカイブ ファイルをスキャンするかどうかを示します。|
|defenderScanDownloads|Boolean|ダウンロードをスキャンするかどうかを示します。|
|defenderScanNetworkFiles|Boolean|ネットワーク フォルダーから開かれたファイルをスキャンするかどうかを示します。|
|defenderScanIncomingMail|Boolean|受信メール メッセージをスキャンするかどうかを示します。|
|defenderScanMappedNetworkDrivesDuringFullScan|Boolean|フル スキャン時に、マップされたネットワーク ドライブをスキャンするかどうかを示します。|
|defenderScanRemovableDrivesDuringFullScan|Boolean|フル スキャン時に、リムーバブル ドライブをスキャンするかどうかを示します。|
|defenderScanScriptsLoadedInInternetExplorer|Boolean|Internet Explorer ブラウザーに読み込まれるスクリプトをスキャンするかどうかを示します。|
|defenderSignatureUpdateIntervalInHours|Int32|署名を更新する間隔 (時間)。 確認しない場合は 0 を指定します。 有効な値は 0 から 24 までです|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|Defender システム スキャンの種類。 可能な値は、`userDefined`、`disabled`、`quick`、`full` です。|
|defenderScheduledScanTime|TimeOfDay|システムのスキャンの Defender 時刻。|
|defenderScheduledQuickScanTime|TimeOfDay|毎日のクイック スキャンを実行する時刻。|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|クラウド配信の保護レベルを指定します。 可能な値は、`notConfigured`、`high`、`highPlus`、`zeroTolerance` です。|
|defenderCloudExtendedTimeout|Int32|クラウドでスキャンするファイルの拡張子をタイムアウトします。 有効な値は 0 から 50 までです|
|defenderCloudExtendedTimeoutInSeconds|Int32|クラウドでスキャンするファイルの拡張子をタイムアウトします。 有効な値は 0 から 50 までです|
|defenderBlockOnAccessProtection|ブール値|Windows Defender のアクセスの保護機能を許可または拒否します。|
|defenderScheduleScanDay|[defenderScheduleScanDay](../resources/intune-deviceconfig-defenderschedulescanday.md)|Windows Defender スキャンを実行する日を選択します。 可能な値は、`everyday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`sunday`、`noScheduledScan` です。|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|ユーザーに対するチェック データを送信する Windows Defender のレベルに同意するものです。 可能な値は、`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically` です。|
|lockScreenAllowTimeoutConfiguration|Boolean|Windows 10 Mobile デバイスのロック画面で、画面のタイムアウトを制御するユーザー構成可能な設定を表示するかどうかを指定します。 このポリシーが [許可] に設定されている場合は、lockScreenTimeoutInSeconds によって設定された値は無視されます。|
|lockScreenBlockActionCenterNotifications|Boolean|ロック画面上のアクション センター通知を禁止するかどうかを示します。|
|lockScreenBlockCortana|Boolean|システムのロック中にユーザーが音声認識を使用して Cortana と対話できるかどうかを示します。|
|lockScreenBlockToastNotifications|Boolean|デバイスのロック画面へのトースト通知を許可するかどうかを示します。|
|lockScreenTimeoutInSeconds|Int32|Windows 10 Mobile デバイスで画面をロックしてから画面をオフにするまでの時間 (秒) を設定します。 サポートされている値は 11 から 1800 までです。 有効な値は 11 から 1800 までです|
|passwordBlockSimple|Boolean|"1111" や "1234" などの PIN またはパスワードを許可するかどうかを指定します。 Windows 10 デスクトップでは、ピクチャ パスワードの使用も制御します。|
|passwordExpirationDays|Int32|パスワードの有効期限 (日数)。 有効な値は 0 から 730 までです|
|passwordMinimumLength|Int32|パスワードの最小文字数。 有効な値は 4 から 16 までです|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|passwordMinimumCharacterSetCount|Int32|パスワードに必要な文字セットの数。|
|passwordPreviousPasswordBlockCount|Int32|再使用を禁止する、以前のパスワードの数。 有効な値は 0 から 50 までです|
|passwordRequired|Boolean|ユーザーにパスワードを要求するかどうかを指定します。|
|passwordRequireWhenResumeFromIdleState|Boolean|アイドル状態からの再開時にパスワードを要求するかどうかを示します。|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必要なパスワードの種類。 可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|出荷時の設定にリセットされるサインインの失敗回数。 有効な値は 0 から 999 までです|
|passwordMinimumAgeInDays|Int32|このセキュリティ設定の期間 (日数) をパスワードにする必要がある期間を決定する前に、ユーザーが変更できるために使用します。 有効な値 0 を 998|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|広告識別子の使用を有効または無効にします。 Windows 10 バージョン 1607 で追加されました。 可能な値は、`notConfigured`、`blocked`、`allowed` です。|
|privacyAutoAcceptPairingAndConsentPrompts|Boolean|アプリの起動時に、ペアリングとプライバシーに関するユーザーの同意ダイアログの自動受け入れを許可するかどうかを示します。|
|privacyBlockInputPersonalization|Boolean|Cortana、音声入力、ストア アプリケーションに対するクラウド ベースの音声サービスの使用を禁止するかどうかを示します。|
|privacyBlockPublishUserActivities|ブール値|タスク切り替え等で最近使用したリソースの共有の経験と発見をブロックします。|
|privacyBlockActivityFeed|ブール値|Cortana、ディクテーション、またはストアのアプリケーションをクラウド ベースの音声認識サービスの使用をブロックします。|
|startBlockUnpinningAppsFromTaskbar|Boolean|ユーザーがタスク バーからアプリのピン留めを外すことを禁止するかどうかを示します。|
|startMenuAppListVisibility|[windowsStartMenuAppListVisibilityType](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|この値を設定すると、アプリ リストを折りたたんだり、アプリ リスト全体を削除したり、設定アプリで対応する切り替えを無効にしたりできます。 可能な値は、`userDefined`、`collapse`、`remove`、`disableSettingsApp` です。|
|startMenuHideChangeAccountSettings|Boolean|このポリシーを有効にすると、スタート メニューのユーザー タイルに [アカウント設定の変更] が表示されなくなります。|
|startMenuHideFrequentlyUsedApps|Boolean|このポリシーを有効にすると、よく使われるアプリがスタート メニューに表示されなくなり、設定アプリで対応する切り替えが無効になります。|
|startMenuHideHibernate|Boolean|このポリシーを有効にすると、スタート メニューの電源ボタンに [休止状態] が表示されなくなります。|
|startMenuHideLock|Boolean|このポリシーを有効にすると、スタート メニューのユーザー タイルに [ロック] が表示されなくなります。|
|startMenuHidePowerButton|Boolean|このポリシーを有効にすると、スタート メニューに電源ボタンが表示されなくなります。|
|startMenuHideRecentJumpLists|Boolean|このポリシーを有効にすると、最近開いた項目のジャンプ リストがスタート メニュー/タスクバーに表示されなくなり、設定アプリで対応する切り替えが無効になります。|
|startMenuHideRecentlyAddedApps|Boolean|このポリシーを有効にすると、最近追加したアプリがスタート メニューに表示されなくなり、設定アプリで対応する切り替えが無効になります。|
|startMenuHideRestartOptions|Boolean|このポリシーを有効にすると、スタート メニューの電源ボタンに [再起動]/[更新して再起動] が表示されなくなります。|
|startMenuHideShutDown|Boolean|このポリシーを有効にすると、スタート メニューの電源ボタンに [シャットダウン]/[更新してシャットダウン] が表示されなくなります。|
|startMenuHideSignOut|Boolean|このポリシーを有効にすると、スタート メニューのユーザー タイルに [サインアウト] が表示されなくなります。|
|startMenuHideSleep|Boolean|このポリシーを有効にすると、スタート メニューの電源ボタンに [スリープ] が表示されなくなります。|
|startMenuHideSwitchAccount|Boolean|このポリシーを有効にすると、スタート メニューのユーザー タイルに [アカウントの切り替え] が表示されなくなります。|
|startMenuHideUserTile|Boolean|このポリシーを有効にすると、スタート メニューにユーザー タイルが表示されなくなります。|
|startMenuLayoutEdgeAssetsXml|Binary|このポリシー設定では、Edge アセットをインポートして startMenuLayoutXml ポリシーで使用することができます。 スタートのレイアウトには、Edge アプリからのセカンダリ タイルを含めることができ、このタイルは Edge のローカル アセット ファイルを検索します。 Edge のローカル アセットは存在しないことがあり、その場合は Edge のセカンダリ タイルが空で表示されます。 このポリシーは、startMenuLayoutXml ポリシーが変更された場合にのみ適用されます。 値は、UTF-8 の Base64 でエンコードされたバイト配列にする必要があります。|
|startMenuLayoutXml|Binary|管理者がスタート メニューの既定のレイアウトを上書きし、ユーザーがこれを変更できないようにすることを許可します。 レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。 XML は、UTF8 エンコードのバイト配列形式である必要があります。|
|startMenuMode|[windowsStartMenuModeType](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|管理者がスタート メニューの表示方法を決めることを許可します。 可能な値は、`userDefined`、`fullScreen`、`nonFullScreen` です。|
|startMenuPinnedFolderDocuments|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|スタート メニューへのドキュメント フォルダー ショートカットの表示/非表示を強制します。 可能な値は、`notConfigured`、`hide`、`show` です。|
|startMenuPinnedFolderDownloads|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|スタート メニューへのダウンロード フォルダー ショートカットの表示/非表示を強制します。 可能な値は、`notConfigured`、`hide`、`show` です。|
|startMenuPinnedFolderFileExplorer|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|スタート メニューへのエクスプローラー ショートカットの表示/非表示を強制します。 可能な値は、`notConfigured`、`hide`、`show` です。|
|startMenuPinnedFolderHomeGroup|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|スタート メニューへのホームグループ フォルダー ショートカットの表示/非表示を強制します。 可能な値は、`notConfigured`、`hide`、`show` です。|
|startMenuPinnedFolderMusic|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|スタート メニューへのミュージック フォルダー ショートカットの表示/非表示を強制します。 可能な値は、`notConfigured`、`hide`、`show` です。|
|startMenuPinnedFolderNetwork|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|スタート メニューへのネットワーク フォルダー ショートカットの表示/非表示を強制します。 可能な値は、`notConfigured`、`hide`、`show` です。|
|startMenuPinnedFolderPersonalFolder|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|スタート メニューへの個人用フォルダー ショートカットの表示/非表示を強制します。 可能な値は、`notConfigured`、`hide`、`show` です。|
|startMenuPinnedFolderPictures|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|スタート メニューへのピクチャ フォルダー ショートカットの表示/非表示を強制します。 可能な値は、`notConfigured`、`hide`、`show` です。|
|startMenuPinnedFolderSettings|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|スタート メニューへの設定フォルダー ショートカットの表示/非表示を強制します。 可能な値は、`notConfigured`、`hide`、`show` です。|
|startMenuPinnedFolderVideos|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|スタート メニューへのビデオ フォルダー ショートカットの表示/非表示を強制します。 可能な値は、`notConfigured`、`hide`、`show` です。|
|settingsBlockSettingsApp|Boolean|設定アプリへのアクセスを禁止するかどうかを示します。|
|settingsBlockSystemPage|Boolean|設定アプリ内の [システム] へのアクセスを禁止するかどうかを示します。|
|settingsBlockDevicesPage|Boolean|設定アプリ内の [デバイス] へのアクセスを禁止するかどうかを示します。|
|settingsBlockNetworkInternetPage|Boolean|設定アプリ内の [ネットワークとインターネット] へのアクセスを禁止するかどうかを示します。|
|settingsBlockPersonalizationPage|Boolean|設定アプリ内の [個人用設定] へのアクセスを禁止するかどうかを示します。|
|settingsBlockAccountsPage|Boolean|設定アプリ内の [アカウント] へのアクセスを禁止するかどうかを示します。|
|settingsBlockTimeLanguagePage|Boolean|設定アプリ内の [時刻と言語] へのアクセスを禁止するかどうかを示します。|
|settingsBlockEaseOfAccessPage|Boolean|設定アプリ内の [簡単操作] へのアクセスを禁止するかどうかを示します。|
|settingsBlockPrivacyPage|Boolean|設定アプリ内の [プライバシー] へのアクセスを禁止するかどうかを示します。|
|settingsBlockUpdateSecurityPage|Boolean|設定アプリ内の [更新とセキュリティ] へのアクセスを禁止するかどうかを示します。|
|settingsBlockAppsPage|Boolean|設定アプリ内の [アプリ] へのアクセスを禁止するかどうかを示します。|
|settingsBlockGamingPage|Boolean|設定アプリ内の [ゲーム] へのアクセスを禁止するかどうかを示します。|
|windowsSpotlightBlockConsumerSpecificFeatures|Boolean|通常はコンシューマー向けのエクスペリエンスを IT 管理者が禁止できるようにします。たとえば、開始時の提案、メンバーシップ通知、OOBE 後のアプリ インストール、リダイレクト タイルなどです。|
|windowsSpotlightBlocked|Boolean|IT 管理者が Windows スポットライトのすべての機能をオフにできるようにします|
|windowsSpotlightBlockOnActionCenter|Boolean|各 OS のクリーン インストールやアップグレードの後、またはその後も継続的に、新しい機能や変更された機能を Microsoft からユーザーに紹介することを禁止します|
|windowsSpotlightBlockTailoredExperiences|Boolean|ユーザーのデバイスの使用状況に基づいて Windows スポットライトのコンテンツをカスタマイズすることを禁止します。|
|windowsSpotlightBlockThirdPartyNotifications|Boolean|Windows スポットライト経由でサード パーティのコンテンツを配信することを禁止します|
|windowsSpotlightBlockWelcomeExperience|Boolean|Windows スポットライトからの Windows へようこそのエクスペリエンスを禁止します|
|windowsSpotlightBlockWindowsTips|Boolean|Windows のヒントのポップアップを IT 管理者がオフにできるようにします。|
|windowsSpotlightConfigureOnLockScreen|[windowsSpotlightEnablementSettings](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|スポット ライトの種類を指定します。 可能な値は、`notConfigured`、`disabled`、`enabled` です。|
|networkProxyApplySettingsDeviceWide|Boolean|オンに設定すると、プロキシの設定がデバイスのすべてのプロセスとアカウントに適用されます。 それ以外の場合は、MDM に登録されているユーザー アカウントに適用されます。|
|networkProxyDisableAutoDetect|Boolean|設定の自動検出を無効にします。 有効にした場合、システムはプロキシ自動構成 (PAC) スクリプトへのパスを検索します。|
|networkProxyAutomaticConfigurationUrl|String|使用するプロキシ自動構成 (PAC) スクリプトのアドレス。|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune-deviceconfig-windows10networkproxyserver.md)|プロキシ サーバーの設定を手動で指定します。|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。|
|antiTheftModeBlocked|Boolean|ユーザーが盗難防止モードの設定を選択することを禁止するかどうかを示します (Windows 10 Mobile のみ)。|
|bluetoothBlocked|Boolean|ユーザーが Bluetooth を使用することを禁止するかどうか。|
|cameraBlocked|Boolean|ユーザーがデバイスのカメラにアクセスすることを禁止するかどうか。|
|connectedDevicesServiceBlocked|Boolean|他のデバイスの検出と接続、リモート メッセージング、リモート アプリ セッション、その他のデバイス間エクスペリエンスを可能にする、接続されているデバイスのサービスを禁止するかどうか。|
|certificatesBlockManualRootCertificateInstallation|Boolean|ユーザーが手動でルート証明書をインストールすることを禁止するかどうか。|
|copyPasteBlocked|Boolean|ユーザーがコピーと貼り付けを使用することを禁止するかどうか。|
|cortanaBlocked|Boolean|ユーザーが Cortana を使用することを禁止するかどうか。|
|deviceManagementBlockFactoryResetOnMobile|Boolean|ユーザーが携帯電話をリセットすることを禁止するかどうかを示します。|
|deviceManagementBlockManualUnenroll|Boolean|ユーザーがデバイス管理から手動で登録解除を行うことを禁止するかどうかを示します。|
|safeSearchFilter|[safeSearchFilterType](../resources/intune-deviceconfig-safesearchfiltertype.md)|セーフ サーチに必要なフィルター レベルを指定します。 可能な値は、`userDefined`、`strict`、`moderate` です。|
|edgeBlockPopups|Boolean|ポップアップをブロックするかどうかを示します。|
|edgeBlockSearchSuggestions|Boolean|ユーザーがアドレス バーで検索候補を使用することを禁止するかどうかを示します。|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Boolean|ユーザーが Edge から Internet Explorer にイントラネット トラフィックを送信することを禁止するかどうかを示します。|
|edgeRequireSmartScreen|Boolean|スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。|
|edgeEnterpriseModeSiteListLocation|String|エンタープライズ モードのサイト リストの場所を示します。 ローカル ファイル、ローカル ネットワーク、http の場所が該当します。|
|edgeFirstRunUrl|String|Edge ブラウザーを初めて開いたときに最初に実行される URL です。|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)|IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。|
|edgeHomepageUrls|String コレクション|MDM に登録されているデバイスの Edge ブラウザーに表示されるホームページの URL の一覧です。|
|edgeBlockAccessToAboutFlags|Boolean|Edge ブラウザーの about:flags へのアクセスを禁止するかどうかを示します。|
|smartScreenBlockPromptOverride|Boolean|悪意のある Web サイトの可能性があるサイトに関する SmartScreen フィルターの警告をユーザーが無視できるかどうかを示します。|
|smartScreenBlockPromptOverrideForFiles|Boolean|未検証のファイルのダウンロードに関する SmartScreen フィルターの警告をユーザーが無視できるかどうかを示します|
|webRtcBlockLocalhostIpAddress|Boolean|WebRTC を使用して通話を発信しているときにユーザーのローカル ホストの IP アドレスが表示されるかどうかを示します|
|internetSharingBlocked|Boolean|ユーザーがインターネット共有を使用することを禁止するかどうかを示します。|
|settingsBlockAddProvisioningPackage|Boolean|ユーザーがプロビジョニング パッケージをインストールすることを禁止するかどうかを示します。|
|settingsBlockRemoveProvisioningPackage|Boolean|ランタイム構成エージェントがプロビジョニング パッケージを削除することを禁止するかどうかを示します。|
|settingsBlockChangeSystemTime|Boolean|ユーザーが日付と時刻の設定を変更することを禁止するかどうかを示します。|
|settingsBlockEditDeviceName|Boolean|ユーザーがデバイス名を編集することを禁止するかどうかを示します。|
|settingsBlockChangeRegion|Boolean|ユーザーがリージョン設定を変更することを禁止するかどうかを示します。|
|settingsBlockChangeLanguage|Boolean|ユーザーが言語の設定を変更することを禁止するかどうかを示します。|
|settingsBlockChangePowerSleep|Boolean|ユーザーが電源とスリープの設定を変更することを禁止するかどうかを示します。|
|locationServicesBlocked|Boolean|ユーザーが位置情報サービスを使用することを禁止するかどうかを示します。|
|microsoftAccountBlocked|Boolean|Microsoft アカウントを禁止するかどうかを示します。|
|microsoftAccountBlockSettingsSync|Boolean|Microsoft アカウントの設定の同期を禁止するかどうかを示します。|
|nfcBlocked|Boolean|ユーザーが近距離無線通信を使用することを禁止するかどうかを示します。|
|resetProtectionModeBlocked|Boolean|ユーザーが保護モードをリセットすることを禁止するかどうかを示します。|
|screenCaptureBlocked|Boolean|ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。|
|storageBlockRemovableStorage|Boolean|ユーザーがリムーバブル記憶域を使用することを禁止するかどうかを示します。|
|storageRequireMobileDeviceEncryption|Boolean|モバイル デバイスでの暗号化が必要かどうかを示します。|
|usbBlocked|Boolean|ユーザーが USB 接続を使用することを禁止するかどうかを示します。|
|voiceRecordingBlocked|Boolean|ユーザーが音声録音を使用することを禁止するかどうかを示します。|
|wiFiBlockAutomaticConnectHotspots|Boolean|Wi-Fi ホットスポットへの自動接続を禁止するかどうかを示します。 Wi-Fi がブロックされていれば、この値は関係ありません。|
|wiFiBlocked|Boolean|ユーザーが Wi-Fi を使用することを禁止するかどうかを示します。|
|wiFiBlockManualConfiguration|Boolean|ユーザーが Wi-Fi の手動構成を使用することを禁止するかどうかを示します。|
|wiFiScanInterval|Int32|Wi-Fi ネットワークに対するデバイス スキャンの頻度を指定します。 サポートされている値は 1 から 500 まで、既定値は 100、500 は最低頻度です。 有効な値は 1 から 500 までです|
|wirelessDisplayBlockProjectionToThisDevice|Boolean|他のデバイスがこの PC をプロジェクター用に検出することを許可するかどうかを示します。|
|wirelessDisplayBlockUserInputFromReceiver|Boolean|ワイヤレス ディスプレイ レシーバーからのユーザー入力を許可するかどうかを示します。|
|wirelessDisplayRequirePinForPairing|Boolean|新しいデバイスがペアリングを開始するときに PIN が必要かどうかを示します。|
|windowsStoreBlocked|Boolean|ユーザーが Windows ストアを使用することを禁止するかどうかを示します。|
|appsAllowTrustedAppsSideloading|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|信頼された証明書で署名した AppX パッケージからアプリをサイドローディングできるかどうかを示します。 可能な値は、`notConfigured`、`blocked`、`allowed` です。|
|windowsStoreBlockAutoUpdate|Boolean|Windows ストアからのアプリの自動更新を禁止するかどうかを示します。|
|developerUnlockSetting|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|開発者によるロック解除を許可するかどうかを示します。 可能な値は、`notConfigured`、`blocked`、`allowed` です。|
|sharedUserAppDataAllowed|Boolean|同じアプリの複数のユーザーによるデータ共有を禁止するかどうかを示します。|
|appsBlockWindowsStoreOriginatedApps|Boolean|プレインストールまたはダウンロードによって取得したすべての Windows ストア アプリの起動を無効にするかどうかを示します。|
|windowsStoreEnablePrivateStoreOnly|Boolean|プライベート ストアのみを有効にするかどうかを示します。|
|storageRestrictAppDataToSystemVolume|Boolean|アプリケーションのデータがシステム ドライブに制限されているかどうかを示します。|
|storageRestrictAppInstallToSystemVolume|Boolean|アプリケーションのインストールがシステム ドライブに制限されているかどうかを示します。|
|gameDvrBlocked|Boolean|DVR とブロードキャストを禁止するかどうかを示します。|
|experienceBlockDeviceDiscovery|Boolean|デバイス検出 UX を有効にするかどうかを示します。|
|experienceBlockErrorDialogWhenNoSIM|Boolean|SIM カードが検出されない場合にエラー ダイアログを表示することを許可するかどうかを示します。|
|experienceBlockTaskSwitcher|Boolean|デバイスでのタスクの切り替えを有効にするかどうかを示します。|
|logonBlockFastUserSwitching|Boolean|同時にログオンしているユーザー間での切り替えをログオフなしで迅速に行う機能を無効にします。|
|tenantLockdownRequireNetworkDuringOutOfBoxExperience|ブール値|かどうか、デバイスがネットワークに接続する必要があります。|
|appManagementMSIAllowUserControlOverInstall|ブール値|このポリシー設定は、通常は、システム管理者のみが利用可能なインストール オプションを変更するユーザーを許可します。|
|appManagementMSIAlwaysInstallWithElevatedPrivileges|ブール値|このポリシー設定では、Windows インストーラーがシステム上で任意のプログラムをインストールするときに、昇格されたアクセス許可を使用するように指示します。|
|dataProtectionBlockDirectMemoryAccess|ブール値|このポリシー設定によって、ユーザーが Windows にログインするまですべてホット プラグ可能なダウン ストリーム システムが不安定を使用すると、ダイレクト メモリ アクセス (DMA) をブロックするができます。|



## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) オブジェクトを返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 12202

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "assignedAccessSingleModeUserName": "Assigned Access Single Mode User Name value",
  "assignedAccessSingleModeAppUserModelId": "Assigned Access Single Mode App User Model Id value",
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationAllowFIDODevice": true,
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
  "printerBlockAddition": true,
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableUseLocation": true,
  "searchDisableLocation": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "searchBlockWebResults": true,
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderBlockOnAccessProtection": true,
  "defenderScheduleScanDay": "monday",
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 12310

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "assignedAccessSingleModeUserName": "Assigned Access Single Mode User Name value",
  "assignedAccessSingleModeAppUserModelId": "Assigned Access Single Mode App User Model Id value",
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationAllowFIDODevice": true,
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
  "printerBlockAddition": true,
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableUseLocation": true,
  "searchDisableLocation": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "searchBlockWebResults": true,
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderBlockOnAccessProtection": true,
  "defenderScheduleScanDay": "monday",
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true
}
```






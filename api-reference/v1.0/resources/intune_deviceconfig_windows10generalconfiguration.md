# <a name="windows10generalconfiguration-resource-type"></a>windows10GeneralConfiguration リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このトピックでは、windows10GeneralConfiguration リソースによって公開される、宣言されたメソッド、プロパティ、リレーションシップについて説明します。

[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windows10GeneralConfigurationsをリストする](../api/intune_deviceconfig_windows10generalconfiguration_list.md)|[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) コレクション|[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[windows10GeneralConfigurationを取得する](../api/intune_deviceconfig_windows10generalconfiguration_get.md)|[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md)|[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windows10GeneralConfiguration の作成](../api/intune_deviceconfig_windows10generalconfiguration_create.md)|[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md)|新しい [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) オブジェクトを作成します。|
|[windows10GeneralConfigurationを削除する](../api/intune_deviceconfig_windows10generalconfiguration_delete.md)|なし|[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) を削除します。|
|[windows10GeneralConfigurationを更新する](../api/intune_deviceconfig_windows10generalconfiguration_update.md)|[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md)|[windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|ID|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|説明|文字列|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|displayName|文字列|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|バージョン|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|enterpriseCloudPrintDiscoveryEndPoint|文字列|クラウド プリンターを検出するエンドポイント。|
|enterpriseCloudPrintOAuthAuthority|文字列|OAuth トークンを取得するための認証エンドポイント。|
|enterpriseCloudPrintOAuthClientIdentifier|文字列|OAuth 認証機関から OAuth トークンを取得することを承認されているクライアント アプリケーションの GUID。|
|enterpriseCloudPrintResourceIdentifier|文字列|Azure Portal で構成されている印刷サービスの OAuth リソース URI。|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|検出エンドポイントからクエリを実行する必要があるプリンターの最大数。 これはモバイルのみでの設定です。 有効な値は 1 から 65535 までです|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|文字列|Azure Portal で構成されているプリンター検出サービスの OAuth リソース URI。|
|searchBlockDiacritics|ブール値|検索で分音記号を使用できるかどうかを指定します。|
|searchDisableAutoLanguageDetection|ブール値|コンテンツとプロパティのインデックスを作成するときに、自動言語検出を使用するかどうかを指定します。|
|searchDisableIndexingEncryptedItems|ブール値|Cortana またはエクスプローラーの検索結果に表示されないようにするため、WIP で保護されているアイテムのインデックス作成を禁止するかどうかを示します。|
|searchEnableRemoteQueries|ブール値|このコンピューターのインデックスに対するリモート クエリをブロックするかどうかを示します。|
|searchDisableIndexerBackoff|ブール値|インデクサー バックオフの検索機能を無効にするかどうかを示します。|
|searchDisableIndexingRemovableDrive|ブール値|リムーバブル ドライブ上の場所をライブラリに追加してインデックスを作成することをユーザーに許可するかどうかを示します。|
|searchEnableAutomaticIndexSizeManangement|ブール値|インデックスの場所と同じドライブ上のハード ドライブ領域の最小値を指定して、その最小値を下回ったらインデックス作成を停止するかどうかを示します。|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune_deviceconfig_diagnosticdatasubmissionmode.md)|Watsonのような診断および使用遠隔測定法データを送信するためのデバイス用の値を取得または設定する。可能な値は: `userDefined`, `none`, `basic`, `enhanced`, `full`です。|
|oneDriveDisableFileSync|ブール値|アプリや機能から OneDrive 上のファイルを操作することを IT 管理者が禁止できるかどうかを示す値を取得または設定します。|
|smartScreenEnableAppInstallControl|ブール値|ユーザーがストア以外の場所からアプリをインストールできるかどうかを IT 管理者が制御することを許可します。|
|personalizationDesktopImageUrl|文字列|ダウンロードしてデスクトップ画像として使用する必要がある jpg、jpeg、png 画像の http または https URL、あるいはデスクトップ画像として使用する必要があるファイル システム上のローカル画像のファイル URL。|
|personalizationLockScreenImageUrl|文字列|ダウンロードしてロック画面画像として使用する必要がある jpg、jpeg、png 画像の http または https URL、あるいはロック画面画像として使用する必要があるファイル システム上のローカル画像のファイル URL。|
|bluetoothAllowedServices|String コレクション|許可されている Bluetooth サービスおよびプロファイルの一覧を 16 進形式の文字列として指定します。|
|bluetoothBlockAdvertising|ブール値|ユーザーが Bluetooth 広告を使用することを禁止するかどうか。|
|bluetoothBlockDiscoverableMode|ブール値|ユーザーが Bluetooth の発見可能モードを使用することを禁止するかどうか。|
|bluetoothBlockPrePairing|ブール値|バンドルされた特定のいくつかの Bluetooth 周辺機器を自動的にホスト デバイスとペアにすることを禁止するかどうか。|
|edgeBlockAutofill|ブール値|自動入力を禁止するかどうかを示します。|
|edgeBlocked|ブール値|ユーザーが Edge ブラウザーを使用することを禁止するかどうかを示します。|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune_deviceconfig_edgecookiepolicy.md)|どのクッキーがEdgeブラウザーをブロックするかを表示します。可能な値は: `userDefined`、 `allow`、`blockThirdParty`、 `blockAll` です。|
|edgeBlockDeveloperTools|ブール値|Edge ブラウザー内の開発者ツールを禁止するかどうかを示します。|
|edgeBlockSendingDoNotTrackHeader|ブール値|ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。|
|edgeBlockExtensions|ブール値|Edge ブラウザーの拡張機能を禁止するかどうかを示します。|
|edgeBlockInPrivateBrowsing|ブール値|Edge ブラウザーで会社のネットワークの InPrivate ブラウズを禁止するかどうかを示します。|
|edgeBlockJavaScript|ブール値|ユーザーが JavaScript を使用することを禁止するかどうかを示します。|
|edgeBlockPasswordManager|ブール値|パスワード マネージャーを禁止するかどうかを示します。|
|edgeBlockAddressBarDropdown|ブール値|Microsoft Edge のアドレス バー ドロップダウン機能を禁止します。 Microsoft Edge から Microsoft サービスへのネットワーク接続を最小限に抑えるには、この設定を無効にします。|
|edgeBlockCompatibilityList|ブール値|Microsoft Edge での Microsoft 互換性リストを禁止します。 Microsoft ではこのリストを利用して、既知の互換性の問題があるサイトを Edge で正しく表示できるようにします。|
|edgeClearBrowsingDataOnExit|ブール値|Microsoft Edge の終了時にブラウズ データを消去します。|
|edgeAllowStartPagesModification|ブール値|Edge のスタート ページをユーザーが変更することを許可します。 ユーザーが Edge を開いたときに既定で表示されるスタート ページを指定するには、EdgeHomepageUrls を使用します。|
|edgeDisableFirstRunPage|ブール値|Microsoft Edge の初回使用時に表示される Microsoft の Web ページを禁止します。 このポリシーでは、ゼロ エミッション構成に登録している企業などが、このページの表示を禁止できます。|
|edgeBlockLiveTileDataCollection|ブール値|ユーザーが Microsoft Edge からスタートにサイトをピン留めしたときに、ライブ タイルを作成するために Microsoft が情報を収集することを禁止します。|
|edgeSyncFavoritesWithInternetExplorer|ブール値|Internet Explorer と Microsoft Edge の間でお気に入りの同期を有効にします。 お気に入りの追加、削除、変更、順序変更が、ブラウザー間で共有されます。|
|cellularBlockDataWhenRoaming|ブール値|ローミング中に携帯電話上でユーザーがデータを使用することを禁止するかどうか。|
|cellularBlockVpn|ブール値|携帯電話上でユーザーが VPN を使用することを禁止するかどうか。|
|cellularBlockVpnWhenRoaming|ブール値|ローミング時に携帯電話上でユーザーが VPN を使用することを禁止するかどうか。|
|defenderBlockEndUserAccess|ブール値|エンド ユーザーが Defender にアクセスすることを禁止するかどうか。|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|検疫済みのマルウェアを削除するまでの日数。 有効な値は 0 から 90 までです|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune_deviceconfig_defenderdetectedmalwareactions.md)|検出されたマルウェアに対する Defender のアクションを脅威レベルごとに取得または設定します。|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune_deviceconfig_weeklyschedule.md)|Defender 曜日システム スキャンをします。使用可能な値: `userDefined`、 `everyday`、 `sunday`、 `monday`、 `tuesday`、 `wednesday`、 `thursday`、 `friday`、 `saturday`。|
|defenderFilesAndFoldersToExclude|String コレクション|スキャンとリアルタイム保護から除外するファイルとフォルダー。|
|defenderFileExtensionsToExclude|String コレクション|スキャンとリアルタイム保護から除外するファイル拡張子。|
|defenderScanMaxCpu|Int32|スキャン中の最大 CPU 使用率。 有効な値は 0 から 100 までです|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune_deviceconfig_defendermonitorfileactivity.md)|ファイル・アクティビティを監視するための値です。使用可能な値は: `userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`です。|
|defenderProcessesToExclude|String コレクション|スキャンとリアルタイム保護から除外するプロセス。|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune_deviceconfig_defenderpromptforsamplesubmission.md)|ユーザーにサンプルの送信を要求する方法の設定。可能な値は、  `userDefined`、`alwaysPrompt`、 `promptBeforeSendingPersonalData`、 `neverSendData`、 `sendAllDataWithoutPrompting`です。|
|defenderRequireBehaviorMonitoring|ブール値|動作の監視が必要かどうかを示します。|
|defenderRequireCloudProtection|ブール値|クラウドの保護が必要かどうかを示します。|
|defenderRequireNetworkInspectionSystem|ブール値|ネットワーク検査システムが必要かどうかを示します。|
|defenderRequireRealTimeMonitoring|ブール値|リアルタイムの監視が必要かどうかを示します。|
|defenderScanArchiveFiles|ブール値|アーカイブ ファイルをスキャンするかどうかを示します。|
|defenderScanDownloads|ブール値|ダウンロードをスキャンするかどうかを示します。|
|defenderScanNetworkFiles|ブール値|ネットワーク フォルダーから開かれたファイルをスキャンするかどうかを示します。|
|defenderScanIncomingMail|ブール値|受信メール メッセージをスキャンするかどうかを示します。|
|defenderScanMappedNetworkDrivesDuringFullScan|ブール値|フル スキャン時に、マップされたネットワーク ドライブをスキャンするかどうかを示します。|
|defenderScanRemovableDrivesDuringFullScan|ブール値|フル スキャン時に、リムーバブル ドライブをスキャンするかどうかを示します。|
|defenderScanScriptsLoadedInInternetExplorer|ブール値|Internet Explorer ブラウザーに読み込まれるスクリプトをスキャンするかどうかを示します。|
|defenderSignatureUpdateIntervalInHours|Int32|署名を更新する間隔 (時間)。 確認しない場合は 0 を指定します。 有効な値は 0 から 24 までです|
|defenderScanType|[defenderScanType](../resources/intune_deviceconfig_defenderscantype.md)|Defender のシステム スキャンの種類。可能な値は、 、 、 、 です。 `userDefined``disabled` `quick` `full`|
|defenderScheduledScanTime|TimeOfDay|システムのスキャンの Defender 時刻。|
|defenderScheduledQuickScanTime|TimeOfDay|毎日のクイック スキャンを実行する時刻。|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune_deviceconfig_defendercloudblockleveltype.md)|クラウドが提供する保護のレベルを指定します。可能な値は、`notConfigured`、`high`、`highPlus`、`zeroTolerance`です。|
|lockScreenAllowTimeoutConfiguration|ブール値|Windows 10 Mobile デバイスのロック画面で、画面のタイムアウトを制御するユーザー構成可能な設定を表示するかどうかを指定します。 このポリシーが [許可] に設定されている場合は、lockScreenTimeoutInSeconds によって設定された値は無視されます。|
|lockScreenBlockActionCenterNotifications|ブール値|ロック画面上のアクション センター通知を禁止するかどうかを示します。|
|lockScreenBlockCortana|ブール値|システムのロック中にユーザーが音声認識を使用して Cortana と対話できるかどうかを示します。|
|lockScreenBlockToastNotifications|ブール値|デバイスのロック画面へのトースト通知を許可するかどうかを示します。|
|lockScreenTimeoutInSeconds|Int32|Windows 10 Mobile デバイスで画面をロックしてから画面をオフにするまでの時間 (秒) を設定します。 サポートされている値は 11 から 1800 までです。 有効な値は 11 から 1800 までです|
|passwordBlockSimple|ブール値|"1111" や "1234" などの PIN またはパスワードを許可するかどうかを指定します。 Windows 10 デスクトップでは、ピクチャ パスワードの使用も制御します。|
|passwordExpirationDays|Int32|パスワードの有効期限 (日数)。 有効な値は 0 から 730 までです|
|passwordMinimumLength|Int32|パスワードの最小文字数。 有効な値は 4 から 16 までです|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|passwordMinimumCharacterSetCount|Int32|パスワードに必要な文字セットの数。|
|passwordPreviousPasswordBlockCount|Int32|再使用を禁止する、以前のパスワードの数。 有効な値は 0 から 50 までです|
|passwordRequired|ブール値|ユーザーにパスワードを要求するかどうかを指定します。|
|passwordRequireWhenResumeFromIdleState|ブール値|アイドル状態からの再開時にパスワードを要求するかどうかを示します。|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|必要なパスワードの種類です。使用可能な値は`deviceDefault`、`alphanumeric`、`numeric` です。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|出荷時の設定にリセットされるサインインの失敗回数。 有効な値は 0 から 999 までです|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|広告IDの使用を有効化または非有効化します。バージョン1607のWindows 10に追加されています。可能な値は: `notConfigured`, `blocked`, `allowed`です。|
|privacyAutoAcceptPairingAndConsentPrompts|ブール値|アプリの起動時に、ペアリングとプライバシーに関するユーザーの同意ダイアログの自動受け入れを許可するかどうかを示します。|
|privacyBlockInputPersonalization|ブール値|Cortana、音声入力、ストア アプリケーションに対するクラウド ベースの音声サービスの使用を禁止するかどうかを示します。|
|startBlockUnpinningAppsFromTaskbar|ブール値|ユーザーがタスク バーからアプリのピン留めを外すことを禁止するかどうかを示します。|
|startMenuAppListVisibility|[windowsStartMenuAppListVisibilityType](../resources/intune_deviceconfig_windowsstartmenuapplistvisibilitytype.md)|この値を設定すると、アプリ リストを折りたたんだり、アプリ リスト全体を削除したり、設定アプリで対応する切り替えが無効になります。可能な値は、 `userDefined`, `collapse`, `remove`, `disableSettingsApp` です。|
|startMenuHideChangeAccountSettings|ブール値|このポリシーを有効にすると、スタート メニューのユーザー タイルに [アカウント設定の変更] が表示されなくなります。|
|startMenuHideFrequentlyUsedApps|ブール値|このポリシーを有効にすると、よく使われるアプリがスタート メニューに表示されなくなり、設定アプリで対応する切り替えが無効になります。|
|startMenuHideHibernate|ブール値|このポリシーを有効にすると、スタート メニューの電源ボタンに [休止状態] が表示されなくなります。|
|startMenuHideLock|ブール値|このポリシーを有効にすると、スタート メニューのユーザー タイルに [ロック] が表示されなくなります。|
|startMenuHidePowerButton|ブール値|このポリシーを有効にすると、スタート メニューに電源ボタンが表示されなくなります。|
|startMenuHideRecentJumpLists|ブール値|このポリシーを有効にすると、最近開いた項目のジャンプ リストがスタート メニュー/タスクバーに表示されなくなり、設定アプリで対応する切り替えが無効になります。|
|startMenuHideRecentlyAddedApps|ブール値|このポリシーを有効にすると、最近追加したアプリがスタート メニューに表示されなくなり、設定アプリで対応する切り替えが無効になります。|
|startMenuHideRestartOptions|ブール値|このポリシーを有効にすると、スタート メニューの電源ボタンに [再起動]/[更新して再起動] が表示されなくなります。|
|startMenuHideShutDown|ブール値|このポリシーを有効にすると、スタート メニューの電源ボタンに [シャットダウン]/[更新してシャットダウン] が表示されなくなります。|
|startMenuHideSignOut|ブール値|このポリシーを有効にすると、スタート メニューのユーザー タイルに [サインアウト] が表示されなくなります。|
|startMenuHideSleep|ブール値|このポリシーを有効にすると、スタート メニューの電源ボタンに [スリープ] が表示されなくなります。|
|startMenuHideSwitchAccount|ブール値|このポリシーを有効にすると、スタート メニューのユーザー タイルに [アカウントの切り替え] が表示されなくなります。|
|startMenuHideUserTile|ブール値|このポリシーを有効にすると、スタート メニューにユーザー タイルが表示されなくなります。|
|startMenuLayoutEdgeAssetsXml|バイナリ|このポリシー設定では、Edge アセットをインポートして startMenuLayoutXml ポリシーで使用することができます。 スタートのレイアウトには、Edge アプリからのセカンダリ タイルを含めることができ、このタイルは Edge のローカル アセット ファイルを検索します。 Edge のローカル アセットは存在しないことがあり、その場合は Edge のセカンダリ タイルが空で表示されます。 このポリシーは、startMenuLayoutXml ポリシーが変更された場合にのみ適用されます。 値は、UTF-8 の Base64 でエンコードされたバイト配列にする必要があります。|
|startMenuLayoutXml|バイナリ|管理者がスタート メニューの既定のレイアウトを上書きし、ユーザーがこれを変更できないようにすることを許可します。 レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。 XML は、UTF8 エンコードのバイト配列形式である必要があります。|
|startMenuMode|[windowsStartMenuModeType](../resources/intune_deviceconfig_windowsstartmenumodetype.md)|管理者は、[スタート]メニューの表示方法を決定できます。可能な値は、`userDefined`, `fullScreen`, `nonFullScreen` です。|
|startMenuPinnedFolderDocuments|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|スタート メニューへのドキュメント フォルダー ショートカットの表示/非表示を強制します。可能な値は、 `notConfigured`, `hide`, `show` です。|
|startMenuPinnedFolderDownloads|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|スタート メニューへのダウンロード フォルダー ショートカットの表示/非表示を強制します。可能な値は、`notConfigured`, `hide`, `show` です。|
|startMenuPinnedFolderFileExplorer|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|スタート メニューへのファイル エクスプローラー ショートカットの表示/非表示を強制します。可能な値は、  `notConfigured`, `hide`, `show` です。|
|startMenuPinnedFolderHomeGroup|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|スタート メニューへのホームグループ フォルダー ショートカットの表示/非表示を強制します。可能な値は、 `notConfigured`, `hide`, `show` です。|
|startMenuPinnedFolderMusic|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|スタート メニューへのミュージック フォルダー ショートカットの表示/非表示を強制します。可能な値は、 `notConfigured`, `hide`, `show`  です。|
|startMenuPinnedFolderNetwork|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|スタート メニューへのネットワーク フォルダー ショートカットの表示/非表示を強制します。可能な値は、 `notConfigured`, `hide`, `show` です。|
|startMenuPinnedFolderPersonalFolder|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|スタート メニューへの個人用フォルダー ショートカットの表示/非表示を強制します。可能な値は、   `notConfigured`, `hide`, `show`  です。|
|startMenuPinnedFolderPictures|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|スタート メニューへのピクチャ フォルダー ショートカットの表示/非表示を強制します。可能な値は、 `notConfigured`, `hide`, `show` です。|
|startMenuPinnedFolderSettings|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|スタートメニューへのピクチャフォルダー ショートカットの表示/非表示を強制します。可能な値は、`notConfigured`, `hide`, `show` です。|
|startMenuPinnedFolderVideos|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|スタート メニューへのビデオ フォルダー ショートカットの表示/非表示を強制します。可能な値は、 `notConfigured`, `hide`, `show` です。|
|settingsBlockSettingsApp|ブール値|設定アプリへのアクセスを禁止するかどうかを示します。|
|settingsBlockSystemPage|ブール値|設定アプリ内の [システム] へのアクセスを禁止するかどうかを示します。|
|settingsBlockDevicesPage|ブール値|設定アプリ内の [デバイス] へのアクセスを禁止するかどうかを示します。|
|settingsBlockNetworkInternetPage|ブール値|設定アプリ内の [ネットワークとインターネット] へのアクセスを禁止するかどうかを示します。|
|settingsBlockPersonalizationPage|ブール値|設定アプリ内の [個人用設定] へのアクセスを禁止するかどうかを示します。|
|settingsBlockAccountsPage|ブール値|設定アプリ内の [アカウント] へのアクセスを禁止するかどうかを示します。|
|settingsBlockTimeLanguagePage|ブール値|設定アプリ内の [時刻と言語] へのアクセスを禁止するかどうかを示します。|
|settingsBlockEaseOfAccessPage|ブール値|設定アプリ内の [簡単操作] へのアクセスを禁止するかどうかを示します。|
|settingsBlockPrivacyPage|ブール値|設定アプリ内の [プライバシー] へのアクセスを禁止するかどうかを示します。|
|settingsBlockUpdateSecurityPage|ブール値|設定アプリ内の [更新とセキュリティ] へのアクセスを禁止するかどうかを示します。|
|settingsBlockAppsPage|ブール値|設定アプリ内の [アプリ] へのアクセスを禁止するかどうかを示します。|
|settingsBlockGamingPage|ブール値|設定アプリ内の [ゲーム] へのアクセスを禁止するかどうかを示します。|
|windowsSpotlightBlockConsumerSpecificFeatures|ブール値|通常はコンシューマー向けのエクスペリエンスを IT 管理者が禁止できるようにします。たとえば、開始時の提案、メンバーシップ通知、OOBE 後のアプリ インストール、リダイレクト タイルなどです。|
|windowsSpotlightBlocked|ブール値|IT 管理者が Windows スポットライトのすべての機能をオフにできるようにします|
|windowsSpotlightBlockOnActionCenter|ブール値|各 OS のクリーン インストールやアップグレードの後、またはその後も継続的に、新しい機能や変更された機能を Microsoft からユーザーに紹介することを禁止します|
|windowsSpotlightBlockTailoredExperiences|ブール値|ユーザーのデバイスの使用状況に基づいて Windows スポットライトのコンテンツをカスタマイズすることを禁止します。|
|windowsSpotlightBlockThirdPartyNotifications|ブール値|Windows スポットライト経由でサード パーティのコンテンツを配信することを禁止します|
|windowsSpotlightBlockWelcomeExperience|ブール値|Windows スポットライトからの Windows へようこそのエクスペリエンスを禁止します|
|windowsSpotlightBlockWindowsTips|ブール値|Windows のヒントのポップアップを IT 管理者がオフにできるようにします。|
|windowsSpotlightConfigureOnLockScreen|[windowsSpotlightEnablementSettings](../resources/intune_deviceconfig_windowsspotlightenablementsettings.md)|スポットライトの種類を指定します。可能な値は、`notConfigured`、`disabled`、`enabled`です。|
|networkProxyApplySettingsDeviceWide|ブール値|オンに設定すると、プロキシの設定がデバイスのすべてのプロセスとアカウントに適用されます。 それ以外の場合は、MDM に登録されているユーザー アカウントに適用されます。|
|networkProxyDisableAutoDetect|ブール値|設定の自動検出を無効にします。 有効にした場合、システムはプロキシ自動構成 (PAC) スクリプトへのパスを検索します。|
|networkProxyAutomaticConfigurationUrl|文字列|使用するプロキシ自動構成 (PAC) スクリプトのアドレス。|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune_deviceconfig_windows10networkproxyserver.md)|プロキシ サーバーの設定を手動で指定します。|
|accountsBlockAddingNonMicrosoftAccountEmail|ブール値|Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。|
|antiTheftModeBlocked|ブール値|ユーザーが盗難防止モードの設定を選択することを禁止するかどうかを示します (Windows 10 Mobile のみ)。|
|bluetoothBlocked|ブール値|ユーザーが Bluetooth を使用することを禁止するかどうか。|
|cameraBlocked|ブール値|ユーザーがデバイスのカメラにアクセスすることを禁止するかどうか。|
|connectedDevicesServiceBlocked|ブール値|他のデバイスの検出と接続、リモート メッセージング、リモート アプリ セッション、その他のデバイス間エクスペリエンスを可能にする、接続されているデバイスのサービスを禁止するかどうか。|
|certificatesBlockManualRootCertificateInstallation|ブール値|ユーザーが手動でルート証明書をインストールすることを禁止するかどうか。|
|copyPasteBlocked|ブール値|ユーザーがコピーと貼り付けを使用することを禁止するかどうか。|
|cortanaBlocked|ブール値|ユーザーが Cortana を使用することを禁止するかどうか。|
|deviceManagementBlockFactoryResetOnMobile|ブール値|ユーザーが携帯電話をリセットすることを禁止するかどうかを示します。|
|deviceManagementBlockManualUnenroll|ブール値|ユーザーがデバイス管理から手動で登録解除を行うことを禁止するかどうかを示します。|
|safeSearchFilter|[safeSearchFilterType](../resources/intune_deviceconfig_safesearchfiltertype.md)|安全な検索が必要なフィルターレベルを指定します。可能な値は、`userDefined`、`strict`、`moderate`です。|
|edgeBlockPopups|ブール値|ポップアップをブロックするかどうかを示します。|
|edgeBlockSearchSuggestions|ブール値|ユーザーがアドレス バーで検索候補を使用することを禁止するかどうかを示します。|
|edgeBlockSendingIntranetTrafficToInternetExplorer|ブール値|ユーザーが Edge から Internet Explorer にイントラネット トラフィックを送信することを禁止するかどうかを示します。|
|edgeRequireSmartScreen|ブール値|スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。|
|edgeEnterpriseModeSiteListLocation|文字列|エンタープライズ モードのサイト リストの場所を示します。 ローカル ファイル、ローカル ネットワーク、http の場所が該当します。|
|edgeFirstRunUrl|文字列|Edge ブラウザーを初めて開いたときに最初に実行される URL です。|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)|IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。|
|edgeHomepageUrls|String コレクション|MDM に登録されているデバイスの Edge ブラウザーに表示されるホームページの URL の一覧です。|
|edgeBlockAccessToAboutFlags|ブール値|Edge ブラウザーの about:flags へのアクセスを禁止するかどうかを示します。|
|smartScreenBlockPromptOverride|ブール値|悪意のある Web サイトの可能性があるサイトに関する SmartScreen フィルターの警告をユーザーが無視できるかどうかを示します。|
|smartScreenBlockPromptOverrideForFiles|ブール値|未検証のファイルのダウンロードに関する SmartScreen フィルターの警告をユーザーが無視できるかどうかを示します|
|webRtcBlockLocalhostIpAddress|ブール値|WebRTC を使用して通話を発信しているときにユーザーのローカル ホストの IP アドレスが表示されるかどうかを示します|
|internetSharingBlocked|ブール値|ユーザーがインターネット共有を使用することを禁止するかどうかを示します。|
|settingsBlockAddProvisioningPackage|ブール値|ユーザーがプロビジョニング パッケージをインストールすることを禁止するかどうかを示します。|
|settingsBlockRemoveProvisioningPackage|ブール値|ランタイム構成エージェントがプロビジョニング パッケージを削除することを禁止するかどうかを示します。|
|settingsBlockChangeSystemTime|ブール値|ユーザーが日付と時刻の設定を変更することを禁止するかどうかを示します。|
|settingsBlockEditDeviceName|ブール値|ユーザーがデバイス名を編集することを禁止するかどうかを示します。|
|settingsBlockChangeRegion|ブール値|ユーザーがリージョン設定を変更することを禁止するかどうかを示します。|
|settingsBlockChangeLanguage|ブール値|ユーザーが言語の設定を変更することを禁止するかどうかを示します。|
|settingsBlockChangePowerSleep|ブール値|ユーザーが電源とスリープの設定を変更することを禁止するかどうかを示します。|
|locationServicesBlocked|ブール値|ユーザーが位置情報サービスを使用することを禁止するかどうかを示します。|
|microsoftAccountBlocked|ブール値|Microsoft アカウントを禁止するかどうかを示します。|
|microsoftAccountBlockSettingsSync|ブール値|Microsoft アカウントの設定の同期を禁止するかどうかを示します。|
|nfcBlocked|ブール値|ユーザーが近距離無線通信を使用することを禁止するかどうかを示します。|
|resetProtectionModeBlocked|ブール値|ユーザーが保護モードをリセットすることを禁止するかどうかを示します。|
|screenCaptureBlocked|ブール値|ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。|
|storageBlockRemovableStorage|ブール値|ユーザーがリムーバブル記憶域を使用することを禁止するかどうかを示します。|
|storageRequireMobileDeviceEncryption|ブール値|モバイル デバイスでの暗号化が必要かどうかを示します。|
|usbBlocked|ブール値|ユーザーが USB 接続を使用することを禁止するかどうかを示します。|
|voiceRecordingBlocked|ブール値|ユーザーが音声録音を使用することを禁止するかどうかを示します。|
|wiFiBlockAutomaticConnectHotspots|ブール値|Wi-Fi ホットスポットへの自動接続を禁止するかどうかを示します。 Wi-Fi がブロックされていれば、この値は関係ありません。|
|wiFiBlocked|ブール値|ユーザーが Wi-Fi を使用することを禁止するかどうかを示します。|
|wiFiBlockManualConfiguration|ブール値|ユーザーが Wi-Fi の手動構成を使用することを禁止するかどうかを示します。|
|wiFiScanInterval|Int32|Wi-Fi ネットワークに対するデバイス スキャンの頻度を指定します。 サポートされている値は 1 から 500 まで、既定値は 100、500 は最低頻度です。 有効な値は 1 から 500 までです|
|wirelessDisplayBlockProjectionToThisDevice|ブール値|他のデバイスがこの PC をプロジェクター用に検出することを許可するかどうかを示します。|
|wirelessDisplayBlockUserInputFromReceiver|ブール値|ワイヤレス ディスプレイ レシーバーからのユーザー入力を許可するかどうかを示します。|
|wirelessDisplayRequirePinForPairing|ブール値|新しいデバイスがペアリングを開始するときに PIN が必要かどうかを示します。|
|windowsStoreBlocked|ブール値|ユーザーが Windows ストアを使用することを禁止するかどうかを示します。|
|appsAllowTrustedAppsSideloading|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|AppX パッケージが信頼できる証明書で署名されてからアプリケーションが読み込まれる側にできるかどうかを示します。可能な値は、 `notConfigured`、 `blocked`、 `allowed` です。|
|windowsStoreBlockAutoUpdate|ブール値|Windows ストアからのアプリの自動更新を禁止するかどうかを示します。|
|developerUnlockSetting|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|開発者によるロック解除を許可するかどうかを示します。可能な値は、 `notConfigured`, `blocked`, `allowed` です。|
|sharedUserAppDataAllowed|ブール値|同じアプリの複数のユーザーによるデータ共有を禁止するかどうかを示します。|
|appsBlockWindowsStoreOriginatedApps|ブール値|プレインストールまたはダウンロードによって取得したすべての Windows ストア アプリの起動を無効にするかどうかを示します。|
|windowsStoreEnablePrivateStoreOnly|ブール値|プライベート ストアのみを有効にするかどうかを示します。|
|storageRestrictAppDataToSystemVolume|ブール値|アプリケーションのデータがシステム ドライブに制限されているかどうかを示します。|
|storageRestrictAppInstallToSystemVolume|ブール値|アプリケーションのインストールがシステム ドライブに制限されているかどうかを示します。|
|gameDvrBlocked|ブール値|DVR とブロードキャストを禁止するかどうかを示します。|
|experienceBlockDeviceDiscovery|ブール値|デバイス検出 UX を有効にするかどうかを示します。|
|experienceBlockErrorDialogWhenNoSIM|ブール値|SIM カードが検出されない場合にエラー ダイアログを表示することを許可するかどうかを示します。|
|experienceBlockTaskSwitcher|ブール値|デバイスでのタスクの切り替えを有効にするかどうかを示します。|
|logonBlockFastUserSwitching|ブール値|同時にログオンしているユーザー間での切り替えをログオフなしで迅速に行う機能を無効にします。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|割り当て|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10GeneralConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "enterpriseCloudPrintDiscoveryEndPoint": "String",
  "enterpriseCloudPrintOAuthAuthority": "String",
  "enterpriseCloudPrintOAuthClientIdentifier": "String",
  "enterpriseCloudPrintResourceIdentifier": "String",
  "enterpriseCloudPrintDiscoveryMaxLimit": 1024,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "String",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "String",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "String",
  "personalizationLockScreenImageUrl": "String",
  "bluetoothAllowedServices": [
    "String"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "String",
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
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 1024,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "String",
    "moderateSeverity": "String",
    "highSeverity": "String",
    "severeSeverity": "String"
  },
  "defenderSystemScanSchedule": "String",
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderScanMaxCpu": 1024,
  "defenderMonitorFileActivity": "String",
  "defenderProcessesToExclude": [
    "String"
  ],
  "defenderPromptForSampleSubmission": "String",
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
  "defenderSignatureUpdateIntervalInHours": 1024,
  "defenderScanType": "String",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderCloudBlockLevel": "String",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 1024,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "privacyAdvertisingId": "String",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "String",
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
  "startMenuLayoutEdgeAssetsXml": "binary",
  "startMenuLayoutXml": "binary",
  "startMenuMode": "String",
  "startMenuPinnedFolderDocuments": "String",
  "startMenuPinnedFolderDownloads": "String",
  "startMenuPinnedFolderFileExplorer": "String",
  "startMenuPinnedFolderHomeGroup": "String",
  "startMenuPinnedFolderMusic": "String",
  "startMenuPinnedFolderNetwork": "String",
  "startMenuPinnedFolderPersonalFolder": "String",
  "startMenuPinnedFolderPictures": "String",
  "startMenuPinnedFolderSettings": "String",
  "startMenuPinnedFolderVideos": "String",
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
  "windowsSpotlightConfigureOnLockScreen": "String",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "String",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "String",
    "exceptions": [
      "String"
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
  "safeSearchFilter": "String",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "String",
  "edgeFirstRunUrl": "String",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "String"
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
  "wiFiScanInterval": 1024,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "String",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "String",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true
}
```









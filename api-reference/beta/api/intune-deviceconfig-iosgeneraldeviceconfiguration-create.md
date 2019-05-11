---
title: Create iosGeneralDeviceConfiguration
description: 新しい iosGeneralDeviceConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ea0f0e23f63f839e3dfa79e3888aa356eee1376
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923476"
---
# <a name="create-iosgeneraldeviceconfiguration"></a>Create iosGeneralDeviceConfiguration

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトを作成します。

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
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、iosGeneralDeviceConfiguration オブジェクトの JSON 表記を指定します。

次の表に、iosGeneralDeviceConfiguration の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|description|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|accountBlockModification|Boolean|デバイスが監視モードのときに、アカウントの変更を許可するかどうかを示します。|
|activationLockAllowWhenSupervised|Boolean|デバイスが監視モードのときに、アクティベーション ロックを許可するかどうかを示します。|
|airDropBlocked|Boolean|デバイスが監視モードのときに、AirDrop を許可するかどうかを示します。|
|airDropForceUnmanagedDropTarget|Boolean|AirDrop を管理対象外のドロップ ターゲットと見なすかどうかを示します (iOS 9.0 以降)。|
|airPlayForcePairingPasswordForOutgoingRequests|Boolean|ペアリング パスワードを使用するために、このデバイスからの AirPlay 要求を受信するすべてのデバイスを適用するかどうかを示します。|
|appleWatchBlockPairing|Boolean|デバイスが監視モードのときに、Apple Watch のペアリングを許可するかどうかを示します (iOS 9.0 以降)。|
|appleWatchForceWristDetection|Boolean|ペアリングされている Apple Watch に手首検出機能を強制的に使用させるかどうかを示します (iOS 8.2 以降)。|
|appleNewsBlocked|Boolean|デバイスが監視モードのときに、ユーザーによる News の使用を禁止するかどうかを示します (iOS 9.0 以降)。|
|appsSingleAppModeList|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|単一アプリ モードに自律的に入ることが許可されている iOS アプリのリストを取得または設定します。 監視モードのみ。 iOS 7.0 以降。 このコレクションには、最大で 500 個の要素を含めることができます。|
|appsVisibilityList|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|可視性リストにあるアプリのリスト (iOS 9.3 以降で、AppVisibilityListType によって制御される、表示可能/起動可能なアプリのリスト、または非表示/起動できないアプリのリスト)。 このコレクションには、最大で 10000 個の要素を含めることができます。|
|appsVisibilityListType|[アプライアンスの種類](../resources/intune-deviceconfig-applisttype.md)|AppsVisibilityList 内にあるリストの種類です。 可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。|
|appStoreBlockAutomaticDownloads|Boolean|デバイスが監視モードのときに、他のデバイスで購入したアプリの自動ダウンロードをブロックするかどうかを示します (iOS 9.0 以降)。|
|appStoreBlocked|Boolean|ユーザーによる App Store の使用を禁止するかどうかを示します。|
|appStoreBlockInAppPurchases|Boolean|ユーザーによるアプリの購入を禁止するかどうかを示します。|
|appStoreBlockUIAppInstallation|Boolean|ホスト アプリによるインストールを制限せずに、App Store アプリをブロックするかどうかを示します。 監視モードのみに適用されます (iOS 9.0 以降)。|
|appStoreRequirePassword|Boolean|App Store 使用時に、パスワードを要求するかどうかを指定します。|
|autoFillForceAuthentication|Boolean|Safari や、監視対象デバイスの他のアプリで、パスワードとクレジットカード情報を自動入力する前に、ユーザー認証を強制するかどうかを示します。|
|bluetoothBlockModification|Boolean|デバイスが監視モードのときに、Bluetooth の設定の変更を許可するかどうかを示します (iOS 10.0 以降)。|
|cameraBlocked|Boolean|ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。|
|cellularBlockDataRoaming|Boolean|データ ローミングをブロックするかどうかを示します。|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Boolean|ローミング中に、グローバルなバックグラウンド フェッチをブロックするかどうかを示します。|
|cellularBlockPerAppDataModification|Boolean|デバイスが監視モードのときに、携帯ネットワーク アプリのデータの使用設定の変更を許可するかどうかを示します。|
|cellularBlockPersonalHotspot|Boolean|個人用ホットスポットをブロックするかどうかを示します。|
|Cellularblockplan の変更|Boolean|ユーザーが、監視対象デバイスの携帯電話プランの設定を変更することを許可するかどうかを示します。|
|cellularBlockVoiceRoaming|Boolean|音声通話ローミングをブロックするかどうかを示します。|
|certificatesBlockUntrustedTlsCertificates|Boolean|信頼されていない TLS の証明書をブロックするかどうかを示します。|
|classroomAppBlockRemoteScreenObservation|Boolean|デバイスが監視モードのときに、Classroom アプリによるリモート画面の監視を許可するかどうかを示します (iOS 9.3 以降)。|
|classroomAppForceUnpromptedScreenObservation|Boolean|デバイスが監視モードになっているときに、Classroom アプリでの管理対象コースの教師に、メッセージを表示せずに学生の画面を表示する許可を自動的に与えるかどうかを示します。|
|classroomForceAutomaticallyJoinClasses|Boolean|デバイスが監視モードのときに、学生に確認せずに教師の要求に対して自動的にアクセス許可を付与するかどうかを示します。|
|classroomForceUnpromptedAppAndDeviceLock|Boolean|学生にメッセージを表示せずに、アプリまたはデバイスのロックを教師に許可するかどうかを示します。 監視モードのみ。|
|compliantAppsList|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。 このコレクションには、最大で 10000 個の要素を含めることができます。|
|compliantAppListType|[アプライアンスの種類](../resources/intune-deviceconfig-applisttype.md)|AppComplianceList 内にあるリスト。 可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。|
|configurationProfileBlockChanges|Boolean|デバイスが監視モードのときに、ユーザーが構成プロファイルと証明書を対話形式でインストールするのをブロックするかどうかを示します。|
|definitionLookupBlocked|Boolean|デバイスが監視モードのときに、定義の検索を禁止するかどうかを示します (iOS 8.1.3 以降)。|
|deviceBlockEnableRestrictions|Boolean|デバイスが監視モードのときに、ユーザーがデバイス設定の制限を有効にできるようにするかどうかを示します。|
|deviceBlockEraseContentAndSettings|Boolean|デバイスが監視モードのときに、デバイスの [すべてのコンテンツと設定を消去] オプションの使用を許可するかどうかを示します。|
|deviceBlockNameModification|Boolean|デバイスが監視モードのときに、デバイス名の変更を許可するかどうかを示します (iOS 9.0 以降)。|
|diagnosticDataBlockSubmission|Boolean|診断データの送信をブロックするかどうかを示します。|
|diagnosticDataBlockSubmissionModification|Boolean|デバイスが監視モードのときに、診断の送信の設定変更を許可するかどうかを示します (iOS 9.3.2 以降)。|
|documentsBlockManagedDocumentsInUnmanagedApps|Boolean|ユーザーによる非管理対象アプリでの管理対象ドキュメントの表示を禁止するかどうかを示します。|
|documentsBlockUnmanagedDocumentsInManagedApps|Boolean|ユーザーによる管理対象アプリでの非管理対象ドキュメントの表示を禁止するかどうかを示します。|
|emailInDomainSuffixes|String コレクション|これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。|
|enterpriseAppBlockTrust|Boolean|ユーザーによるエンタープライズ アプリの信頼を禁止するかどうかを示します。|
|enterpriseAppBlockTrustModification|Boolean|ユーザーによるエンタープライズ アプリの信頼の設定の変更を禁止するかどうかを示します。|
|esimBlockModification|Boolean|監視対象デバイスの eSIM での携帯電話プランの追加または削除を許可するかどうかを示します。|
|faceTimeBlocked|Boolean|ユーザーによる FaceTime の使用を禁止するかどうかを示します。|
|findMyFriendsBlocked|Boolean|デバイスが監視モードのときに、"友達を探す" をブロックするかどうかを示します。|
|gamingBlockGameCenterFriends|Boolean|ユーザーによる Game Center での友達の追加を禁止するかどうかを示します。|
|gamingBlockMultiplayer|Boolean|ユーザーによるマルチプレイヤー ゲームの使用を禁止するかどうかを示します。|
|gameCenterBlocked|Boolean|デバイスが監視モードのときに、ユーザーによる Game Center の使用を禁止するかどうかを示します。|
|hostPairingBlocked|Boolean|iOS デバイスが監視モードのときに、iOS デバイスがペアリングできるデバイスをホスト ペアリングで制御できるようにするかどうかを示します。|
|iBooksStoreBlocked|Boolean|デバイスが監視モードのときに、ユーザーによる iBooks Store の使用を禁止するかどうかを示します。|
|iBooksStoreBlockErotica|Boolean|アダルトのフラグが付いている iBookstore からのメディアのダウンロードをブロックするかどうかを示します。|
|iCloudBlockActivityContinuation|ブール型|ユーザーが iOS デバイスで開始された作業を別の iOS デバイスまたは macOS デバイスに継続して実行することを禁止するかどうかを示します。|
|iCloudBlockBackup|Boolean|iCloud バックアップを禁止するかどうかを示します。|
|iCloudBlockDocumentSync|Boolean|iCloud のドキュメントの同期を禁止するかどうかを示します。|
|iCloudBlockManagedAppsSync|Boolean|管理対象アプリのクラウドの同期を禁止するかどうかを示します。|
|iCloudBlockPhotoLibrary|Boolean|iCloud フォト ライブラリを禁止するかどうかを示します。|
|iCloudBlockPhotoStreamSync|Boolean|iCloud フォトのストリームの同期を禁止するかどうかを示します。|
|iCloudBlockSharedPhotoStream|Boolean|共有フォト ストリームの同期を禁止するかどうかを示します。|
|iCloudRequireEncryptedBackup|Boolean|iCloud のバックアップを暗号化する必要があるかどうかを示します。|
|iTunesBlockExplicitContent|Boolean|ユーザーによる iTunes および App Store の過激な描写のコンテンツへのアクセスをブロックするかどうかを指定します。|
|iTunesBlockMusicService|Boolean|デバイスが監視モードのときに、Music サービスをブロックして Music アプリをクラシック モードに戻すかどうかを示します (iOS 9.3 以降および macOS 10.12 以降)。|
|iTunesBlockRadio|Boolean|デバイスが監視モードのときに、ユーザーによる iTunes Radio の使用を禁止するかどうかを示します (iOS 9.3 以降)。|
|keyboardBlockAutoCorrect|Boolean|デバイスが監視モードのときに、キーボードの自動修正を禁止するかどうかを示します (iOS 8.13 以降)。|
|keyboardBlockDictation|Boolean|デバイスが監視モードのときに、ユーザーによるディクテーション入力の使用を禁止するかどうかを示します。|
|keyboardBlockPredictive|Boolean|デバイスが監視モードのときに、予測キーボードを禁止するかどうかを示します (iOS 8.1.3 以降)。|
|keyboardBlockShortcuts|Boolean|デバイスが監視モードのときに、キーボード ショートカットを禁止するかどうかを示します (iOS 9.0 以降)。|
|keyboardBlockSpellCheck|Boolean|デバイスが監視モードのときに、キーボードのスペル チェックを禁止するかどうかを示します (iOS 8.13 以降)。|
|kioskModeAllowAssistiveSpeak|Boolean|キオスク モード時の補助音声を許可するかどうかを示します。|
|kioskModeAllowAssistiveTouchSettings|Boolean|キオスク モード時の Assistive Touch の設定へのアクセスを許可するかどうかを示します。|
|kioskModeAllowAutoLock|Boolean|キオスク モード時のデバイスの自動ロックを許可するかどうかを示します。 このプロパティの機能は、OS の既定値と重複しています。非推奨です。 代わりに KioskModeBlockAutoLock を使用します。|
|kioskModeBlockAutoLock|Boolean|キオスクモード時にデバイスの自動ロックをブロックするかどうかを示します。|
|kioskModeAllowColorInversionSettings|Boolean|キオスク モード時の色反転の設定へのアクセスを許可するかどうかを示します。|
|kioskModeAllowRingerSwitch|Boolean|キオスク モード時の着信音スイッチの使用を許可するかどうかを示します。 このプロパティの機能は、OS の既定値と重複しています。非推奨です。 代わりに KioskModeBlockRingerSwitch を使用します。|
|kioskModeBlockRingerSwitch|Boolean|キオスクモード時の着信音スイッチの使用を禁止するかどうかを示します。|
|kioskModeAllowScreenRotation|Boolean|キオスク モード時の画面の回転を許可するかどうかを示します。 このプロパティの機能は、OS の既定値と重複しています。非推奨です。 代わりに KioskModeBlockScreenRotation を使用します。|
|kioskModeBlockScreenRotation|Boolean|キオスクモード時の画面の回転を禁止するかどうかを示します。|
|kioskModeAllowSleepButton|Boolean|キオスク モード時のスリープ ボタンの使用を許可するかどうかを示します。 このプロパティの機能は、OS の既定値と重複しています。非推奨です。 代わりに KioskModeBlockSleepButton を使用します。|
|kioskModeBlockSleepButton|Boolean|キオスクモード時のスリープボタンの使用を禁止するかどうかを示します。|
|kioskModeAllowTouchscreen|Boolean|キオスク モード時のタッチスクリーンの使用を許可するかどうかを示します。 このプロパティの機能は、OS の既定値と重複しています。非推奨です。 代わりに KioskModeBlockTouchscreen を使用します。|
|kioskModeBlockTouchscreen|Boolean|キオスクモード時のタッチスクリーンの使用を禁止するかどうかを示します。|
|kioskModeAllowVoiceOverSettings|Boolean|キオスク モード時のボイス オーバーの設定へのアクセスを許可するかどうかを示します。|
|kioskModeAllowVolumeButtons|Boolean|キオスク モード時のボリューム ボタンの使用を許可するかどうかを示します。 このプロパティの機能は、OS の既定値と重複しています。非推奨です。 代わりに KioskModeBlockVolumeButtons を使用します。|
|kioskModeBlockVolumeButtons|Boolean|キオスク モード中にボリューム ボタンをブロックするかどうかを示します。|
|kioskModeAllowZoomSettings|Boolean|キオスク モード時のズーム設定へのアクセスを許可するかどうかを示します。|
|kioskModeAppStoreUrl|String|キオスク モード用に使用するアプリへの、App Store 内の URL。 KioskModeManagedAppId が不明な場合に使用します。|
|kioskModeBuiltInAppId|String|キオスクモード用に使用する組み込みアプリの ID。 KioskModeManagedAppId および KioskModeAppStoreUrl が設定されていない場合に使用します。|
|kioskModeRequireAssistiveTouch|Boolean|キオスク モード時に Assistive Touch が必要かどうかを示します。|
|kioskModeRequireColorInversion|Boolean|キオスク モード時に色反転が必要かどうかを示します。|
|kioskModeRequireMonoAudio|Boolean|キオスク モード時にモノラル オーディオが必要かどうかを示します。|
|kioskModeRequireVoiceOver|Boolean|キオスク モード時にボイス オーバーが必要かどうかを示します。|
|kioskModeRequireZoom|Boolean|キオスク モード時にズームが必要かどうかを示します。|
|kioskModeManagedAppId|String|キオスク モード用に使用するアプリの管理対象アプリ ID。 KioskModeManagedAppId が指定されている場合は、KioskModeAppStoreUrl は無視されます。|
|lockScreenBlockControlCenter|Boolean|ユーザーによるロック画面でのコントロール センターの使用を禁止するかどうかを示します。|
|lockScreenBlockNotificationView|Boolean|ユーザーによるロック画面での通知ビューの使用を禁止するかどうかを示します。|
|lockScreenBlockPassbook|Boolean|デバイスがロックされているときに、ユーザーによる Passbook の使用を禁止するかどうかを示します。|
|lockScreenBlockTodayView|Boolean|ユーザーによるロック画面での本日のビューの使用を禁止するかどうかを示します。|
|mediaContentRatingAustralia|[mediaContentRatingAustralia](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|メディア コンテンツの評価の設定 (オーストラリア向け)|
|mediaContentRatingCanada|[mediaContentRatingCanada](../resources/intune-deviceconfig-mediacontentratingcanada.md)|メディア コンテンツの評価の設定 (カナダ向け)|
|mediaContentRatingFrance|[mediaContentRatingFrance](../resources/intune-deviceconfig-mediacontentratingfrance.md)|メディア コンテンツの評価の設定 (フランス向け)|
|mediaContentRatingGermany|[mediaContentRatingGermany](../resources/intune-deviceconfig-mediacontentratinggermany.md)|メディア コンテンツの評価の設定 (ドイツ向け)|
|mediaContentRatingIreland|[mediaContentRatingIreland](../resources/intune-deviceconfig-mediacontentratingireland.md)|メディア コンテンツの評価の設定 (アイルランド向け)|
|mediaContentRatingJapan|[mediaContentRatingJapan](../resources/intune-deviceconfig-mediacontentratingjapan.md)|メディア コンテンツの評価の設定 (日本向け)|
|mediaContentRatingNewZealand|[mediaContentRatingNewZealand](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|メディア コンテンツの評価の設定 (ニュージーランド向け)|
|mediaContentRatingUnitedKingdom|[mediaContentRatingUnitedKingdom](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|メディア コンテンツの評価の設定 (英国向け)|
|mediaContentRatingUnitedStates|[mediaContentRatingUnitedStates](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|メディア コンテンツの評価の設定 (米国向け)|
|networkUsageRules|[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) コレクション|管理対象アプリと、それらに適用されるネットワーク ルールのリストです。 このコレクションには、最大で 1000 個の要素を含めることができます。|
|mediaContentRatingApps|[ratingAppsType](../resources/intune-deviceconfig-ratingappstype.md)|アプリのメディアコンテンツの評価の設定。 使用可能な値: `allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。|
|messagesBlocked|Boolean|ユーザーによる監視対象デバイスでのメッセージ アプリの使用を禁止するかどうかを示します。|
|notificationsBlockSettingsModification|Boolean|通知の設定の変更を許可するかどうかを示します (iOS 9.3 以降)。|
|passcodeBlockFingerprintUnlock|Boolean|指紋によるロック解除を禁止するかどうかを示します。|
|passcodeBlockFingerprintModification|Boolean|監視モードの際の、登録済みの Touch ID の指紋認証の修正を禁止します。|
|passcodeBlockModification|Boolean|監視対象デバイスでのパスコードの変更を許可するかどうかを示します (iOS 9.0 以降)。|
|passcodeBlockSimple|Boolean|単純なパスコードを禁止するかどうかを示します。|
|passcodeExpirationDays|Int32|パスコードの有効期限が切れるまでの日数。 有効な値は 1 から 65535 までです|
|passcodeMinimumLength|Int32|パスコードの最小の長さ。 有効な値は 4 から 14 までです|
|passcodeMinutesOfInactivityBeforeLock|Int32|パスコードが要求されるまでの非アクティブ時間 (分)。|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|passcodeMinimumCharacterSetCount|Int32|パスコードが含まなければならない文字セットの数。 有効な値は 0 から 4 までです|
|passcodePreviousPasscodeBlockCount|Int32|ブロックする、以前のパスコードの数。 有効な値は 1 から 24 までです|
|passcodeSignInFailureCountBeforeWipe|Int32|デバイスをワイプするまでの、失敗が許可されるサインインの回数。 有効な値は 4 から 11 までです|
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必要なパスコードの種類。 可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。|
|passcodeRequired|Boolean|パスコードを要求するかどうかを指定します。|
|podcastsBlocked|Boolean|ユーザーによる監視対象デバイスでのポッドキャストの使用を禁止するかどうかを示します (iOS 8.0 以降)。|
|proximityBlockSetupToNewDevice|Boolean|監視対象デバイスで近くのデバイスをセットアップするためのプロンプトを有効にするかどうかを示します。|
|safariBlockAutofill|Boolean|ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。|
|safariBlockJavaScript|Boolean|Safari 内で JavaScript をブロックするかどうかを示します。|
|safariBlockPopups|Boolean|Safari 内でポップアップをブロックするかどうかを示します。|
|safariBlocked|Boolean|ユーザーによる Safari の使用を禁止するかどうかを示します。|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Safari の Cookie の設定。 可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。|
|safariManagedDomains|String collection|ここに記載されているパターンに一致する URL は管理対象と見なされます。|
|safariPasswordAutoFillDomains|String コレクション|ユーザーは、ここに記載されているパターンに一致する URL からのみ、パスワードを Safari に保存できます。 監視モードのデバイスに適用されます (iOS 9.3 以降)。|
|safariRequireFraudWarning|Boolean|Safari での不正行為の警告を必要とするかどうかを示します。|
|screenCaptureBlocked|Boolean|ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。|
|siriBlocked|Boolean|ユーザーによる Siri の使用を禁止するかどうかを示します。|
|siriBlockedWhenLocked|Boolean|ロックされている場合に、ユーザーによる Siri の使用を禁止するかどうかを示します。|
|siriBlockUserGeneratedContent|Boolean|監視対象デバイスでの使用時に、Siri による、ユーザー生成コンテンツに対するクエリの実行をブロックするかどうかを示します。|
|siriRequireProfanityFilter|Boolean|Siri が監視対象デバイスで不適切な言葉をディクテーションまたは読み上げないようにするかどうかを示します。|
|softwareUpdatesEnforcedDelayInDays|Int32|監視対象デバイスに対してソフトウェア更新プログラムが delyed される日数を設定します。 有効な値は 0 から 90 までです|
|ソフトウェアの更新 Force延期|Boolean|デバイスが監視モードのときに、ユーザーのソフトウェア更新プログラムの表示を延期するかどうかを示します。|
|spotlightBlockInternetResults|Boolean|監視対象デバイスで Spotlight 検索がインターネットでの結果を返すのをブロックするかどうかを示します。|
|voiceDialingBlocked|Boolean|音声ダイヤルをブロックするかどうかを示します。|
|wallpaperBlockModification|Boolean|監視対象デバイスでの壁紙の変更を許可するかどうかを示します (iOS 9.0 以降)。|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|デバイスが監視モードのときに、構成プロファイルからの Wi-Fi ネットワークのみを使用するようデバイスに強制するかどうかを示します。|
|classroomForceRequestPermissionToLeaveClasses|Boolean|教室経由で管理されていないコースに登録された学生が、コースを離れるときに教師にアクセス許可を要求するかどうかを示します (iOS 11.3 以降)。|
|keychainBlockCloudSync|Boolean|ICloud のキーチェーン同期がブロックされるかどうかを示します。|
|pkiBlockOTAUpdates|Boolean|空軍の PKI 更新がブロックされるかどうかを示します。 この制限を false に設定しても、CRL および OCSP チェック (iOS 7.0 以降) は無効になりません。|
|privacyForceLimitAdTracking|Boolean|Ad の追跡が制限されているかどうかを示します。(iOS 7.0 以降)。|
|enterpriseBookBlockBackup|Boolean|エンタープライズブックのバックアップがブロックされるかどうかを示します。|
|enterpriseBookBlockMetadataSync|Boolean|エンタープライズブックのメモと強調表示の同期がブロックされているかどうかを示します。|
|airPrintBlocked|Boolean|放映印刷をブロックするかどうかを示します (iOS 11.0 以降)。|
|airPrintBlockCredentialsStorage|Boolean|放映された印刷に対して、ユーザー名とパスワードのキーチェーンストレージをブロックするかどうかを示します (iOS 11.0 以降)。|
|airPrintForceTrustedTLS|Boolean|TLS 印刷通信 (iOS 11.0 以降) に対して信頼できる証明書が必要かどうかを示します。|
|airPrintBlockiBeaconDiscovery|Boolean|放映された印刷プリンターの iBeacon 検出をブロックするかどうかを示します。 これにより、ネットワークトラフィック (iOS 11.0 以降) では、フィッシングからの Bluetooth ビーコンを誤って印刷することがなくなります。|
|blockSystemAppRemoval 削除|Boolean|デバイスからのシステムアプリの削除が、監視対象デバイスでブロックされているかどうかを示します (iOS 11.0 以降)。|
|vpnBlockCreation 作成|Boolean|VPN 構成の作成がブロックされるかどうかを示します (iOS 11.0 以降)。|
|appRemovalBlocked|Boolean|アプリの削除が許可されているかどうかを示します。|
|usbRestrictedModeBlocked|Boolean|デバイスがロックされているときに USB アクセサリへの接続が許可されるかどうかを示します (iOS 11.4.1 以降)。|
|passwordBlockAutoFill フィル|Boolean|パスワードのオートフィル機能が許可されているかどうかを示します (iOS 12.0 以降)。|
|passwordBlockProximityRequests|Boolean|近くのデバイスからのパスワードの要求をブロックするかどうかを示します (iOS 12.0 以降)。|
|Passwordblockエア Drop共有|Boolean|通話ドロップパスワード機能 iOS 12.0 以降) でのパスワードの共有を禁止するかどうかを示します。|
|dateAndTimeForceSetAutomatically に|Boolean|ユーザーが日付と時刻を自動的に設定する機能が有効であるかどうか、およびユーザーが無効にすることができないかどうかを示します (iOS 12.0 以降)。|
|contactsAllowManagedToUnmanagedWrite|Boolean|管理対象アプリが、管理されていない連絡先アカウントに連絡先を書き込むことができるかどうかを示します (iOS 12.0 以降)。|
|contactsAllowUnmanagedToManagedRead|Boolean|管理対象外アプリが管理された連絡先から読み取ることができるかどうかを示します (iOS 12.0 以降)。|
|cellularBlockPersonalHotspotModification|Boolean|ユーザーが個人用ホットスポットの設定を変更することを禁止するかどうかを示します (iOS 12.2 以降)。|
|siriDisableServerLogging|Boolean|サーバー側の Siri ログが無効かどうかを示します (iOS 12.2 以降)。|



## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 9386

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "siriDisableServerLogging": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9558

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "siriDisableServerLogging": true
}
```





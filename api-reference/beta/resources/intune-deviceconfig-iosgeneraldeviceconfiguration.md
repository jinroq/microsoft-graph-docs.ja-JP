---
title: iosGeneralDeviceConfiguration リソース タイプ
description: このトピックでは、iosGeneralDeviceConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dba0349ddfe7b0e4fd71193bbea7dd35dcf0a04
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776956"
---
# <a name="iosgeneraldeviceconfiguration-resource-type"></a>iosGeneralDeviceConfiguration リソース タイプ

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このトピックでは、iosGeneralDeviceConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[iosGeneralDeviceConfigurations のリスト](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-list.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) コレクション|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-get.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-create.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|新しい [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトを作成します。|
|[Delete iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-delete.md)|なし|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) を削除します。|
|[Update iosGeneralDeviceConfiguration](../api/intune-deviceconfig-iosgeneraldeviceconfiguration-update.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md)|[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
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
|autofillforceauthentication|Boolean|Safari や、監視対象デバイスの他のアプリで、パスワードとクレジットカード情報を自動入力する前に、ユーザー認証を強制するかどうかを示します。|
|bluetoothBlockModification|Boolean|デバイスが監視モードのときに、Bluetooth の設定の変更を許可するかどうかを示します (iOS 10.0 以降)。|
|cameraBlocked|Boolean|ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。|
|cellularBlockDataRoaming|Boolean|データ ローミングをブロックするかどうかを示します。|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Boolean|ローミング中に、グローバルなバックグラウンド フェッチをブロックするかどうかを示します。|
|cellularBlockPerAppDataModification|Boolean|デバイスが監視モードのときに、携帯ネットワーク アプリのデータの使用設定の変更を許可するかどうかを示します。|
|cellularBlockPersonalHotspot|Boolean|個人用ホットスポットをブロックするかどうかを示します。|
|cellularblockplan の変更|Boolean|ユーザーが、監視対象デバイスの携帯電話プランの設定を変更することを許可するかどうかを示します。|
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
|esimblockmodification|Boolean|監視対象デバイスの eSIM での携帯電話プランの追加または削除を許可するかどうかを示します。|
|faceTimeBlocked|Boolean|ユーザーによる FaceTime の使用を禁止するかどうかを示します。|
|findMyFriendsBlocked|Boolean|デバイスが監視モードのときに、"友達を探す" をブロックするかどうかを示します。|
|gamingBlockGameCenterFriends|Boolean|ユーザーによる Game Center での友達の追加を禁止するかどうかを示します。|
|gamingBlockMultiplayer|Boolean|ユーザーによるマルチプレイヤー ゲームの使用を禁止するかどうかを示します。|
|gameCenterBlocked|Boolean|デバイスが監視モードのときに、ユーザーによる Game Center の使用を禁止するかどうかを示します。|
|hostPairingBlocked|Boolean|iOS デバイスが監視モードのときに、iOS デバイスがペアリングできるデバイスをホスト ペアリングで制御できるようにするかどうかを示します。|
|iBooksStoreBlocked|Boolean|デバイスが監視モードのときに、ユーザーによる iBooks Store の使用を禁止するかどうかを示します。|
|iBooksStoreBlockErotica|Boolean|アダルトのフラグが付いている iBookstore からのメディアのダウンロードをブロックするかどうかを示します。|
|iCloudBlockActivityContinuation|ブール型|ユーザーが ios デバイスで開始された作業を別の ios デバイスまたは macOS デバイスに継続して実行することを禁止するかどうかを示します。|
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
|kioskModeAllowAutoLock|Boolean|キオスク モード時のデバイスの自動ロックを許可するかどうかを示します。|
|kioskModeAllowColorInversionSettings|Boolean|キオスク モード時の色反転の設定へのアクセスを許可するかどうかを示します。|
|kioskModeAllowRingerSwitch|Boolean|キオスク モード時の着信音スイッチの使用を許可するかどうかを示します。|
|kioskModeAllowScreenRotation|Boolean|キオスク モード時の画面の回転を許可するかどうかを示します。|
|kioskModeAllowSleepButton|Boolean|キオスク モード時のスリープ ボタンの使用を許可するかどうかを示します。|
|kioskModeAllowTouchscreen|Boolean|キオスク モード時のタッチスクリーンの使用を許可するかどうかを示します。|
|kioskModeAllowVoiceOverSettings|Boolean|キオスク モード時のボイス オーバーの設定へのアクセスを許可するかどうかを示します。|
|kioskModeAllowVolumeButtons|Boolean|キオスク モード時のボリューム ボタンの使用を許可するかどうかを示します。|
|kioskModeBlockVolumeButtons|Boolean|キオスク モード中にボリューム ボタンをブロックするかどうかを示します。|
|kioskModeAllowZoomSettings|Boolean|キオスク モード時のズーム設定へのアクセスを許可するかどうかを示します。|
|kioskModeAppStoreUrl|文字列|キオスク モード用に使用するアプリへの、App Store 内の URL。 KioskModeManagedAppId が不明な場合に使用します。|
|kioskModeBuiltInAppId|文字列|キオスクモード用に使用する組み込みアプリの ID。 KioskModeManagedAppId および KioskModeAppStoreUrl が設定されていない場合に使用します。|
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
|mediaContentRatingApps|[ratingAppsType](../resources/intune-deviceconfig-ratingappstype.md)|アプリのメディアコンテンツの評価の設定。 可能な値は `allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17` です。|
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
|passcodeRequiredType|[requiredpasswordtype](../resources/intune-deviceconfig-requiredpasswordtype.md)|必要なパスコードの種類。 可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。|
|passcodeRequired|Boolean|パスコードを要求するかどうかを指定します。|
|podcastsBlocked|Boolean|ユーザーによる監視対象デバイスでのポッドキャストの使用を禁止するかどうかを示します (iOS 8.0 以降)。|
|proximityBlockSetupToNewDevice|Boolean|監視対象デバイスで近くのデバイスをセットアップするためのプロンプトを有効にするかどうかを示します。|
|safariBlockAutofill|Boolean|ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。|
|safariBlockJavaScript|Boolean|Safari 内で JavaScript をブロックするかどうかを示します。|
|safariBlockPopups|Boolean|Safari 内でポップアップをブロックするかどうかを示します。|
|safariBlocked|Boolean|ユーザーによる Safari の使用を禁止するかどうかを示します。|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Safari の Cookie の設定。 可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。|
|safariManagedDomains|String コレクション|ここに記載されているパターンに一致する URL は管理対象と見なされます。|
|safariPasswordAutoFillDomains|String コレクション|ユーザーは、ここに記載されているパターンに一致する URL からのみ、パスワードを Safari に保存できます。 監視モードのデバイスに適用されます (iOS 9.3 以降)。|
|safariRequireFraudWarning|Boolean|Safari での不正行為の警告を必要とするかどうかを示します。|
|screenCaptureBlocked|Boolean|ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。|
|siriBlocked|Boolean|ユーザーによる Siri の使用を禁止するかどうかを示します。|
|siriBlockedWhenLocked|Boolean|ロックされている場合に、ユーザーによる Siri の使用を禁止するかどうかを示します。|
|siriBlockUserGeneratedContent|Boolean|監視対象デバイスでの使用時に、Siri による、ユーザー生成コンテンツに対するクエリの実行をブロックするかどうかを示します。|
|siriRequireProfanityFilter|Boolean|Siri が監視対象デバイスで不適切な言葉をディクテーションまたは読み上げないようにするかどうかを示します。|
|softwareUpdatesEnforcedDelayInDays|Int32|監視対象デバイスに対してソフトウェア更新プログラムが delyed される日数を設定します。 有効な値は 0 から 90 までです|
|ソフトウェアの更新 force延期|Boolean|デバイスが監視モードのときに、ユーザーのソフトウェア更新プログラムの表示を延期するかどうかを示します。|
|spotlightBlockInternetResults|Boolean|監視対象デバイスで Spotlight 検索がインターネットでの結果を返すのをブロックするかどうかを示します。|
|voiceDialingBlocked|Boolean|音声ダイヤルをブロックするかどうかを示します。|
|wallpaperBlockModification|Boolean|監視対象デバイスでの壁紙の変更を許可するかどうかを示します (iOS 9.0 以降)。|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|デバイスが監視モードのときに、構成プロファイルからの Wi-Fi ネットワークのみを使用するようデバイスに強制するかどうかを示します。|
|classroomForceRequestPermissionToLeaveClasses|Boolean|教室経由で管理されていないコースに登録された学生が、コースを離れるときに教師にアクセス許可を要求するかどうかを示します (iOS 11.3 以降)。|
|keychainBlockCloudSync|Boolean|iCloud のキーチェーン同期がブロックされるかどうかを示します。|
|pkiBlockOTAUpdates|Boolean|空軍の PKI 更新がブロックされるかどうかを示します。 この制限を false に設定しても、CRL および OCSP チェック (iOS 7.0 以降) は無効になりません。|
|privacyforcelimitadtracking|Boolean|ad の追跡が制限されているかどうかを示します。(iOS 7.0 以降)。|
|enterprisebookblockbackup|Boolean|エンタープライズブックのバックアップがブロックされるかどうかを示します。|
|enterprisebookblockmetadatasync|Boolean|エンタープライズブックのメモと強調表示の同期がブロックされているかどうかを示します。|
|airPrintBlocked|Boolean|放映印刷をブロックするかどうかを示します (iOS 11.0 以降)。|
|airPrintBlockCredentialsStorage|Boolean|放映された印刷に対して、ユーザー名とパスワードのキーチェーンストレージをブロックするかどうかを示します (iOS 11.0 以降)。|
|airPrintForceTrustedTLS|Boolean|TLS 印刷通信 (iOS 11.0 以降) に対して信頼できる証明書が必要かどうかを示します。|
|airPrintBlockiBeaconDiscovery|Boolean|放映された印刷プリンターの ibeacon 検出をブロックするかどうかを示します。 これにより、ネットワークトラフィック (iOS 11.0 以降) では、フィッシングからの Bluetooth ビーコンを誤って印刷することがなくなります。|
|blocksystemappremoval 削除|Boolean|デバイスからのシステムアプリの削除が、監視対象デバイスでブロックされているかどうかを示します (iOS 11.0 以降)。|
|vpnblockcreation 作成|Boolean|VPN 構成の作成がブロックされるかどうかを示します (iOS 11.0 以降)。|
|appRemovalBlocked|Boolean|アプリの削除が許可されているかどうかを示します。|
|usbRestrictedModeBlocked|Boolean|デバイスがロックされているときに USB アクセサリへの接続が許可されるかどうかを示します (iOS 11.4.1 以降)。|
|passwordblockautofill フィル|Boolean|パスワードのオートフィル機能が許可されているかどうかを示します (iOS 12.0 以降)。|
|passwordBlockProximityRequests|Boolean|近くのデバイスからのパスワードの要求をブロックするかどうかを示します (iOS 12.0 以降)。|
|passwordblockエア drop共有|Boolean|通話ドロップパスワード機能 iOS 12.0 以降) でのパスワードの共有を禁止するかどうかを示します。|
|dateandtimeforcesetautomatically に|Boolean|ユーザーが日付と時刻を自動的に設定する機能が有効であるかどうか、およびユーザーが無効にすることができないかどうかを示します (iOS 12.0 以降)。|
|contactsAllowManagedToUnmanagedWrite|Boolean|管理対象アプリが、管理されていない連絡先アカウントに連絡先を書き込むことができるかどうかを示します (iOS 12.0 以降)。|
|contactsAllowUnmanagedToManagedRead|Boolean|管理対象外アプリが管理された連絡先から読み取ることができるかどうかを示します (iOS 12.0 以降)。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
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
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsVisibilityListType": "String",
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
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
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
    "String"
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
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "String",
  "kioskModeBuiltInAppId": "String",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "String",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "String",
    "tvRating": "String"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "String",
          "publisher": "String",
          "appStoreUrl": "String",
          "appId": "String"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "String",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 1024,
  "passcodeMinimumLength": 1024,
  "passcodeMinutesOfInactivityBeforeLock": 1024,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passcodeMinimumCharacterSetCount": 1024,
  "passcodePreviousPasscodeBlockCount": 1024,
  "passcodeSignInFailureCountBeforeWipe": 1024,
  "passcodeRequiredType": "String",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "String",
  "safariManagedDomains": [
    "String"
  ],
  "safariPasswordAutoFillDomains": [
    "String"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 1024,
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
  "contactsAllowUnmanagedToManagedRead": true
}
```






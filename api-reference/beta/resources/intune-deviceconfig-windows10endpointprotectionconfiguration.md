---
title: windows10EndpointProtectionConfiguration リソース タイプ
description: このトピックでは、Windows10EndpointProtectionConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f759ee9601ce8afe53c73a2bfdb92f49fec38739
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425975"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a>windows10EndpointProtectionConfiguration リソース タイプ

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このトピックでは、Windows10EndpointProtectionConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List windows10EndpointProtectionConfigurations](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-list.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) コレクション|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-get.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-create.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|新しい [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを作成します。|
|[Delete windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-delete.md)|なし|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) を削除します。|
|[Update windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-update.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|dmaGuardDeviceEnumerationPolicy|[dmaGuardDeviceEnumerationPolicyType](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|このポリシーは、外部の DMA 機能を持つデバイスに対して追加のセキュリティを提供します。 これにより外部の DMA 対応デバイスの列挙体をより細かく制御互換性のないデバイスと DMA Remapping メモリの分離レベルとサンド ボックス化できます。 このポリシーは、カーネルの DMA の保護がサポートされていて、システムのファームウェアで有効になっている場合にのみ有効です。 カーネル DMA の保護は、ポリシーを使用して、またはエンド ・ ユーザーが制御できないプラットフォーム機能です。 製造時にシステムでサポートする必要があります。 システムがカーネルの DMA の保護をサポートしているかを確認するには、MSINFO32.exe の概要] ページでカーネルの DMA 保護フィールドを確認してください。 可能な値は、`deviceDefault`、`blockAll`、`allowAll` です。|
|userRightsAccessCredentialManagerAsTrustedCaller|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利のバックアップ/リストアの実行中に資格情報マネージャーで表示されます。 他のエンティティにこの特権が与えられた場合、ユーザーの保存された資格情報が危険にさらされる可能性があります。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsAllowAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、どのユーザーを決定し、グループがネットワーク経由でコンピューターに接続できます。 許可の状態がサポートされています。|
|userRightsBlockAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、どのユーザーとグループは、ネットワーク経由でコンピューターへの接続からのブロックを決定します。 ステート ブロックがサポートされています。|
|userRightsActAsPartOfTheOperatingSystem|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利では、認証なしのすべてのユーザーを偽装するプロセスを使用できます。 プロセスをユーザーと同じローカル リソースへのアクセスを得ることができます。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、コンピューターにログオンできるユーザーを決定します。 状態 NotConfigured、許可とブロックのすべてをサポートします。 |
|userRightsBackupData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利では、回避できるユーザー ファイル、ディレクトリ、レジストリ、およびその他の永続的なオブジェクトのアクセス許可ファイルとディレクトリをバックアップするときを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsChangeSystemTime|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、どのユーザーとグループは、コンピューターの内部時計の日付と時刻を変更できますを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsCreateGlobalObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このセキュリティ設定は、ユーザーがすべてのセッションに使用可能なグローバル オブジェクトを作成できるかどうかを決定します。 グローバル オブジェクトを作成できるユーザーに影響を与える他のユーザーのセッションは、アプリケーションの障害やデータの破損につながる可能性の下で実行するプロセスです。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsCreatePageFile|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、どのユーザーおよびグループを作成し、ページファイルのサイズを変更する内部 API を呼び出すことができますを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsCreatePermanentSharedObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利では、マネージャー オブジェクトを使用してディレクトリ オブジェクトを作成するプロセスで使用できるアカウントを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsCreateSymbolicLinks|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、ユーザーが、ログオンしているコンピューターからシンボリック リンクを作成できるかどうかを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsCreateToken|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利では、プロセスでは、内部の API を使用して、アクセス トークンを作成するときに、ローカル リソースへのアクセスを取得するために使用するトークンを作成するプロセスにするユーザーまたはグループを使用することができますを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsDebugPrograms|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、ユーザーが任意のプロセスまたはカーネルにデバッガーをアタッチできるを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsRemoteDesktopServicesLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利では、リモート デスクトップ サービス クライアントとしてログオン拒否するユーザーとグループを指定します。 NotConfigured および受信拒否の状態のみがサポートされています。|
|userRightsDelegation|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、ユーザーまたはコンピューター オブジェクトの委任に対して信頼されるように設定できるユーザーを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsGenerateSecurityAudits|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利では、セキュリティ ログにエントリを追加するのにはプロセスが使用できるアカウントを決定します。 セキュリティ ログは、承認されていないシステムへのアクセスを追跡に使用します。  NotConfigured と許可の状態のみがサポートされています。|
|userRightsImpersonateClient|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|ユーザーには、このユーザー権利を割り当てるには、クライアントを偽装するには、そのユーザーに代わって実行されるプログラムすることができます。 により承認されていないユーザーが自分が作成したサービスに接続するクライアントを納得させることと、偽装して、クライアントに許可されていないユーザーのアクセス許可を昇格させるという、この種の偽装にこのユーザー権利を必要とします。管理者レベルまたはシステム レベル。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsIncreaseSchedulingPriority|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、取引先企業は他のプロセスに割り当てられている実行の優先順位を上げる別のプロセスに対するプロパティの書き込みアクセスを持つプロセスを使用することができますを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsLoadUnloadDrivers|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、ユーザーが動的にロードおよびデバイス ドライバーやカーネル モードでは、他のコードをアンロードするを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsLockMemory|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利では、ディスク上の仮想メモリを物理メモリにデータを保持するプロセスを使用できるアカウントを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsManageAuditingAndSecurityLogs|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、オブジェクト アクセスの監査ファイル、Active Directory オブジェクト、レジストリ キーなどの個々 のリソースのオプションを指定できるユーザーを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsManageVolumes|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利では、リモート最適化などのボリュームの保守タスクを実行できるユーザーおよびグループを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsModifyFirmwareEnvironment|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利では、ファームウェアの環境値を変更できるユーザーを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsModifyObjectLabels|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、ユーザー アカウントは、ファイル、レジストリ キー、またはその他のユーザーが所有するプロセスなどのオブジェクトの整合性ラベルを変更できますを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsProfileSingleProcess|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利では、システム プロセスのパフォーマンスを監視するパフォーマンス監視ツールを使用できるユーザーを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsRemoteShutdown|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利は、ネットワーク上のリモートの場所からコンピューターをシャット ダウンできるユーザーを決定します。 このユーザー権利が誤用されると、サービス拒否攻撃があります。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsRestoreData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利では、ファイル、ディレクトリ、レジストリ、およびその他の永続的なオブジェクトのファイルおよびディレクトリをバックアップ、復元するときのアクセス許可を回避できるユーザーを決定し、オブジェクトの所有者として有効なセキュリティ プリンシパルを設定できるユーザーを決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsTakeOwnership|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|所有権をユーザーのセキュリティ保護可能なオブジェクトの Active Directory オブジェクト、ファイル、フォルダー、プリンター、レジストリ キー、プロセス、およびスレッドを含め、システムでこのユーザー権利を決定します。 NotConfigured と許可の状態のみがサポートされています。|
|userRightsRegisterProcessAsService|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このセキュリティ設定は、サービスとしてプロセスを登録できないサービス アカウントを決定します。 注: このセキュリティ設定は、システム、ローカル サービス、またはネットワーク サービス アカウントには適用されません。 ブロックがサポートされているだけの状態です。|
|xboxServicesEnableXboxGameSaveTask|Boolean|この設定は、xbox ゲームの保存が有効 (1) または無効 (0) かどうかを判断します。|
|xboxServicesAccessoryManagementServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|この設定は、付属品の管理サービスの開始の種類は、Automatic(2)、Manual(3)、Disabled(4) かどうかを決定します。 既定: マニュアルです。 可能な値は、`manual`、`automatic`、`disabled` です。|
|xboxServicesLiveAuthManagerServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|この設定は、認証マネージャーの Live サービスの開始の種類は、Automatic(2)、Manual(3)、Disabled(4) かどうかを決定します。 既定: マニュアルです。 可能な値は、`manual`、`automatic`、`disabled` です。|
|xboxServicesLiveGameSaveServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|保存サービスの開始のタイプのゲームのライブは Automatic(2)、Manual(3)、Disabled(4) であるかどうかを決定します。 既定: マニュアルです。 可能な値は、`manual`、`automatic`、`disabled` です。|
|xboxServicesLiveNetworkingServiceStartupMode|[serviceStartType](../resources/intune-deviceconfig-servicestarttype.md)|この設定は、ネットワーク サービスの開始の種類は、Automatic(2)、Manual(3)、Disabled(4) かどうかを決定します。 既定: マニュアルです。 可能な値は、`manual`、`automatic`、`disabled` です。|
|localSecurityOptionsBlockMicrosoftAccounts|Boolean|ユーザーがこのコンピューターに Microsoft の新しいアカウントを追加するを防ぐ。|
|localSecurityOptionsBlockRemoteLogonWithBlankPassword|Boolean|物理デバイス以外の場所からのログオンにパスワードで保護していないローカルのアカウントを有効にします。既定値が有効になっています。|
|localSecurityOptionsDisableAdministratorAccount|Boolean|ローカル管理者アカウントを有効または無効にするかどうかを決定します。|
|localSecurityOptionsAdministratorAccountName|String|"Administrator"アカウントのセキュリティ識別子 (SID) に関連する別のアカウント名を定義します。|
|localSecurityOptionsDisableGuestAccount|Boolean|Guest アカウントが有効か無効になっているかどうかを決定します。|
|localSecurityOptionsGuestAccountName|String|"Guest"アカウントのセキュリティ識別子 (SID) に関連する別のアカウント名を定義します。|
|localSecurityOptionsAllowUndockWithoutHavingToLogon|Boolean|ポータブル コンピューターを防ぐため、ログインしなくても接続されているからです。|
|localSecurityOptionsBlockUsersInstallingPrinterDrivers|Boolean|管理者だけが使用する共有プリンターへの接続の一部としてプリンター ドライバーをインストールを制限します。|
|localSecurityOptionsBlockRemoteOpticalDriveAccess|Boolean|CD-ROM メディアにアクセスする唯一の対話形式でログオンしているユーザーは、この設定を有効にできます。|
|localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser|[localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|リムーバブル NTFS メディアを取り出すことができるユーザーを定義します。 可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。|
|localSecurityOptionsMachineInactivityLimit|Int32|対話型デスクトップのログイン画面でスクリーン セーバーの実行まで最大分続くとを定義します。 有効な値の 0 から 9999 まで|
|localSecurityOptionsMachineInactivityLimitInMinutes|Int32|対話型デスクトップのログイン画面でスクリーン セーバーの実行まで最大分続くとを定義します。 有効な値の 0 から 9999 まで|
|localSecurityOptionsDoNotRequireCtrlAltDel|Boolean|CTRL + ALT + DEL を押す前に、ユーザーがログオンできる必要があります。|
|localSecurityOptionsHideLastSignedInUser|Boolean|このデバイス上で最後署名した人のユーザー名は表示されません。|
|localSecurityOptionsHideUsernameAtSignIn|Boolean|資格情報を入力した後、デバイスのデスクトップが表示される前にこのデバイスに署名した人のユーザー名は表示されません。|
|localSecurityOptionsLogOnMessageTitle|String|ログオン ユーザーのメッセージのタイトルを設定します。|
|localSecurityOptionsLogOnMessageText|String|ログオン ユーザーのメッセージ テキストを設定します。|
|localSecurityOptionsAllowPKU2UAuthenticationRequests|Boolean|ブロック PKU2U 認証要求をこのデバイスにオンライン id を使用します。|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool|Boolean|UI ヘルパー LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager エンティティのブール値|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|String|または、SAM にリモート呼び出しを行うには、ユーザーとグループを拒否する既定のセキュリティ記述子定義言語の文字列を編集します。|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|このセキュリティ設定では、クライアントが 128 ビット暗号化、または NTLMv2 セッション セキュリティのネゴシエーションを必要とすることができます。 可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|このセキュリティ設定は、128 ビット暗号化、または NTLMv2 セッション セキュリティのネゴシエーションを必要とするサーバーです。 可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。|
|lanManagerAuthenticationLevel|[lanManagerAuthenticationLevel](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|このセキュリティ設定は、ネットワーク ログオン時に使用するチャレンジ/レスポンス認証プロトコルを決定します。 使用可能な値: `lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。|
|lanManagerWorkstationDisableInsecureGuestLogons|Boolean|有効な場合、SMB クライアントはセキュリティ保護されていないゲスト ログオンを使用できます。 構成されていない場合、SMB クライアントはセキュリティ保護されていないゲスト ログオンを拒否します。|
|localSecurityOptionsClearVirtualMemoryPageFile|Boolean|このセキュリティ設定は、システムのシャット ダウン時に仮想メモリのページファイルがオフになっているかどうかを決定します。|
|localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn|Boolean|このセキュリティ設定は、Windows にログオンしなくてもコンピューターをシャット ダウンできるかどうかを決定します。|
|localSecurityOptionsAllowUIAccessApplicationElevation|Boolean|UIAccess アプリケーションをセキュリティで保護されたデスクトップを使用せず、昇格のプロンプトを許可します。|
|localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations|Boolean|ファイルとレジストリの書き込みエラーをユーザーの場所ごとに仮想化します。|
|localSecurityOptionsOnlyElevateSignedExecutables|Boolean|実行が許可される前に、実行可能ファイルに、PKI 証明書パス検証を強制します。|
|localSecurityOptionsAdministratorElevationPromptBehavior|[localSecurityOptionsAdministratorElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|管理者承認モードでは、管理者に対する昇格時のプロンプトの動作を定義します。 可能な値は、`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries` です。|
|localSecurityOptionsStandardUserElevationPromptBehavior|[localSecurityOptionsStandardUserElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|標準ユーザーに対する昇格時のプロンプトの動作を定義します。 可能な値は、`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials` です。|
|localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation|Boolean|セキュリティで保護されたデスクトップではなく、対話ユーザーのデスクトップに移動するすべての昇格要求を有効にします。 管理者および標準ユーザーに対するプロンプトの動作ポリシー設定が使用されます。|
|localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation|Boolean|システム特権を必要とするアプリケーションのインストールは、管理者の資格情報を求められます。既定値が有効になっています。|
|localSecurityOptionsAllowUIAccessApplicationsForSecureLocations|Boolean|UIAccess アプリケーションをセキュリティで保護されたデスクトップを使用せず、昇格のプロンプトを許可します。既定値が有効になっています。|
|localSecurityOptionsUseAdminApprovalMode|Boolean|ビルトイン管理者アカウントが管理者承認モードを使用して、または完全な管理者特権を持つすべてのアプリケーションを実行するかどうかを定義します。既定値が有効になっています。|
|localSecurityOptionsUseAdminApprovalModeForAdministrators|Boolean|管理者承認モードおよびすべての UAC ポリシー設定を有効にするかどうかを定義する既定値が有効になっています。|
|localSecurityOptionsInformationShownOnLockScreen|[localSecurityOptionsInformationShownOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|セッションがロックされているときに表示されるユーザー情報を構成します。 構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。 可能な値は、`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser` です。|
|localSecurityOptionsInformationDisplayedOnLockScreen|[localSecurityOptionsInformationDisplayedOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|セッションがロックされているときに表示されるユーザー情報を構成します。 構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。 可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。|
|localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees|Boolean|このセキュリティ設定は、SMB クライアントが SMB パケット署名をネゴシエートしようとしたかどうかを決定します。|
|localSecurityOptionsClientDigitallySignCommunicationsAlways|Boolean|このセキュリティ設定は、SMB クライアント コンポーネントでパケット署名が必要かどうかを決定します。|
|localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers|Boolean|このセキュリティ設定が有効の場合、サーバー メッセージ ブロック (SMB) リダイレクターは、認証時にパスワード暗号化をサポートしない Microsoft 以外の SMB サーバーにプレーン テキスト パスワードを送信するのには。|
|localSecurityOptionsDisableServerDigitallySignCommunicationsAlways|Boolean|このセキュリティ設定は、SMB サーバー コンポーネントがパケット署名が必要かどうかを決定します。|
|localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees|Boolean|このセキュリティ設定は、SMB サーバーが SMB パケット署名を要求するクライアントをネゴシエートするかどうかを決定します。|
|localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares|Boolean|既定では、このセキュリティ設定は共有とパイプは匿名でアクセスできる名前付きパイプおよび匿名でアクセスできる共有の設定に匿名アクセスを制限します。|
|localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts|Boolean|このセキュリティ設定は、どのような追加のアクセス許可をコンピューターへの匿名接続を許可しますを指定します。|
|localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares|Boolean|このセキュリティ設定は、ドメイン アカウントやネットワーク共有の名前の列挙など、特定の操作を実行するのには匿名ユーザーを許可するかどうかを決定します。|
|localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange|Boolean|このセキュリティ設定は、かどうかは、次のパスワードの変更で新しいパスワードの LAN Manager (LM) ハッシュ値が格納されているを決定します。 既定では格納されません。|
|localSecurityOptionsSmartCardRemovalBehavior|[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|このセキュリティ設定は、ユーザーのログオン用のスマート カードがスマート カード リーダーから削除されたときの動作を決定します。 可能な値は、`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession` です。|
|defenderSecurityCenterDisableAppBrowserUI|Boolean|アプリケーションとブラウザーの保護領域の表示を無効にする場合に使用されます。|
|defenderSecurityCenterDisableFamilyUI|Boolean|ファミリのオプション領域の表示を無効にするために使用します。|
|defenderSecurityCenterDisableHealthUI|Boolean|デバイスのパフォーマンスと稼働状態の領域の表示を無効にするために使用します。|
|defenderSecurityCenterDisableNetworkUI|Boolean|ファイアウォールとネットワークの保護領域の表示を無効にする場合に使用されます。|
|defenderSecurityCenterDisableVirusUI|Boolean|ウイルスと脅威の保護領域の表示を無効にする場合に使用されます。|
|defenderSecurityCenterDisableAccountUI|Boolean|アカウントの保護領域の表示を無効にする場合に使用されます。|
|defenderSecurityCenterDisableHardwareUI|Boolean|ハードウェアの保護領域の表示を無効にする場合に使用されます。|
|defenderSecurityCenterDisableRansomwareUI|Boolean|Ransomware 保護領域の表示を無効にする場合に使用されます。 |
|defenderSecurityCenterDisableSecureBootUI|Boolean|[デバイスのセキュリティ、セキュリティで保護されたブート領域の表示を無効にする場合に使用されます。|
|defenderSecurityCenterDisableTroubleshootingUI|Boolean|[デバイスのセキュリティのトラブルシューティング、セキュリティ プロセスの表示を無効にする場合に使用されます。|
|defenderSecurityCenterOrganizationDisplayName|String|ユーザーに表示される会社名です。|
|defenderSecurityCenterHelpEmail|String|ユーザーに表示される電子メール アドレスです。|
|defenderSecurityCenterHelpPhone|String|電話番号または Skype ID のユーザーに表示されます。|
|defenderSecurityCenterHelpURL|String|ヘルプ ポータルの URL をユーザーに表示されます。|
|defenderSecurityCenterNotificationsFromApp|[defenderSecurityCenterNotificationsFromAppType](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|アプリケーションの表示領域を表示するのに通知します。 可能な値は、`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications` です。|
|defenderSecurityCenterITContactDisplay|[defenderSecurityCenterITContactDisplayType](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|IT の連絡先を表示する場所を構成するエンド ・ ユーザーへの情報です。 可能な値は、`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications` です。|
|firewallBlockStatefulFTP|Boolean|デバイスへのステートフル FTP 接続をブロックします|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。 これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。 有効な値は 300 から 3600 までです|
|firewallPreSharedKeyEncodingMethod|[firewallPreSharedKeyEncodingMethodType](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|事前共有キーを使用するエンコーディングを選択します。 可能な値は、`deviceDefault`、`none`、`utF8` です。|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolean|IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します|
|firewallIPSecExemptionsAllowICMP|Boolean|IPSec 除外を構成し、ICMP を許可します|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolean|IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します|
|firewallIPSecExemptionsAllowDHCP|Boolean|IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します|
|firewallCertificateRevocationListCheckMethod|[firewallCertificateRevocationListCheckMethodType](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|証明書失効リストを適用する方法を指定します。 可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。|
|firewallMergeKeyingModuleSettings|Boolean|認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|トンネルのゲートウェイでパケットのキューイングを適用する方法を構成します。 可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します|
|defenderAttackSurfaceReductionExcludedPaths|String コレクション|攻撃回避規則から除外する exe ファイルとフォルダーのリスト|
|defenderOfficeAppsOtherProcessInjectionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|他のプロセス内に挿入する Office アプリケーションの動作を示す値です。 可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderOfficeAppsOtherProcessInjection|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|他のプロセス内に挿入する Office アプリケーションの動作を示す値です。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderOfficeAppsExecutableContentCreationOrLaunchType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Office アプリケーションとマクロを作成または実行可能なコンテンツを起動する動作を示す値です。 可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderOfficeAppsExecutableContentCreationOrLaunch|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Office アプリケーションとマクロを作成または実行可能なコンテンツを起動する動作を示す値です。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderOfficeAppsLaunchChildProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|子プロセスを起動する Office アプリケーションの動作を示す値です。 可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderOfficeAppsLaunchChildProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|子プロセスを起動する Office アプリケーションの動作を示す値です。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderOfficeMacroCodeAllowWin32ImportsType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Win32 の動作は、Office でマクロ コードからインポートするかを示す値です。 可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderOfficeMacroCodeAllowWin32Imports|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Win32 の動作は、Office でマクロ コードからインポートするかを示す値です。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderScriptObfuscatedMacroCodeType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Js、vbs、ps/マクロの難読化されたコードの動作を示す値です。 可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderScriptObfuscatedMacroCode|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Js、vbs、ps/マクロの難読化されたコードの動作を示す値です。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderScriptDownloadedPayloadExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Js と vbs のペイロードの実行の動作を示す値は、インターネットからダウンロードします。 可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderScriptDownloadedPayloadExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Js と vbs のペイロードの実行の動作を示す値は、インターネットからダウンロードします。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderPreventCredentialStealingType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|資格情報が Windows のローカル セキュリティ機関サブシステムから盗むことが許可されているかどうかを示す値です。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderProcessCreationType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|PSExec と WMI のコマンドから生成されるプロセスを作成することを示す応答を値です。 可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderProcessCreation|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|PSExec と WMI のコマンドから生成されるプロセスを作成することを示す応答を値です。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderUntrustedUSBProcessType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|USB から実行している信頼されていない、署名のないプロセスへの応答を示す値です。 可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderUntrustedUSBProcess|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|USB から実行している信頼されていない、署名のないプロセスへの応答を示す値です。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderUntrustedExecutableType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|蔓延状況、年齢、または信頼される側のリストに一致しない実行可能ファイルへの応答を示す基準です。 可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderUntrustedExecutable|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|蔓延状況、年齢、または信頼される側のリストに一致しない実行可能ファイルへの応答を示す基準です。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderEmailContentExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|メール (web メール/メール ・ クライアント) から (exe、dll、ps、js、vbs など) の実行可能なコンテンツの実行を削除する必要があるかどうかを示す値です。 可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderEmailContentExecution|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|メール (web メール/メール ・ クライアント) から (exe、dll、ps、js、vbs など) の実行可能なコンテンツの実行を削除する必要があるかどうかを示す値です。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderAdvancedRansomewareProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Ransomeware に対して高度な保護の使用を示す値です。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderGuardMyFoldersType|[folderProtectionType](../resources/intune-deviceconfig-folderprotectiontype.md)|保護されたフォルダーの動作を示す値です。 可能な値は、`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification` です。|
|defenderGuardedFoldersAllowedAppPaths|String コレクション|保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト|
|defenderAdditionalGuardedFolders|String コレクション|保護されたフォルダーのリストに追加されるフォルダー パスのリスト|
|defenderNetworkProtectionType|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|NetworkProtection の動作を示す値です。 可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderExploitProtectionXml|Binary|Exploit Protection の詳細に関する情報を含む XML コンテンツ。|
|defenderExploitProtectionXmlFileName|String|DefenderExploitProtectionXml の取得元となるファイルの名前。|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|管理者がデバイスで許可するアプリの種類を選択できるようにします。 可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。|
|deviceGuardLocalSystemAuthorityCredentialGuardSettings|[deviceGuardLocalSystemAuthorityCredentialGuardType](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|プラットフォームのセキュリティ レベルとセキュリティで保護されたブートし、仮想化ベースのセキュリティの両方が有効である場合は、資格情報の保護にします。 可能な値は、`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock` です。|
|deviceGuardEnableVirtualizationBasedSecurity|Boolean|Security(VBS) を仮想化をオンに基づいています。|
|deviceGuardEnableSecureBootWithDMA|Boolean|プラットフォームのセキュリティ レベルが次の再起動時に有効になっているかどうかを指定します。|
|deviceGuardLaunchSystemGuard|[有効化](../resources/intune-shared-enablement
.md)|ガードのシステムの起動を構成するのには IT 管理者を使用できます。 可能な値は、`notConfigured`、`enabled`、`disabled` です。|
|smartScreenEnableInShell|Boolean|IT 管理者が Windows 用の SmartScreen を構成することを許可します。|
|smartScreenBlockOverrideForFiles|Boolean|ユーザーが SmartScreen 警告を無視し、悪意のあるファイルを実行できるかどうかを IT 管理者が制御することを許可します。|
|applicationGuardEnabled|Boolean|Windows Defender Application Guard を有効にします|
|applicationGuardEnabledOptions|[applicationGuardEnabledOptions](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|新しい Windows のビルドの Windows Defender のアプリケーション保護を有効にします。 可能な値は、`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice` です。|
|applicationGuardBlockFileTransfer|[applicationGuardBlockFileTransferType](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|イメージ ファイルの転送、テキスト ファイルのいずれかにクリップボードをブロックします。 可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。|
|applicationGuardBlockNonEnterpriseContent|Boolean|サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします|
|applicationGuardAllowPersistence|Boolean|App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します|
|applicationGuardForceAuditing|Boolean|監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます|
|applicationGuardBlockClipboardSharing|[applicationGuardBlockClipboardSharingType](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。 可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。|
|applicationGuardAllowPrintToPDF|Boolean|コンテナーから PDF への出力を許可します|
|applicationGuardAllowPrintToXPS|Boolean|コンテナーから XPS への出力を許可します|
|applicationGuardAllowPrintToLocalPrinters|Boolean|コンテナーからローカル プリンターへの出力を許可します|
|applicationGuardAllowPrintToNetworkPrinters|Boolean|コンテナーからネットワーク プリンターへの出力を許可します|
|applicationGuardAllowVirtualGPU|Boolean|仮想 GPU を使用するアプリケーションの保護を許可します。|
|applicationGuardAllowFileSaveOnHost|Boolean|アプリケーション ガード コンテナーの端からファイルをダウンロードし、ホスト上でファイル システムを保存するユーザーを許可します。|
|bitLockerAllowStandardUserEncryption|Boolean|Azure AD に参加中に encrpytion を有効にする標準のユーザーに許可するのには管理者を使用できます。|
|bitLockerDisableWarningForOtherDiskEncryption|Boolean|管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|管理者が BitLocker を使用して暗号化をオンにすることを許可します。 このポリシーは、モバイルの SKU に対してのみ有効です。
|
|bitLockerEncryptDevice|Boolean|管理者が BitLocker を使用して暗号化をオンにすることを許可します。|
|bitLockerSystemDrivePolicy|[bitLockerSystemDrivePolicy](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|BitLocker のシステム ドライブのポリシーです。|
|bitLockerFixedDrivePolicy|[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|BitLocker は、ドライブのポリシーを修正します。|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|BitLocker リムーバブル ドライブ ポリシー。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
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
  "dmaGuardDeviceEnumerationPolicy": "String",
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "String",
  "xboxServicesLiveAuthManagerServiceStartupMode": "String",
  "xboxServicesLiveGameSaveServiceStartupMode": "String",
  "xboxServicesLiveNetworkingServiceStartupMode": "String",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "String",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "String",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "String",
  "localSecurityOptionsMachineInactivityLimit": 1024,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 1024,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "String",
  "localSecurityOptionsLogOnMessageText": "String",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "String",
  "lanManagerAuthenticationLevel": "String",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "String",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "String",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "String",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "String",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "String",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "String",
  "defenderSecurityCenterHelpEmail": "String",
  "defenderSecurityCenterHelpPhone": "String",
  "defenderSecurityCenterHelpURL": "String",
  "defenderSecurityCenterNotificationsFromApp": "String",
  "defenderSecurityCenterITContactDisplay": "String",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "String",
  "defenderOfficeAppsOtherProcessInjection": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "String",
  "defenderOfficeAppsLaunchChildProcessType": "String",
  "defenderOfficeAppsLaunchChildProcess": "String",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "String",
  "defenderOfficeMacroCodeAllowWin32Imports": "String",
  "defenderScriptObfuscatedMacroCodeType": "String",
  "defenderScriptObfuscatedMacroCode": "String",
  "defenderScriptDownloadedPayloadExecutionType": "String",
  "defenderScriptDownloadedPayloadExecution": "String",
  "defenderPreventCredentialStealingType": "String",
  "defenderProcessCreationType": "String",
  "defenderProcessCreation": "String",
  "defenderUntrustedUSBProcessType": "String",
  "defenderUntrustedUSBProcess": "String",
  "defenderUntrustedExecutableType": "String",
  "defenderUntrustedExecutable": "String",
  "defenderEmailContentExecutionType": "String",
  "defenderEmailContentExecution": "String",
  "defenderAdvancedRansomewareProtectionType": "String",
  "defenderGuardMyFoldersType": "String",
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderNetworkProtectionType": "String",
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "String",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardLaunchSystemGuard": "String",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "String",
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "String",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "String",
    "startupAuthenticationTpmPinUsage": "String",
    "startupAuthenticationTpmKeyUsage": "String",
    "startupAuthenticationTpmPinAndKeyUsage": "String",
    "minimumPinLength": 1024,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "String",
    "prebootRecoveryUrl": "String"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```





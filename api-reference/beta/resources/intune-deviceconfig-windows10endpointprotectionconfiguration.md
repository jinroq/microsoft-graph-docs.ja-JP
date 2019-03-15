---
title: windows10EndpointProtectionConfiguration リソース タイプ
description: このトピックでは、Windows10EndpointProtectionConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4f034a6b35c1ae8bd8172a20c5da0ee2e818623
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571705"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a>windows10EndpointProtectionConfiguration リソース タイプ

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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
|id|文字列型 (String)|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|description|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|dmaGuardDeviceEnumerationPolicy|[dmaGuardDeviceEnumerationPolicyType](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|このポリシーは、外部 DMA 対応デバイスに対して追加のセキュリティを提供することを目的としています。 これにより、dma リマップ/デバイスメモリの分離とサンドボックスと互換性のない外部 DMA 対応デバイスの列挙を制御することができます。 このポリシーは、カーネル DMA 保護がサポートされていて、システムファームウェアによって有効になっている場合にのみ有効になります。 カーネル DMA 保護は、ポリシーまたはエンドユーザーによって制御できないプラットフォーム機能です。 これは、製造時にシステムによってサポートされる必要があります。 システムがカーネル dma 保護をサポートしているかどうかを確認するには、MSINFO32 の要約ページにある「kernel dma 保護」フィールドを確認してください。 使用可能な値は、`deviceDefault`、`blockAll`、`allowAll` です。|
|firewallRules|[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)コレクション|ファイアウォール規則の設定を構成します。 このコレクションには、最大150個の要素を含めることができます。|
|userRightsAccessCredentialManagerAsTrustedCaller|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、バックアップ/復元中に Credential Manager によって使用されます。 この特権が他のエンティティに付与されている場合、ユーザーの保存された資格情報が侵害される可能性があります。 NotConfigured および許可されている状態のみがサポートされる|
|userRightsAllowAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、ネットワーク経由でコンピューターに接続できるユーザーとグループを決定します。 State Allowed がサポートされています。|
|userRightsBlockAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、ネットワーク経由でコンピューターへの接続をブロックするユーザーとグループを決定します。 ステートブロックがサポートされています。|
|userRightsActAsPartOfTheOperatingSystem|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利により、プロセスは認証なしで任意のユーザーになりすますことができます。 そのため、このプロセスは、そのユーザーと同じローカルリソースにアクセスできるようになります。 NotConfigured および許可されている状態のみがサポートされる|
|userRightsLocalLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、コンピューターにログオンできるユーザーを決定します。 NotConfigured、許可およびブロックされる状態のすべてがサポートされています。 |
|userRightsBackupData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、ファイルやディレクトリをバックアップするときに、ファイル、ディレクトリ、レジストリ、およびその他の固定オブジェクトのアクセス許可をバイパスできるユーザーを決定します。 NotConfigured および許可されている状態のみがサポートされる|
|userRightsChangeSystemTime|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、コンピューターの内部時計の日時を変更できるユーザーとグループを決定します。 NotConfigured および許可されている状態のみがサポートされる|
|userRightsCreateGlobalObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このセキュリティ設定は、ユーザーがすべてのセッションで使用できるグローバルオブジェクトを作成できるかどうかを決定します。 グローバルオブジェクトを作成できるユーザーは、他のユーザーのセッションで実行されるプロセスに影響を与える可能性があります。これにより、アプリケーション障害またはデータ破損が発生する可能性があります。 NotConfigured および許可されている状態のみがサポートされる|
|userRightsCreatePageFile|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、内部 API を呼び出してページファイルのサイズを作成および変更できるユーザーとグループを決定します。 NotConfigured および許可されている状態のみがサポートされる|
|userRightsCreatePermanentSharedObjects|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、オブジェクトマネージャーを使用してディレクトリオブジェクトを作成するために、プロセスで使用できるアカウントを決定します。 NotConfigured および許可されている状態のみがサポートされる|
|userRightsCreateSymbolicLinks|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、ユーザーがログオンしているコンピューターからシンボリックリンクを作成できるかどうかを決定します。 NotConfigured および許可されている状態のみがサポートされる|
|userRightsCreateToken|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、プロセスが内部 API を使用してアクセストークンを作成するときにローカルリソースへのアクセスを取得するために使用できるトークンを作成するために、プロセスで使用できるユーザーまたはグループを決定します。 NotConfigured および許可されている状態のみがサポートされる|
|userRightsDebugPrograms|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、任意のプロセスまたはカーネルにデバッガーをアタッチできるユーザーを決定します。 NotConfigured および許可されている状態のみがサポートされる|
|userRightsRemoteDesktopServicesLogOn|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、リモートデスクトップサービスクライアントとしてのログオンを禁止するユーザーとグループを決定します。 NotConfigured とブロックのみがサポートされています。|
|userRightsDelegation|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、ユーザーまたはコンピューターオブジェクトで委任に対して信頼されている設定を設定できるユーザーを決定します。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsGenerateSecurityAudits|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、プロセスがセキュリティログにエントリを追加するために使用できるアカウントを決定します。 セキュリティログは、承認されていないシステムアクセスを追跡するために使用されます。  サポートされているのは、NotConfigured と許可の状態のみです。|
|user/シムの個人ユーザー|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザー権利をユーザーに割り当てると、そのユーザーの代わりに実行しているプログラムがクライアントを偽装できるようになります。 この種の偽装に対してこのユーザー権限を要求することで、権限のないユーザーが作成したサービスに接続して、そのクライアントを偽装して、権限のないユーザーのアクセス許可を昇格させることができるようになります。管理レベルまたはシステムレベル。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsIncreaseSchedulingPriority|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、他のプロセスに割り当てられている実行の優先度を上げるために、プロパティの書き込みアクセス権を持つプロセスを使用できるアカウントを決定します。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsLoadUnloadDrivers|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、デバイスドライバーまたはその他のコードをカーネルモードに動的にロードおよびアンロードできるユーザーを決定します。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsLockMemory|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、プロセスを使用してデータを物理メモリに保持できるアカウントを決定します。これにより、システムはデータをディスク上の仮想メモリにページングすることができなくなります。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsManageAuditingAndSecurityLogs|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、ファイル、Active Directory オブジェクト、レジストリキーなど、個々のリソースに対してオブジェクトアクセスの監査オプションを指定できるユーザーを決定します。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsManageVolumes|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、リモートの最適化など、ボリューム上で保守タスクを実行できるユーザーとグループを決定します。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsModifyFirmwareEnvironment|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、ファームウェア環境の値を変更できるユーザーを決定します。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsModifyObjectLabels|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、ファイル、レジストリキー、他のユーザーが所有するプロセスなど、オブジェクトの整合性ラベルを変更できるユーザーアカウントを決定します。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsProfileSingleProcess|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、パフォーマンス監視ツールを使用してシステムプロセスのパフォーマンスを監視できるユーザーを決定します。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsRemoteShutdown|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、ネットワーク上のリモートの場所からコンピューターをシャットダウンできるユーザーを決定します。 このユーザーの権利を誤用すると、サービス拒否が発生する可能性があります。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsRestoreData|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、バックアップされたファイルとディレクトリを復元するときに、ファイル、ディレクトリ、レジストリ、およびその他の固定オブジェクトのアクセス許可をバイパスできるユーザーを決定し、任意のユーザーが任意の有効なセキュリティプリンシパルをオブジェクトの所有者として設定できるようにします。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsTakeOwnership|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このユーザーの権利は、Active Directory オブジェクト、ファイルとフォルダー、プリンター、レジストリキー、プロセス、スレッドなど、システム内のセキュリティ保護可能なオブジェクトの所有権を取得できるユーザーを決定します。 サポートされているのは、NotConfigured と許可の状態のみです。|
|userRightsRegisterProcessAsService|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|このセキュリティ設定は、サービスとしてのプロセスの登録を禁止するサービスアカウントを決定します。 注: このセキュリティ設定は、システム、ローカルサービス、またはネットワークサービスアカウントには適用されません。 サポートされている状態はブロックされます。|
|xboxServicesEnableXboxGameSaveTask|Boolean|この設定では、xbox ゲームの保存を有効にするか (1)、無効にするか (0) を指定します。|
|xboxServicesAccessoryManagementServiceStartupMode|[servicestarttype](../resources/intune-deviceconfig-servicestarttype.md)|この設定では、アクセサリ管理サービスの開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。 既定値: Manual。 使用可能な値は、`manual`、`automatic`、`disabled` です。|
|xboxServicesLiveAuthManagerServiceStartupMode|[servicestarttype](../resources/intune-deviceconfig-servicestarttype.md)|この設定では、Live Auth Manager サービスの開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。 既定値: Manual。 使用可能な値は、`manual`、`automatic`、`disabled` です。|
|xboxServicesLiveGameSaveServiceStartupMode|[servicestarttype](../resources/intune-deviceconfig-servicestarttype.md)|この設定では、Live Game save service の開始の種類が自動 (2)、手動 (3)、無効 (4) であるかどうかを決定します。 既定値: Manual。 使用可能な値は、`manual`、`automatic`、`disabled` です。|
|xboxServicesLiveNetworkingServiceStartupMode|[servicestarttype](../resources/intune-deviceconfig-servicestarttype.md)|この設定では、ネットワークサービスの開始の種類を自動 (2)、手動 (3)、無効 (4) のいずれにするかを指定します。 既定値: Manual。 使用可能な値は、`manual`、`automatic`、`disabled` です。|
|localsecurityoptionsenableadministratoraccount|Boolean|ユーザーがこのコンピューターに新しい Microsoft アカウントを追加できないようにします。|
|localsecurityoptionsblockremotelogonwithpassword|Boolean|パスワードで保護されていないローカルアカウントで、物理デバイス以外の場所からログオンできるようにします。既定値を有効にする|
|localsecurityoptionsdisableアドミニストレーターアカウント|Boolean|ローカル管理者アカウントを有効にするか無効にするかを指定します。|
|localsecurityoptionsadministratoraccountname|String|アカウント "Administrator" のセキュリティ識別子 (SID) に関連付けられる別のアカウント名を定義します。|
|localsecurityoptionsdisableguestaccount|Boolean|ゲストアカウントを有効にするか無効にするかを指定します。|
|localsecurityoptionsguestaccountname|String|アカウント "Guest" のセキュリティ識別子 (SID) に関連付けられる別のアカウント名を定義します。|
|localSecurityOptionsAllowUndockWithoutHavingToLogon|Boolean|ログインせずに、ポータブルコンピューターをアンドックできないようにします。|
|localsecurityoptionsblockユーザーのドライバー|Boolean|共有プリンターへの接続の一部として、プリンタードライバーのインストールを管理者のみに制限します。|
|localsecurityoptionsblockremoteop' aldrive access|Boolean|この設定を有効にすると、対話的にログオンしたユーザーのみが、cd-rom メディアにアクセスできます。|
|localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser|[localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|リムーバブル NTFS メディアの書式設定と取り出しが許可されているユーザーを定義します。 可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。|
|localsecurityoptionsmachineinactivitylimit|Int32|スクリーンセーバーが実行されるまで、対話デスクトップのログイン画面で非アクティブな最大時間 (分) を定義します。 有効な値は 0 ~ 9999|
|localsecurityoptionsallowremotecallstosecurityaccountsmanagerhelperbool|Int32|スクリーンセーバーが実行されるまで、対話デスクトップのログイン画面で非アクティブな最大時間 (分) を定義します。 有効な値は 0 ~ 9999|
|localSecurityOptionsDoNotRequireCtrlAltDel|Boolean|ユーザーがログオンできるようにするには、CTRL + ALT + DEL キーを押しておく必要があります。|
|localsecurityoption佐々木 delastsignedinuser|Boolean|このデバイスに最後にサインインしたユーザーのユーザー名を表示しません。|
|localSecurityOptionsHideUsernameAtSignIn|Boolean|資格情報を入力した後、デバイスのデスクトップが表示される前に、このデバイスにサインインしているユーザーのユーザー名を表示しません。|
|localsecurityoptionslogonmessagetitle|String|ログインを試行するユーザーのメッセージのタイトルを設定します。|
|localsecurityoptionslogonmessagetext|String|ログインを試行するユーザーのメッセージテキストを設定します。|
|localSecurityOptionsAllowPKU2UAuthenticationRequests|Boolean|オンライン id を使用するために、このデバイスへの PKU2U 認証要求をブロックします。|
|localsecurityoptionsinformationshownonlockscreen|Boolean|LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager エンティティの UI ヘルパーの boolean|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|String|既定のセキュリティ記述子定義言語文字列を編集して、ユーザーおよびグループに SAM へのリモート呼び出しを許可または拒否します。|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|このセキュリティ設定を使用すると、クライアントは128ビット暗号化と NTLMv2 セッションセキュリティのいずれかまたは両方のネゴシエーションを要求できます。 可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|このセキュリティ設定を使用すると、サーバーで128ビット暗号化と NTLMv2 セッションセキュリティのどちらかまたは両方のネゴシエーションが要求されます。 可能な値は、`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption` です。|
|lanManagerAuthenticationLevel|[lanManagerAuthenticationLevel](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|このセキュリティ設定は、ネットワークログオンに使用するチャレンジ/応答認証プロトコルを決定します。 可能な値は `lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm` です。|
|lanmanagerwork ステーション disableinsecureguestログオン|Boolean|有効にした場合、SMB クライアントは安全でないゲストログオンを許可します。 構成されていない場合、SMB クライアントは安全でないゲストログオンを拒否します。|
|localSecurityOptionsClearVirtualMemoryPageFile|Boolean|このセキュリティ設定は、システムのシャットダウン時に仮想メモリのページファイルをクリアするかどうかを決定します。|
|localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn|Boolean|このセキュリティ設定は、Windows にログオンせずに、コンピューターをシャットダウンできるかどうかを決定します。|
|localsecurityoptionsallowuiaccessapplicationelevation|Boolean|セキュリティで保護されたデスクトップを使用せずに、UIAccess アプリで昇格を確認できるようにします。|
|localsecurityoptionsvirtualizefileandregistrywritefailurestoperuserlocations|Boolean|ユーザーごとの場所に対するファイルおよびレジストリの書き込みエラーを仮想化する|
|localSecurityOptionsOnlyElevateSignedExecutables|Boolean|指定した実行可能ファイルに対して、実行が許可される前に、PKI 証明書パス検証を強制します。|
|localSecurityOptionsAdministratorElevationPromptBehavior|[localSecurityOptionsAdministratorElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|管理者承認モードでの管理者の昇格時のプロンプトの動作を定義します。 可能な値は、`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries` です。|
|localSecurityOptionsStandardUserElevationPromptBehavior|[localSecurityOptionsStandardUserElevationPromptBehaviorType](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|標準ユーザーの昇格時のプロンプトの動作を定義します。 可能な値は、`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials` です。|
|localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation|Boolean|セキュリティで保護されたデスクトップではなく、対話ユーザーのデスクトップにアクセスするすべての昇格要求を有効にします。 管理者および標準ユーザーのプロンプト動作ポリシー設定が使用されます。|
|localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation|Boolean|昇格した権限が必要なアプリのインストールでは、管理者の資格情報の入力を求められます既定値を有効にする|
|localsecurityoptionsallowuiaccessapplicationsforsecurelocations|Boolean|セキュリティで保護されたデスクトップを使用せずに、UIAccess アプリで昇格を確認できるようにします。既定値を有効にする|
|localsecurityoptionsuseadminapprovalmode|Boolean|組み込みの管理者アカウントが管理者承認モードを使用するか、完全な管理者特権を持つすべてのアプリを実行するかを定義します。既定値を有効にする|
|localsecurityoptionsuseadminapprovalmodeforadministrators|Boolean|管理者承認モードとすべての UAC ポリシー設定を有効にするかどうかを定義し、既定値を有効にする|
|localsecurityoptionsinformationshownonlockscreen ロックアウト|[localSecurityOptionsInformationShownOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|セッションがロックされているときに表示されるユーザー情報を構成します。 構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。 可能な値は、`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser` です。|
|localSecurityOptionsInformationDisplayedOnLockScreen|[localSecurityOptionsInformationDisplayedOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|セッションがロックされているときに表示されるユーザー情報を構成します。 構成されていない場合は、ユーザーの表示名、ドメインおよびユーザー名が表示されます。 可能な値は、`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers` です。|
|localsecurityoptionsclientsendunencryptedpasswordtothirdpartysmbservers|Boolean|このセキュリティ設定は、smb クライアントが smb パケット署名のネゴシエートを試行するかどうかを決定します。|
|localSecurityOptionsClientDigitallySignCommunicationsAlways|Boolean|このセキュリティ設定は、SMB クライアントコンポーネントがパケット署名を必要とするかどうかを決定します。|
|localsecurityoptionsdisableserverdigitallysigncommunicationsalways|Boolean|このセキュリティ設定が有効になっている場合、サーバーメッセージブロック (SMB) リダイレクターは、認証時にパスワード暗号化をサポートしていない Microsoft 以外の SMB サーバーにプレーンテキストのパスワードを送信することを許可されます。|
|localSecurityOptionsDisableServerDigitallySignCommunicationsAlways|Boolean|このセキュリティ設定は、SMB サーバーコンポーネントがパケット署名を必要とするかどうかを決定します。|
|localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees|Boolean|このセキュリティ設定は、smb サーバーが smb パケットの署名を要求するクライアントとの間で smb パケットの署名をネゴシエートするかどうかを決定します。|
|localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares|Boolean|既定では、このセキュリティ設定では、匿名アクセス可能な名前付きパイプと、匿名でアクセスできる共有の設定に対して、共有とパイプへの匿名アクセスが制限されます。|
|localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts|Boolean|このセキュリティ設定は、コンピューターへの匿名接続に付与される追加のアクセス許可を決定します。|
|localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares|Boolean|このセキュリティ設定は、匿名ユーザーが特定の操作 (ドメインアカウントやネットワーク共有の名前の列挙など) を実行できるようにするかどうかを決定します。|
|localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange|Boolean|このセキュリティ設定は、次のパスワード変更時に新しいパスワードの LAN Manager (LM) ハッシュ値が保存されるかどうかを決定します。 既定では保存されません。|
|localSecurityOptionsSmartCardRemovalBehavior|[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|このセキュリティ設定は、ログオンしているユーザーのスマートカードがスマートカード読み取り装置から削除されたときの動作を決定します。 可能な値は、`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession` です。|
|defendersecuritycenterdisablehealthui|Boolean|アプリとブラウザーの保護領域の表示を無効にするために使用されます。|
|defendersecuritycenterdisablenetworkui|Boolean|[ファミリオプション] 領域の表示を無効にするために使用します。|
|defenderSecurityCenterDisableHealthUI|Boolean|[デバイスのパフォーマンスと正常性] 領域の表示を無効にするために使用されます。|
|defenderSecurityCenterDisableNetworkUI|Boolean|ファイアウォールとネットワーク保護領域の表示を無効にするために使用されます。|
|defenderSecurityCenterDisableVirusUI|Boolean|ウイルスおよび脅威保護領域の表示を無効にするために使用されます。|
|defenderSecurityCenterDisableAccountUI|Boolean|[アカウントの保護] 領域の表示を無効にするために使用します。|
|defenderSecurityCenterDisableClearTpmUI|Boolean|[TPM のクリア] ボタンの表示を無効にするために使用されます。|
|defendersecurityセンター disableハードウェア ui|Boolean|[ハードウェア保護] 領域の表示を無効にするために使用されます。|
|defenderSecurityCenterDisableNotificationAreaUI|Boolean|通知領域コントロールの表示を無効にするために使用されます。 この設定を有効にするには、ユーザーはサインアウトしてからサインインするか、コンピューターを再起動する必要があります。|
|defenderSecurityCenterDisableRansomwareUI|Boolean|ランサムウェア対策領域の表示を無効にするために使用されます。 |
|defenderSecurityCenterDisableSecureBootUI|Boolean|デバイスセキュリティの下でのセキュアブート領域の表示を無効にするために使用されます。|
|defendersecurityセンター disableトラブルシューティング ui|Boolean|[デバイスのセキュリティ] の下にあるセキュリティプロセスのトラブルシューティングの表示を無効にするために使用されます。|
|defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI|Boolean|脆弱なファームウェアが検出された場合に、更新プログラムの TPM ファームウェアの表示を無効にするために使用されます。|
|defendersecurityセンター組織 displayname|String|ユーザーに表示される会社名。|
|defendersecurityセンター helpemail|String|ユーザーに表示される電子メールアドレス。|
|defendersecurityセンター helpphone|String|ユーザーに表示される電話番号または Skype ID。|
|defenderSecurityCenterHelpURL|String|ヘルプポータルの URL これは、ユーザーに表示されます。|
|defenderSecurityCenterNotificationsFromApp|[defenderSecurityCenterNotificationsFromAppType](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|アプリの表示領域から表示する通知。 使用可能な値は、`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications` です。|
|defendersecurityセンター itcontactdisplay|[defendersecurityセンター itcontactdisplaytype](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|エンドユーザーに対して IT の連絡先情報を表示する場所を構成します。 可能な値は、`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications` です。|
|firewallBlockStatefulFTP|Boolean|デバイスへのステートフル FTP 接続をブロックします|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。 これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。 有効な値は 300 から 3600 までです|
|firewallPreSharedKeyEncodingMethod|[firewallPreSharedKeyEncodingMethodType](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|使用する事前共有キーのエンコードを選択します。 使用可能な値は、`deviceDefault`、`none`、`utF8` です。|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolean|IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します|
|firewallIPSecExemptionsAllowICMP|Boolean|IPSec 除外を構成し、ICMP を許可します|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolean|IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します|
|firewallIPSecExemptionsAllowDHCP|Boolean|IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します|
|firewallCertificateRevocationListCheckMethod|[firewallCertificateRevocationListCheckMethodType](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|証明書失効リストの適用方法を指定します。 可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。|
|firewallMergeKeyingModuleSettings|Boolean|認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|トンネルゲートウェイのシナリオでパケットキューを適用する方法を構成します。 可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します|
|defenderAdobeReaderLaunchChildProcess|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|子プロセスの作成による Adobe Reader の動作を示す値。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderAttackSurfaceReductionExcludedPaths|String コレクション|攻撃回避規則から除外する exe ファイルとフォルダーのリスト|
|defenderOfficeAppsOtherProcessInjectionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|他のプロセスに挿入される Office アプリケーションの動作を示す値。 使用可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderofficeappsexecutablecontentcreationorlaunch|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|他のプロセスに挿入される Office アプリケーションの動作を示す値。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderOfficeCommunicationAppsLaunchChildProcess|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|子プロセスの作成からの Office コミュニケーションアプリケーション (Microsoft Outlook を含む) の動作を示す値。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderOfficeAppsExecutableContentCreationOrLaunchType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Office アプリケーション/マクロの動作を示す値です。実行可能なコンテンツを作成または起動します。 使用可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderofficeappslaunchchildprocess|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|Office アプリケーション/マクロの動作を示す値です。実行可能なコンテンツを作成または起動します。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderofficeappslaunchchildprocesstype|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Office アプリケーションの開始子プロセスの動作を示す値。 使用可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderofficeappslaunchchildprocess|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|Office アプリケーションの開始子プロセスの動作を示す値。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderOfficeMacroCodeAllowWin32ImportsType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Office のマクロコードからの Win32 インポートの動作を示す値です。 使用可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderOfficeMacroCodeAllowWin32Imports|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|Office のマクロコードからの Win32 インポートの動作を示す値です。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderScriptObfuscatedMacroCodeType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|難読化された js/vbs/ps/マクロコードの動作を示す値。 使用可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderScriptObfuscatedMacroCode|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|難読化された js/vbs/ps/マクロコードの動作を示す値。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderScriptDownloadedPayloadExecutionType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|インターネットからダウンロードされた、js/vbs のペイロード実行の動作を示す値。 使用可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderScriptDownloadedPayloadExecution|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|インターネットからダウンロードされた、js/vbs のペイロード実行の動作を示す値。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderPreventCredentialStealingType|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|Windows ローカルセキュリティ機関サブシステムからの資格情報の盗用が許可されているかどうかを示す値。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderprocessの種類|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|PSExec および WMI コマンドからのプロセス作成に対する応答を示す値。 使用可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderprocesscreation|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|PSExec および WMI コマンドからのプロセス作成に対する応答を示す値。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderアン trustedusbprocesstype|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|USB から実行される信頼されていないおよび署名されていないプロセスへの応答を示す値。 使用可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderアン trustedusbプロセス|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|USB から実行される信頼されていないおよび署名されていないプロセスへの応答を示す値。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderUntrustedExecutableType|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|流行、年齢、または信頼できるリストの条件を満たさない実行可能ファイルへの応答を示す値。 使用可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderUntrustedExecutable|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|流行、年齢、または信頼できるリストの条件を満たさない実行可能ファイルへの応答を示す値。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderemailcontentexecutiontype|[defenderAttackSurfaceType](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|実行可能コンテンツ (exe、dll、ps、js、vbs など) の実行を電子メール (webmail/メールクライアント) から削除する必要があるかどうかを示す値。 使用可能な値は、`userDefined`、`block`、`auditMode` です。|
|defenderemailcontentexecution|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|実行可能コンテンツ (exe、dll、ps、js、vbs など) の実行を電子メール (webmail/メールクライアント) から削除する必要があるかどうかを示す値。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderAdvancedRansomewareProtectionType|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|ranware に対して高度な保護を使用することを示す値。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defendergu/myfolderstype|[folderprotectiontype](../resources/intune-deviceconfig-folderprotectiontype.md)|保護されたフォルダーの動作を示す値。 可能な値は、`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification` です。|
|defenderGuardedFoldersAllowedAppPaths|String collection|保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト|
|defenderAdditionalGuardedFolders|String コレクション|保護されたフォルダーのリストに追加されるフォルダー パスのリスト|
|defendernetworkprotectiontype|[defenderprotectiontype](../resources/intune-deviceconfig-defenderprotectiontype.md)|networkprotection の動作を示す値です。 使用可能な値は、`userDefined`、`enable`、`auditMode` です。|
|defenderExploitProtectionXml|Binary|Exploit Protection の詳細に関する情報を含む XML コンテンツ。|
|defenderExploitProtectionXmlFileName|String|DefenderExploitProtectionXml の取得元となるファイルの名前。|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|管理者がデバイスで許可するアプリの種類を選択できるようにします。 可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。|
|deviceGuardLocalSystemAuthorityCredentialGuardSettings|[deviceGuardLocalSystemAuthorityCredentialGuardType](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|セキュリティで保護されたブートと仮想化ベースのセキュリティがあるプラットフォームセキュリティレベルが両方とも有効になっている場合は、Credential Guard をオンにします。 使用可能な値は、`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock` です。|
|deviceGuardEnableVirtualizationBasedSecurity|Boolean|仮想化ベースのセキュリティ (VBS) を有効にします。|
|deviceGuardEnableSecureBootWithDMA|Boolean|次回の再起動時にプラットフォームセキュリティレベルを有効にするかどうかを指定します。|
|devicegu//systemguard|[購入](../resources/intune-shared-enablement.md)|IT 管理者がシステムガードの起動を構成できるようにします。 使用可能な値は、`notConfigured`、`enabled`、`disabled` です。|
|smartScreenEnableInShell|Boolean|IT 管理者が Windows 用の SmartScreen を構成することを許可します。|
|smartScreenBlockOverrideForFiles|Boolean|ユーザーが SmartScreen 警告を無視し、悪意のあるファイルを実行できるかどうかを IT 管理者が制御することを許可します。|
|applicationGuardEnabled|Boolean|Windows Defender Application Guard を有効にします|
|applicationGuardEnabledOptions|[applicationGuardEnabledOptions](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|新しい windows ビルドに対して windows Defender Application Guard を有効にします。 可能な値は、`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice` です。|
|applicationGuardBlockFileTransfer|[applicationgu/blockfiletransfertype](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|画像ファイル、テキストファイル、またはそのどちらも転送しないように、クリップボードをブロックします。 可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。|
|applicationGuardBlockNonEnterpriseContent|Boolean|サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします|
|applicationGuardAllowPersistence|Boolean|App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します|
|applicationGuardForceAuditing|Boolean|監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます|
|applicationGuardBlockClipboardSharing|[applicationgu/blockクリップボード sharingtype](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。 可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。|
|applicationGuardAllowPrintToPDF|Boolean|コンテナーから PDF への出力を許可します|
|applicationGuardAllowPrintToXPS|Boolean|コンテナーから XPS への出力を許可します|
|applicationGuardAllowPrintToLocalPrinters|Boolean|コンテナーからローカル プリンターへの出力を許可します|
|applicationGuardAllowPrintToNetworkPrinters|Boolean|コンテナーからネットワーク プリンターへの出力を許可します|
|applicationGuardAllowVirtualGPU|Boolean|application guard が仮想 GPU を使用できるようにする|
|applicationGuardAllowFileSaveOnHost|Boolean|アプリケーションガードコンテナーのエッジからファイルをダウンロードし、ホストファイルシステムに保存することをユーザーに許可する|
|bitlockerallowstandarduserencryption|Boolean|管理者は、Azure AD Join 時に encrpytion を有効にすることを標準ユーザーに許可します。|
|bitLockerDisableWarningForOtherDiskEncryption|Boolean|管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|管理者が BitLocker を使用して暗号化をオンにすることを許可します。 このポリシーは、携帯電話の SKU に対してのみ有効です。|
|bitLockerEncryptDevice|Boolean|管理者が BitLocker を使用して暗号化をオンにすることを許可します。|
|bitLockerSystemDrivePolicy|[bitLockerSystemDrivePolicy](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|BitLocker システムドライブポリシー。|
|bitLockerFixedDrivePolicy|[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|BitLocker 固定ドライブポリシー。|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|BitLocker リムーバブル ドライブ ポリシー。|

## <a name="relationships"></a>関係
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
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "String",
      "description": "String",
      "packageFamilyName": "String",
      "filePath": "String",
      "serviceName": "String",
      "protocol": 1024,
      "localPortRanges": [
        "String"
      ],
      "remotePortRanges": [
        "String"
      ],
      "localAddressRanges": [
        "String"
      ],
      "remoteAddressRanges": [
        "String"
      ],
      "profileTypes": "String",
      "action": "String",
      "trafficDirection": "String",
      "interfaceTypes": "String",
      "localUserAuthorizations": "String"
    }
  ],
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
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
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
  "defenderAdobeReaderLaunchChildProcess": "String",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "String",
  "defenderOfficeAppsOtherProcessInjection": "String",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "String",
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





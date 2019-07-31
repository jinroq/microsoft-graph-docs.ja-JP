---
title: Advanced Bitlockerstate 列挙型
description: 高度な BitLocker 状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8916392d2870aa7f6279b757487c5a67ac8b99d8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011905"
---
# <a name="advancedbitlockerstate-enum-type"></a>Advanced Bitlockerstate 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

高度な BitLocker 状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|success|.0|高度な BitLocker 状態の成功|
|noUserConsent|1-d|ユーザーが暗号化の同意を与えていません|
|osVolumeEncryptionMethodMismatch|pbm-2|OS ボリュームの暗号化方法がポリシーで設定されたものと異なります|
|osVolumeTpmRequired|2/4|TPM は OS ボリュームの保護には使用されませんが、ポリシーによって必要になります。|
|Osvolumetpmonrequired が必要です|8 |TPM のみの保護は OS ボリュームには使用されませんが、ポリシーによって必要になります。|
|osVolumeTpmPinRequired|16|TPM + PIN 保護は OS ボリュームには使用されませんが、ポリシーによって必要になります。|
|osVolumeTpmStartupKeyRequired|32|TPM + スタートアップキー保護は OS ボリュームには使用されませんが、ポリシーによって必要になります。|
|osVolumeTpmPinStartupKeyRequired|64|TPM + PIN + スタートアップキーは OS ボリュームでは使用されませんが、ポリシーによって必要になります。|
|osVolumeUnprotected なし|128|保護されていない OS ボリュームが検出された|
|recoveryKeyBackupFailed|256|回復キーのバックアップが失敗した|
|fixedDriveNotEncrypted|512|固定ドライブが暗号化されていない|
|Fixeddrive Encryptionmethodミスマッチ|1024|固定ドライブの暗号化方法が、ポリシーで設定されたものと異なります。|
|loggedOnUserNonAdmin|2048|ログオンしているユーザーが管理者ではない。これには、"AllowStandardUserEncryption" ポリシーが1に設定されている必要があります。|
|windowsRecoveryEnvironmentNotConfigured|4096|WinRE が構成されていません|
|tpmNotAvailable|8192|BitLocker では TPM を使用できません。 これは、TPM が存在しないこと、または TPM が使用できないレジストリの上書きが設定されているか、またはホスト OS がポータブル/ローマ可能なドライブにあることを意味します。|
|tpmNotReady|16384|TPM は BitLocker の準備ができていません|
|networkError|32768|ネットワークを使用できません。 これは、回復キーのバックアップに必要です。 ドライブ暗号化対応デバイスの場合は、このレポートが表示されます。|






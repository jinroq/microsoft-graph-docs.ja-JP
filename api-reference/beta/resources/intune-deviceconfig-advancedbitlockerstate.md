---
title: advanced bitlockerstate 列挙型
description: 高度な BitLocker 状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8515f59b6fbba65f590b07c6a17fda55b4e9bd4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178144"
---
# <a name="advancedbitlockerstate-enum-type"></a>advanced bitlockerstate 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

高度な BitLocker 状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|success|.0|高度な BitLocker 状態の成功|
|noUserConsent|1-d|ユーザーが暗号化の同意を与えていません|
|osvolumeencryptionmethodmismatch|pbm-2|OS ボリュームの暗号化方法がポリシーで設定されたものと異なります|
|osvolumetpmrequired|2/4|TPM は OS ボリュームの保護には使用されませんが、ポリシーによって必要になります。|
|osvolumetpmonrequired が必要です|~|TPM のみの保護は OS ボリュームには使用されませんが、ポリシーによって必要になります。|
|osvolumetpmpinrequired|16|TPM + PIN 保護は OS ボリュームには使用されませんが、ポリシーによって必要になります。|
|osvolumetpmstartupkeyrequired|32|TPM + スタートアップキー保護は OS ボリュームには使用されませんが、ポリシーによって必要になります。|
|osvolumetpmpinstartupkeyrequired|64|TPM + PIN + スタートアップキーは OS ボリュームでは使用されませんが、ポリシーによって必要になります。|
|osvolumeunprotected なし| 
128 
|保護されていない OS ボリュームが検出された|
|recoverykeybackupfailed|256|回復キーのバックアップが失敗した|
|fixedDriveNotEncrypted|512|固定ドライブが暗号化されていない|
|fixeddrive encryptionmethodミスマッチ|1024|固定ドライブの暗号化方法が、ポリシーで設定されたものと異なります。|
|loggedOnUserNonAdmin|2048|ログオンしているユーザーが管理者ではない。これには、"allowstandarduserencryption" ポリシーが1に設定されている必要があります。|
|windowsRecoveryEnvironmentNotConfigured|4096|WinRE が構成されていません|
|tpmNotAvailable|8192|BitLocker では TPM を使用できません。 これは、tpm が存在しないこと、または tpm が使用できないレジストリの上書きが設定されているか、またはホスト OS がポータブル/ローマ可能なドライブにあることを意味します。|
|tpmNotReady|16384|TPM は BitLocker の準備ができていません|
|networkerror|32768|ネットワークを使用できません。 これは、回復キーのバックアップに必要です。 ドライブ暗号化対応デバイスの場合は、このレポートが表示されます。|





---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597b49f65027ae2d01cbfddf741ff8ca08f83eb2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460528"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a>localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|Not Configured|
|elevateWithoutPrompting|1-d|メッセージを表示せずに昇格します。|
|promptForCredentialsOnTheSecureDesktop|pbm-2|セキュリティで保護されたデスクトップで資格情報の入力を求める|
|promptForConsentOnTheSecureDesktop|1/3|セキュリティで保護されたデスクトップで同意を求める|
|promptforcredentials|2/4|資格情報の入力を求める|
|promptforconsent|5|同意を求めるメッセージ|
|promptforconfornonwindowsバイナリー|シックス|Windows 以外のバイナリの同意を求める|






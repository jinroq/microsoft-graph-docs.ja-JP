---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 978436bca4ac0ca281fde61e046e854ba3725c73
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413760"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a>localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|構成されていません|
|elevateWithoutPrompting|1|メッセージを表示せずに昇格します。|
|promptForCredentialsOnTheSecureDesktop|2|セキュリティで保護されたデスクトップで資格情報の入力を求める|
|promptForConsentOnTheSecureDesktop|3|セキュリティで保護されたデスクトップで同意を求める|
|promptForCredentials|4|資格情報の入力を求める|
|promptForConsent|5|同意を求める|
|promptForConsentForNonWindowsBinaries|6|Windows 以外のバイナリの同意を要求します。|





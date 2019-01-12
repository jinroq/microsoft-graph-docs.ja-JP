---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ae886f6c7696150cb85a17cb2caa65823705e121
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916825"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a>localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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






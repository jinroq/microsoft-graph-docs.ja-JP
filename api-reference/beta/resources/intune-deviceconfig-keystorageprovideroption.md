---
title: keyStorageProviderOption 列挙型
description: キー記憶域プロバイダー (KSP) のインポートのオプションです。
ms.openlocfilehash: 236489d288ec0be70a818e1c51b8c634ad3933a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067376"
---
# <a name="keystorageprovideroption-enum-type"></a>keyStorageProviderOption 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

キー記憶域プロバイダー (KSP) のインポートのオプションです。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|インポートするトラステッド プラットフォーム モジュール (TPM) KSP が存在する場合は、それ以外の場合、ソフトウェア KSP にインポートします。|
|useTpmKspOtherwiseFail|1|インポートするトラステッド プラットフォーム モジュール (TPM) KSP が存在する場合はそれ以外の場合失敗します。|
|usePassportForWorkKspOtherwiseFail|2|作業 KSP の passport のサイトにインポート可能な場合、失敗します。|
|useSoftwareKsp|3|ソフトウェア KSP にインポートします。|






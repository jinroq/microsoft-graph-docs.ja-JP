---
title: keyStorageProviderOption 列挙型
description: キー記憶域プロバイダー (KSP) のインポートのオプションです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f3a8169b4bb6cd2357f02aa7fec89ba640780f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946554"
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






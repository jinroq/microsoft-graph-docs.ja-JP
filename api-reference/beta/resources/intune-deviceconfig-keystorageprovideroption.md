---
title: keyStorageProviderOption 列挙型
description: キー記憶域プロバイダー (KSP) のインポートのオプションです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6993d7e241ef94c572975c709c286a14f6eabf5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424225"
---
# <a name="keystorageprovideroption-enum-type"></a>keyStorageProviderOption 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

キー記憶域プロバイダー (KSP) のインポートのオプションです。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|インポートするトラステッド プラットフォーム モジュール (TPM) KSP が存在する場合は、それ以外の場合、ソフトウェア KSP にインポートします。|
|useTpmKspOtherwiseFail|1|インポートするトラステッド プラットフォーム モジュール (TPM) KSP が存在する場合はそれ以外の場合失敗します。|
|usePassportForWorkKspOtherwiseFail|2|作業 KSP の passport のサイトにインポート可能な場合、失敗します。|
|useSoftwareKsp|3|ソフトウェア KSP にインポートします。|





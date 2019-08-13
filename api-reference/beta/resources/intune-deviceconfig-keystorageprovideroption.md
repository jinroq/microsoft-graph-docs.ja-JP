---
title: keyStorageProviderOption 列挙型
description: キーストレージプロバイダー (KSP) のインポートオプション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 21a2e72bc226fdd7a965fbfb3f6ddd7735a4f351
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325506"
---
# <a name="keystorageprovideroption-enum-type"></a>keyStorageProviderOption 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

キーストレージプロバイダー (KSP) のインポートオプション。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|.0|トラステッドプラットフォームモジュール (TPM) KSP がある場合は、それ以外の場合は、ソフトウェア KSP にインポートします。|
|useTpmKspOtherwiseFail|1-d|トラステッドプラットフォームモジュール (TPM) KSP (存在する場合) にインポートします (それ以外の場合は失敗します)。|
|usePassportForWorkKspOtherwiseFail|pbm-2|利用可能な場合は Passport にインポートし、それ以外の場合は失敗します。|
|その他の方法|1/3|ソフトウェア KSP にインポートします。|




---
title: keystorageprovideroption 列挙型
description: キーストレージプロバイダー (KSP) のインポートオプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ddc1cffe1f4e6056d53a151a3b36b2622c9bf4b5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153019"
---
# <a name="keystorageprovideroption-enum-type"></a>keystorageprovideroption 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

キーストレージプロバイダー (KSP) のインポートオプション。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|.0|トラステッドプラットフォームモジュール (TPM) ksp がある場合は、それ以外の場合は、ソフトウェア ksp にインポートします。|
|useTpmKspOtherwiseFail|1-d|トラステッドプラットフォームモジュール (TPM) KSP (存在する場合) にインポートします (それ以外の場合は失敗します)。|
|usePassportForWorkKspOtherwiseFail|pbm-2|利用可能な場合は Passport にインポートし、それ以外の場合は失敗します。|
|その他の方法|1/3|ソフトウェア KSP にインポートします。|





---
title: deviceManagementExchangeConnectorType 列挙型
description: Exchange コネクタの種類です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 49e61dc3a2a6ba7eee80891846cd2f58c2a22485
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876105"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a>deviceManagementExchangeConnectorType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Exchange コネクタの種類です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|onPremises|0|オンプレミスの Exchange 環境に接続します。|
|ホスト|1|O365 マルチ テナント型の Exchange 環境に接続します。|
|serviceToService|2|O365 マルチ テナント型の Exchange 環境に直接 Intune サービスに接続します。|
|専用|3|O365 専用の Exchange 環境に接続します。|






---
title: deviceManagementExchangeAccessLevel 列挙型
description: Exchange のアクセス レベルです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 03588e51a301bfcc4aac5eb3f9c0bfe0fbba9ea9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889552"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a>deviceManagementExchangeAccessLevel 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Exchange のアクセス レベルです。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|Exchange では、デバイス アクセス ルールが構成されていません。|
|許可します。|1|デバイスの Exchange へのアクセスを許可します。|
|ブロック|2|デバイスから Exchange へのアクセスをブロックします。|
|検査|3|デバイスを Exchange で隔離します。|






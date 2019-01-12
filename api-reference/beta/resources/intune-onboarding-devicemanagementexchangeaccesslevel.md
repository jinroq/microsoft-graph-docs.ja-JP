---
title: deviceManagementExchangeAccessLevel 列挙型
description: Exchange のアクセス レベルです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1d9654e526aec7263f12d0fdcb3af8c68f7ba20e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950033"
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






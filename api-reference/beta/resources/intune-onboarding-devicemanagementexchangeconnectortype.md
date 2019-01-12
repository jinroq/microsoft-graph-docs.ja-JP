---
title: deviceManagementExchangeConnectorType 列挙型
description: Exchange コネクタの種類です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c05410c3b3b7c889840d0b47aca05f6457564eb4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934954"
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






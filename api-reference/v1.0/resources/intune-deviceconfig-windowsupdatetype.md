---
title: windowsUpdateType 列挙型
description: 分岐デバイスから更新を受け取ります。
ms.openlocfilehash: b489f17da5dc02dd7f7e72350eef282e56643dd0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023874"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

分岐デバイスから更新を受け取ります。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|設定するユーザーを許可します。|
|all|1|半年のチャネル (対象となる)。 デバイスでは、半年のチャネル (対象) からすべての適用可能な機能の更新を取得します。|
|businessReadyOnly|2|半年チャンネルです。 デバイスは、半年のチャネルからの機能の更新を取得します。|
|windowsInsiderBuildFast|3|Windows の内部からのビルド - 高速|
|windowsInsiderBuildSlow|4|Windows 内部からビルド時間がかかる|
|windowsInsiderBuildRelease|5|リリース ビルドの Windows の内部から|




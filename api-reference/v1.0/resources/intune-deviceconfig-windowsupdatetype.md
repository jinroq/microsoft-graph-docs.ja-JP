---
title: windowsUpdateType 列挙型
description: 分岐デバイスから更新を受け取ります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 198b5f8db5698d309199964e4cb69f8981ceeb1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838970"
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




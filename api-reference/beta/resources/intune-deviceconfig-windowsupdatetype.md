---
title: windowsUpdateType 列挙型
description: 分岐デバイスから更新を受け取ります。
author: tfitzmac
ms.openlocfilehash: b41fea0254cbbb6a590d240c2db9e4fb7aa0e6eb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309626"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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






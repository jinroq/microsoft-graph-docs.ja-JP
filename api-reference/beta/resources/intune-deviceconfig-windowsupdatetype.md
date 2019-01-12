---
title: windowsUpdateType 列挙型
description: 分岐デバイスから更新を受け取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1444af64043ac38685ca022b56b8856be77a0b70
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944349"
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






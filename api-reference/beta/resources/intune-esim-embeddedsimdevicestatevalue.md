---
title: embeddedSIMDeviceStateValue 列挙型
description: SIM の埋め込みのライセンス認証コードのさまざまな状態をについて説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 67dd3850db1e759ded578f551eb41636ec231084
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985964"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>embeddedSIMDeviceStateValue 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

SIM の埋め込みのライセンス認証コードのさまざまな状態をについて説明します。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notEvaluated|0|SIM の埋め込みのライセンス認証コードが空き時間と、デバイスに割り当てられる利用可能なことを指定します。|
|失敗しました。|1|Intune サービスがデバイスにこのプロファイルを提供する失敗したことを指定します。|
|インストール|2|SIM の埋め込みのライセンス認証コードは、デバイスに割り当てられているし、デバイスが、トークンをインストールすることを指定します。|
|インストールされています。|3|SIM の埋め込みのライセンス認証コードがターゲット ・ デバイスを正常にインストールされているかを指定します。|
|削除|4|Intune サービスがデバイスのプロファイルを削除しようとしていることを指定します。|
|エラー|5|このプロファイルを使用してエラーがあることを指定します。|
|deleted|6|デバイスからプロファイルを削除することを指定します。|
|removedByUser|7|ユーザーがデバイスからプロファイルが削除されるかを指定します。|






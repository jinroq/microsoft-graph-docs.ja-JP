---
title: embeddedSIMDeviceStateValue 列挙型
description: SIM の埋め込みのライセンス認証コードのさまざまな状態をについて説明します。
author: tfitzmac
ms.openlocfilehash: 51e550669d9cd29d7d5bb246fe2cba017b02187c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320595"
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






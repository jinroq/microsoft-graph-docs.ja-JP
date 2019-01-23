---
title: embeddedSIMDeviceStateValue 列挙型
description: SIM の埋め込みのライセンス認証コードのさまざまな状態をについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2da255ef2d0cf192dd09a6351bbd337f3cd9b5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421327"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>embeddedSIMDeviceStateValue 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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





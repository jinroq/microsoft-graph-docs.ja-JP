---
title: embeddedSIMDeviceStateValue 列挙型
description: 埋め込まれた SIM のアクティブ化コードのさまざまな状態について説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bdc3250605de7db7a3778d64b5e743a415de4c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145424"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>embeddedSIMDeviceStateValue 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

埋め込まれた SIM のアクティブ化コードのさまざまな状態について説明します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|注評価|.0|埋め込まれている SIM ライセンス認証コードが無料で、デバイスに割り当てることができることを指定します。|
|フェール|1-d|Intune サービスがこのプロファイルをデバイスに配信できなかったことを指定します。|
|インストール|pbm-2|埋め込まれた SIM ライセンス認証コードがデバイスに割り当てられており、デバイスがトークンをインストールしていることを指定します。|
|れる|1/3|埋め込まれた SIM ライセンス認証コードがターゲットデバイスに正常にインストールされたことを指定します。|
|削除|2/4|Intune サービスがデバイスからプロファイルを削除しようとしていることを指定します。|
|エラー|5|このプロファイルにエラーがあることを指定します。|
|deleted|シックス|プロファイルがデバイスから削除されることを指定します。|
|removedbyuser|7|ユーザーがプロファイルをデバイスから削除することを指定します。|





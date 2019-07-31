---
title: embeddedSIMDeviceStateValue 列挙型
description: 埋め込まれた SIM のアクティブ化コードのさまざまな状態について説明します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c36d6739e13027f2a4136899e0e60a4dbff8d990
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998780"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>embeddedSIMDeviceStateValue 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

埋め込まれた SIM のアクティブ化コードのさまざまな状態について説明します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|注評価|.0|埋め込まれている SIM ライセンス認証コードが無料で、デバイスに割り当てることができることを指定します。|
|フェール|1-d|Intune サービスがこのプロファイルをデバイスに配信できなかったことを指定します。|
|インストール|pbm-2|埋め込まれた SIM ライセンス認証コードがデバイスに割り当てられており、デバイスがトークンをインストールしていることを指定します。|
|れる|1/3|埋め込まれた SIM ライセンス認証コードがターゲットデバイスに正常にインストールされたことを指定します。|
|と|2/4|Intune サービスがデバイスからプロファイルを削除しようとしていることを指定します。|
|error|5|このプロファイルにエラーがあることを指定します。|
|deleted|シックス|プロファイルがデバイスから削除されることを指定します。|
|removedByUser|7|ユーザーがプロファイルをデバイスから削除することを指定します。|






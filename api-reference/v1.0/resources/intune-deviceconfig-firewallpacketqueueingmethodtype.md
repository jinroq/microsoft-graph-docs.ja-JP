---
title: firewallPacketQueueingMethodType 列挙型
description: firewallPacketQueueingMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdd9dc0279abc332bbf7b686f7f429fbd8db8883
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541309"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>firewallPacketQueueingMethodType 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

firewallPacketQueueingMethod に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない|
|党|1 |パケットキューを無効にする|
|queueinbound|2 |暗号化された着信パケットをキューに保存する|
|queueoutbound|3 |転送のためにキューに復号化された送信パケット|
|queueboth|4 |受信パケットと送信パケットの両方をキューにする|




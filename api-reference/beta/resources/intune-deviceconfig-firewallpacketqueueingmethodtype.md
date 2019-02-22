---
title: firewallPacketQueueingMethodType 列挙型
description: firewallPacketQueueingMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1b8543df5fa2a50cfdfa56c7cb2d96199ba44e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172206"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>firewallPacketQueueingMethodType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

firewallPacketQueueingMethod に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない|
|党|1-d|パケットキューを無効にする|
|queueinbound|pbm-2|暗号化された着信パケットをキューに保存する|
|queueoutbound|1/3|転送のためにキューに復号化された送信パケット|
|queueboth|2/4|受信パケットと送信パケットの両方をキューにする|





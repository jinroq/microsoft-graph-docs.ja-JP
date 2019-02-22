---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f04d8c0fddb966504675e3b4c677dfd0bbabe64c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144626"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス登録の状態。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notregistered 済み|.0|デバイスが登録されていません。|
|い|pbm-2|デバイスは登録されています。|
|破棄|1/3|デバイスがブロックされているか、ワイプされているか、破棄されています。|
|keyconflict|2/4|デバイスにキーの競合があります。|
|approvalpending|5|デバイスの承認が保留中です。|
|certificateReset|シックス|デバイス証明書がリセットされました。|
|notregisteredpendingenrollment|7|デバイスは登録されておらず、登録が保留されていません。|
|不明|~|デバイス登録の状態が不明です。|





---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3bee7ab56f07dd6f27c20c771329ba84edbb19
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264135"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 列挙型

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




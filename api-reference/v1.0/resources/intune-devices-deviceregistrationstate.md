---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3bee7ab56f07dd6f27c20c771329ba84edbb19
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580975"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス登録の状態。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notregistered 済み|.0|デバイスが登録されていません。|
|い|2 |デバイスは登録されています。|
|破棄|3 |デバイスがブロックされているか、ワイプされているか、破棄されています。|
|keyconflict|4 |デバイスにキーの競合があります。|
|approvalpending|5 |デバイスの承認が保留中です。|
|certificateReset|6 |デバイス証明書がリセットされました。|
|notregisteredpendingenrollment|7 |デバイスは登録されておらず、登録が保留されていません。|
|不明|8 |デバイス登録の状態が不明です。|




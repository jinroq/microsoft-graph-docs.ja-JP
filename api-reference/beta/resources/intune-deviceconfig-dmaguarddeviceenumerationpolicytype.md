---
title: dmaGuardDeviceEnumerationPolicyType 列挙型
description: DmaGuardDeviceEnumerationPolicy の使用可能な値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5baa0cfd5c80f954036e10f0e4d04d2b83e57f2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430454"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>dmaGuardDeviceEnumerationPolicyType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

DmaGuardDeviceEnumerationPolicy の使用可能な値です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|既定値です。 DMA の互換性のないドライバーを再割り当てを持つデバイスは、ユーザー画面のロックを解除した後にのみ列挙されます。|
|これ|1|DMA の互換性のないドライバーを再割り当てを持つデバイスは、起動し、いつでも DMA を実行するのには許可されません。|
|すべて許可が次|2|いつでもすべての外部 DMA 対応 PCIe デバイスが列挙されます。|





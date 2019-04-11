---
title: dmaGuardDeviceEnumerationPolicyType 列挙型
description: DmaGuardDeviceEnumerationPolicy の可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6910172ef4ab733b09d837dcc9a7196893402ab
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776648"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>dmaGuardDeviceEnumerationPolicyType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

DmaGuardDeviceEnumerationPolicy の可能な値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|既定値です。 DMA が再マッピングされているデバイス互換性のないドライバーは、ユーザーが画面をロック解除した後にのみ列挙されます。|
|blockall|1-d|dma がマッピングされていないデバイス互換性のないドライバーは、いつでも dma を開始して実行することはできません。|
|allowAll|pbm-2|すべての外部 DMA 対応 PCIe デバイスは、いつでも列挙されます。|






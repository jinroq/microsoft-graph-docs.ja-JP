---
title: dmaGuardDeviceEnumerationPolicyType 列挙型
description: DmaGuardDeviceEnumerationPolicy の可能な値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4e534fca412c6d48ab9ea006f308a114c73def2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989918"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>dmaGuardDeviceEnumerationPolicyType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

DmaGuardDeviceEnumerationPolicy の可能な値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|.0|既定値です。 DMA が再マッピングされているデバイス互換性のないドライバーは、ユーザーが画面をロック解除した後にのみ列挙されます。|
|blockAll|1-d|DMA がマッピングされていないデバイス互換性のないドライバーは、いつでも DMA を開始して実行することはできません。|
|allowAll|pbm-2|すべての外部 DMA 対応 PCIe デバイスは、いつでも列挙されます。|






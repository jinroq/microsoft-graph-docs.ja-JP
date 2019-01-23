---
title: 列挙型の有効化
description: Intune は、複数のワークフローをサポートするため Microsoft グラフ API の対応の列挙体について説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 538b52790cf7748453adfda2a6bea8334a36fb87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399564"
---
# <a name="enablement-enum-type"></a>列挙型の有効化

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

値は、デバイスの状態を示すために使用します。 

間に違いがあることに注意が無効になり、構成されていません。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|デバイスの既定値でことを目的しません。|
|enabled|1|デバイスの設定を有効にします。|
|無効になっています。|2|デバイスの設定を無効にします。|

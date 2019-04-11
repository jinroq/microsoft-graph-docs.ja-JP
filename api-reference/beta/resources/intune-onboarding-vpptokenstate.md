---
title: vpptokenstate 列挙型
description: Apple volume purchase program のトークンに関連付けられている状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbc62b855035ebf68fefae3d628582b566804449
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781149"
---
# <a name="vpptokenstate-enum-type"></a>vpptokenstate 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Apple volume purchase program のトークンに関連付けられている状態。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|既定の状態です。|
|有効な|1-d|トークンが有効です。|
|終了|pbm-2|トークンの有効期限が切れています。|
|無効です|1/3|トークンが無効です。|
|assignedToExternalMDM|2/4|トークンは別の MDM サービスによって管理されています。|






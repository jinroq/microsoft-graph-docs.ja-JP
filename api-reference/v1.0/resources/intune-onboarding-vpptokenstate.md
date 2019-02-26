---
title: vpptokenstate 列挙型
description: Apple volume purchase program のトークンに関連付けられている状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 573fe27064881f670e642e7c3727b8c9eb7db5a9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254934"
---
# <a name="vpptokenstate-enum-type"></a>vpptokenstate 列挙型

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




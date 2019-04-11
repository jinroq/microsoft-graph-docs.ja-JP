---
title: certificateRevocationStatus 列挙型
description: 証明書の失効状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fd9a6cd34df322a057d16e3d803d8685f7cd173
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782808"
---
# <a name="certificaterevocationstatus-enum-type"></a>certificateRevocationStatus 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

証明書の失効状態。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|取り消されません。|
|対する|1-d|失効が保留中です。|
|発行|pbm-2|失効コマンドが発行されました。|
|フェール|1/3|取り消しに失敗しました。|
|破棄|2/4|破棄.|






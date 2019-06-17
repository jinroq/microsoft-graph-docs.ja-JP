---
title: certificateRevocationStatus 列挙型
description: 証明書の失効状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef7181707e6e80c9ad816f345f2a299dbce147e7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990114"
---
# <a name="certificaterevocationstatus-enum-type"></a>certificateRevocationStatus 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

証明書の失効状態。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|取り消されません。|
|対する|1-d|失効が保留中です。|
|発行|pbm-2|失効コマンドが発行されました。|
|フェール|1/3|取り消しに失敗しました。|
|破棄|2/4|破棄.|






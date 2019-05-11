---
title: certificateRevocationStatus 列挙型
description: 証明書の失効状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4544968e473c41d787df606112801c9b60e2cb98
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947429"
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





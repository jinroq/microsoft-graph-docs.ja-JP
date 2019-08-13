---
title: certificateRevocationStatus 列挙型
description: 証明書の失効状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 68f510771370e5be95a8360526d0058ff8c307b1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333703"
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




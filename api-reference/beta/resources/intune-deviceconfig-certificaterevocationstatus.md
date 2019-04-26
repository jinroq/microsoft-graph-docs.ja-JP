---
title: certificateRevocationStatus 列挙型
description: 証明書の失効状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fd9a6cd34df322a057d16e3d803d8685f7cd173
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549383"
---
# <a name="certificaterevocationstatus-enum-type"></a>certificateRevocationStatus 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

証明書の失効状態。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|なし|.0|取り消されません。|
|対する|1 |失効が保留中です。|
|発行|2 |失効コマンドが発行されました。|
|フェール|3 |取り消しに失敗しました。|
|破棄|4 |破棄.|






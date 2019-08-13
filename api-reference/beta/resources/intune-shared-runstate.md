---
title: runState 列挙型
description: デバイス管理スクリプトの実行状態の種類を示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d77f3ef9a2d7fd37edeaf2b4cc25d5e6d5bfcf4f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347851"
---
# <a name="runstate-enum-type"></a>runState 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス管理スクリプトの実行状態の種類を示します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|不明な結果です。|
|success|1-d|スクリプトは正常に実行されます。|
|fail|pbm-2|スクリプトの実行に失敗しました。|
|error|1/3|検出スクリプトヒットエラー。|
|対する|2/4|スクリプトの実行が保留中です。|




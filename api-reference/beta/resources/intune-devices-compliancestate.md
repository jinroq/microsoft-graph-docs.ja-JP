---
title: complianceState 列挙型
description: コンプライアンス状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 04f77da451970a302dbf249e8820aa5a2a8f0ebc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392739"
---
# <a name="compliancestate-enum-type"></a>complianceState 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

コンプライアンス状態です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|不明。|
|準拠|1|準拠していません。|
|準拠していません。|2|デバイスは非準拠、企業のリソースがブロックされました。|
|競合|3|その他の規則と競合しています。|
|エラー|4|エラー。|
|inGracePeriod|254|デバイスは非準拠ですが、社内リソースへのアクセスにはまだ|
|configManager|255|構成マネージャーによって管理されます。|





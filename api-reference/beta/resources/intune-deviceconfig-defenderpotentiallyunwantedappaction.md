---
title: defenderPotentiallyUnwantedAppAction 列挙型
description: 検出された望ましくない可能性があるアプリケーション (PUA) に対して実行する、Defender のアクション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02ac5da63c2787c2b87479a23899c9d2980c54c4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173354"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>defenderPotentiallyUnwantedAppAction 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

検出された望ましくない可能性があるアプリケーション (PUA) に対して実行する、Defender のアクション。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|PUA の保護がオフになっています。 Defender は望ましくない可能性があるアプリケーションに対する保護を行いません。|
|拒否|1-d|PUA の保護がオンになっています。 検出されたアイテムはブロックされます。 これらのメンバーは、他の脅威と共に履歴に表示されます。|
|監査|pbm-2|監査モード。 Defender は望ましくない可能性があるアプリケーションを検出しますが、アクションは実行しません。 イベントビューアーで、defender によって作成されたイベントを検索することによって、アプリケーション defender が操作を実行したことについての情報を確認できます。|





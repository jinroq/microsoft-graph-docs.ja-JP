---
title: defenderPotentiallyUnwantedAppAction 列挙型
description: 検出された望ましくない可能性があるアプリケーション (PUA) に対して実行する、Defender のアクション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1949ec58c7cfd2d896308f740b7eca16f2646b3e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534809"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>defenderPotentiallyUnwantedAppAction 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

検出された望ましくない可能性があるアプリケーション (PUA) に対して実行する、Defender のアクション。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|PUA の保護がオフになっています。 Defender は望ましくない可能性があるアプリケーションに対する保護を行いません。|
|拒否|1 |PUA の保護がオンになっています。 検出されたアイテムはブロックされます。 これらのメンバーは、他の脅威と共に履歴に表示されます。|
|監査|2 |監査モード。 Defender は望ましくない可能性があるアプリケーションを検出しますが、アクションは実行しません。 イベントビューアーで、defender によって作成されたイベントを検索することによって、アプリケーション defender が操作を実行したことについての情報を確認できます。|






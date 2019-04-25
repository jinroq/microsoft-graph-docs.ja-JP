---
title: edgeKioskModeRestrictionType 列挙型
description: Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74b03555456c058411c9a50c7392f29fe60d3aed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524513"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a>edgeKioskModeRestrictionType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|未構成 (無制限)。|
|digitalSignage|1 |シングルアプリモードでのインタラクティブ/デジタル信号。|
|normalmode|2 |標準モード (完全版の Microsoft Edge)。|
|publicた singsingleapp|3 |単一アプリモードでのパブリックブラウズ。|
|publicbrowsingmultiapp|4 |マルチアプリモードでのパブリックブラウズ (inPrivate)。|






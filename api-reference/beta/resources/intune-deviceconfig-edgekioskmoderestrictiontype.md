---
title: edgeKioskModeRestrictionType 列挙型
description: Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bbd3d13ad39b6acda5fd67d69c8cb2de2f2e7c55
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001468"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a>edgeKioskModeRestrictionType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|未構成 (無制限)。|
|digitalSignage|1-d|シングルアプリモードでのインタラクティブ/デジタル信号。|
|normalMode|pbm-2|標準モード (完全版の Microsoft Edge)。|
|Publicた Singsingleapp|1/3|単一アプリモードでのパブリックブラウズ。|
|publicBrowsingMultiApp|2/4|マルチアプリモードでのパブリックブラウズ (inPrivate)。|






---
title: edgeKioskModeRestrictionType 列挙型
description: Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 014025b04974df90dc6e22e55f3597fc265b207d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946743"
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





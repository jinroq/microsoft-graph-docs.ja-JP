---
title: Devicemanagementdomainjoinコネクタ状態列挙型
description: ODJ 要求の状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a584a77c0a921b9d5864270c5a42a9991123eb8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001917"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a>Devicemanagementdomainjoinコネクタ状態列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ODJ 要求の状態。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|active|.0|コネクタは、アクティブな Intune に ping を行います。|
|error|1-d|過去1時間のコネクタからのハートビートはありません。|
|未使用|pbm-2|過去5日間のコネクタからのハートビートはありません。|






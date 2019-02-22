---
title: complianceState 列挙型
description: コンプライアンスの状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29357c5248aea78ffca8af464ecf4c3af17bdbc3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172927"
---
# <a name="compliancestate-enum-type"></a>complianceState 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

コンプライアンスの状態です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|わかり.|
|要件|1-d|要件.|
|互換性|pbm-2|デバイスは非準拠で、企業リソースからブロックされます。|
|異なる|1/3|他のルールと競合しています。|
|エラー|2/4|エラー。|
|inGracePeriod|254|デバイスは準拠していないが、会社のリソースにアクセスできる|
|configmanager|255|構成マネージャーによる管理|





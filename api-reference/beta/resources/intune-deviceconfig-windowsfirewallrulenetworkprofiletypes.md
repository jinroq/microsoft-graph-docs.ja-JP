---
title: windowsFirewallRuleNetworkProfileTypes 列挙型
description: ファイアウォールルールに適用されるネットワークプロファイルの種類を表すフラグ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe8df940a3389d742224a2eca2c215135e751297
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944055"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a>windowsFirewallRuleNetworkProfileTypes 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ファイアウォールルールに適用されるネットワークプロファイルの種類を表すフラグ。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|フラグは設定しません。|
|domain|1-d|ドメインに接続されているネットワークのプロファイル。|
|機密性|pbm-2|プライベートネットワークのプロファイル。|
|public|2/4|パブリックネットワークのプロファイル。|





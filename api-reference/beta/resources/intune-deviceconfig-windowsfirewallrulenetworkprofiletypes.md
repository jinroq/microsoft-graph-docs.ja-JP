---
title: windowsFirewallRuleNetworkProfileTypes 列挙型
description: ファイアウォールルールに適用されるネットワークプロファイルの種類を表すフラグ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9aad571c5563427343ebd6686073f98b7ac703cb
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631571"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a>windowsFirewallRuleNetworkProfileTypes 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ファイアウォールルールに適用されるネットワークプロファイルの種類を表すフラグ。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|フラグは設定しません。|
|domain|1|ドメインに接続されているネットワークのプロファイル。|
|機密性|2|プライベートネットワークのプロファイル。|
|public|2/4|パブリックネットワークのプロファイル。|





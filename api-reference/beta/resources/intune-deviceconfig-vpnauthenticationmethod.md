---
title: vpnAuthenticationMethod 列挙型
description: VPN 認証方法。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f75c7ec53f406e7f998a89faa8d1dabf4c650de
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944622"
---
# <a name="vpnauthenticationmethod-enum-type"></a>vpnAuthenticationMethod 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN 認証方法。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|certificate|.0|証明書を使用して認証します。|
|usernameAndPassword|1-d|認証にユーザー名とパスワードを使用します。|
|derivedCredential|1/3|認証に派生した資格情報を使用します。  IOS に対してのみ有効です。|





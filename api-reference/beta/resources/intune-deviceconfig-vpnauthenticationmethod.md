---
title: vpnAuthenticationMethod 列挙型
description: VPN 認証方法。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 20374a3008e84b00ce7622019f4a3b8306a07318
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969521"
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
|sharedSecret|pbm-2|認証に共有シークレットを使用します。  IOS IKEv2 に対してのみ有効です。|
|derivedCredential|1/3|認証に派生した資格情報を使用します。  IOS に対してのみ有効です。|






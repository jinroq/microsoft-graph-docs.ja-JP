---
title: nonEapAuthenticationMethodForEapTtlsType 列挙型
description: 認証の非 EAP メソッドです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f14c98118541e6eeb6cb48fd54ac3fb69a722b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425597"
---
# <a name="noneapauthenticationmethodforeapttlstype-enum-type"></a>nonEapAuthenticationMethodForEapTtlsType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

認証の非 EAP メソッドです。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|unencryptedPassword|0|暗号化されていないパスワード (PAP) です。|
|challengeHandshakeAuthenticationProtocol|1|チャレンジ ハンドシェイク認証プロトコル (CHAP)。|
|microsoftChap|2| Microsoft CHAP (MS-CHAP)。|
|microsoftChapVersionTwo|3|Microsoft CHAP バージョン 2 (MS-CHAP v2)。|





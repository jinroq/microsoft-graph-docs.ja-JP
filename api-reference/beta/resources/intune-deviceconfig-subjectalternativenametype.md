---
title: subjectAlternativeNameType 列挙型
description: サブジェクト代替名のオプションです。
author: tfitzmac
ms.openlocfilehash: 2c1249c90998a24eca63da7d80e580ac497aa9b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326657"
---
# <a name="subjectalternativenametype-enum-type"></a>subjectAlternativeNameType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

サブジェクト代替名のオプションです。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|サブジェクト代替名がありません。|
|emailAddress|1|電子メール アドレスです。|
|userPrincipalName|2|ユーザー プリンシパル名 (UPN)。|
|customAzureADAttribute|4|Azure の AD 属性をカスタムします。|
|domainNameService|8|ドメイン ネーム サービス (DNS)。|






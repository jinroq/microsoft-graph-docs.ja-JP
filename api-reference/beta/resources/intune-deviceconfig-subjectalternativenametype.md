---
title: subjectAlternativeNameType 列挙型
description: サブジェクト代替名のオプションです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 47ee2bc7e8a6c53d48f0b167983f85e0a18f4f4e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984207"
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






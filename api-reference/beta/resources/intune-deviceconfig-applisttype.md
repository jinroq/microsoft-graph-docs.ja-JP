---
title: appListType 列挙型
description: 準拠のアプリケーションのリストで使用できる値です。
ms.openlocfilehash: 3fcfecde8dbc9efe92f842e9d2b45b7f1579c217
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071505"
---
# <a name="applisttype-enum-type"></a>appListType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

準拠のアプリケーションのリストで使用できる値です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|既定値でことを目的しません。|
|appsInListCompliant|1|一覧は、考慮される準拠 (準拠では、リスト上のアプリ) 専用のアプリケーションを表します。|
|appsNotInListCompliant|2|リストと見なされます非準拠のアプリケーションを表します (すべてのアプリケーション準拠では、リスト上のアプリを除く)。|






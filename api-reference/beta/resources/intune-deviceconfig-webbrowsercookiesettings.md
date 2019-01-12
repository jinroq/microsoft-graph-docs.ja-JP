---
title: webBrowserCookieSettings 列挙型
description: Web ブラウザーの Cookie の設定です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 54fe38b9227c38f3af13ec242ece2d0bd6c144fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927395"
---
# <a name="webbrowsercookiesettings-enum-type"></a>webBrowserCookieSettings 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Web ブラウザーの Cookie の設定です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|browserDefault|0|ブラウザーの既定値でことを目的しません。|
|blockAlways|1|常に cookie をブロックします。|
|allowCurrentWebSite|2|現在の Web サイトからの cookie を許可します。|
|allowFromWebsitesVisited|3|訪問した web サイトからの Cookie を許可します。|
|allowAlways|4|常に cookie を許可します。|






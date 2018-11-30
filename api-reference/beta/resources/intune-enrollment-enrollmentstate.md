---
title: enrollmentState 列挙型
description: まだ文書化されていません
ms.openlocfilehash: 8e8e20c0fd04e4da57eddfa7384052a6ab468152
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072418"
---
# <a name="enrollmentstate-enum-type"></a>enrollmentState 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|デバイス登録の状態は不明です。|
|登録|1|デバイスを登録します。|
|pendingReset|2|登録され、登録プロファイルを使用して登録されているが、登録されているプロファイルが割り当てられているプロファイルとは異なる。|
|失敗しました。|3|登録していない登録に失敗したレコードがあるとします。|
|notContacted|4|デバイスをインポートしていますが、登録していません。|
|ブロック|5|デバイスが、userless として登録されて、アプリケーションのインストールに失敗したため、ユーザー登録への移動がブロックされます。|






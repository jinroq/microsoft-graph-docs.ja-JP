---
title: diagnosticDataSubmissionMode 列挙型
description: ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。
ms.openlocfilehash: b09a4bf334af5981c3ce6dabbab0ac64e2b24887
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023270"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|設定するユーザーを許可します。|
|none|1|OS コンポーネントからは、遠隔測定データは送信されません。 注: この値は、エンタープライズとサーバのデバイスに適用されるのみです。 その他のデバイスでこの設定を使用して、1 の値を設定するのと同じです。|
|基本的な|2|基本的な遠隔測定データを送信します。|
|強化|3|送信には、使用状況と情報のデータを含む遠隔測定データが強化されています。|
|フル|4|システム状態などの診断データを含む完全な遠隔測定データを送信します。|




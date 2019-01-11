---
title: 優先受信トレイを管理する
description: '重要なメッセージを表示することにより、フォーカスのある受信トレイ、 `Focused` 、受信トレイで受信トレイのメッセージの残りの部分のタブ、 `Other` ] タブ。分類システム '
localization_priority: Normal
ms.openlocfilehash: b4c6ceca3248a03f814e42298c9892a1447dd2a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826727"
---
# <a name="manage-focused-inbox"></a>優先受信トレイを管理する

優先受信トレイでは、受信トレイの `Focused` タブに重要メッセージを表示し、その他の受信トレイのメッセージを `Other` タブに表示します。システム主体の分類方法によって、既定の方法で受信トレイのメッセージが整理されます。ユーザー インターフェイスまたはプログラムを介して、時間の経過によってシステムを修正し、学習させることができます。使用頻度が増えるほど、システムは、受信したメッセージの重要性をより高い精度で予想できるようになります。

プログラム レベルでは、優先受信トレイ REST API は指定のユーザー メッセージで機能し、メッセージごとの **inferenceClassification** プロパティをサポートします。使用可能な値は `Focused` と `Other` であり、ユーザーがそれぞれのメッセージの重要性をどのように見なしているかを示しています。システムがメッセージを分類する方法を修正するには [該当するメッセージの inferenceClassification プロパティを更新します](../api/message-update.md)。時間の経過と共に、これらの修正によっても、メッセージの分類システムが改善されます。

優先受信トレイ REST API では、オーバーライドを作成することもできます。それぞれのオーバーライドは [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) インスタンスで表され、分類システムが常に一貫した方法 (常に "優先" または "その他") で、それまでに学習した方法に関係なく、特定の送信者からのメッセージを指定するように指示するものです。指定したユーザーのオーバーライドを[作成](../api/inferenceclassification-post-overrides.md)、[一覧表示](../api/inferenceclassification-list-overrides.md)、[更新](../api/inferenceclassificationoverride-update.md)、[削除](../api/inferenceclassificationoverride-delete.md)することができます。そのユーザーのオーバーライド (ある場合) は、**inferenceClassificationOverride** インスタンスのコレクションである、**inferenceClassification** ナビゲーション プロパティでアクセスできます。オーバーライドでは、ユーザーは受信メッセージの分類をさらに細かく制御でき、分類システムの信頼性を高めることができます。

分類システムでは受信トレイの受信メッセージについてのみ分類を学習し、適用することに注意してください。その他のフォルダーにあるメッセージは、既定で "優先" になっています。オーバーライドの設定は、今後、受信トレイに入ってくるメッセージに反映され、オーバーライドでは、受信トレイを含むフォルダーにある既存のメッセージの **inferenceClassification** プロパティは変更されません。

## <a name="focused-inbox-api"></a>優先受信トレイ API

**メッセージ分類システムの記憶**

[メッセージの inferenceClassification プロパティの更新](../api/message-update.md)


**オーバーライドを使用した、送信者ごとに一貫した分類**

[送信者のオーバーライドを作成する](../api/inferenceclassification-post-overrides.md) | [ユーザーのすべてのオーバーライドを一覧表示する](../api/inferenceclassification-list-overrides.md) |

[送信者のオーバーライドを更新する](../api/inferenceclassificationoverride-update.md) | [送信者のオーバーライドを削除する](../api/inferenceclassificationoverride-delete.md) 

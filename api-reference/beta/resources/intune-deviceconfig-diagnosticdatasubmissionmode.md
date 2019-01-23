---
title: diagnosticDataSubmissionMode 列挙型
description: ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b587d6872bcd3610c3b878ae7a672c3e776ea01
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422258"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|設定するユーザーを許可します。|
|none|1|OS コンポーネントからは、遠隔測定データは送信されません。 注: この値は、エンタープライズとサーバのデバイスに適用されるのみです。 その他のデバイスでこの設定を使用して、1 の値を設定するのと同じです。|
|基本的な|2|基本的な遠隔測定データを送信します。|
|強化|3|送信には、使用状況と情報のデータを含む遠隔測定データが強化されています。|
|フル|4|システム状態などの診断データを含む完全な遠隔測定データを送信します。|





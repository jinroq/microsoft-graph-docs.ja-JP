---
title: enrollmentState 列挙型
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71f41d459e3fdb50fd853c62a855b4591a8ca8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419108"
---
# <a name="enrollmentstate-enum-type"></a>enrollmentState 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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





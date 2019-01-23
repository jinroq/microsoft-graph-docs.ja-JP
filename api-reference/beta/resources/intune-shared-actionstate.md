---
title: actionState 列挙型
description: デバイス上のアクションの状態
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 54f9a636cb579a234097f86aba8cf4e8fb8fefd0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421614"
---
# <a name="actionstate-enum-type"></a>actionState 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス上のアクションの状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|アクションが有効な状態ではなく|
|保留中|1|操作が保留中です。|
|キャンセル|2|アクションが取り消されました。|
|アクティブです|3|影響はありません。|
|done|4|操作がエラーなく完了しました。|
|失敗しました。|5|操作が失敗しました|
|notSupported|6|アクションはサポートされていません。|





---
title: actionState 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af8bb3869171faee5907b4a3f1921bcb70044aec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829905"
---
# <a name="actionstate-enum-type"></a>actionState 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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






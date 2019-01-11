---
title: applicationGuardBlockClipboardSharingType 列挙型
description: ApplicationGuardBlockClipboardSharingType に指定できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6fe418aa1f91c0e65770b797781dda9e29803d86
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865976"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>applicationGuardBlockClipboardSharingType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ApplicationGuardBlockClipboardSharingType に指定できる値
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|構成されていません|
|blockBoth|1|ブロックのクリップボード データのコンテナーにホストとホスト コンテナーの両方を共有するには|
|blockHostToContainer|2|コンテナーにホストからのデータを共有するためのブロックのクリップボード|
|blockContainerToHost|3|コンテナーからホストへのデータを共有するためのブロックのクリップボード|
|blockNone|4|ブロックのクリップボード データのコンテナーにホストもホストするためのコンテナーを共有するには|




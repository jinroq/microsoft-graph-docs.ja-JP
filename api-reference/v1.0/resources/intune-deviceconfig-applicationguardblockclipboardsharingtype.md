---
title: applicationGuardBlockClipboardSharingType 列挙型
description: ApplicationGuardBlockClipboardSharingType に指定できる値
author: tfitzmac
ms.openlocfilehash: af1843a8d7515e5ca14997256968942f485eab64
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304082"
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




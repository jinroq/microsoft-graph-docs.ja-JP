---
title: applicationGuardBlockClipboardSharingType 列挙型
description: ApplicationGuardBlockClipboardSharingType に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cba0a3fcd25c9f4672d7590718c25e977edf635b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949144"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>applicationGuardBlockClipboardSharingType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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






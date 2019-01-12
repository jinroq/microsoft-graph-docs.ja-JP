---
title: managedAppClipboardSharingLevel 列挙型
description: アプリケーションとの間にデバイスのクリップボードを共有する可能性がありますレベルを表します
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 41983b9bb30880768fff0ee02883c32fcb5305a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968418"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>managedAppClipboardSharingLevel 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アプリケーションとの間にデバイスのクリップボードを共有する可能性がありますレベルを表します
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|allApps|0|かを管理するすべてのアプリケーション間での共有は|
|managedAppsWithPasteIn|1|共有間で許可されてすべてのマネージ アプリケーションでの貼り付けを有効になっています。|
|managedApps|2|すべてのマネージ アプリケーションの間で許可を共有|
|ブロック|3|アプリケーション間での共有が無効になっています。|






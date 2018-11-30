---
title: folderProtectionType 列挙型
description: フォルダーの保護の使用可能な値
ms.openlocfilehash: a02f1602f8b9a962124fb7bf2a9731662a6f3057
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069354"
---
# <a name="folderprotectiontype-enum-type"></a>folderProtectionType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

フォルダーの保護の使用可能な値
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|デバイスの既定値でことを目的しません。|
|有効にします。|1|機能をブロックします。|
|auditMode|2|機能を許可するが、ログを生成します。|
|blockDiskModification|3|ディスク ・ セクターへの書き込みから信頼されていないアプリケーションをブロックします。|
|auditDiskModification|4|信頼されていないアプリケーションがディスクのセクターに書き込むときは、ログを生成します。|






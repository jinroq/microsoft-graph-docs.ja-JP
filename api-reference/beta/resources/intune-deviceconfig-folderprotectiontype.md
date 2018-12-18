---
title: folderProtectionType 列挙型
description: フォルダーの保護の使用可能な値
author: tfitzmac
ms.openlocfilehash: 93df62da9bb5d849cba86b52384f45bfe7bd760f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350604"
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






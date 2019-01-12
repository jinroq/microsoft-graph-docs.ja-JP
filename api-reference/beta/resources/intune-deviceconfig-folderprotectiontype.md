---
title: folderProtectionType 列挙型
description: フォルダーの保護の使用可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 427bdb4fcb93a831ab120aa0c7eefcbf97675fa8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973753"
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






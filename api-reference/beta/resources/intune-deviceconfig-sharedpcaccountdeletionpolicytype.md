---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有 PC でアカウントを削除する場合に使用できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0e9c98a40992bd9404f101f07640014a3f4b6ab5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367996"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a>sharedPCAccountDeletionPolicyType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

共有 PC でアカウントを削除する場合に使用できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|瞬時|.0|すぐに削除します。|
|ディスクスペースしきい値|1-d|ディスク容量のしきい値で削除します。|
|diskSpaceThresholdOrInactiveThreshold|pbm-2|ディスク容量のしきい値または非アクティブなしきい値での削除。|




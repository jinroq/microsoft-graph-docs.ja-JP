---
title: windowsPrivacyDataAccessLevel 列挙型
description: Windows プライバシー データの特定のカテゴリへのアクセス レベルを決定します。
author: tfitzmac
ms.openlocfilehash: 6eb1c1ea6eff28d90979da3ff998fd8442df353a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332411"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>windowsPrivacyDataAccessLevel 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows プライバシー データの特定のカテゴリへのアクセス レベルを決定します。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|目的なしアクセス レベルが指定されませんでした。 デバイスは、UserInControl や ForceAllow のように動作可能性があります。 プライバシー ・ データによりますが、されたバージョンの Windows およびその他の要素にアクセスします。|
|forceAllow|1|アプリケーションは、指定したプライバシー データへのアクセスが許可されます。|
|forceDeny|2|指定したプライバシー ・ データにアクセスするアプリケーションは拒否されます。|
|userInControl|3|アプリケーションが指定したプライバシー ・ データにアクセスしようとした場合、ユーザーが要求されます。|






---
title: windowsPrivacyDataAccessLevel 列挙型
description: Windows プライバシー データの特定のカテゴリへのアクセス レベルを決定します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 64db5eb78708a0cfa835bd695ba01b2c267fc4fd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959317"
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






---
title: windowsPrivacyDataAccessLevel 列挙型
description: 特定の Windows プライバシーデータカテゴリへのアクセスレベルを決定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 507252538606ccb47d72e8dc60710de04acc9b09
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369648"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>windowsPrivacyDataAccessLevel 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

特定の Windows プライバシーデータカテゴリへのアクセスレベルを決定します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|指定されたアクセスレベルはありません。意図的なものではありません。 デバイスは UserInControl または ForceAllow のどちらかの動作をすることがあります。 アクセスされたプライバシーデータ、Windows のバージョン、その他の要因によって異なる場合があります。|
|forceAllow|1-d|アプリは、指定されたプライバシーデータにアクセスできるようになります。|
|forceDeny|pbm-2|アプリは、指定されたプライバシーデータにアクセスすることを拒否されます。|
|userInControl|1/3|アプリが指定されたプライバシーデータにアクセスしようとすると、ユーザーにメッセージが表示されます。|




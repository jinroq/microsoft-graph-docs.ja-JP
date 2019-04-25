---
title: windowsPrivacyDataAccessLevel 列挙型
description: 特定の Windows プライバシーデータカテゴリへのアクセスレベルを決定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10486899094cf275cb3fb9254114d92cb7d12388
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541350"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>windowsPrivacyDataAccessLevel 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

特定の Windows プライバシーデータカテゴリへのアクセスレベルを決定します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|指定されたアクセスレベルはありません。意図的なものではありません。 デバイスは userincontrol または forceallow のどちらかの動作をすることがあります。 アクセスされたプライバシーデータ、Windows のバージョン、その他の要因によって異なる場合があります。|
|forceallow|1 |アプリは、指定されたプライバシーデータにアクセスできるようになります。|
|forcedeny|2 |アプリは、指定されたプライバシーデータにアクセスすることを拒否されます。|
|userincontrol|3 |アプリが指定されたプライバシーデータにアクセスしようとすると、ユーザーにメッセージが表示されます。|





